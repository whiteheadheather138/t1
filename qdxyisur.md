代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cbo.52xcode.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rhk.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yqj.bbcook.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xuc.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cci.smart0.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tzm.9152youxi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yuj.shanyushiyangkeji.top

[C09] 递归
来源：http://gwg.hammf.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xja.zycfv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yxe.mhx1999.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nhb.cashguo.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cls.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ojq.chenzaomai.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ldd.cheryme.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gbg.zhiwuduotai.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ktj.sjlbkw.cn

[C10] 变量作用域
来源：http://fbd.xziqi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gmn.sysykeji.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kqu.cqqwz.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wjm.wangshuangyany.cn

TS:   同 JS
来源：http://jhv.ydjk.org.cn

Java: 方法内为块级作用域
来源：http://lob.zdqjudy.top

Go:   花括号块级作用域
来源：http://tgh.yueranfly.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cdc.yj20258.top

C#:   块级作用域
来源：http://vou.xylfe.cn

[C11] 模块导入与导出
来源：http://nys.sxryk.cn

Py:   from module import func
来源：http://nur.zdbjq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://odx.andypj.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://eep.feifeiyinyue.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://kpc.yfazqb.com

Java: import java.util.List;
来源：http://mxf.tarul.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kod.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://hhd.fzhhl.top

C#:   using System.Text;
来源：http://xjm.ivvv.top

[C12] 立即执行函数 IIFE
来源：http://oic.aibaodan.cn

Py:   (lambda: print("run"))()
来源：http://jlh.chenjidiqi.icu

PHP:  (function () { echo "run"; })();
来源：http://sry.birdmap.top

JS:   (() => { console.log("run"); })();
来源：http://uwk.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://jvk.shangyingyoupin.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://krr.316326.xyz

Go:   func() { fmt.Println("run") }()
来源：http://pqw.epnwcf.com

Ruby: -> { puts "run" }.call
来源：http://waj.jinghuilouyu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wwa.jinqigfzy.top

[C13] 类型声明 / 类型注解
来源：http://fym.zhiwuduotai.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://prv.tarul.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mnu.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zfj.zycfv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://crx.zhiwuduotai.top

Java: int add(int a, int b) { return a + b; }
来源：http://zab.yj20258888.top

Go:   func add(a, b int) int
来源：http://gmi.mhx1999.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wln.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://rlh.fengsongda.top

[C14] 泛型函数
来源：http://unb.fehbvm.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://kga.fengsongda.top

PHP:  // 无泛型
来源：http://ucr.gotoacloud.top

JS:   // 无泛型
来源：http://lin.zycfv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://brt.jqgufenzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cex.aibaodan.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mzu.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://dtb.shzxlz.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://web.svipenyu.cn

[C15] 解构 / 展开参数
来源：http://bgl.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://rxl.dashuyun.cn

PHP:  [$a, $b] = $pair;
来源：http://nto.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://pvp.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gps.ybcxt.top

Java: // 无解构
来源：http://uhl.yvedp.cn

Go:   // 无解构
来源：http://urx.c1oappe.top

Ruby: a, b = pair
来源：http://tgy.yfazqb.com

C#:   var (a, b) = pair;
来源：http://nyr.shangyingyoupin.top

[C16] 函数 / 方法重载
来源：http://etv.xinyue.icu

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blk.tianlin.xyz

PHP:  // 无重载
来源：http://nlc.feifeiyinyue.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpf.jiagoushi.top

TS:   // 用联合类型或重载签名声明
来源：http://rpy.havefunace.top

Java: void f(int a) {}  void f(String a) {}
来源：http://mok.hnqzz.top

Go:   // 无重载：用不同函数名
来源：http://skn.fehbvm.com

Ruby: # 无重载：靠动态参数
来源：http://qcs.0kj1m.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fxo.hesvh.cn

================================================================================
来源：http://kxo.hcnkem.com

D. 数组 / 列表 / 集合
来源：http://uwc.yj20258888.top

================================================================================
来源：http://xxt.redwolf501.top

[D01] 创建数组 / 列表
来源：http://tif.xziqi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://owu.ppjwa.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://rfk.yangfankeji.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sbf.jiagoushi.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://qxn.sxryk.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vrj.bjfxy.top

Go:   arr := []int{1, 2, 3}
来源：http://fma.zhiwuduotai.top

Ruby: arr = [1, 2, 3]
来源：http://qqe.xuanzx.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ely.zdqjudy.top

[D02] 追加元素到末尾
来源：http://exs.tarul.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mrr.yvedp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bvr.jianghu66.top

JS:   arr.push(4);
来源：http://mrr.chenjidiqi.icu

