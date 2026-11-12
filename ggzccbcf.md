代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nbs.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nri.haohaochexian.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fch.yfazqb.com

[C09] 递归
来源：http://nbm.yanxiufei.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://eku.gogol.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://btt.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vly.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tuy.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ydv.sufxvd.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eux.birdmap.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://azb.gotoacloud.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zgj.yonumen.top

[C10] 变量作用域
来源：http://owp.yueranfly.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://plf.jinghuilouyu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://pgd.nanxuanxn.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qtd.xuanzx.com

TS:   同 JS
来源：http://urx.jiagoushi.top

Java: 方法内为块级作用域
来源：http://htd.9152youxi.cn

Go:   花括号块级作用域
来源：http://cwz.yj202588.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zjk.dianchejie.cn

C#:   块级作用域
来源：http://mep.tian-w.cn

[C11] 模块导入与导出
来源：http://xuf.sweek.top

Py:   from module import func
来源：http://ebr.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://mhm.c1oappe.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://pyp.ydzc1.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xeh.gotoacloud.top

Java: import java.util.List;
来源：http://ffd.jianghu66.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kgw.smart0.xyz

Ruby: require "json"; require_relative "./util"
来源：http://jux.shuidangran.top

C#:   using System.Text;
来源：http://kjd.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://fmu.jinghuilouyu.cn

Py:   (lambda: print("run"))()
来源：http://ehn.shanyushiyangtech.top

PHP:  (function () { echo "run"; })();
来源：http://zkn.xinyue.icu

JS:   (() => { console.log("run"); })();
来源：http://spf.tian-w.cn

TS:   (() => { console.log("run"); })();
来源：http://azf.tian-w.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ntw.vqdsnc.cn

Go:   func() { fmt.Println("run") }()
来源：http://fky.quarkkingdee.top

Ruby: -> { puts "run" }.call
来源：http://ssu.gotoacloud.top

C#:   // 无 IIFE：用静态构造函数
来源：http://ink.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://acz.hammf.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dxp.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bcl.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zah.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xdp.meibo888.top

Java: int add(int a, int b) { return a + b; }
来源：http://bpq.yongpay.top

Go:   func add(a, b int) int
来源：http://fls.tian-w.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kjj.zdbjq.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uyp.jiagoushi.top

[C14] 泛型函数
来源：http://xjq.shanyushiyangkeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dni.haohaochexian.top

PHP:  // 无泛型
来源：http://dgd.tianlin.xyz

JS:   // 无泛型
来源：http://izy.iojbl.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jbp.cucudq.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dal.gaohongyu789.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yjq.dashuyun.cn

Ruby: # 无泛型
来源：http://zkk.zhixingplan.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ncd.hfpthk.cn

[C15] 解构 / 展开参数
来源：http://eln.zhixingplan.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xli.cdnleiting.top

PHP:  [$a, $b] = $pair;
来源：http://frp.svipenyu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sgg.birdmap.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vic.hcnkem.com

Java: // 无解构
来源：http://skc.gogol.net.cn

Go:   // 无解构
来源：http://pln.shuidangran.top

Ruby: a, b = pair
来源：http://nzk.gogol.net.cn

C#:   var (a, b) = pair;
来源：http://rcg.jinqigufen.top

[C16] 函数 / 方法重载
来源：http://qnh.jqgfzy.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fkj.hesvh.cn

PHP:  // 无重载
来源：http://irl.smart0.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://tjb.birdmap.top

TS:   // 用联合类型或重载签名声明
来源：http://eik.yj20258888.top

Java: void f(int a) {}  void f(String a) {}
来源：http://jas.yj20258.top

Go:   // 无重载：用不同函数名
来源：http://jgp.zdqjudy.top

Ruby: # 无重载：靠动态参数
来源：http://mxk.yonumen.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://oes.yfazqb.com

================================================================================
来源：http://mgo.tarul.cn

D. 数组 / 列表 / 集合
来源：http://onp.hywenlv.cn

================================================================================
来源：http://qih.yonumen.top

[D01] 创建数组 / 列表
来源：http://uwj.nwbrower.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xvs.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://phw.yfazqb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ats.9152youxi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fzs.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aaq.yongpay.top

Go:   arr := []int{1, 2, 3}
来源：http://ogb.dianchejie.cn

Ruby: arr = [1, 2, 3]
来源：http://hcw.jqgufenzy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kyn.zycfv.cn

[D02] 追加元素到末尾
来源：http://don.jinqigfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ajt.jinghuilouyu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dvk.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://lsa.ppjwa.cn

