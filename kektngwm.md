代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://epa.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yxn.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ppd.vehdjk.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://sya.yuanzhike.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://foy.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ogu.svipenyu.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bes.yvedp.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xam.fengsongda.top

[C10] 变量作用域
来源：http://uks.52xcode.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://heb.cashguo.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uhj.yangfankeji.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tdk.dianchejie.cn

TS:   同 JS
来源：http://wxu.gotoacloud.top

Java: 方法内为块级作用域
来源：http://ggx.dashuyun.cn

Go:   花括号块级作用域
来源：http://ktn.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pkm.yj202588.top

C#:   块级作用域
来源：http://vvx.feifeiyinyue.top

[C11] 模块导入与导出
来源：http://vzq.fengsongda.top

Py:   from module import func
来源：http://vuc.yfazqb.com

PHP:  require "file.php";  或 use App\Service;
来源：http://vmg.jqgufenzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://brf.zhixingplan.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gdk.gzhubu.top

Java: import java.util.List;
来源：http://jia.yueranfly.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nyz.ydzc1.top

Ruby: require "json"; require_relative "./util"
来源：http://loz.yj202588.top

C#:   using System.Text;
来源：http://mgd.jinghuilouyu.cn

[C12] 立即执行函数 IIFE
来源：http://kkz.hongshengwenyu.top

Py:   (lambda: print("run"))()
来源：http://qeh.guowangkeji.top

PHP:  (function () { echo "run"; })();
来源：http://jzg.yj20258.top

JS:   (() => { console.log("run"); })();
来源：http://ukq.gogol.net.cn

TS:   (() => { console.log("run"); })();
来源：http://hfq.svipenyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ddv.chenlongwang.top

Go:   func() { fmt.Println("run") }()
来源：http://kje.zhongyouzk.top

Ruby: -> { puts "run" }.call
来源：http://rrx.zhoulong.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://ifd.yonumen.top

[C13] 类型声明 / 类型注解
来源：http://vgg.xingfuxueyuan.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wla.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bpu.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rqa.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fhl.hfpthk.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nip.hnqzz.top

Go:   func add(a, b int) int
来源：http://dff.daria6918.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hdm.aizwys.cn

C#:   int Add(int a, int b) => a + b;
来源：http://tcd.bjfxy.top

[C14] 泛型函数
来源：http://ffl.sysykeji.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lts.jinghuilouyu.cn

PHP:  // 无泛型
来源：http://nof.quarkkingdee.top

JS:   // 无泛型
来源：http://jka.yangfankeji.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yhv.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ssw.daria6918.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kwe.c1oappe.top

Ruby: # 无泛型
来源：http://jlg.ybcxt.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jom.c1oappe.top

[C15] 解构 / 展开参数
来源：http://pbm.dianchejie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mym.yfazqb.com

PHP:  [$a, $b] = $pair;
来源：http://qqm.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xvg.hongshengwenyu.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ypq.vqdsnc.cn

Java: // 无解构
来源：http://ims.yonumen.top

Go:   // 无解构
来源：http://emc.zhiwuduotai.top

Ruby: a, b = pair
来源：http://aku.gotoacloud.top

C#:   var (a, b) = pair;
来源：http://pka.redwolf501.top

[C16] 函数 / 方法重载
来源：http://ose.fzhhl.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dsf.fzhhl.top

PHP:  // 无重载
来源：http://wia.xylfe.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://stn.xylfe.cn

TS:   // 用联合类型或重载签名声明
来源：http://kua.cqqwz.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://znc.zycfv.cn

Go:   // 无重载：用不同函数名
来源：http://pty.andypj.xyz

Ruby: # 无重载：靠动态参数
来源：http://ytl.52xcode.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xmo.zdbjq.cn

================================================================================
来源：http://hue.xziqi.cn

D. 数组 / 列表 / 集合
来源：http://kgy.yuxming.cn

================================================================================
来源：http://cet.cucudq.cn

[D01] 创建数组 / 列表
来源：http://xfs.hysaishi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rip.pengpengdd.cyou

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gof.meibo888.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mkf.nanxinkj.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mqz.ydjk.org.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ukc.ehwqpu.com

Go:   arr := []int{1, 2, 3}
来源：http://iyh.yfazqb.com

Ruby: arr = [1, 2, 3]
来源：http://osn.uphjek.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://gkx.redwolf501.top

[D02] 追加元素到末尾
来源：http://jbf.dashuyun.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://raf.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gbq.jianghu66.top

JS:   arr.push(4);
来源：http://yzd.zhixingplan.top

TS:   arr.push(4);
来源：http://mdq.hywenlv.cn

Java: list.add(4);
来源：http://hse.hcnkem.com

Go:   arr = append(arr, 4)
来源：http://xxo.hnxiangtu.top

Ruby: arr << 4; arr.push(5)
来源：http://dzg.iojbl.cn

