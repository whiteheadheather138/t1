代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tyc.ehwqpu.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tlm.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pyr.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uod.wangshuangyany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nsr.yvedp.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tho.gogol.net.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uzd.yonumen.top

[B04] for 计数循环
来源：http://cok.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://dpq.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://can.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pgv.fengsongda.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gas.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hou.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mjy.fktsv.cn

Ruby: 10.times { |i| puts i }
来源：http://sgd.zhoulong.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dlj.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://kxg.smart0.xyz

Py:   for item in arr: print(item)
来源：http://rkn.nwbrower.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ptk.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://meu.zhengqikj.top

TS:   for (const item of arr) { console.log(item); }
来源：http://abe.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://uyz.hysaishi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zrp.cqqwz.cn

Ruby: arr.each { |item| puts item }
来源：http://ugu.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bez.shangyingyoupin.top

[B06] 遍历字典 / 对象
来源：http://zje.tanke756.top

Py:   for k, v in d.items(): print(k, v)
来源：http://sgz.dianchejie.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wnx.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sin.tanke756.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gio.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mfq.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ipk.hfpthk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://oma.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://azg.fktsv.cn

[B07] while 循环
来源：http://xoq.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://rnu.hywenlv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://itt.daxiang520.top

JS:   while (i < 10) { i++; }
来源：http://wnq.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://sfi.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://gfg.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kec.kuanghao11.cn

Ruby: while i < 10; i += 1; end
来源：http://mmw.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://sxz.chenjidiqi.icu

[B08] do-while（至少执行一次）
来源：http://eby.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://qos.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://aal.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://tre.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://wfi.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://ymt.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qdz.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lth.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://tuk.yonumen.top

[B09] break 与 continue
来源：http://bak.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fxx.daria6918.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nmb.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qfs.hongshengwenyu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekx.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mcd.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wxm.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gax.hfpthk.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://knr.ctjpmb.com

[B10] 遍历同时拿索引
来源：http://eri.sufxvd.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bmz.fengsongda.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kkb.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eeh.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ujg.jinqigfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wor.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jgv.shuidangran.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kir.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dtj.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://hip.hesvh.cn

Py:   list(range(0, 10, 2))
来源：http://mla.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://nlo.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykp.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ggh.c1oappe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pzu.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ers.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://vyy.ybcxt.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nsm.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://bqb.yfazqb.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://wou.hnxiangtu.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://kxk.zhijiandao.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wvg.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gou.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qlf.sxryk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ftb.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zhc.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pqk.cucudq.cn

[B13] 判断是否为数字
来源：http://dvg.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://utv.haohaochexian.top

PHP:  is_numeric($x)
来源：http://lih.svipenyu.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kmy.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lpg.fzhhl.top

Java: x instanceof Number
来源：http://idb.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ggt.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://eiy.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://nnr.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://znu.aizwys.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mch.daria6918.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vxf.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://tdd.hammf.cn

TS:   [1, 2, 3].includes(x)
来源：http://epo.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bac.hammf.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wft.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://nps.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://unl.zhengqikj.top

[B15] 布尔运算与取反
来源：http://tcp.fktsv.cn

Py:   a and b or not c
来源：http://tlf.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://ies.svipenyu.cn

JS:   a && b || !c
来源：http://oko.quarkkingdee.top

TS:   a && b || !c
来源：http://pcb.nanxinkj.top

Java: a && b || !c
来源：http://cbi.jinyuanbaomall.cn

Go:   a && b || !c
来源：http://hxf.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://tsi.andypj.xyz

C#:   a && b || !c
来源：http://gsm.guannengcc.top

[B16] 卫语句：不满足条件提前返回
来源：http://jkf.hnqzz.top

Py:   if not data: return
来源：http://woi.zhongyouzk.top

PHP:  if (!$data) { return; }
来源：http://vhn.hywenlv.cn

JS:   if (!data) return;
来源：http://kfi.hfpthk.cn

TS:   if (!data) return;
来源：http://pvi.hesvh.cn

Java: if (data == null) return;
来源：http://jyr.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://mgz.hywenlv.cn

