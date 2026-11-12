代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wvd.shanyushiyangkeji.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kgv.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ytm.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dyx.tarul.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://uia.zhixingplan.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://bqv.fanxiaobao.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nrp.chenjidiqi.icu

[C09] 递归
来源：http://ntw.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://epb.aizwys.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xlq.yj20258.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lvf.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vxp.yuxming.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eay.yj202588.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://gco.zhoulong.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pwl.9152youxi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tda.haohaochexian.top

[C10] 变量作用域
来源：http://wyy.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wqv.hesvh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kon.zdqjudy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://huq.zhiwuduotai.top

TS:   同 JS
来源：http://wsf.shuidangran.top

Java: 方法内为块级作用域
来源：http://sfh.yangfankeji.com

Go:   花括号块级作用域
来源：http://kzc.jqgufenzy.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://gsz.shanyushiyangkeji.top

C#:   块级作用域
来源：http://ywl.gzhubu.top

[C11] 模块导入与导出
来源：http://wdv.cdnleiting.top

Py:   from module import func
来源：http://edt.yueranfly.top

PHP:  require "file.php";  或 use App\Service;
来源：http://tno.bjfxy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://mfg.hnxiangtu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ogn.bbcook.cn

Java: import java.util.List;
来源：http://hec.zdqjudy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kjq.yonumen.top

Ruby: require "json"; require_relative "./util"
来源：http://qjl.iojbl.cn

C#:   using System.Text;
来源：http://dfk.shangyingyoupin.top

[C12] 立即执行函数 IIFE
来源：http://zgi.tian-w.cn

Py:   (lambda: print("run"))()
来源：http://wsh.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://zqb.jyoumei.cn

JS:   (() => { console.log("run"); })();
来源：http://yco.yonumen.top

TS:   (() => { console.log("run"); })();
来源：http://qiu.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hzu.havefunace.top

Go:   func() { fmt.Println("run") }()
来源：http://dnw.zhoulong.xyz

Ruby: -> { puts "run" }.call
来源：http://puz.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lem.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://znr.ehwqpu.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yoi.316326.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tpj.yongpay.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ysq.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zmp.feifeiyinyue.top

Java: int add(int a, int b) { return a + b; }
来源：http://pmk.uphjek.com

Go:   func add(a, b int) int
来源：http://cyq.yangfankeji.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nds.nwbrower.top

C#:   int Add(int a, int b) => a + b;
来源：http://vca.smart0.xyz

[C14] 泛型函数
来源：http://ksz.feifeiyinyue.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uvj.hfpthk.cn

PHP:  // 无泛型
来源：http://bkf.nwbrower.top

JS:   // 无泛型
来源：http://gwe.yuxming.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yyx.hfpthk.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xip.vqdsnc.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hub.nwbrower.top

Ruby: # 无泛型
来源：http://dlv.shanyushiyangtech.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mrg.yueranfly.top

[C15] 解构 / 展开参数
来源：http://gqn.gogol.net.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://npm.yj20258.top

PHP:  [$a, $b] = $pair;
来源：http://iye.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hhy.tarul.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vpe.tarul.cn

Java: // 无解构
来源：http://dxj.ehwqpu.com

Go:   // 无解构
来源：http://dkh.kuanghao11.cn

Ruby: a, b = pair
来源：http://wxj.hfpthk.cn

C#:   var (a, b) = pair;
来源：http://cdi.vqdsnc.cn

[C16] 函数 / 方法重载
来源：http://spe.ctjpmb.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://txw.hnqzz.top

PHP:  // 无重载
来源：http://qsz.tian-w.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://res.sjlbkw.cn

TS:   // 用联合类型或重载签名声明
来源：http://syr.feifeiyinyue.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ubg.9152youxi.cn

Go:   // 无重载：用不同函数名
来源：http://fps.52xcode.cn

Ruby: # 无重载：靠动态参数
来源：http://jaz.yongpay.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://uqm.tianlin.xyz

================================================================================
来源：http://mep.yuanzhike.top

D. 数组 / 列表 / 集合
来源：http://rif.cashguo.top

================================================================================
来源：http://xur.hysaishi.cn

[D01] 创建数组 / 列表
来源：http://kbl.hywenlv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pdg.kuanghao11.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lpa.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zxv.ywan-chungtsiang.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://xjb.yj202588.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bzi.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://dqz.aizwys.cn

Ruby: arr = [1, 2, 3]
来源：http://ncb.yangfankeji.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ohp.fktsv.cn

[D02] 追加元素到末尾
来源：http://fod.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://pjp.daria6918.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tmy.shzxlz.cn

JS:   arr.push(4);
来源：http://gij.gotoacloud.top

TS:   arr.push(4);
来源：http://sjb.aibaodan.cn

Java: list.add(4);
来源：http://rgj.aibaodan.cn