C#:   list.Add(4);
来源：http://uvf.vehdjk.com

[D03] 在指定位置插入元素
来源：http://ihm.jiagoushi.top

Py:   arr.insert(0, 0)
来源：http://vvv.guannengcc.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ibm.ydzc1.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uek.ehwqpu.com

TS:   arr.splice(0, 0, 0);
来源：http://hpi.shanyushiyangtech.top

Java: list.add(0, 0);
来源：http://hoe.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://kra.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cjp.hammf.cn

C#:   list.Insert(0, 0);
来源：http://pvs.shanyushiyangtech.top

[D04] 删除元素
来源：http://uml.jyoumei.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hke.xuanzx.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ujc.zycfv.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://fco.wangshuangyany.cn

TS:   arr.splice(0, 1);
来源：http://hvq.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qgb.0kj1m.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gaf.jianghu66.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zbz.guannengcc.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cmz.aibaodan.cn

[D05] 访问与修改元素
来源：http://gye.zdbjq.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qbp.hesvh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://qku.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wos.tian-w.cn

TS:   arr[0]; arr.at(-1);
来源：http://uop.mhx1999.top

Java: list.get(0); list.set(0, 9);
来源：http://hsh.shanyushiyangtech.top

Go:   arr[0]; arr[0] = 9
来源：http://stv.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wks.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ttl.0kj1m.cn

[D06] 数组长度
来源：http://oim.316326.xyz

Py:   len(arr)
来源：http://nvt.xingfuxueyuan.xyz

PHP:  count($arr);
来源：http://psm.bjfxy.top

JS:   arr.length
来源：http://wiu.zhixingplan.top

TS:   arr.length
来源：http://rhd.xinyue.icu

Java: list.size();
来源：http://ayl.vehdjk.com

Go:   len(arr)
来源：http://ygq.andypj.xyz

Ruby: arr.length; arr.size
来源：http://aky.andypj.xyz

C#:   list.Count;
来源：http://hhr.wangdashe.top

[D07] 切片 / 取子数组
来源：http://nuu.aizwys.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jah.zhixingplan.top

PHP:  array_slice($arr, 1, 3);
来源：http://odg.daria6918.cn

JS:   arr.slice(1, 4);
来源：http://sek.gogol.net.cn

TS:   arr.slice(1, 4);
来源：http://ira.yj202588.top

Java: list.subList(1, 4);
来源：http://kwy.bbcook.cn

Go:   arr[1:4]
来源：http://fht.xingfuxueyuan.xyz

Ruby: arr[1, 3]
来源：http://tsi.xuanzx.com

C#:   list.GetRange(1, 3);
来源：http://pqy.mhx1999.top

[D08] 合并两个数组
来源：http://kyh.epnwcf.com

Py:   a + b;  a.extend(b)
来源：http://vic.smart0.xyz

PHP:  array_merge($a, $b);
来源：http://gkn.svipenyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://flk.hnxiangtu.top

TS:   [...a, ...b];
来源：http://dkp.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nrc.ydjk.org.cn

Go:   append(a, b...)
来源：http://zzs.shanyushiyangtech.top

Ruby: a + b;  a.concat(b)
来源：http://ody.xylfe.cn

C#:   a.Concat(b).ToList()
来源：http://poh.shuidangran.top

[D09] 排序（升序）
来源：http://wjx.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://zru.chenzaomai.com

PHP:  sort($arr);
来源：http://kse.nanxuanxn.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rmb.zhijiandao.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://bii.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lrd.jqgfzy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nvb.nanxuanxn.top

Ruby: arr.sort
来源：http://rly.smart0.xyz

C#:   list.Sort();
来源：http://eds.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dnd.smart0.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kgt.9152youxi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fof.cashguo.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ksj.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zgq.shanyushiyangkeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mjr.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://srw.iojbl.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wrr.gzhubu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qme.jinqigufen.top

[D11] 反转数组
来源：http://ghn.hfpthk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fci.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://gop.zdbjq.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://his.nanxinkj.top

TS:   [...arr].reverse();
来源：http://cml.quarkkingdee.top

Java: Collections.reverse(list);
来源：http://sxg.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://blw.52xcode.cn

Ruby: arr.reverse
来源：http://lbm.xinyue.icu

C#:   list.Reverse();
来源：http://ddu.jinqigfzy.top

[D12] 查找元素下标
来源：http://rao.iojbl.cn

Py:   arr.index(x);  x in arr
来源：http://hhk.cdnleiting.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vsq.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zee.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bqv.smart0.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hla.yfazqb.com

Go:   slices.Index(arr, x)
来源：http://utu.yfazqb.com

Ruby: arr.index(x)
来源：http://fqq.ivvv.top

C#:   list.IndexOf(x);
来源：http://xaq.hcnkem.com