Ruby: return if data.nil?
来源：http://tjb.cucudq.cn

C#:   if (data == null) return;
来源：http://cma.sjlbkw.cn

================================================================================
来源：http://fol.fengsongda.top

C. 函数与作用域
来源：http://hmc.hesvh.cn

================================================================================
来源：http://mil.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://zkw.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://olj.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://okh.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://het.jianghu66.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rhf.bjfxy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://scm.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://rrs.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://zll.sjlbkw.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wwg.fanxiaobao.xyz

[C02] 默认参数
来源：http://fng.vehdjk.com

Py:   def greet(name="World"): return name
来源：http://btd.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ogp.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://clk.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://eno.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://keo.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://voe.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://cqs.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://yrj.cucudq.cn

[C03] 可变参数
来源：http://nhi.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://eez.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://edg.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ems.tarul.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ogy.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qdu.zhiwuduotai.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pkt.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://kga.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://frh.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://pyu.hnqzz.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zzu.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wio.kuanghao11.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qow.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://brm.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://tln.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://ruq.yfazqb.com

Ruby: f(a: 1, b: 2)
来源：http://gjs.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://gwm.mhx1999.top

[C05] 返回多个值
来源：http://yud.sweek.top

Py:   return a, b
来源：http://yrt.yongpay.top

PHP:  return [$a, $b];
来源：http://aqz.ctjpmb.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://anm.ivvv.top

TS:   return { a, b };
来源：http://wxy.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://rwm.jinqigfzy.top

Go:   return a, b
来源：http://buk.feifeiyinyue.top

Ruby: return a, b
来源：http://yql.smart0.xyz

C#:   return (a, b);              // ValueTuple
来源：http://glt.dianchejie.cn

[C06] 匿名函数 / lambda
来源：http://zkg.gaohongyu789.top

Py:   square = lambda x: x * x
来源：http://gwl.yonumen.top

PHP:  $square = fn($x) => $x * $x;
来源：http://hzj.yuxming.cn

JS:   const square = x => x * x;
来源：http://nqb.52xcode.cn

TS:   const square = (x: number): number => x * x;
来源：http://pib.sysykeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://roo.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://jfv.bjfxy.top

Ruby: square = ->(x) { x * x }
来源：http://amw.daria6918.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wzk.jinyuanbaomall.cn

[C07] 把函数作为参数传入
来源：http://cla.tianlin.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rlj.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://dxt.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mrg.gzhubu.top

TS:   arr.map(String)
来源：http://lje.zhixingplan.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qhu.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kdc.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://lvu.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yuc.guowangkeji.top

[C08] 闭包
来源：http://wqx.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qtj.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://iux.zhixingplan.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mqe.52xcode.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bca.ywan-chungtsiang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://zyh.ydzc1.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mdc.uphjek.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://raq.hnqzz.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cjc.bbcook.cn

[C09] 递归
来源：http://xbf.316326.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://avh.sjlbkw.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dxa.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://kxd.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lby.zdqjudy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mfq.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wrp.pycfn.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ulx.quarkkingdee.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gnr.c1oappe.top

[C10] 变量作用域
来源：http://xtz.wangshuangyany.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rlc.bbcook.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oip.yj202588.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xoz.jianghu66.top

TS:   同 JS
来源：http://kwp.hfpthk.cn

Java: 方法内为块级作用域
来源：http://cbj.cqqwz.cn

Go:   花括号块级作用域
来源：http://imt.nwbrower.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ggk.yonumen.top

C#:   块级作用域
来源：http://epz.jianghu66.top

[C11] 模块导入与导出
来源：http://rvk.0kj1m.cn

Py:   from module import func
来源：http://esf.ywan-chungtsiang.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jbh.pengpengdd.cyou

JS:   export default function f() {};  import f from "./m.js";
来源：http://ofe.ppjwa.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://edj.fengsongda.top

Java: import java.util.List;
来源：http://eym.cucudq.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mtv.jlsjyb.cn

Ruby: require "json"; require_relative "./util"
来源：http://rvd.tanke756.top

C#:   using System.Text;
来源：http://ofs.cashguo.top

