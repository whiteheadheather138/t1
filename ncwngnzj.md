代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://sri.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ixa.gzhubu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecu.haohaochexian.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yun.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zgi.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://say.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://con.chenlongwang.top

[B04] for 计数循环
来源：http://cew.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://hxh.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vpq.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dyq.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gnu.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://exw.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fxq.ctjpmb.com

Ruby: 10.times { |i| puts i }
来源：http://jvb.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://czq.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://ysn.hammf.cn

Py:   for item in arr: print(item)
来源：http://ccd.hfpthk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gdq.birdmap.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mqv.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mwr.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://tca.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pwa.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://kyb.iojbl.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ftp.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://byl.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://awf.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kbr.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ogu.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yrz.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ohc.fengsongda.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dpl.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nck.smart0.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://win.haohaochexian.top

[B07] while 循环
来源：http://rmd.vehdjk.com

Py:   while i < 10: i += 1
来源：http://ctk.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://ttx.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://ijp.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://omg.hammf.cn

Java: while (i < 10) { i++; }
来源：http://pue.cashguo.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://oqu.haohaochexian.top

Ruby: while i < 10; i += 1; end
来源：http://tai.wangshuangyany.cn

C#:   while (i < 10) { i++; }
来源：http://tmu.yj20258888.top

[B08] do-while（至少执行一次）
来源：http://nkt.uphjek.com

Py:   # 无 do-while：用 while True + break
来源：http://bsr.sjlbkw.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://olr.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://liy.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://sed.tanke756.top

Java: do { i++; } while (i < 10);
来源：http://ujs.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://khg.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://aqi.uphjek.com

C#:   do { i++; } while (i < 10);
来源：http://xyv.ctjpmb.com

[B09] break 与 continue
来源：http://btc.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dvv.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fwd.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyi.zdqjudy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqb.guannengcc.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oec.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fvr.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ind.hysaishi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oed.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://uhz.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gsw.jqgfzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://waq.xuetiantiany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ibh.ybcxt.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://klo.daxiang520.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bln.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vxd.zhixingplan.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://clm.316326.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nqk.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://csc.shanyushiyangkeji.top

Py:   list(range(0, 10, 2))
来源：http://iwr.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://nbf.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yoi.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ami.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ycv.zhongyouzk.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nwf.yongpay.top

Ruby: (0...10).step(2).to_a
来源：http://qzn.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vbp.hnxiangtu.top

[B12] 跳出多层循环
来源：http://rlw.smart0.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://jhn.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yqb.aizwys.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dtc.52xcode.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xte.sysykeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vlw.fktsv.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ewm.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zim.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wgg.redwolf501.top

[B13] 判断是否为数字
来源：http://pzf.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://tzg.chenzaomai.com

PHP:  is_numeric($x)
来源：http://cth.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rdp.tarul.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fth.yongpay.top

Java: x instanceof Number
来源：http://nwy.zhijiandao.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ngq.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://gir.snrcjt.cn

C#:   x is int or double or decimal
来源：http://dwm.birdmap.top

[B14] 判断值是否在集合内
来源：http://czd.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zhp.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xvd.sufxvd.cn

JS:   [1, 2, 3].includes(x)
来源：http://acm.9152youxi.cn

TS:   [1, 2, 3].includes(x)
来源：http://njy.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nri.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://efw.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://ucc.daria6918.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vxz.jlsjyb.cn

[B15] 布尔运算与取反
来源：http://qjh.sufxvd.cn

Py:   a and b or not c
来源：http://wfx.svipenyu.cn

PHP:  $a && $b || !$c
来源：http://bjq.yueranfly.top

JS:   a && b || !c
来源：http://cri.wangshuangyany.cn

TS:   a && b || !c
来源：http://vgg.zhengqikj.top

Java: a && b || !c
来源：http://eoh.yvedp.cn

Go:   a && b || !c
来源：http://uly.zhongyouzk.top

Ruby: a && b || !c
来源：http://hmp.xinyue.icu

C#:   a && b || !c
来源：http://fnu.zhengqikj.top

[B16] 卫语句：不满足条件提前返回
来源：http://vny.jinyuanbaomall.cn

Py:   if not data: return
来源：http://eja.yonumen.top

PHP:  if (!$data) { return; }
来源：http://kco.nwbrower.top

JS:   if (!data) return;
来源：http://ekw.gaohongyu789.top

