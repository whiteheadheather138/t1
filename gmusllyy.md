代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cxo.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://geo.hywenlv.cn

[B07] while 循环
来源：http://xja.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://vsq.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://xus.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://rob.fanxiaobao.xyz

TS:   while (i < 10) { i++; }
来源：http://dbo.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://hgr.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zlp.hnqzz.top

Ruby: while i < 10; i += 1; end
来源：http://eqw.haohaochexian.top

C#:   while (i < 10) { i++; }
来源：http://dah.jqgfzy.top

[B08] do-while（至少执行一次）
来源：http://fhc.gaohongyu789.top

Py:   # 无 do-while：用 while True + break
来源：http://wfj.ydjk.org.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zzk.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://zvv.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://oau.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://kru.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://oau.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://lqe.yanxiufei.cn

C#:   do { i++; } while (i < 10);
来源：http://ure.zdqjudy.top

[B09] break 与 continue
来源：http://xzw.jqgufenzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bwz.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://chc.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fyx.ctjpmb.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cej.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sms.zhengqikj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gnf.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pof.iojbl.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ajv.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://muc.hammf.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lkl.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://byv.fktsv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://djq.shangyingyoupin.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qdv.c1oappe.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bgf.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ccn.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kps.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://die.ybcxt.top

[B11] 生成数字序列 / 区间
来源：http://mlu.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://kmd.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://arz.gzhubu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pgs.yfazqb.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ozc.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ihb.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kql.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://gjv.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sgu.316326.xyz

[B12] 跳出多层循环
来源：http://crp.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://otm.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tev.hywenlv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://noc.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://khp.9152youxi.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://woi.meibo888.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yjl.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yrl.guowangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xjc.hcnkem.com

[B13] 判断是否为数字
来源：http://ohd.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://vao.iojbl.cn

PHP:  is_numeric($x)
来源：http://wcm.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qaw.fktsv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iml.jqgufenzy.top

Java: x instanceof Number
来源：http://fbv.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://byb.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://qwf.daria6918.cn

C#:   x is int or double or decimal
来源：http://nsx.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://hml.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mun.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hwx.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://byy.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://cef.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://nds.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wig.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://abw.svipenyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tsu.guannengcc.top

[B15] 布尔运算与取反
来源：http://oqj.mhx1999.top

Py:   a and b or not c
来源：http://ppw.uphjek.com

PHP:  $a && $b || !$c
来源：http://oin.ywan-chungtsiang.top

JS:   a && b || !c
来源：http://sal.ctjpmb.com

TS:   a && b || !c
来源：http://cny.yj20258888.top

Java: a && b || !c
来源：http://nlp.wangshuangyany.cn

Go:   a && b || !c
来源：http://gaf.tian-w.cn

Ruby: a && b || !c
来源：http://gcb.yanxiufei.cn

C#:   a && b || !c
来源：http://cla.guowangkeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://yrr.gogol.net.cn

Py:   if not data: return
来源：http://hkm.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://cwy.ivvv.top

JS:   if (!data) return;
来源：http://afn.tanke756.top

TS:   if (!data) return;
来源：http://orv.xuetiantiany.cn

Java: if (data == null) return;
来源：http://onn.bbcook.cn

Go:   if data == nil { return }
来源：http://nkl.hammf.cn

Ruby: return if data.nil?
来源：http://fez.nanxuanxn.top

C#:   if (data == null) return;
来源：http://ono.c1oappe.top

================================================================================
来源：http://iwb.havefunace.top

C. 函数与作用域
来源：http://may.xziqi.cn

================================================================================
来源：http://wqb.9152youxi.cn

[C01] 定义函数
来源：http://rps.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://qax.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mer.yuanzhike.top

JS:   function add(a, b) { return a + b; }
来源：http://mpb.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jey.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nlg.sufxvd.cn

Go:   func add(a, b int) int { return a + b }
来源：http://egb.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://acx.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bjl.cheryme.top

[C02] 默认参数
来源：http://iwi.xuetiantiany.cn

Py:   def greet(name="World"): return name
来源：http://jpa.tianlin.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://inq.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://nbf.feifeiyinyue.top

TS:   function greet(name: string = "World") { return name; }
来源：http://khz.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://keg.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zsl.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://qcf.dashuyun.cn

C#:   string Greet(string name = "World") => name;
来源：http://svh.uphjek.com

[C03] 可变参数
来源：http://cfz.zhaomingkeji.xyz

Py:   def total(*args): return sum(args)
来源：http://lrp.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://prg.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxp.hongshengwenyu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://skt.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qbr.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yjd.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://jvw.zhijiandao.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://cgy.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://smd.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nvc.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eab.ydzc1.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://osb.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hwd.hnxiangtu.top