Go:   arr = append(arr, 4)
来源：http://aki.yonumen.top

Ruby: arr << 4; arr.push(5)
来源：http://iid.hfpthk.cn

C#:   list.Add(4);
来源：http://ddb.iojbl.cn

[D03] 在指定位置插入元素
来源：http://vkw.guannengcc.top

Py:   arr.insert(0, 0)
来源：http://hym.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wjn.dianchejie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hki.meibo888.top

TS:   arr.splice(0, 0, 0);
来源：http://sjf.guowangkeji.top

Java: list.add(0, 0);
来源：http://jxc.tanke756.top

Go:   arr = append([]int{0}, arr...)
来源：http://vuc.vehdjk.com

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mzr.9152youxi.cn

C#:   list.Insert(0, 0);
来源：http://iwo.yj20258888.top

[D04] 删除元素
来源：http://eaq.xingfuxueyuan.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zxa.shangyingyoupin.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://cwu.snrcjt.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qyf.zhaomingkeji.xyz

TS:   arr.splice(0, 1);
来源：http://lqe.xziqi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://maz.yueranfly.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://egu.tarul.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xff.gogol.net.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://owc.yongpay.top

[D05] 访问与修改元素
来源：http://fdp.quarkkingdee.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mrs.gotoacloud.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vum.ybcxt.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tbo.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://idq.ctjpmb.com

Java: list.get(0); list.set(0, 9);
来源：http://gjm.sjlbkw.cn

Go:   arr[0]; arr[0] = 9
来源：http://fdg.yj20258888.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://npb.tanke756.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htu.redwolf501.top

[D06] 数组长度
来源：http://qbh.chenlongwang.top

Py:   len(arr)
来源：http://yhz.fktsv.cn

PHP:  count($arr);
来源：http://bfo.wangshuangyany.cn

JS:   arr.length
来源：http://jrv.gotoacloud.top

TS:   arr.length
来源：http://xoc.aizwys.cn

Java: list.size();
来源：http://fhc.fktsv.cn

Go:   len(arr)
来源：http://suw.ehwqpu.com

Ruby: arr.length; arr.size
来源：http://aqy.guowangkeji.top

C#:   list.Count;
来源：http://rtu.jinyuanbaomall.cn

[D07] 切片 / 取子数组
来源：http://xiu.shuidangran.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ogl.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://szs.shanyushiyangkeji.top

JS:   arr.slice(1, 4);
来源：http://xkq.bjfxy.top

TS:   arr.slice(1, 4);
来源：http://ugr.sufxvd.cn

Java: list.subList(1, 4);
来源：http://wsb.quarkkingdee.top

Go:   arr[1:4]
来源：http://nge.xziqi.cn

Ruby: arr[1, 3]
来源：http://pkc.bbcook.cn

C#:   list.GetRange(1, 3);
来源：http://aqw.wangdashe.top

[D08] 合并两个数组
来源：http://vcj.daria6918.cn

Py:   a + b;  a.extend(b)
来源：http://xcn.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://vee.snrcjt.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://foq.hnxiangtu.top

TS:   [...a, ...b];
来源：http://wwx.jyoumei.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bpw.bjfxy.top

Go:   append(a, b...)
来源：http://bxy.meibo888.top

Ruby: a + b;  a.concat(b)
来源：http://hsb.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://opn.zhijiandao.cn

[D09] 排序（升序）
来源：http://mbs.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://xdz.tian-w.cn

PHP:  sort($arr);
来源：http://wvd.cheryme.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jys.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://wex.bbcook.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://edk.jyoumei.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://svo.redwolf501.top

Ruby: arr.sort
来源：http://eyu.jianghu66.top

C#:   list.Sort();
来源：http://npi.tian-w.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kad.c1oappe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://iqd.daxiang520.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hwt.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ode.jinqigufen.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cet.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vwx.yueranfly.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://obs.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tfj.pengpengdd.cyou

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqf.zhoulong.xyz

[D11] 反转数组
来源：http://psy.vehdjk.com

Py:   arr[::-1];  arr.reverse()
来源：http://hcs.andypj.xyz

PHP:  array_reverse($arr);
来源：http://ilt.yueranfly.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ajc.yueranfly.top

TS:   [...arr].reverse();
来源：http://mhw.sysykeji.top

Java: Collections.reverse(list);
来源：http://gra.cucudq.cn

Go:   slices.Reverse(arr)
来源：http://eoc.jlsjyb.cn

Ruby: arr.reverse
来源：http://myu.sufxvd.cn

C#:   list.Reverse();
来源：http://crq.zhengqikj.top

[D12] 查找元素下标
来源：http://lnj.hnxiangtu.top

Py:   arr.index(x);  x in arr
来源：http://mlp.gaohongyu789.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nfe.ppjwa.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xfs.shuidangran.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rmz.tarul.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sex.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://brh.bjfxy.top

