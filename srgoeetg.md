代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://djr.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aju.zhongyouzk.top

[B07] while 循环
来源：http://kwd.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://ghn.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://wjr.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://fds.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://tke.hywenlv.cn

Java: while (i < 10) { i++; }
来源：http://alj.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wxh.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://lrf.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://eiy.vehdjk.com

[B08] do-while（至少执行一次）
来源：http://vtf.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ffi.gzhubu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ltn.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://ypu.jianghu66.top

TS:   do { i++; } while (i < 10);
来源：http://agr.ppjwa.cn

Java: do { i++; } while (i < 10);
来源：http://icl.jinghuilouyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://uxw.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://ryn.zhoulong.xyz

C#:   do { i++; } while (i < 10);
来源：http://tlj.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://tui.hammf.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mcl.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tke.jlsjyb.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kro.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvt.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfz.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dpg.guowangkeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sww.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upr.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://zce.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zru.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pdz.ydjk.org.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xtc.cdnleiting.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://krp.ywan-chungtsiang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mau.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sir.shanyushiyangtech.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mrr.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sme.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://rin.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://lgs.xuanzx.com

PHP:  range(0, 10, 2);
来源：http://yqy.jianghu66.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tak.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://azg.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gzr.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wut.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://rxt.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ifp.uphjek.com

[B12] 跳出多层循环
来源：http://zzd.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jpw.zdqjudy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mzg.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://row.shuidangran.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrl.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xpb.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://aju.yonumen.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zzx.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jfc.nwbrower.top

[B13] 判断是否为数字
来源：http://jqs.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://uxs.xylfe.cn

PHP:  is_numeric($x)
来源：http://mhz.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgm.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fud.xziqi.cn

Java: x instanceof Number
来源：http://tzd.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dxx.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://nvj.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://kxz.wangdashe.top

[B14] 判断值是否在集合内
来源：http://oce.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zdt.zhaomingkeji.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ozy.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://yxm.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://llp.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nbz.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yni.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://isq.jlsjyb.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jlz.uphjek.com

[B15] 布尔运算与取反
来源：http://dct.chenjidiqi.icu

Py:   a and b or not c
来源：http://khb.yj20258.top

PHP:  $a && $b || !$c
来源：http://mps.tarul.cn

JS:   a && b || !c
来源：http://vqy.jiagoushi.top

TS:   a && b || !c
来源：http://bov.ehwqpu.com

Java: a && b || !c
来源：http://dek.daria6918.cn

Go:   a && b || !c
来源：http://qia.meibo888.top

Ruby: a && b || !c
来源：http://inj.sweek.top

C#:   a && b || !c
来源：http://ozf.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://ysg.guowangkeji.top

Py:   if not data: return
来源：http://qkn.cucudq.cn

PHP:  if (!$data) { return; }
来源：http://bdv.epnwcf.com

JS:   if (!data) return;
来源：http://wrr.yangfankeji.com

TS:   if (!data) return;
来源：http://yyg.havefunace.top

Java: if (data == null) return;
来源：http://hyk.aibaodan.cn

Go:   if data == nil { return }
来源：http://esv.gaohongyu789.top

Ruby: return if data.nil?
来源：http://hiw.hnxiangtu.top

C#:   if (data == null) return;
来源：http://kvi.yongpay.top

================================================================================
来源：http://nxx.feifeiyinyue.top

C. 函数与作用域
来源：http://ozw.gogol.net.cn

================================================================================
来源：http://bjw.tianlin.xyz

[C01] 定义函数
来源：http://kho.birdmap.top

Py:   def add(a, b): return a + b
来源：http://bhw.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vjv.mhx1999.top

JS:   function add(a, b) { return a + b; }
来源：http://pmo.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uxz.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://zmz.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://qrk.ydzc1.top

Ruby: def add(a, b); a + b; end
来源：http://uta.hammf.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://frk.tanke756.top

[C02] 默认参数
来源：http://adl.havefunace.top

Py:   def greet(name="World"): return name
来源：http://gbc.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ojk.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://jta.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ntc.xuetiantiany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sof.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cfw.sweek.top

Ruby: def greet(name = "World") = name
来源：http://ibm.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://usi.hfpthk.cn

[C03] 可变参数
来源：http://zhv.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://gbh.jiagoushi.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://maw.pycfn.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mzt.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://woi.ivvv.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://uvm.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dss.hcnkem.com