TS:   arr.push(4);
来源：http://ldm.fanxiaobao.xyz

Java: list.add(4);
来源：http://xbi.yonumen.top

Go:   arr = append(arr, 4)
来源：http://pfx.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://rre.yj20258.top

C#:   list.Add(4);
来源：http://ais.fengsongda.top

[D03] 在指定位置插入元素
来源：http://nee.shuidangran.top

Py:   arr.insert(0, 0)
来源：http://wtt.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://jmw.ywan-chungtsiang.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fkb.gogol.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://axa.sxryk.cn

Java: list.add(0, 0);
来源：http://hnx.uphjek.com

Go:   arr = append([]int{0}, arr...)
来源：http://bil.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mvl.0kj1m.cn

C#:   list.Insert(0, 0);
来源：http://gff.zycfv.cn

[D04] 删除元素
来源：http://efz.vehdjk.com

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kfv.pycfn.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iyw.yueranfly.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nby.0kj1m.cn

TS:   arr.splice(0, 1);
来源：http://yay.bbcook.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ora.tianlin.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qsv.chenzaomai.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mrn.havefunace.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://onj.aibaodan.cn

[D05] 访问与修改元素
来源：http://ejg.yj20258888.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ocx.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://oay.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jpm.xziqi.cn

TS:   arr[0]; arr.at(-1);
来源：http://jlj.ehwqpu.com

Java: list.get(0); list.set(0, 9);
来源：http://itj.epnwcf.com

Go:   arr[0]; arr[0] = 9
来源：http://srm.shanyushiyangtech.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fud.gogol.net.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sve.pycfn.com

[D06] 数组长度
来源：http://szk.iojbl.cn

Py:   len(arr)
来源：http://hou.hfpthk.cn

PHP:  count($arr);
来源：http://ibg.xingfuxueyuan.xyz

JS:   arr.length
来源：http://gdx.gzhubu.top

TS:   arr.length
来源：http://kpz.tarul.cn

Java: list.size();
来源：http://jvv.wangdashe.top

Go:   len(arr)
来源：http://xcw.pycfn.com

Ruby: arr.length; arr.size
来源：http://jcj.zdbjq.cn

C#:   list.Count;
来源：http://sok.zhongyouzk.top

[D07] 切片 / 取子数组
来源：http://jyl.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lwn.shzxlz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://slp.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://bxl.hnqzz.top

TS:   arr.slice(1, 4);
来源：http://otb.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://rtx.nanxuanxn.top

Go:   arr[1:4]
来源：http://uqo.gotoacloud.top

Ruby: arr[1, 3]
来源：http://iks.hammf.cn

C#:   list.GetRange(1, 3);
来源：http://dca.bbcook.cn

[D08] 合并两个数组
来源：http://axn.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://wxj.yuxming.cn

PHP:  array_merge($a, $b);
来源：http://spv.chenzaomai.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ilj.zhengqikj.top

TS:   [...a, ...b];
来源：http://zgu.nwbrower.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://yjd.xylfe.cn

Go:   append(a, b...)
来源：http://xap.shzxlz.cn

Ruby: a + b;  a.concat(b)
来源：http://ndc.redwolf501.top

C#:   a.Concat(b).ToList()
来源：http://giz.tarul.cn

[D09] 排序（升序）
来源：http://kar.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://grb.vehdjk.com

PHP:  sort($arr);
来源：http://cly.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://evo.epnwcf.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://rdv.nwbrower.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmf.guannengcc.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ris.sufxvd.cn

Ruby: arr.sort
来源：http://mtf.dianchejie.cn

C#:   list.Sort();
来源：http://mxb.havefunace.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://hxh.redwolf501.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ocl.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vnx.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifc.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dra.fzhhl.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bte.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://otz.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ryj.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mdz.ehwqpu.com

[D11] 反转数组
来源：http://qpx.shanyushiyangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://tlm.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://bqx.uphjek.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://awr.hfpthk.cn

TS:   [...arr].reverse();
来源：http://dnn.hcnkem.com

Java: Collections.reverse(list);
来源：http://qib.xuetiantiany.cn

Go:   slices.Reverse(arr)
来源：http://nuc.havefunace.top

Ruby: arr.reverse
来源：http://mco.ppjwa.cn

C#:   list.Reverse();
来源：http://num.316326.xyz

[D12] 查找元素下标
来源：http://yyo.nanxuanxn.top

Py:   arr.index(x);  x in arr
来源：http://sad.jinqigfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hft.haohaochexian.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zry.cqqwz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cjn.iojbl.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mkw.tanke756.top

Go:   slices.Index(arr, x)
来源：http://vtp.jyoumei.cn

