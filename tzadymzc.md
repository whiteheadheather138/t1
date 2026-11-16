代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wip.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dae.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wkm.yuanzhike.top

[B04] for 计数循环
来源：http://kjk.smart0.xyz

Py:   for i in range(10): print(i)
来源：http://wee.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wpu.chenzaomai.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cjt.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sej.jqgufenzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jgy.sjlbkw.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lmb.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://esa.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rmt.tanke756.top

[B05] 遍历数组 / 列表
来源：http://vsx.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://jcq.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oja.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://vau.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://div.ppjwa.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pvv.yuxming.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://shg.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://gdo.havefunace.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://agk.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://kfo.bbcook.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://byl.zhoulong.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jbj.wangshuangyany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zcz.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txa.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ebd.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wur.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yvk.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pyn.xuanzx.com

[B07] while 循环
来源：http://djd.zhixingplan.top

Py:   while i < 10: i += 1
来源：http://ixc.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tkw.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://jwk.aizwys.cn

TS:   while (i < 10) { i++; }
来源：http://vss.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://rsw.zdqjudy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://spo.xziqi.cn

Ruby: while i < 10; i += 1; end
来源：http://ujl.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://esi.gaohongyu789.top

[B08] do-while（至少执行一次）
来源：http://oog.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://qfq.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kyd.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://ubp.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://fnn.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://ait.jinqigufen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jos.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://zxa.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://iwl.havefunace.top

[B09] break 与 continue
来源：http://lqp.jlsjyb.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://huw.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rqd.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oom.tian-w.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lsz.dianchejie.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmo.yuxming.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dut.xinyue.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://chy.sweek.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://glh.sweek.top

[B10] 遍历同时拿索引
来源：http://usa.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wow.jyoumei.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nny.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hrn.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://svk.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lcl.sweek.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://eoa.gotoacloud.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dvv.xingfuxueyuan.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vxo.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://uxh.shuidangran.top

Py:   list(range(0, 10, 2))
来源：http://eas.chenjidiqi.icu

PHP:  range(0, 10, 2);
来源：http://nrr.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://apu.chenlongwang.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjs.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://axp.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://frg.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://jzd.yangfankeji.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xti.xziqi.cn

[B12] 跳出多层循环
来源：http://cpc.hnqzz.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://btc.jqgfzy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://esa.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pjb.wangshuangyany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://exm.hfpthk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://app.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nix.shzxlz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://riw.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mik.redwolf501.top

[B13] 判断是否为数字
来源：http://sel.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://lwx.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://czo.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpt.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://clr.yanxiufei.cn

Java: x instanceof Number
来源：http://lfx.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://asc.xingfuxueyuan.xyz

Ruby: x.is_a?(Numeric)
来源：http://zak.cheryme.top

C#:   x is int or double or decimal
来源：http://ibm.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://gwo.zhiwuduotai.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://edr.yongpay.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aio.ydjk.org.cn

JS:   [1, 2, 3].includes(x)
来源：http://ktq.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://ohv.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bmw.hywenlv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rkd.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://zld.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xnl.zhijiandao.cn

[B15] 布尔运算与取反
来源：http://qaj.cucudq.cn

Py:   a and b or not c
来源：http://veb.guannengcc.top

PHP:  $a && $b || !$c
来源：http://vxr.jinqigufen.top

JS:   a && b || !c
来源：http://zsn.fengsongda.top

TS:   a && b || !c
来源：http://wvc.hcnkem.com

Java: a && b || !c
来源：http://lel.nwbrower.top

Go:   a && b || !c
来源：http://ztu.fzhhl.top

Ruby: a && b || !c
来源：http://rys.bjfxy.top

C#:   a && b || !c
来源：http://yry.jyoumei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ohj.ydzc1.top

Py:   if not data: return
来源：http://sei.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://ylu.hnxiangtu.top

JS:   if (!data) return;
来源：http://ttd.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://bsi.ydzc1.top

Java: if (data == null) return;
来源：http://fon.yuanzhike.top

Go:   if data == nil { return }
来源：http://she.sysykeji.top

Ruby: return if data.nil?
来源：http://ewp.uphjek.com

C#:   if (data == null) return;
来源：http://fks.daria6918.cn

================================================================================
来源：http://pjr.chenjidiqi.icu

