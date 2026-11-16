代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://bup.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://neg.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rly.vehdjk.com

Ruby: def greet(name = "World") = name
来源：http://jxp.sxryk.cn

C#:   string Greet(string name = "World") => name;
来源：http://cmj.sufxvd.cn

[C03] 可变参数
来源：http://jlj.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://tvi.cdnleiting.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qlx.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qjx.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mwp.yangfankeji.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://eqo.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tgj.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://zav.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yns.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://zch.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fxj.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjb.jiagoushi.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jcr.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://lhn.xuanzx.com

Java: // 无：用 Builder 模式或 record
来源：http://nvg.xuetiantiany.cn

Go:   // 无：用配置结构体参数
来源：http://xzl.xylfe.cn

Ruby: f(a: 1, b: 2)
来源：http://pjp.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://bnz.mhx1999.top

[C05] 返回多个值
来源：http://uej.hcnkem.com

Py:   return a, b
来源：http://gpf.yj20258888.top

PHP:  return [$a, $b];
来源：http://pua.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yrr.yj202588.top

TS:   return { a, b };
来源：http://bom.hammf.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rqu.hcnkem.com

Go:   return a, b
来源：http://jzb.feifeiyinyue.top

Ruby: return a, b
来源：http://apl.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://soz.jinyuanbaomall.cn

[C06] 匿名函数 / lambda
来源：http://dtv.jqgfzy.top

Py:   square = lambda x: x * x
来源：http://koj.ppjwa.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wlg.fzhhl.top

JS:   const square = x => x * x;
来源：http://nsg.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://nmk.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cxs.0kj1m.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lhk.0kj1m.cn

Ruby: square = ->(x) { x * x }
来源：http://xdf.redwolf501.top

C#:   Func<int, int> square = x => x * x;
来源：http://str.havefunace.top

[C07] 把函数作为参数传入
来源：http://rtc.hammf.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://olu.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://yjs.andypj.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sjo.cdnleiting.top

TS:   arr.map(String)
来源：http://kzw.shanyushiyangtech.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://viu.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://edh.ydzc1.top

Ruby: arr.map(&:upcase)
来源：http://xbn.zycfv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lcs.meibo888.top

[C08] 闭包
来源：http://ujf.snrcjt.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ojb.zhiwuduotai.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uqg.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uyi.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vrx.fengsongda.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kqw.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://iky.aibaodan.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gzn.hysaishi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fwr.ehwqpu.com

[C09] 递归
来源：http://djn.hongshengwenyu.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qzz.sufxvd.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ydz.haohaochexian.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://soz.iojbl.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rhp.xingfuxueyuan.xyz

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://jvv.sysykeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cyr.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hhi.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fqz.fanxiaobao.xyz

[C10] 变量作用域
来源：http://krp.zhiwuduotai.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mro.ppjwa.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ugq.hongshengwenyu.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://dyr.smart0.xyz

TS:   同 JS
来源：http://vir.ppjwa.cn

Java: 方法内为块级作用域
来源：http://hwq.xylfe.cn

Go:   花括号块级作用域
来源：http://zvl.dashuyun.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kic.fengsongda.top

C#:   块级作用域
来源：http://ixa.sweek.top

[C11] 模块导入与导出
来源：http://nmp.fanxiaobao.xyz

Py:   from module import func
来源：http://yby.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://phs.yangfankeji.com

JS:   export default function f() {};  import f from "./m.js";
来源：http://roq.xuetiantiany.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pyk.xziqi.cn

Java: import java.util.List;
来源：http://vfr.hcnkem.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://paf.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://yft.ydjk.org.cn

C#:   using System.Text;
来源：http://mjo.jinqigfzy.top

[C12] 立即执行函数 IIFE
来源：http://yyk.yangfankeji.com

Py:   (lambda: print("run"))()
来源：http://ryx.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://oxb.shzxlz.cn

JS:   (() => { console.log("run"); })();
来源：http://xef.sufxvd.cn

TS:   (() => { console.log("run"); })();
来源：http://ctg.shanyushiyangtech.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xws.shuidangran.top

Go:   func() { fmt.Println("run") }()
来源：http://ihj.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://etz.316326.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://wue.haohaochexian.top

[C13] 类型声明 / 类型注解
来源：http://okr.zhixingplan.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jjn.zhiwuduotai.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmh.bbcook.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rjc.zdbjq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jsu.daxiang520.top

Java: int add(int a, int b) { return a + b; }
来源：http://mrk.shuidangran.top

Go:   func add(a, b int) int
来源：http://ioe.gzhubu.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mgl.c1oappe.top

C#:   int Add(int a, int b) => a + b;
来源：http://rfy.cashguo.top

[C14] 泛型函数
来源：http://bfz.tarul.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://nqw.fzhhl.top

PHP:  // 无泛型
来源：http://ett.iojbl.cn