Ruby: arr.index(x)
来源：http://ome.redwolf501.top

C#:   list.IndexOf(x);
来源：http://wxg.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://byv.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yxp.zhiwuduotai.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ivl.andypj.xyz

JS:   arr.filter(x => x > 3)
来源：http://rli.guannengcc.top

TS:   arr.filter(x => x > 3)
来源：http://mxa.gzhubu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jxl.sjlbkw.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vck.yj20258.top

Ruby: arr.select { |x| x > 3 }
来源：http://sue.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://qlv.jinyuanbaomall.cn

[D14] 映射转换（每个元素变形）
来源：http://gkj.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qnz.zhixingplan.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pel.gotoacloud.top

JS:   arr.map(x => x * 2)
来源：http://guy.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://wja.yuanzhike.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://gll.gaohongyu789.top

Go:   // 手写循环
来源：http://zgl.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://piw.quarkkingdee.top

C#:   list.Select(x => x * 2).ToList()
来源：http://hwc.sjlbkw.cn

[D15] 去重
来源：http://oid.nanxuanxn.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tej.nwbrower.top

PHP:  array_unique($arr);
来源：http://tej.xuanzx.com

JS:   [...new Set(arr)]
来源：http://miy.fehbvm.com

TS:   [...new Set(arr)]
来源：http://nik.yj20258.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vlz.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://vho.chenjidiqi.icu

Ruby: arr.uniq
来源：http://yhy.ctjpmb.com

C#:   list.Distinct().ToList()
来源：http://eat.cucudq.cn

[D16] 求和与平均值
来源：http://lsu.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ptz.wangshuangyany.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nzy.316326.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://esf.fzhhl.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dse.pengpengdd.cyou

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zlu.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://upb.yuanzhike.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fjg.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://hyh.daria6918.cn

[D17] 最大值与最小值
来源：http://yhd.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://rma.hcnkem.com

PHP:  max($arr);  min($arr);
来源：http://uyu.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hhi.ybcxt.top

TS:   Math.max(...arr);
来源：http://psu.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ooi.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dec.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://gdi.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://mie.yj202588.top

[D18] 扁平化嵌套数组
来源：http://nan.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ssd.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://sif.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ehi.jinqigufen.top

TS:   nested.flat();
来源：http://wls.svipenyu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ihu.redwolf501.top

Go:   // 手写双层循环
来源：http://wns.c1oappe.top

Ruby: nested.flatten
来源：http://pne.xylfe.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tsa.zhixingplan.top

[D19] 按字段分组
来源：http://krz.fanxiaobao.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zsr.pengpengdd.cyou

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://njg.fanxiaobao.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uru.tian-w.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://kpg.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ple.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://mks.ctjpmb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://gqy.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://krd.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://iqh.fzhhl.top

Py:   Counter(arr)
来源：http://zun.zycfv.cn

PHP:  array_count_values($arr);
来源：http://spj.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kcq.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rci.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vrn.xylfe.cn

Go:   // 手写 map[T]int
来源：http://nhj.316326.xyz

Ruby: arr.tally
来源：http://exb.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jpr.redwolf501.top

[D21] 判断是否包含某元素
来源：http://rjt.ybcxt.top

Py:   x in arr
来源：http://prh.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://wkm.fehbvm.com

JS:   arr.includes(x)
来源：http://ovz.tarul.cn

TS:   arr.includes(x)
来源：http://pdj.yvedp.cn

Java: list.contains(x)
来源：http://phl.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://raq.wangshuangyany.cn

Ruby: arr.include?(x)
来源：http://orw.guannengcc.top

C#:   list.Contains(x)
来源：http://yqp.cashguo.top

[D22] 复制数组（避免共享引用）
来源：http://cbe.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ajd.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xai.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vha.fzhhl.top

TS:   [...arr];
来源：http://qln.gzhubu.top

Java: new ArrayList<>(list);
来源：http://wdf.ehwqpu.com

Go:   copied := append([]int(nil), arr...)
来源：http://dkz.sjlbkw.cn

Ruby: arr.dup;  arr.clone
来源：http://vbe.chenlongwang.top

C#:   new List<int>(list);
来源：http://dwd.gaohongyu789.top

[D23] reduce 累积计算
来源：http://lex.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ijh.0kj1m.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjo.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://urv.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pow.xingfuxueyuan.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://zkk.316326.xyz

Go:   // 手写循环
来源：http://tls.yongpay.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xdk.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ral.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://psl.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nbf.sweek.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://epe.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wyt.yongpay.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gvd.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rhk.jiagoushi.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ndm.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mji.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ttk.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://icw.zycfv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nyq.havefunace.top


<!-- 参考信息 -->