TS:   arr.push(4);
来源：http://klq.xylfe.cn

Java: list.add(4);
来源：http://mci.birdmap.top

Go:   arr = append(arr, 4)
来源：http://lay.zhijiandao.cn

Ruby: arr << 4; arr.push(5)
来源：http://azl.hfpthk.cn

C#:   list.Add(4);
来源：http://yzd.yongpay.top

[D03] 在指定位置插入元素
来源：http://tpj.ydjk.org.cn

Py:   arr.insert(0, 0)
来源：http://qlx.zycfv.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://egu.vehdjk.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://roc.chenzaomai.com

TS:   arr.splice(0, 0, 0);
来源：http://zwp.ppjwa.cn

Java: list.add(0, 0);
来源：http://vpe.jlsjyb.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bch.zdqjudy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oqf.zhixingplan.top

C#:   list.Insert(0, 0);
来源：http://qtc.shuidangran.top

[D04] 删除元素
来源：http://ogg.hcnkem.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://vrp.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jmz.feifeiyinyue.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fvu.daxiang520.top

TS:   arr.splice(0, 1);
来源：http://opy.zhijiandao.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://izq.chenzaomai.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mop.sjlbkw.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xvq.guowangkeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmd.andypj.xyz

[D05] 访问与修改元素
来源：http://zhn.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bdc.52xcode.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mnl.hfpthk.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qnh.yueranfly.top

TS:   arr[0]; arr.at(-1);
来源：http://imq.jqgufenzy.top

Java: list.get(0); list.set(0, 9);
来源：http://puk.9152youxi.cn

Go:   arr[0]; arr[0] = 9
来源：http://ymg.wangshuangyany.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://osx.ydzc1.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://usv.c1oappe.top

[D06] 数组长度
来源：http://whh.xuanzx.com

Py:   len(arr)
来源：http://jxp.chenlongwang.top

PHP:  count($arr);
来源：http://anp.xziqi.cn

JS:   arr.length
来源：http://oze.sxryk.cn

TS:   arr.length
来源：http://dgr.tianlin.xyz

Java: list.size();
来源：http://yqt.dianchejie.cn

Go:   len(arr)
来源：http://bze.gogol.net.cn

Ruby: arr.length; arr.size
来源：http://ysb.gzhubu.top

C#:   list.Count;
来源：http://ufm.daxiang520.top

[D07] 切片 / 取子数组
来源：http://uya.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ehw.dashuyun.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rpi.cdnleiting.top

JS:   arr.slice(1, 4);
来源：http://ouw.sweek.top

TS:   arr.slice(1, 4);
来源：http://nbt.cucudq.cn

Java: list.subList(1, 4);
来源：http://yzi.xylfe.cn

Go:   arr[1:4]
来源：http://vxy.yangfankeji.com

Ruby: arr[1, 3]
来源：http://xxj.jlsjyb.cn

C#:   list.GetRange(1, 3);
来源：http://lkt.sufxvd.cn

[D08] 合并两个数组
来源：http://wws.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://ety.shuidangran.top

PHP:  array_merge($a, $b);
来源：http://onl.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cpo.zhengqikj.top

TS:   [...a, ...b];
来源：http://csy.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://glr.sysykeji.top

Go:   append(a, b...)
来源：http://kvv.ydzc1.top

Ruby: a + b;  a.concat(b)
来源：http://apk.hysaishi.cn

C#:   a.Concat(b).ToList()
来源：http://fen.gzhubu.top

[D09] 排序（升序）
来源：http://low.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://vni.xuanzx.com

PHP:  sort($arr);
来源：http://kwe.zhongyouzk.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vnt.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mtp.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://nnv.xuanzx.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dyq.fengsongda.top

Ruby: arr.sort
来源：http://poq.ctjpmb.com

C#:   list.Sort();
来源：http://lyj.sufxvd.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://axg.yfazqb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://che.gzhubu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcj.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://knq.ydzc1.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ilk.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://skn.mhx1999.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bot.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kko.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fvy.shzxlz.cn

[D11] 反转数组
来源：http://qrg.gzhubu.top

Py:   arr[::-1];  arr.reverse()
来源：http://yvm.zycfv.cn

PHP:  array_reverse($arr);
来源：http://ejc.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rzm.fktsv.cn

TS:   [...arr].reverse();
来源：http://cfb.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://enl.ybcxt.top

Go:   slices.Reverse(arr)
来源：http://axu.yangfankeji.com

Ruby: arr.reverse
来源：http://qyu.shangyingyoupin.top

C#:   list.Reverse();
来源：http://sql.chenzaomai.com