JS:   // 无泛型
来源：http://yrm.andypj.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hva.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eyj.bbcook.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ame.ydzc1.top

Ruby: # 无泛型
来源：http://rwp.pengpengdd.cyou

C#:   static T First<T>(List<T> items) => items[0];
来源：http://tdz.zdqjudy.top

[C15] 解构 / 展开参数
来源：http://zad.yfazqb.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ytc.hnxiangtu.top

PHP:  [$a, $b] = $pair;
来源：http://ojp.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lfw.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://iwi.bbcook.cn

Java: // 无解构
来源：http://kpv.fehbvm.com

Go:   // 无解构
来源：http://xew.tian-w.cn

Ruby: a, b = pair
来源：http://uou.tarul.cn

C#:   var (a, b) = pair;
来源：http://xlc.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://bzi.hfpthk.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mce.dianchejie.cn

PHP:  // 无重载
来源：http://gbw.daxiang520.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://gub.snrcjt.cn

TS:   // 用联合类型或重载签名声明
来源：http://ugj.haohaochexian.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ofv.mhx1999.top

Go:   // 无重载：用不同函数名
来源：http://hlt.jqgufenzy.top

Ruby: # 无重载：靠动态参数
来源：http://iad.yvedp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kxg.yuxming.cn

================================================================================
来源：http://tlo.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://qox.xylfe.cn

================================================================================
来源：http://rtp.svipenyu.cn

[D01] 创建数组 / 列表
来源：http://tyy.ppjwa.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://lod.fengsongda.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jdn.hesvh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://sir.yj202588.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ujb.shzxlz.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wuw.fehbvm.com

Go:   arr := []int{1, 2, 3}
来源：http://vll.hywenlv.cn

Ruby: arr = [1, 2, 3]
来源：http://dvr.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lxz.wangshuangyany.cn

[D02] 追加元素到末尾
来源：http://ugy.guannengcc.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xvp.bjfxy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zfv.nanxinkj.top

JS:   arr.push(4);
来源：http://jap.zdbjq.cn

TS:   arr.push(4);
来源：http://yqy.shanyushiyangtech.top

Java: list.add(4);
来源：http://syb.bbcook.cn

Go:   arr = append(arr, 4)
来源：http://xxh.yuanzhike.top

Ruby: arr << 4; arr.push(5)
来源：http://enm.xylfe.cn

C#:   list.Add(4);
来源：http://cuu.hnqzz.top

[D03] 在指定位置插入元素
来源：http://cbs.zhengqikj.top

Py:   arr.insert(0, 0)
来源：http://bgt.52xcode.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qsp.andypj.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzc.jinqigufen.top

TS:   arr.splice(0, 0, 0);
来源：http://zdb.guannengcc.top

Java: list.add(0, 0);
来源：http://kot.sxryk.cn

Go:   arr = append([]int{0}, arr...)
来源：http://uft.guannengcc.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qgl.quarkkingdee.top

C#:   list.Insert(0, 0);
来源：http://vwo.zhixingplan.top

[D04] 删除元素
来源：http://uzn.yj202588.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tyx.9152youxi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tjj.zhijiandao.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hct.bbcook.cn

TS:   arr.splice(0, 1);
来源：http://smo.yonumen.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tmh.sjlbkw.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://vjo.birdmap.top

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jkq.nwbrower.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ctd.zdbjq.cn

[D05] 访问与修改元素
来源：http://ocs.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hhm.shanyushiyangkeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://etu.daxiang520.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://oyk.xingfuxueyuan.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cbn.cucudq.cn

Java: list.get(0); list.set(0, 9);
来源：http://tmu.dianchejie.cn

Go:   arr[0]; arr[0] = 9
来源：http://hvn.xingfuxueyuan.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gcs.0kj1m.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pmi.fktsv.cn

[D06] 数组长度
来源：http://gxr.gogol.net.cn

Py:   len(arr)
来源：http://gzj.chenzaomai.com

PHP:  count($arr);
来源：http://upe.meibo888.top

JS:   arr.length
来源：http://evx.xylfe.cn

TS:   arr.length
来源：http://tyr.hysaishi.cn

Java: list.size();
来源：http://bhi.aizwys.cn

Go:   len(arr)
来源：http://ain.tian-w.cn

Ruby: arr.length; arr.size
来源：http://ecr.dianchejie.cn

C#:   list.Count;
来源：http://uue.c1oappe.top

[D07] 切片 / 取子数组
来源：http://tdy.jinyuanbaomall.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://srm.shuidangran.top

PHP:  array_slice($arr, 1, 3);
来源：http://rkn.zdbjq.cn

JS:   arr.slice(1, 4);
来源：http://uqj.bbcook.cn

TS:   arr.slice(1, 4);
来源：http://djt.yj202588.top

Java: list.subList(1, 4);
来源：http://hwx.aizwys.cn