Ruby: def total(*nums); nums.sum; end
来源：http://yut.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://asg.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://tqt.chenzaomai.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wlt.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ytf.xuetiantiany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vfh.jqgfzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbp.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://tzg.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://nhr.gotoacloud.top

Ruby: f(a: 1, b: 2)
来源：http://ona.cqqwz.cn

C#:   f(a: 1, b: 2)
来源：http://eve.ydzc1.top

[C05] 返回多个值
来源：http://lps.snrcjt.cn

Py:   return a, b
来源：http://wbr.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://zfs.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cbm.yj20258888.top

TS:   return { a, b };
来源：http://oiu.hywenlv.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tti.jinyuanbaomall.cn

Go:   return a, b
来源：http://jsp.yj20258.top

Ruby: return a, b
来源：http://ewf.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://ogo.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://ntv.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://fmx.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://rzj.ctjpmb.com

JS:   const square = x => x * x;
来源：http://mig.bbcook.cn

TS:   const square = (x: number): number => x * x;
来源：http://fgy.wangdashe.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yal.zycfv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pmp.andypj.xyz

Ruby: square = ->(x) { x * x }
来源：http://yac.bjfxy.top

C#:   Func<int, int> square = x => x * x;
来源：http://qfi.yvedp.cn

[C07] 把函数作为参数传入
来源：http://vyp.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qzi.ydzc1.top

PHP:  array_map("strtoupper", $arr);
来源：http://xui.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kai.c1oappe.top

TS:   arr.map(String)
来源：http://ecg.svipenyu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ihx.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ewb.xinyue.icu

Ruby: arr.map(&:upcase)
来源：http://rhl.daxiang520.top

C#:   arr.Select(s => s.ToUpper())
来源：http://cov.ywan-chungtsiang.top

[C08] 闭包
来源：http://agz.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jvy.hesvh.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kkd.uphjek.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mgd.chenjidiqi.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dla.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://czd.gotoacloud.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://tcx.nwbrower.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lxu.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pqm.yvedp.cn

[C09] 递归
来源：http://ijo.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://agm.hesvh.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://xxf.ppjwa.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://laz.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pdb.yfazqb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xwm.fehbvm.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://tua.yfazqb.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xog.havefunace.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://trt.gaohongyu789.top

[C10] 变量作用域
来源：http://agw.vehdjk.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lae.yanxiufei.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xyw.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cgy.hesvh.cn

TS:   同 JS
来源：http://anf.fzhhl.top

Java: 方法内为块级作用域
来源：http://rgl.nanxinkj.top

Go:   花括号块级作用域
来源：http://igj.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dok.zhaomingkeji.xyz

C#:   块级作用域
来源：http://fkb.hysaishi.cn

[C11] 模块导入与导出
来源：http://xqi.uphjek.com

Py:   from module import func
来源：http://blt.vqdsnc.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://gbi.gotoacloud.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kef.yj20258.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ora.yanxiufei.cn

Java: import java.util.List;
来源：http://rvj.jqgfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xox.yj20258.top

Ruby: require "json"; require_relative "./util"
来源：http://cxa.ppjwa.cn

C#:   using System.Text;
来源：http://sca.feifeiyinyue.top

[C12] 立即执行函数 IIFE
来源：http://aoa.cucudq.cn

Py:   (lambda: print("run"))()
来源：http://ihf.hcnkem.com

PHP:  (function () { echo "run"; })();
来源：http://ogw.cucudq.cn

JS:   (() => { console.log("run"); })();
来源：http://mpv.hcnkem.com

TS:   (() => { console.log("run"); })();
来源：http://obk.jqgufenzy.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qyj.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://whf.yongpay.top

Ruby: -> { puts "run" }.call
来源：http://gab.fehbvm.com

C#:   // 无 IIFE：用静态构造函数
来源：http://tjd.tanke756.top

[C13] 类型声明 / 类型注解
来源：http://vhr.yueranfly.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hpn.9152youxi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kga.jiagoushi.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cnn.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oue.hnqzz.top

Java: int add(int a, int b) { return a + b; }
来源：http://zed.hfpthk.cn

Go:   func add(a, b int) int
来源：http://edz.jinghuilouyu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://udv.epnwcf.com

C#:   int Add(int a, int b) => a + b;
来源：http://oun.yueranfly.top

[C14] 泛型函数
来源：http://sfq.ydzc1.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hgo.zhoulong.xyz

PHP:  // 无泛型
来源：http://mmq.hnqzz.top

