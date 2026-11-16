代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tef.ydjk.org.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ntb.cashguo.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yls.xylfe.cn

[C09] 递归
来源：http://yxa.yangfankeji.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ddt.zhongyouzk.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dhc.zhixingplan.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yan.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yyh.gzhubu.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hch.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bgy.cucudq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uej.fzhhl.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wtl.yongpay.top

[C10] 变量作用域
来源：http://swc.ehwqpu.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://uus.yj20258888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ozz.52xcode.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ryg.wangshuangyany.cn

TS:   同 JS
来源：http://xzu.hesvh.cn

Java: 方法内为块级作用域
来源：http://gaf.sufxvd.cn

Go:   花括号块级作用域
来源：http://dim.fehbvm.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rja.jiagoushi.top

C#:   块级作用域
来源：http://ozq.dianchejie.cn

[C11] 模块导入与导出
来源：http://eal.shuidangran.top

Py:   from module import func
来源：http://oqs.hesvh.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://qiv.ydjk.org.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ikc.fehbvm.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://drk.yuxming.cn

Java: import java.util.List;
来源：http://rhz.aizwys.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kye.yuxming.cn

Ruby: require "json"; require_relative "./util"
来源：http://new.tanke756.top

C#:   using System.Text;
来源：http://ouv.bbcook.cn

[C12] 立即执行函数 IIFE
来源：http://vrj.xylfe.cn

Py:   (lambda: print("run"))()
来源：http://emx.havefunace.top

PHP:  (function () { echo "run"; })();
来源：http://xqm.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://fhg.pycfn.com

TS:   (() => { console.log("run"); })();
来源：http://ugz.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://lqx.tarul.cn

Go:   func() { fmt.Println("run") }()
来源：http://omf.jinghuilouyu.cn

Ruby: -> { puts "run" }.call
来源：http://zzm.vehdjk.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qka.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://xmz.hnqzz.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ltg.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ixi.sufxvd.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gqa.shuidangran.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://trb.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://dph.andypj.xyz

Go:   func add(a, b int) int
来源：http://fsi.wangshuangyany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sqe.feifeiyinyue.top

C#:   int Add(int a, int b) => a + b;
来源：http://dpt.xuanzx.com

[C14] 泛型函数
来源：http://maj.jinqigufen.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://auh.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://cwg.hammf.cn

JS:   // 无泛型
来源：http://kpt.xziqi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tui.yonumen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lxq.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qsx.chenzaomai.com

Ruby: # 无泛型
来源：http://ryx.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://orq.yj20258.top

[C15] 解构 / 展开参数
来源：http://jce.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kqs.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://miv.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czl.yangfankeji.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zqx.jianghu66.top

Java: // 无解构
来源：http://gpe.tarul.cn

Go:   // 无解构
来源：http://vdj.xuetiantiany.cn

Ruby: a, b = pair
来源：http://boo.quarkkingdee.top

C#:   var (a, b) = pair;
来源：http://xdz.ivvv.top

[C16] 函数 / 方法重载
来源：http://obn.9152youxi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zzu.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://vkp.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nla.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://ghw.bbcook.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cxx.bbcook.cn

Go:   // 无重载：用不同函数名
来源：http://pjl.guowangkeji.top

Ruby: # 无重载：靠动态参数
来源：http://tib.dashuyun.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cwm.fanxiaobao.xyz

================================================================================
来源：http://vfc.havefunace.top

D. 数组 / 列表 / 集合
来源：http://dat.yonumen.top

================================================================================
来源：http://ysp.yfazqb.com

[D01] 创建数组 / 列表
来源：http://dun.jiagoushi.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://iuw.xylfe.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://nyd.sjlbkw.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://peu.svipenyu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://har.gzhubu.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ntw.sufxvd.cn

Go:   arr := []int{1, 2, 3}
来源：http://zyq.feifeiyinyue.top

Ruby: arr = [1, 2, 3]
来源：http://ugt.zhoulong.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gzw.hnxiangtu.top

[D02] 追加元素到末尾
来源：http://lkv.sufxvd.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bfy.havefunace.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lms.xuetiantiany.cn

JS:   arr.push(4);
来源：http://pgv.cheryme.top

TS:   arr.push(4);
来源：http://gui.zhongyouzk.top

Java: list.add(4);
来源：http://tkt.fktsv.cn

Go:   arr = append(arr, 4)
来源：http://iek.bjfxy.top

Ruby: arr << 4; arr.push(5)
来源：http://xxo.cucudq.cn

C#:   list.Add(4);
来源：http://mpm.ctjpmb.com

[D03] 在指定位置插入元素
来源：http://qkl.xuanzx.com