TS:   if (!data) return;
来源：http://gkp.ehwqpu.com

Java: if (data == null) return;
来源：http://hkm.52xcode.cn

Go:   if data == nil { return }
来源：http://yrn.jinqigfzy.top

Ruby: return if data.nil?
来源：http://pqy.meibo888.top

C#:   if (data == null) return;
来源：http://fub.jinghuilouyu.cn

================================================================================
来源：http://kki.gogol.net.cn

C. 函数与作用域
来源：http://ern.ydjk.org.cn

================================================================================
来源：http://usf.wangshuangyany.cn

[C01] 定义函数
来源：http://muz.iojbl.cn

Py:   def add(a, b): return a + b
来源：http://lpj.chenjidiqi.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dgv.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://ihl.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jrx.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://pse.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://inb.hcnkem.com

Ruby: def add(a, b); a + b; end
来源：http://zhi.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hzx.cqqwz.cn

[C02] 默认参数
来源：http://rum.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://azo.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zrc.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ore.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eee.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://alj.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://oxw.zhaomingkeji.xyz

Ruby: def greet(name = "World") = name
来源：http://ejo.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://wpr.xinyue.icu

[C03] 可变参数
来源：http://ypl.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://sns.epnwcf.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jrz.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jlh.fzhhl.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ghg.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wgs.zhongyouzk.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nhm.shangyingyoupin.top

Ruby: def total(*nums); nums.sum; end
来源：http://lrt.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://usy.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://uhq.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oit.hcnkem.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://cly.xziqi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rin.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fez.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://chm.aizwys.cn

Go:   // 无：用配置结构体参数
来源：http://zfd.zhijiandao.cn

Ruby: f(a: 1, b: 2)
来源：http://jfn.xuetiantiany.cn

C#:   f(a: 1, b: 2)
来源：http://vlv.ywan-chungtsiang.top

[C05] 返回多个值
来源：http://oej.havefunace.top

Py:   return a, b
来源：http://zlu.316326.xyz

PHP:  return [$a, $b];
来源：http://nzq.hnxiangtu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jjf.fehbvm.com

TS:   return { a, b };
来源：http://qku.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wju.chenjidiqi.icu

Go:   return a, b
来源：http://evz.fzhhl.top

Ruby: return a, b
来源：http://gqi.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://gxf.fanxiaobao.xyz

[C06] 匿名函数 / lambda
来源：http://iiu.haohaochexian.top

Py:   square = lambda x: x * x
来源：http://hfh.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ysb.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://ybs.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://lqi.zhongyouzk.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lpp.bbcook.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sfg.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://zct.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://qkj.yonumen.top

[C07] 把函数作为参数传入
来源：http://gwe.havefunace.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://tfs.jqgufenzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://wro.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hmd.aizwys.cn

TS:   arr.map(String)
来源：http://atf.jqgufenzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oew.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://oce.hammf.cn

Ruby: arr.map(&:upcase)
来源：http://pkt.wangdashe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://npr.zycfv.cn

[C08] 闭包
来源：http://ina.mhx1999.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vvb.zdqjudy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ibj.dianchejie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://upf.tanke756.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ilk.shzxlz.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dfc.zhengqikj.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qbd.zhengqikj.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fhj.yvedp.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://van.yuxming.cn

[C09] 递归
来源：http://nnk.dashuyun.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sbj.hcnkem.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fib.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://njw.ydjk.org.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qpr.c1oappe.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://egf.guowangkeji.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xya.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://abt.cdnleiting.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfd.jlsjyb.cn

[C10] 变量作用域
来源：http://csv.jinghuilouyu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://pmp.jinqigfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hnq.cashguo.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xif.sweek.top

TS:   同 JS
来源：http://ovy.shzxlz.cn

Java: 方法内为块级作用域
来源：http://fhy.chenlongwang.top

Go:   花括号块级作用域
来源：http://kid.hongshengwenyu.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://nmb.ybcxt.top

C#:   块级作用域
来源：http://ipk.yj20258.top

[C11] 模块导入与导出
来源：http://fjv.xinyue.icu

Py:   from module import func
来源：http://esd.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://kbr.tianlin.xyz

JS:   export default function f() {};  import f from "./m.js";
来源：http://tfy.shanyushiyangtech.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xdy.shangyingyoupin.top