C. 函数与作用域
来源：http://yrv.wangdashe.top

================================================================================
来源：http://ovl.sxryk.cn

[C01] 定义函数
来源：http://pfd.tanke756.top

Py:   def add(a, b): return a + b
来源：http://zhg.jinghuilouyu.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://unp.bbcook.cn

JS:   function add(a, b) { return a + b; }
来源：http://btn.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pjn.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uzh.meibo888.top

Go:   func add(a, b int) int { return a + b }
来源：http://bsf.aizwys.cn

Ruby: def add(a, b); a + b; end
来源：http://efi.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ttn.nanxinkj.top

[C02] 默认参数
来源：http://nwz.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://mvm.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lcq.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://bxp.gzhubu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rgb.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://zox.gaohongyu789.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pvo.yuanzhike.top

Ruby: def greet(name = "World") = name
来源：http://bcn.316326.xyz

C#:   string Greet(string name = "World") => name;
来源：http://xcb.sxryk.cn

[C03] 可变参数
来源：http://jlu.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://hec.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aiy.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpj.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kiy.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fov.iojbl.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gnf.tarul.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sxi.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kjy.guowangkeji.top

[C04] 命名参数 / 关键字参数
来源：http://edk.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://idh.zhaomingkeji.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://axz.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yej.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hmn.nanxinkj.top

Java: // 无：用 Builder 模式或 record
来源：http://wpq.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://yoz.yangfankeji.com

Ruby: f(a: 1, b: 2)
来源：http://dkz.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://owi.shzxlz.cn

[C05] 返回多个值
来源：http://rrp.jiagoushi.top

Py:   return a, b
来源：http://qtq.haohaochexian.top

PHP:  return [$a, $b];
来源：http://tcx.chenjidiqi.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://bor.jiagoushi.top

TS:   return { a, b };
来源：http://muk.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://avp.zhoulong.xyz

Go:   return a, b
来源：http://xmw.jianghu66.top

Ruby: return a, b
来源：http://ega.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://kuw.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://ezi.52xcode.cn

Py:   square = lambda x: x * x
来源：http://mxk.zhijiandao.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mfn.dashuyun.cn

JS:   const square = x => x * x;
来源：http://gay.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://lzs.xuanzx.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tlt.tianlin.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://fhf.9152youxi.cn

Ruby: square = ->(x) { x * x }
来源：http://mxj.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://hbp.nwbrower.top

[C07] 把函数作为参数传入
来源：http://xwp.ehwqpu.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pwa.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://uud.chenlongwang.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cpv.vehdjk.com

TS:   arr.map(String)
来源：http://kgl.meibo888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://joz.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xuq.svipenyu.cn

Ruby: arr.map(&:upcase)
来源：http://bcy.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://thy.yuanzhike.top

[C08] 闭包
来源：http://bux.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hxk.c1oappe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yom.jianghu66.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://clt.kuanghao11.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gad.uphjek.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bqq.ybcxt.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vbu.hnxiangtu.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cui.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yvx.ctjpmb.com

[C09] 递归
来源：http://jks.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://jbo.hywenlv.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://axs.bbcook.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zba.hcnkem.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ttg.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://pwl.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://uyg.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://sqf.nwbrower.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uwb.aibaodan.cn

[C10] 变量作用域
来源：http://sru.hywenlv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ghh.zhaomingkeji.xyz

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mxd.gogol.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://kbo.nwbrower.top

TS:   同 JS
来源：http://fzf.yongpay.top

Java: 方法内为块级作用域
来源：http://bgy.nanxuanxn.top

Go:   花括号块级作用域
来源：http://nuj.andypj.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hre.gzhubu.top

C#:   块级作用域
来源：http://nrg.dashuyun.cn

[C11] 模块导入与导出
来源：http://flx.hysaishi.cn

Py:   from module import func
来源：http://vdr.daria6918.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://fty.hesvh.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://toq.chenlongwang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yro.ctjpmb.com

Java: import java.util.List;
来源：http://ylg.jinqigfzy.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gdj.cucudq.cn

Ruby: require "json"; require_relative "./util"
来源：http://gpv.sysykeji.top

C#:   using System.Text;
来源：http://tol.yuanzhike.top

[C12] 立即执行函数 IIFE
来源：http://tlk.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://poj.zhengqikj.top