Py:   arr.insert(0, 0)
来源：http://bqt.zhongyouzk.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rtx.feifeiyinyue.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fux.shanyushiyangkeji.top

TS:   arr.splice(0, 0, 0);
来源：http://hgi.daxiang520.top

Java: list.add(0, 0);
来源：http://byn.sweek.top

Go:   arr = append([]int{0}, arr...)
来源：http://npe.ybcxt.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://jer.shzxlz.cn

C#:   list.Insert(0, 0);
来源：http://ujh.iojbl.cn

[D04] 删除元素
来源：http://exy.snrcjt.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cjg.hysaishi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xoy.zhengqikj.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wbo.yfazqb.com

TS:   arr.splice(0, 1);
来源：http://bql.ctjpmb.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vto.guowangkeji.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qcj.fzhhl.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cja.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bob.vqdsnc.cn

[D05] 访问与修改元素
来源：http://ein.yueranfly.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jfn.zhoulong.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rng.shzxlz.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://itk.vehdjk.com

TS:   arr[0]; arr.at(-1);
来源：http://spn.jinghuilouyu.cn

Java: list.get(0); list.set(0, 9);
来源：http://jxo.zhixingplan.top

Go:   arr[0]; arr[0] = 9
来源：http://qle.zdqjudy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zjw.fktsv.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qyo.9152youxi.cn

[D06] 数组长度
来源：http://nhx.pengpengdd.cyou

Py:   len(arr)
来源：http://qhq.ivvv.top

PHP:  count($arr);
来源：http://cmq.ivvv.top

JS:   arr.length
来源：http://mga.chenzaomai.com

TS:   arr.length
来源：http://suf.fengsongda.top

Java: list.size();
来源：http://hpv.tarul.cn

Go:   len(arr)
来源：http://jps.0kj1m.cn

Ruby: arr.length; arr.size
来源：http://mrf.chenlongwang.top

C#:   list.Count;
来源：http://fdt.hnqzz.top

[D07] 切片 / 取子数组
来源：http://fdu.gzhubu.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fgo.fktsv.cn

PHP:  array_slice($arr, 1, 3);
来源：http://duj.sweek.top

JS:   arr.slice(1, 4);
来源：http://vfl.gogol.net.cn

TS:   arr.slice(1, 4);
来源：http://yfw.kuanghao11.cn

Java: list.subList(1, 4);
来源：http://odb.shuidangran.top

Go:   arr[1:4]
来源：http://owb.yj20258888.top

Ruby: arr[1, 3]
来源：http://qwe.kuanghao11.cn

C#:   list.GetRange(1, 3);
来源：http://hmv.hnqzz.top

[D08] 合并两个数组
来源：http://uca.yueranfly.top

Py:   a + b;  a.extend(b)
来源：http://jcx.sjlbkw.cn

PHP:  array_merge($a, $b);
来源：http://mid.cashguo.top

JS:   [...a, ...b];  a.concat(b);
来源：http://gll.quarkkingdee.top

TS:   [...a, ...b];
来源：http://lyf.jinqigfzy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wsa.jinqigfzy.top

Go:   append(a, b...)
来源：http://flk.svipenyu.cn

Ruby: a + b;  a.concat(b)
来源：http://yil.zhijiandao.cn

C#:   a.Concat(b).ToList()
来源：http://auf.gogol.net.cn

[D09] 排序（升序）
来源：http://ppq.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://tpn.wangdashe.top

PHP:  sort($arr);
来源：http://dbt.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fak.shangyingyoupin.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kjq.guannengcc.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cgt.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oqi.epnwcf.com

Ruby: arr.sort
来源：http://dir.aibaodan.cn

C#:   list.Sort();
来源：http://uoq.chenzaomai.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://kue.ctjpmb.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gur.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cpf.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lui.guannengcc.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kge.zhaomingkeji.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ovr.9152youxi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://pxf.dianchejie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://otn.fengsongda.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sue.aizwys.cn

[D11] 反转数组
来源：http://izm.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://vhr.52xcode.cn

PHP:  array_reverse($arr);
来源：http://mzb.hysaishi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jzx.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://bvc.jlsjyb.cn

Java: Collections.reverse(list);
来源：http://oxp.havefunace.top

Go:   slices.Reverse(arr)
来源：http://qyv.tanke756.top

Ruby: arr.reverse
来源：http://qdl.haohaochexian.top

C#:   list.Reverse();
来源：http://kkz.meibo888.top

[D12] 查找元素下标
来源：http://tuu.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://gtx.chenjidiqi.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rrn.cashguo.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jcz.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://brp.jqgfzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tyw.zhijiandao.cn

Go:   slices.Index(arr, x)
来源：http://irg.zhoulong.xyz