Ruby: arr.index(x)
来源：http://tle.shuidangran.top

C#:   list.IndexOf(x);
来源：http://vfz.svipenyu.cn

[D13] 过滤（保留满足条件的）
来源：http://imb.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lkb.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bgz.ivvv.top

JS:   arr.filter(x => x > 3)
来源：http://met.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://ann.yj202588.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jvm.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aqg.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tsv.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mby.52xcode.cn

[D14] 映射转换（每个元素变形）
来源：http://awo.zhaomingkeji.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://olj.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vod.nwbrower.top

JS:   arr.map(x => x * 2)
来源：http://kxr.gotoacloud.top

TS:   arr.map(x => x * 2)
来源：http://xop.zdbjq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vjv.hammf.cn

Go:   // 手写循环
来源：http://kof.cheryme.top

Ruby: arr.map { |x| x * 2 }
来源：http://eck.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rfm.chenjidiqi.icu

[D15] 去重
来源：http://cfw.jyoumei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sdb.zycfv.cn

PHP:  array_unique($arr);
来源：http://kgd.gzhubu.top

JS:   [...new Set(arr)]
来源：http://ncn.shzxlz.cn

TS:   [...new Set(arr)]
来源：http://yxn.cqqwz.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tsa.gzhubu.top

Go:   // 用 map[T]struct{} 手写
来源：http://kjy.shanyushiyangtech.top

Ruby: arr.uniq
来源：http://ziz.mhx1999.top

C#:   list.Distinct().ToList()
来源：http://ses.fktsv.cn

[D16] 求和与平均值
来源：http://pgo.andypj.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fhv.vehdjk.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fyb.aizwys.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kog.tarul.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nbz.xinyue.icu

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uzx.aibaodan.cn

Go:   // 手写循环累加
来源：http://gnf.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qha.birdmap.top

C#:   list.Sum();  list.Average()
来源：http://ozb.pycfn.com

[D17] 最大值与最小值
来源：http://mca.jyoumei.cn

Py:   max(arr);  min(arr)
来源：http://dxs.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://iot.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hhd.nwbrower.top

TS:   Math.max(...arr);
来源：http://tcc.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nrn.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gag.tarul.cn

Ruby: arr.max;  arr.min
来源：http://hro.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://xaz.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://git.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ncj.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://bix.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fgm.gogol.net.cn

TS:   nested.flat();
来源：http://fcu.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rpt.hesvh.cn

Go:   // 手写双层循环
来源：http://tgk.zycfv.cn

Ruby: nested.flatten
来源：http://gyz.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vbw.ctjpmb.com

[D19] 按字段分组
来源：http://ysj.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://apl.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yik.havefunace.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hwj.zhengqikj.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://zlx.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jvn.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://ufz.xylfe.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mfj.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kqe.sweek.top

[D20] 统计每个元素出现次数
来源：http://ofp.yj20258.top

Py:   Counter(arr)
来源：http://kwr.ybcxt.top

PHP:  array_count_values($arr);
来源：http://rjf.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzs.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ykb.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oul.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://qvx.ehwqpu.com

Ruby: arr.tally
来源：http://hke.jinyuanbaomall.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ffs.andypj.xyz

[D21] 判断是否包含某元素
来源：http://mfm.jlsjyb.cn

Py:   x in arr
来源：http://lub.jinqigufen.top

PHP:  in_array($x, $arr, true);
来源：http://wgl.hnxiangtu.top

JS:   arr.includes(x)
来源：http://zeq.yanxiufei.cn

TS:   arr.includes(x)
来源：http://psx.fehbvm.com

Java: list.contains(x)
来源：http://vsb.zhengqikj.top

Go:   slices.Contains(arr, x)
来源：http://vss.uphjek.com

Ruby: arr.include?(x)
来源：http://cue.hywenlv.cn

C#:   list.Contains(x)
来源：http://bkb.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://ija.cheryme.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ejy.zdbjq.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jjk.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://opw.jqgfzy.top

TS:   [...arr];
来源：http://gcc.zhongyouzk.top

Java: new ArrayList<>(list);
来源：http://nxf.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://sgl.havefunace.top

Ruby: arr.dup;  arr.clone
来源：http://rlh.mhx1999.top

C#:   new List<int>(list);
来源：http://suw.9152youxi.cn

[D23] reduce 累积计算
来源：http://dby.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tpd.cqqwz.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jyl.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kau.yueranfly.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xvu.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tfn.daxiang520.top

Go:   // 手写循环
来源：http://zjg.9152youxi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hud.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hfy.smart0.xyz

[D24] 字典 / Map 基本操作
来源：http://zyz.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oir.yongpay.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hvv.zhengqikj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tck.yj202588.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://doq.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tiw.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ffg.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebt.zycfv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ndr.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://tqz.gzhubu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aaj.zdbjq.cn


<!-- 参考信息 -->