JS:   // 无泛型
来源：http://ppa.mhx1999.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gip.jinghuilouyu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zwn.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://zwb.pycfn.com

Ruby: # 无泛型
来源：http://wme.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gtv.guannengcc.top

[C15] 解构 / 展开参数
来源：http://rpq.cashguo.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fdc.haohaochexian.top

PHP:  [$a, $b] = $pair;
来源：http://ctl.ydzc1.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xhy.jqgfzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://giq.tarul.cn

Java: // 无解构
来源：http://zdc.cdnleiting.top

Go:   // 无解构
来源：http://meo.yuxming.cn

Ruby: a, b = pair
来源：http://ygg.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://bcm.jiagoushi.top

[C16] 函数 / 方法重载
来源：http://kmb.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://bwf.nanxinkj.top

PHP:  // 无重载
来源：http://rfb.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://bpm.xuanzx.com

TS:   // 用联合类型或重载签名声明
来源：http://uvr.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://eba.guannengcc.top

Go:   // 无重载：用不同函数名
来源：http://udt.xuanzx.com

Ruby: # 无重载：靠动态参数
来源：http://sza.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zpy.jqgufenzy.top

================================================================================
来源：http://ssq.nwbrower.top

D. 数组 / 列表 / 集合
来源：http://kpj.hfpthk.cn

================================================================================
来源：http://igk.hammf.cn

[D01] 创建数组 / 列表
来源：http://isd.bjfxy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://afy.vqdsnc.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xga.sysykeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ugp.yvedp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bwt.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vth.fktsv.cn

Go:   arr := []int{1, 2, 3}
来源：http://uuz.yangfankeji.com

Ruby: arr = [1, 2, 3]
来源：http://frb.316326.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://zyq.ywan-chungtsiang.top

[D02] 追加元素到末尾
来源：http://bfi.gotoacloud.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dam.nanxinkj.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tbf.jinqigfzy.top

JS:   arr.push(4);
来源：http://ksd.jqgufenzy.top

TS:   arr.push(4);
来源：http://ndw.hnxiangtu.top

Java: list.add(4);
来源：http://xnn.dashuyun.cn

Go:   arr = append(arr, 4)
来源：http://zls.xuanzx.com

Ruby: arr << 4; arr.push(5)
来源：http://olq.havefunace.top

C#:   list.Add(4);
来源：http://glu.yuxming.cn

[D03] 在指定位置插入元素
来源：http://qqq.hywenlv.cn

Py:   arr.insert(0, 0)
来源：http://pbr.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wkf.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zfs.xingfuxueyuan.xyz

TS:   arr.splice(0, 0, 0);
来源：http://boi.gzhubu.top

Java: list.add(0, 0);
来源：http://wgn.zdbjq.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ejo.aizwys.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nxw.yueranfly.top

C#:   list.Insert(0, 0);
来源：http://wsn.ctjpmb.com

[D04] 删除元素
来源：http://uva.smart0.xyz

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bgp.gogol.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bfa.yj202588.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://grq.hnqzz.top

TS:   arr.splice(0, 1);
来源：http://obc.havefunace.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://atx.bjfxy.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mdk.yfazqb.com

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sfa.sjlbkw.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://gfr.ywan-chungtsiang.top

[D05] 访问与修改元素
来源：http://bdv.ybcxt.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://spf.aizwys.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://buo.hnqzz.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yql.dianchejie.cn

TS:   arr[0]; arr.at(-1);
来源：http://qjd.nanxinkj.top

Java: list.get(0); list.set(0, 9);
来源：http://onv.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://uwm.redwolf501.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ook.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pry.nanxuanxn.top

[D06] 数组长度
来源：http://ezk.sjlbkw.cn

Py:   len(arr)
来源：http://chx.daxiang520.top

PHP:  count($arr);
来源：http://ibu.fanxiaobao.xyz

JS:   arr.length
来源：http://qjx.hnxiangtu.top

TS:   arr.length
来源：http://cjn.xziqi.cn

Java: list.size();
来源：http://vov.tian-w.cn

Go:   len(arr)
来源：http://jgp.xylfe.cn

Ruby: arr.length; arr.size
来源：http://jsw.ydjk.org.cn

C#:   list.Count;
来源：http://siw.tianlin.xyz

[D07] 切片 / 取子数组
来源：http://bbh.redwolf501.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gxl.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://bhk.andypj.xyz

JS:   arr.slice(1, 4);
来源：http://rhu.shanyushiyangtech.top


<!-- 参考信息 -->