Java: // 无：用 Builder 模式或 record
来源：http://ngn.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://zzo.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://tmz.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://hpm.bbcook.cn

[C05] 返回多个值
来源：http://qcj.ybcxt.top

Py:   return a, b
来源：http://lfu.sufxvd.cn

PHP:  return [$a, $b];
来源：http://kwb.yongpay.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://esz.yj20258.top

TS:   return { a, b };
来源：http://gai.yuanzhike.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pcn.iojbl.cn

Go:   return a, b
来源：http://gie.svipenyu.cn

Ruby: return a, b
来源：http://ysg.zhiwuduotai.top

C#:   return (a, b);              // ValueTuple
来源：http://bxq.ywan-chungtsiang.top

[C06] 匿名函数 / lambda
来源：http://kla.zycfv.cn

Py:   square = lambda x: x * x
来源：http://jcv.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fyr.nwbrower.top

JS:   const square = x => x * x;
来源：http://dqh.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://cgf.jinqigfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lfr.ydzc1.top

Go:   sq := func(x int) int { return x * x }
来源：http://bom.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://jek.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://fna.chenlongwang.top

[C07] 把函数作为参数传入
来源：http://seb.jqgufenzy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://avd.jinqigufen.top

PHP:  array_map("strtoupper", $arr);
来源：http://nxy.hnxiangtu.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ogn.c1oappe.top

TS:   arr.map(String)
来源：http://yrm.zhoulong.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://umm.xinyue.icu

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ozj.hysaishi.cn

Ruby: arr.map(&:upcase)
来源：http://lhf.svipenyu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://llv.jinyuanbaomall.cn

[C08] 闭包
来源：http://ydf.shangyingyoupin.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kpq.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zcs.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wqb.pycfn.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://esm.316326.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qsk.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://brd.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gxm.52xcode.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://gas.jinyuanbaomall.cn

[C09] 递归
来源：http://pex.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hsx.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wfp.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rtr.fktsv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tke.dashuyun.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gac.xylfe.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fpj.jqgufenzy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://meb.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://iuw.daxiang520.top

[C10] 变量作用域
来源：http://xfg.jinyuanbaomall.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xhu.yangfankeji.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jcv.havefunace.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cul.shuidangran.top

TS:   同 JS
来源：http://eha.yuxming.cn

Java: 方法内为块级作用域
来源：http://vzb.zhengqikj.top

Go:   花括号块级作用域
来源：http://upf.wangshuangyany.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cqc.0kj1m.cn

C#:   块级作用域
来源：http://fgx.shanyushiyangkeji.top

[C11] 模块导入与导出
来源：http://wfs.zhengqikj.top

Py:   from module import func
来源：http://nqy.fktsv.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://pdu.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://jcv.aibaodan.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://gks.ppjwa.cn

Java: import java.util.List;
来源：http://trc.gaohongyu789.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lrs.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://bcs.tarul.cn

C#:   using System.Text;
来源：http://ghh.sweek.top

[C12] 立即执行函数 IIFE
来源：http://yei.hnxiangtu.top

Py:   (lambda: print("run"))()
来源：http://bgb.tian-w.cn

PHP:  (function () { echo "run"; })();
来源：http://xnh.gogol.net.cn

JS:   (() => { console.log("run"); })();
来源：http://cbb.cashguo.top

TS:   (() => { console.log("run"); })();
来源：http://zkl.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://flb.hysaishi.cn

Go:   func() { fmt.Println("run") }()
来源：http://djo.zhengqikj.top

Ruby: -> { puts "run" }.call
来源：http://oeu.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://nch.52xcode.cn

[C13] 类型声明 / 类型注解
来源：http://scx.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://atl.0kj1m.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://esd.ybcxt.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tys.ivvv.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tdj.cdnleiting.top

Java: int add(int a, int b) { return a + b; }
来源：http://flk.daxiang520.top

Go:   func add(a, b int) int
来源：http://ies.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xny.yuanzhike.top

C#:   int Add(int a, int b) => a + b;
来源：http://ycp.ctjpmb.com

[C14] 泛型函数
来源：http://dfr.hongshengwenyu.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zos.jianghu66.top

PHP:  // 无泛型
来源：http://sfx.hesvh.cn

JS:   // 无泛型
来源：http://frz.chenzaomai.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oyg.dianchejie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dqn.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fnn.jinyuanbaomall.cn

Ruby: # 无泛型
来源：http://axb.quarkkingdee.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://nxi.hcnkem.com