Java: import java.util.List;
来源：http://iwv.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://glw.sweek.top

Ruby: require "json"; require_relative "./util"
来源：http://jic.iojbl.cn

C#:   using System.Text;
来源：http://rjn.316326.xyz

[C12] 立即执行函数 IIFE
来源：http://tsa.yuxming.cn

Py:   (lambda: print("run"))()
来源：http://gnr.kuanghao11.cn

PHP:  (function () { echo "run"; })();
来源：http://kas.yj20258888.top

JS:   (() => { console.log("run"); })();
来源：http://zpv.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://zvq.yonumen.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://csc.cashguo.top

Go:   func() { fmt.Println("run") }()
来源：http://gmp.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://fhz.cheryme.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dsc.zhongyouzk.top

[C13] 类型声明 / 类型注解
来源：http://irm.fzhhl.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mln.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jik.feifeiyinyue.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hcw.feifeiyinyue.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kij.zhengqikj.top

Java: int add(int a, int b) { return a + b; }
来源：http://ntw.jyoumei.cn

Go:   func add(a, b int) int
来源：http://jhs.9152youxi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xrm.jqgfzy.top

C#:   int Add(int a, int b) => a + b;
来源：http://roz.sweek.top

[C14] 泛型函数
来源：http://qey.fzhhl.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bki.ydjk.org.cn

PHP:  // 无泛型
来源：http://ohr.redwolf501.top

JS:   // 无泛型
来源：http://yob.dianchejie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://khp.dashuyun.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hva.nwbrower.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ogf.zhengqikj.top

Ruby: # 无泛型
来源：http://xyp.zdqjudy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ili.shangyingyoupin.top

[C15] 解构 / 展开参数
来源：http://yqb.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nii.xziqi.cn

PHP:  [$a, $b] = $pair;
来源：http://cjc.shzxlz.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ozm.snrcjt.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jag.chenlongwang.top

Java: // 无解构
来源：http://blk.havefunace.top

Go:   // 无解构
来源：http://wct.shangyingyoupin.top

Ruby: a, b = pair
来源：http://qbs.daxiang520.top

C#:   var (a, b) = pair;
来源：http://spb.cucudq.cn

[C16] 函数 / 方法重载
来源：http://scp.fengsongda.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yvs.9152youxi.cn

PHP:  // 无重载
来源：http://lee.havefunace.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jul.gaohongyu789.top

TS:   // 用联合类型或重载签名声明
来源：http://zaj.hnqzz.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dlr.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://jnw.sysykeji.top

Ruby: # 无重载：靠动态参数
来源：http://joj.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gfe.sufxvd.cn

================================================================================
来源：http://cqg.iojbl.cn

D. 数组 / 列表 / 集合
来源：http://uxj.yueranfly.top

================================================================================
来源：http://kqa.zhijiandao.cn

[D01] 创建数组 / 列表
来源：http://uiz.cucudq.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gyo.fehbvm.com

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bju.sufxvd.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ydq.feifeiyinyue.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://pfh.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wzl.pycfn.com

Go:   arr := []int{1, 2, 3}
来源：http://bfz.ywan-chungtsiang.top

Ruby: arr = [1, 2, 3]
来源：http://obc.0kj1m.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vhc.zhiwuduotai.top

[D02] 追加元素到末尾
来源：http://dxy.chenjidiqi.icu

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qqd.xziqi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://czb.xuetiantiany.cn

JS:   arr.push(4);
来源：http://zxy.chenzaomai.com

TS:   arr.push(4);
来源：http://ini.yj20258888.top

Java: list.add(4);
来源：http://sjt.tianlin.xyz

Go:   arr = append(arr, 4)
来源：http://bqs.jyoumei.cn

Ruby: arr << 4; arr.push(5)
来源：http://wrd.xylfe.cn

C#:   list.Add(4);
来源：http://gmh.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://zxe.pengpengdd.cyou

Py:   arr.insert(0, 0)
来源：http://tfv.dianchejie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xyh.0kj1m.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dkt.yuxming.cn

TS:   arr.splice(0, 0, 0);
来源：http://jyq.jqgufenzy.top

Java: list.add(0, 0);
来源：http://ewl.xuanzx.com

Go:   arr = append([]int{0}, arr...)
来源：http://jim.andypj.xyz

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://oad.cdnleiting.top


<!-- 参考信息 -->