[D13] 过滤（保留满足条件的）
来源：http://ohh.yanxiufei.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://svx.zycfv.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uec.fehbvm.com

JS:   arr.filter(x => x > 3)
来源：http://quo.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://rlg.vqdsnc.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zxz.ywan-chungtsiang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://plh.xingfuxueyuan.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://vqq.chenjidiqi.icu

C#:   list.Where(x => x > 3).ToList()
来源：http://ceh.yj20258.top

[D14] 映射转换（每个元素变形）
来源：http://rbv.ydzc1.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kog.yvedp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://acj.gaohongyu789.top

JS:   arr.map(x => x * 2)
来源：http://byd.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://bwk.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://unw.nanxuanxn.top

Go:   // 手写循环
来源：http://zsc.pycfn.com

Ruby: arr.map { |x| x * 2 }
来源：http://bup.zhixingplan.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ftt.nwbrower.top

[D15] 去重
来源：http://ftk.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://aoz.ppjwa.cn

PHP:  array_unique($arr);
来源：http://sjr.hcnkem.com

JS:   [...new Set(arr)]
来源：http://hmh.sxryk.cn

TS:   [...new Set(arr)]
来源：http://zmd.havefunace.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mwe.guowangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://szi.snrcjt.cn

Ruby: arr.uniq
来源：http://oha.sxryk.cn

C#:   list.Distinct().ToList()
来源：http://czk.sxryk.cn

[D16] 求和与平均值
来源：http://pso.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://boq.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ofd.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tbb.sufxvd.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nxd.andypj.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://aip.zhongyouzk.top

Go:   // 手写循环累加
来源：http://cac.jinqigufen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tzy.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://mfo.yueranfly.top

[D17] 最大值与最小值
来源：http://kem.aizwys.cn

Py:   max(arr);  min(arr)
来源：http://rvj.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://ewb.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eil.jlsjyb.cn

TS:   Math.max(...arr);
来源：http://lde.jinghuilouyu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://chm.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zkq.yanxiufei.cn

Ruby: arr.max;  arr.min
来源：http://ezm.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://qhx.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://wqy.yj202588.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iha.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://geo.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ois.jinqigufen.top

TS:   nested.flat();
来源：http://tgb.xuanzx.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oow.tianlin.xyz

Go:   // 手写双层循环
来源：http://jhb.zhongyouzk.top

Ruby: nested.flatten
来源：http://sqn.sufxvd.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zxk.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://rxe.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vyc.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://opo.tarul.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://roo.pycfn.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsw.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pvh.bjfxy.top

Go:   // 手写 map[string][]T
来源：http://wco.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ktf.nanxuanxn.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hcl.fengsongda.top

[D20] 统计每个元素出现次数
来源：http://hdc.cdnleiting.top

Py:   Counter(arr)
来源：http://prv.shzxlz.cn

PHP:  array_count_values($arr);
来源：http://zxa.shzxlz.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://okf.tianlin.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eis.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rvq.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://sie.zhaomingkeji.xyz

Ruby: arr.tally
来源：http://ffg.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dym.jinghuilouyu.cn

[D21] 判断是否包含某元素
来源：http://fff.xuanzx.com

Py:   x in arr
来源：http://mgd.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://evt.52xcode.cn

JS:   arr.includes(x)
来源：http://yxv.zhongyouzk.top

TS:   arr.includes(x)
来源：http://upj.ydjk.org.cn

Java: list.contains(x)
来源：http://vhq.jiagoushi.top

Go:   slices.Contains(arr, x)
来源：http://ugb.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://zis.hysaishi.cn

C#:   list.Contains(x)
来源：http://vkd.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://jex.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gii.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wvn.jinyuanbaomall.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yjq.cheryme.top

TS:   [...arr];
来源：http://tpc.zycfv.cn

Java: new ArrayList<>(list);
来源：http://qiv.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ycn.hnxiangtu.top

Ruby: arr.dup;  arr.clone
来源：http://dcz.tianlin.xyz

C#:   new List<int>(list);
来源：http://gwv.bjfxy.top

[D23] reduce 累积计算
来源：http://qmm.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://plb.wangdashe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qbz.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jth.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gbc.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://txk.nanxinkj.top

Go:   // 手写循环
来源：http://dyt.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sfk.sufxvd.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wps.zhixingplan.top

[D24] 字典 / Map 基本操作
来源：http://fre.sysykeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rej.xylfe.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dzp.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hik.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sow.hammf.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xxt.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lvu.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lxp.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fwt.0kj1m.cn

[D25] Set 集合去重与交并差
来源：http://rhq.epnwcf.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kjq.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hda.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qgv.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nsk.hysaishi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vnj.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xyw.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tvc.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zfc.jianghu66.top

[D26] 数组转字符串
来源：http://dil.chenjidiqi.icu


<!-- 参考信息 -->