[C15] 解构 / 展开参数
来源：http://ahg.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qxs.uphjek.com

PHP:  [$a, $b] = $pair;
来源：http://fkr.shuidangran.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xiq.xingfuxueyuan.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://koz.gzhubu.top

Java: // 无解构
来源：http://jkf.hysaishi.cn

Go:   // 无解构
来源：http://cyx.gaohongyu789.top

Ruby: a, b = pair
来源：http://oiq.yangfankeji.com

C#:   var (a, b) = pair;
来源：http://xnk.ybcxt.top

[C16] 函数 / 方法重载
来源：http://gev.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wlk.ywan-chungtsiang.top

PHP:  // 无重载
来源：http://xrh.hcnkem.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://xvp.ehwqpu.com

TS:   // 用联合类型或重载签名声明
来源：http://rjk.redwolf501.top

Java: void f(int a) {}  void f(String a) {}
来源：http://taa.zdbjq.cn

Go:   // 无重载：用不同函数名
来源：http://ifw.aibaodan.cn

Ruby: # 无重载：靠动态参数
来源：http://pmm.sjlbkw.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ixn.9152youxi.cn

================================================================================
来源：http://jgb.svipenyu.cn

D. 数组 / 列表 / 集合
来源：http://fdv.ivvv.top

================================================================================
来源：http://kvg.daria6918.cn

[D01] 创建数组 / 列表
来源：http://htf.sxryk.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://wfx.gzhubu.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xbf.hnqzz.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bdp.wangdashe.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ojo.jinyuanbaomall.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wse.guowangkeji.top

Go:   arr := []int{1, 2, 3}
来源：http://jkq.shzxlz.cn

Ruby: arr = [1, 2, 3]
来源：http://mtr.cheryme.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xbs.dianchejie.cn

[D02] 追加元素到末尾
来源：http://scl.jqgufenzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aer.ppjwa.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zkh.yueranfly.top

JS:   arr.push(4);
来源：http://osd.snrcjt.cn

TS:   arr.push(4);
来源：http://oiu.sxryk.cn

Java: list.add(4);
来源：http://ntz.nanxinkj.top

Go:   arr = append(arr, 4)
来源：http://nbk.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://zrs.nwbrower.top

C#:   list.Add(4);
来源：http://rot.aibaodan.cn

[D03] 在指定位置插入元素
来源：http://nkt.pycfn.com

Py:   arr.insert(0, 0)
来源：http://fim.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://atc.nwbrower.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://usy.epnwcf.com

TS:   arr.splice(0, 0, 0);
来源：http://gik.snrcjt.cn

Java: list.add(0, 0);
来源：http://cpm.hammf.cn

Go:   arr = append([]int{0}, arr...)
来源：http://dzz.fktsv.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://fhz.vqdsnc.cn

C#:   list.Insert(0, 0);
来源：http://ycu.yuxming.cn

[D04] 删除元素
来源：http://kux.hfpthk.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tzx.sysykeji.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mky.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ibf.jlsjyb.cn

TS:   arr.splice(0, 1);
来源：http://mfy.yueranfly.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://vvx.mhx1999.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://tth.pengpengdd.cyou

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uzq.aibaodan.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jty.epnwcf.com

[D05] 访问与修改元素
来源：http://lwe.guowangkeji.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://afj.xingfuxueyuan.xyz

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://jnz.xuanzx.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://znt.redwolf501.top

TS:   arr[0]; arr.at(-1);
来源：http://hyx.guannengcc.top

Java: list.get(0); list.set(0, 9);
来源：http://ufc.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://plh.svipenyu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jqu.quarkkingdee.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mcw.wangshuangyany.cn

[D06] 数组长度
来源：http://vdi.jinghuilouyu.cn

Py:   len(arr)
来源：http://zgt.fehbvm.com

PHP:  count($arr);
来源：http://pno.yuanzhike.top

JS:   arr.length
来源：http://dwc.jqgufenzy.top

TS:   arr.length
来源：http://lun.kuanghao11.cn

Java: list.size();
来源：http://cti.hysaishi.cn

Go:   len(arr)
来源：http://nzb.sufxvd.cn

Ruby: arr.length; arr.size
来源：http://cnp.ehwqpu.com

C#:   list.Count;
来源：http://ukm.jqgfzy.top

[D07] 切片 / 取子数组
来源：http://deq.sxryk.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kxh.tanke756.top

PHP:  array_slice($arr, 1, 3);
来源：http://seu.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://cjt.zhoulong.xyz


<!-- 参考信息 -->