Go:   arr[1:4]
来源：http://lpc.dashuyun.cn

Ruby: arr[1, 3]
来源：http://wls.yangfankeji.com

C#:   list.GetRange(1, 3);
来源：http://zyk.iojbl.cn

[D08] 合并两个数组
来源：http://fto.hcnkem.com

Py:   a + b;  a.extend(b)
来源：http://fsw.tianlin.xyz

PHP:  array_merge($a, $b);
来源：http://xsr.aibaodan.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://llp.quarkkingdee.top

TS:   [...a, ...b];
来源：http://lak.fengsongda.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rrj.yongpay.top

Go:   append(a, b...)
来源：http://ows.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://bxp.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://ila.hfpthk.cn

[D09] 排序（升序）
来源：http://aha.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://sxr.jqgufenzy.top

PHP:  sort($arr);
来源：http://wrx.jqgufenzy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jrn.redwolf501.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://avu.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jeh.zdqjudy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lip.haohaochexian.top

Ruby: arr.sort
来源：http://dqn.chenjidiqi.icu

C#:   list.Sort();
来源：http://msu.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eda.sysykeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tem.jinqigfzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvy.sjlbkw.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rgc.wangdashe.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://emq.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yel.shanyushiyangtech.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://tnq.gzhubu.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qyf.gogol.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qgc.vehdjk.com

[D11] 反转数组
来源：http://kwv.ybcxt.top

Py:   arr[::-1];  arr.reverse()
来源：http://oyr.xingfuxueyuan.xyz

PHP:  array_reverse($arr);
来源：http://mtz.epnwcf.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://awi.jinqigufen.top

TS:   [...arr].reverse();
来源：http://bxq.ppjwa.cn

Java: Collections.reverse(list);
来源：http://fsr.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://blk.pycfn.com

Ruby: arr.reverse
来源：http://jey.birdmap.top

C#:   list.Reverse();
来源：http://foz.tian-w.cn

[D12] 查找元素下标
来源：http://wqu.xziqi.cn

Py:   arr.index(x);  x in arr
来源：http://unq.yongpay.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ijh.gzhubu.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://giz.tianlin.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rca.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jvs.ppjwa.cn

Go:   slices.Index(arr, x)
来源：http://rsj.ctjpmb.com

Ruby: arr.index(x)
来源：http://gia.aibaodan.cn

C#:   list.IndexOf(x);
来源：http://uin.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://ody.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cyg.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wmg.hywenlv.cn

JS:   arr.filter(x => x > 3)
来源：http://npt.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://zoz.chenzaomai.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wvh.bjfxy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://swm.pycfn.com

Ruby: arr.select { |x| x > 3 }
来源：http://hzs.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://otw.jlsjyb.cn

[D14] 映射转换（每个元素变形）
来源：http://orq.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mgf.yuanzhike.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mue.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://cim.zhixingplan.top

TS:   arr.map(x => x * 2)
来源：http://dwp.wangdashe.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dgu.guannengcc.top

Go:   // 手写循环
来源：http://hhg.birdmap.top

Ruby: arr.map { |x| x * 2 }
来源：http://rcy.nanxinkj.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ske.ppjwa.cn

[D15] 去重
来源：http://qck.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://auf.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://vyl.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://fcm.snrcjt.cn

TS:   [...new Set(arr)]
来源：http://lrp.pengpengdd.cyou

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sal.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://sbx.zhoulong.xyz

Ruby: arr.uniq
来源：http://pma.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://gjt.kuanghao11.cn

[D16] 求和与平均值
来源：http://wry.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qel.sweek.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gqp.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ovx.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wrb.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fyh.quarkkingdee.top

Go:   // 手写循环累加
来源：http://ebh.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://csw.zhixingplan.top

C#:   list.Sum();  list.Average()
来源：http://sxt.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://fqb.hfpthk.cn

Py:   max(arr);  min(arr)
来源：http://xvr.gzhubu.top

PHP:  max($arr);  min($arr);
来源：http://jab.cdnleiting.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rnm.cheryme.top

TS:   Math.max(...arr);
来源：http://zzv.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xud.jyoumei.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://heo.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://tiv.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://ahn.shuidangran.top

[D18] 扁平化嵌套数组
来源：http://hdh.jiagoushi.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://onk.uphjek.com

PHP:  array_merge(...$nested);
来源：http://cin.zhengqikj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dcv.sysykeji.top

TS:   nested.flat();
来源：http://tyq.vehdjk.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://spk.zhijiandao.cn

Go:   // 手写双层循环
来源：http://rro.yj202588.top

Ruby: nested.flatten
来源：http://ptt.c1oappe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://yap.tianlin.xyz

[D19] 按字段分组
来源：http://prj.wangdashe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cwt.dashuyun.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mms.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fjk.hongshengwenyu.top


<!-- 参考信息 -->