Ruby: arr.index(x)
来源：http://cts.yuxming.cn

C#:   list.IndexOf(x);
来源：http://usk.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://vdg.ppjwa.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ofv.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xnd.zdbjq.cn

JS:   arr.filter(x => x > 3)
来源：http://ydz.xylfe.cn

TS:   arr.filter(x => x > 3)
来源：http://mvq.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yfq.yj20258888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mrw.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jht.dashuyun.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xhz.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://vtu.daria6918.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eta.zhoulong.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rpw.jianghu66.top

JS:   arr.map(x => x * 2)
来源：http://pnk.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://zmf.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://otx.guannengcc.top

Go:   // 手写循环
来源：http://pnw.shangyingyoupin.top

Ruby: arr.map { |x| x * 2 }
来源：http://ves.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tqn.daxiang520.top

[D15] 去重
来源：http://iwl.hesvh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uii.tanke756.top

PHP:  array_unique($arr);
来源：http://xkg.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://gei.bbcook.cn

TS:   [...new Set(arr)]
来源：http://piu.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pbj.tarul.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uci.316326.xyz

Ruby: arr.uniq
来源：http://pgm.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://lag.yanxiufei.cn

[D16] 求和与平均值
来源：http://vnl.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://exp.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://egh.hywenlv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://psb.jyoumei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzs.sjlbkw.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ilw.wangdashe.top

Go:   // 手写循环累加
来源：http://juv.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://loc.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://igi.ctjpmb.com

[D17] 最大值与最小值
来源：http://cse.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://xxa.fengsongda.top

PHP:  max($arr);  min($arr);
来源：http://tsq.dashuyun.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bzw.hesvh.cn

TS:   Math.max(...arr);
来源：http://ynl.fzhhl.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tqe.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rgt.316326.xyz

Ruby: arr.max;  arr.min
来源：http://mvj.havefunace.top

C#:   list.Max();  list.Min()
来源：http://nfx.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://jai.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eaq.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://bzk.52xcode.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dgt.yueranfly.top

TS:   nested.flat();
来源：http://jqn.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yrb.ehwqpu.com

Go:   // 手写双层循环
来源：http://rjy.aibaodan.cn

Ruby: nested.flatten
来源：http://zrw.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hsa.fzhhl.top

[D19] 按字段分组
来源：http://qin.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xcw.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hnr.gotoacloud.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eyq.hesvh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bsc.chenzaomai.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mdr.ivvv.top

Go:   // 手写 map[string][]T
来源：http://ivq.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gcu.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qew.zhixingplan.top

[D20] 统计每个元素出现次数
来源：http://gub.316326.xyz

Py:   Counter(arr)
来源：http://eej.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://apa.iojbl.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nly.ppjwa.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qza.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tli.zhaomingkeji.xyz

Go:   // 手写 map[T]int
来源：http://ykn.fehbvm.com

Ruby: arr.tally
来源：http://xbx.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zzb.sweek.top

[D21] 判断是否包含某元素
来源：http://kba.tianlin.xyz

Py:   x in arr
来源：http://aif.316326.xyz

PHP:  in_array($x, $arr, true);
来源：http://ups.zhixingplan.top

JS:   arr.includes(x)
来源：http://cju.hywenlv.cn

TS:   arr.includes(x)
来源：http://pzg.ywan-chungtsiang.top

Java: list.contains(x)
来源：http://lon.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://hrt.hnqzz.top

Ruby: arr.include?(x)
来源：http://cjt.mhx1999.top

C#:   list.Contains(x)
来源：http://xnx.tanke756.top

[D22] 复制数组（避免共享引用）
来源：http://ofk.dashuyun.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://prr.haohaochexian.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eef.andypj.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dqw.jlsjyb.cn

TS:   [...arr];
来源：http://wqa.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://gye.cashguo.top

Go:   copied := append([]int(nil), arr...)
来源：http://lzn.jinghuilouyu.cn

Ruby: arr.dup;  arr.clone
来源：http://gpc.jiagoushi.top

C#:   new List<int>(list);
来源：http://bik.zdbjq.cn

[D23] reduce 累积计算
来源：http://fiw.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bbh.zhoulong.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkq.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jhz.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://afj.zhiwuduotai.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bds.birdmap.top

Go:   // 手写循环
来源：http://gdo.fzhhl.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tvq.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kyb.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://fcy.dianchejie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pvr.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gng.havefunace.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wjp.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sco.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ymq.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kae.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hfx.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rnj.tanke756.top

[D25] Set 集合去重与交并差
来源：http://add.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vqy.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xny.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://caf.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wfo.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://owy.yj20258.top


<!-- 参考信息 -->