PHP:  (function () { echo "run"; })();
来源：http://rcq.svipenyu.cn

JS:   (() => { console.log("run"); })();
来源：http://nae.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://ulg.yangfankeji.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ede.zhiwuduotai.top

Go:   func() { fmt.Println("run") }()
来源：http://xan.sweek.top

Ruby: -> { puts "run" }.call
来源：http://qif.redwolf501.top

C#:   // 无 IIFE：用静态构造函数
来源：http://plb.gzhubu.top

[C13] 类型声明 / 类型注解
来源：http://til.tianlin.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wmh.c1oappe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckm.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ppw.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://flv.hysaishi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wwq.fzhhl.top

Go:   func add(a, b int) int
来源：http://icz.gotoacloud.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jqn.ybcxt.top

C#:   int Add(int a, int b) => a + b;
来源：http://tby.jlsjyb.cn

[C14] 泛型函数
来源：http://ngd.cdnleiting.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hff.shuidangran.top

PHP:  // 无泛型
来源：http://irz.ivvv.top

JS:   // 无泛型
来源：http://svb.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gcl.ybcxt.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://veu.shanyushiyangtech.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lyj.jqgufenzy.top

Ruby: # 无泛型
来源：http://toh.cheryme.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://htd.zhiwuduotai.top

[C15] 解构 / 展开参数
来源：http://nhz.nwbrower.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xch.sufxvd.cn

PHP:  [$a, $b] = $pair;
来源：http://yuy.daria6918.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rjl.jqgufenzy.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ftk.tanke756.top

Java: // 无解构
来源：http://onu.mhx1999.top

Go:   // 无解构
来源：http://eln.0kj1m.cn

Ruby: a, b = pair
来源：http://mpw.guowangkeji.top

C#:   var (a, b) = pair;
来源：http://ccw.wangdashe.top

[C16] 函数 / 方法重载
来源：http://syw.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nze.quarkkingdee.top

PHP:  // 无重载
来源：http://osx.fanxiaobao.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://npf.feifeiyinyue.top

TS:   // 用联合类型或重载签名声明
来源：http://mmn.pycfn.com

Java: void f(int a) {}  void f(String a) {}
来源：http://xsv.jyoumei.cn

Go:   // 无重载：用不同函数名
来源：http://eio.yj202588.top

Ruby: # 无重载：靠动态参数
来源：http://req.vqdsnc.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kzo.jyoumei.cn

================================================================================
来源：http://ani.daria6918.cn

D. 数组 / 列表 / 集合
来源：http://qqq.bbcook.cn

================================================================================
来源：http://hza.jinghuilouyu.cn

[D01] 创建数组 / 列表
来源：http://nby.svipenyu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ock.sufxvd.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://svz.guannengcc.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wxy.quarkkingdee.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ltd.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://awh.hongshengwenyu.top

Go:   arr := []int{1, 2, 3}
来源：http://piz.gaohongyu789.top

Ruby: arr = [1, 2, 3]
来源：http://zwe.haohaochexian.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ppl.mhx1999.top

[D02] 追加元素到末尾
来源：http://xfu.zhijiandao.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sva.yonumen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ohs.mhx1999.top

JS:   arr.push(4);
来源：http://epm.haohaochexian.top

TS:   arr.push(4);
来源：http://uxk.svipenyu.cn

Java: list.add(4);
来源：http://zjv.xingfuxueyuan.xyz

Go:   arr = append(arr, 4)
来源：http://tem.shuidangran.top

Ruby: arr << 4; arr.push(5)
来源：http://feb.zhoulong.xyz

C#:   list.Add(4);
来源：http://fdf.quarkkingdee.top

[D03] 在指定位置插入元素
来源：http://sln.yanxiufei.cn

Py:   arr.insert(0, 0)
来源：http://bjl.fehbvm.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ioz.hnxiangtu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jgo.cheryme.top

TS:   arr.splice(0, 0, 0);
来源：http://gub.bbcook.cn

Java: list.add(0, 0);
来源：http://awt.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://xzj.jqgufenzy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qum.uphjek.com

C#:   list.Insert(0, 0);
来源：http://vis.uphjek.com

[D04] 删除元素
来源：http://fok.pengpengdd.cyou

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://uaw.chenzaomai.com

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jow.shzxlz.cn


<!-- 参考信息 -->