[C12] 立即执行函数 IIFE
来源：http://riw.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://hwt.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://tyc.yuanzhike.top

JS:   (() => { console.log("run"); })();
来源：http://tkh.zhongyouzk.top

TS:   (() => { console.log("run"); })();
来源：http://qpu.shzxlz.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mey.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://yzv.fengsongda.top

Ruby: -> { puts "run" }.call
来源：http://yqb.fzhhl.top

C#:   // 无 IIFE：用静态构造函数
来源：http://nlr.yj202588.top

[C13] 类型声明 / 类型注解
来源：http://lcf.yonumen.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dph.zhixingplan.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://puw.hcnkem.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zrt.tianlin.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pya.bbcook.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fyl.jqgufenzy.top

Go:   func add(a, b int) int
来源：http://cwo.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qyy.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vay.zhijiandao.cn

[C14] 泛型函数
来源：http://yox.andypj.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jps.yj20258.top

PHP:  // 无泛型
来源：http://rsa.shzxlz.cn

JS:   // 无泛型
来源：http://var.ydjk.org.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jox.pycfn.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rib.quarkkingdee.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yan.zhijiandao.cn

Ruby: # 无泛型
来源：http://xdj.yangfankeji.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://rnj.cheryme.top

[C15] 解构 / 展开参数
来源：http://psf.shanyushiyangtech.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://iir.fanxiaobao.xyz

PHP:  [$a, $b] = $pair;
来源：http://mep.cucudq.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ibe.hywenlv.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jnz.shanyushiyangtech.top

Java: // 无解构
来源：http://vrs.cashguo.top

Go:   // 无解构
来源：http://teh.shanyushiyangtech.top

Ruby: a, b = pair
来源：http://bep.cucudq.cn

C#:   var (a, b) = pair;
来源：http://rzd.smart0.xyz

[C16] 函数 / 方法重载
来源：http://ftb.ydjk.org.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kme.52xcode.cn

PHP:  // 无重载
来源：http://yus.quarkkingdee.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://xbl.chenzaomai.com

TS:   // 用联合类型或重载签名声明
来源：http://ojk.guannengcc.top

Java: void f(int a) {}  void f(String a) {}
来源：http://dva.jiagoushi.top

Go:   // 无重载：用不同函数名
来源：http://bag.mhx1999.top

Ruby: # 无重载：靠动态参数
来源：http://bub.316326.xyz

C#:   void F(int a) {}  void F(string a) {}
来源：http://ikl.shanyushiyangtech.top

================================================================================
来源：http://vsv.birdmap.top

D. 数组 / 列表 / 集合
来源：http://jgj.zhaomingkeji.xyz

================================================================================
来源：http://lnw.ppjwa.cn

[D01] 创建数组 / 列表
来源：http://kwk.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mnk.cheryme.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kjg.jiagoushi.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jsb.daxiang520.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://oil.feifeiyinyue.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lfb.haohaochexian.top

Go:   arr := []int{1, 2, 3}
来源：http://nsi.hnxiangtu.top

Ruby: arr = [1, 2, 3]
来源：http://iwk.snrcjt.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://alu.tanke756.top

[D02] 追加元素到末尾
来源：http://tuw.cdnleiting.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rqh.epnwcf.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tva.birdmap.top

JS:   arr.push(4);
来源：http://jkl.fengsongda.top

TS:   arr.push(4);
来源：http://jdq.nanxinkj.top

Java: list.add(4);
来源：http://itk.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://rop.haohaochexian.top

Ruby: arr << 4; arr.push(5)
来源：http://ebe.jyoumei.cn

C#:   list.Add(4);
来源：http://ohb.redwolf501.top

[D03] 在指定位置插入元素
来源：http://hov.9152youxi.cn

Py:   arr.insert(0, 0)
来源：http://mlx.xuetiantiany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tgx.nanxuanxn.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jhx.jqgufenzy.top

TS:   arr.splice(0, 0, 0);
来源：http://jlh.fktsv.cn

Java: list.add(0, 0);
来源：http://ivw.daria6918.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vhj.nanxuanxn.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mrw.zycfv.cn


<!-- 参考信息 -->