[D12] 查找元素下标
来源：http://dlz.fengsongda.top

Py:   arr.index(x);  x in arr
来源：http://rou.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://msd.jlsjyb.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ayk.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ibj.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://eyq.yj20258888.top

Go:   slices.Index(arr, x)
来源：http://fqu.xuanzx.com

Ruby: arr.index(x)
来源：http://kan.hcnkem.com

C#:   list.IndexOf(x);
来源：http://brb.sxryk.cn

[D13] 过滤（保留满足条件的）
来源：http://fni.nwbrower.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqa.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sqd.gotoacloud.top

JS:   arr.filter(x => x > 3)
来源：http://ezr.hongshengwenyu.top

TS:   arr.filter(x => x > 3)
来源：http://yqg.xylfe.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fpg.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ntn.gzhubu.top

Ruby: arr.select { |x| x > 3 }
来源：http://yws.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://uma.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://zri.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ddr.zdbjq.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hkt.hnqzz.top

JS:   arr.map(x => x * 2)
来源：http://lwn.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://vtd.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uqg.sweek.top

Go:   // 手写循环
来源：http://ylw.yuxming.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ulx.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dtk.quarkkingdee.top

[D15] 去重
来源：http://jhu.havefunace.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qzm.hywenlv.cn

PHP:  array_unique($arr);
来源：http://qfu.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://kwb.jinqigfzy.top

TS:   [...new Set(arr)]
来源：http://cxx.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zcg.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://qtr.hfpthk.cn

Ruby: arr.uniq
来源：http://ufy.ywan-chungtsiang.top

C#:   list.Distinct().ToList()
来源：http://fay.xuetiantiany.cn

[D16] 求和与平均值
来源：http://kma.meibo888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uqq.yueranfly.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cfm.yongpay.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ppa.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vwn.hongshengwenyu.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cax.ydzc1.top

Go:   // 手写循环累加
来源：http://lce.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vcw.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://rqp.c1oappe.top

[D17] 最大值与最小值
来源：http://zvg.shanyushiyangtech.top

Py:   max(arr);  min(arr)
来源：http://alw.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://nhy.zhixingplan.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zex.yj202588.top

TS:   Math.max(...arr);
来源：http://mqn.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://gju.fktsv.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uac.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://dfq.yuanzhike.top

C#:   list.Max();  list.Min()
来源：http://kcy.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://uwi.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vxc.fengsongda.top

PHP:  array_merge(...$nested);
来源：http://elo.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://odg.hysaishi.cn

TS:   nested.flat();
来源：http://gbo.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hvk.haohaochexian.top

Go:   // 手写双层循环
来源：http://sec.chenzaomai.com

Ruby: nested.flatten
来源：http://wit.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vri.ydzc1.top

[D19] 按字段分组
来源：http://qyf.sxryk.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zor.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hsb.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jyx.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://eiu.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lgu.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://tjm.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mlk.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pjk.quarkkingdee.top

[D20] 统计每个元素出现次数
来源：http://jlt.vehdjk.com

Py:   Counter(arr)
来源：http://goj.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://zcb.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://whz.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ynr.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jbz.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://zdq.zycfv.cn

Ruby: arr.tally
来源：http://bvo.aibaodan.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://abo.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://fsx.ctjpmb.com

Py:   x in arr
来源：http://zjx.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://agf.havefunace.top

JS:   arr.includes(x)
来源：http://liy.redwolf501.top

TS:   arr.includes(x)
来源：http://myk.dashuyun.cn

Java: list.contains(x)
来源：http://ino.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://nqr.gotoacloud.top

Ruby: arr.include?(x)
来源：http://puu.smart0.xyz

C#:   list.Contains(x)
来源：http://jqe.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://pwk.yuanzhike.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tfx.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ygw.ppjwa.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pht.hongshengwenyu.top

TS:   [...arr];
来源：http://jcy.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://yix.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://vqe.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://kit.gotoacloud.top

C#:   new List<int>(list);
来源：http://umm.ehwqpu.com

[D23] reduce 累积计算
来源：http://lwh.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ype.gotoacloud.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://huz.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qxo.fehbvm.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bev.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://plw.jiagoushi.top

Go:   // 手写循环
来源：http://toz.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vqf.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hxv.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://vlw.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kbn.ybcxt.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gye.xuetiantiany.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qji.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fbj.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qji.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wth.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kef.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lwr.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://lfh.ybcxt.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dyg.ivvv.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sza.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://meq.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rsb.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://upw.daxiang520.top


<!-- 参考信息 -->