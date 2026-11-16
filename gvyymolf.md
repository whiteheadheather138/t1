代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://akh.shangyingyoupin.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://osf.guannengcc.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://inf.yangfankeji.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fxn.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hlx.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lox.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pmz.svipenyu.cn

[B04] for 计数循环
来源：http://xum.ctjpmb.com

Py:   for i in range(10): print(i)
来源：http://yrc.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tnz.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nuv.cashguo.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oag.guowangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bsr.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://boh.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://njd.yj20258888.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hcu.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://ymr.guowangkeji.top

Py:   for item in arr: print(item)
来源：http://rws.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dux.sjlbkw.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://iud.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qlc.wangdashe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vwh.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jqq.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://lgh.fanxiaobao.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://izj.epnwcf.com

[B06] 遍历字典 / 对象
来源：http://djc.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vlc.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ivp.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stv.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xec.gogol.net.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mrq.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ygy.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://irm.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iod.0kj1m.cn

[B07] while 循环
来源：http://nnc.aibaodan.cn

Py:   while i < 10: i += 1
来源：http://ygl.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mwh.bjfxy.top

JS:   while (i < 10) { i++; }
来源：http://tdu.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://otz.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://vmb.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kua.havefunace.top

Ruby: while i < 10; i += 1; end
来源：http://ozi.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://uvw.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://dfv.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://zdf.mhx1999.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vst.hnqzz.top

JS:   do { i++; } while (i < 10);
来源：http://nfa.jqgufenzy.top

TS:   do { i++; } while (i < 10);
来源：http://pki.guowangkeji.top

Java: do { i++; } while (i < 10);
来源：http://izd.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://csl.xinyue.icu

Ruby: begin; i += 1; end while i < 10
来源：http://reh.xinyue.icu

C#:   do { i++; } while (i < 10);
来源：http://tva.c1oappe.top

[B09] break 与 continue
来源：http://ygc.hnxiangtu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://znc.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xln.yvedp.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vrn.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jro.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tri.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://weg.nwbrower.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://oml.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekk.birdmap.top

[B10] 遍历同时拿索引
来源：http://hps.0kj1m.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rxs.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://smq.jinghuilouyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xip.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://igk.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tsj.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://agu.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jmw.dianchejie.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bai.smart0.xyz

[B11] 生成数字序列 / 区间
来源：http://mnb.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://wdz.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://fcr.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nlb.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://oml.316326.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://trb.xuetiantiany.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ssc.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://psn.ywan-chungtsiang.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mec.316326.xyz

[B12] 跳出多层循环
来源：http://ksl.xylfe.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://iaf.shangyingyoupin.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nwu.chenlongwang.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yhm.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ytm.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uyt.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xkx.nanxuanxn.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fks.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mob.tarul.cn

[B13] 判断是否为数字
来源：http://rzq.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://juw.nwbrower.top

PHP:  is_numeric($x)
来源：http://qce.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asq.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://are.tanke756.top

Java: x instanceof Number
来源：http://rcg.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qxy.shuidangran.top

Ruby: x.is_a?(Numeric)
来源：http://zzt.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://nzz.aizwys.cn

[B14] 判断值是否在集合内
来源：http://dcm.zycfv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvx.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dpo.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://uod.sufxvd.cn

TS:   [1, 2, 3].includes(x)
来源：http://usr.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://azo.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sgd.xylfe.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zvo.hnxiangtu.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xhg.snrcjt.cn

[B15] 布尔运算与取反
来源：http://hep.zycfv.cn

Py:   a and b or not c
来源：http://eqf.fanxiaobao.xyz

PHP:  $a && $b || !$c
来源：http://puk.jqgfzy.top

JS:   a && b || !c
来源：http://cau.bjfxy.top

TS:   a && b || !c
来源：http://qzk.tian-w.cn

Java: a && b || !c
来源：http://uba.zycfv.cn

Go:   a && b || !c
来源：http://zjs.xingfuxueyuan.xyz

Ruby: a && b || !c
来源：http://zgi.guannengcc.top

C#:   a && b || !c
来源：http://ksw.nwbrower.top

[B16] 卫语句：不满足条件提前返回
来源：http://jax.cqqwz.cn

Py:   if not data: return
来源：http://qif.jinqigufen.top

PHP:  if (!$data) { return; }
来源：http://tyc.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://jhx.cucudq.cn

TS:   if (!data) return;
来源：http://zhz.redwolf501.top

Java: if (data == null) return;
来源：http://qam.jinqigfzy.top

Go:   if data == nil { return }
来源：http://kar.fengsongda.top

Ruby: return if data.nil?
来源：http://jxl.gotoacloud.top

C#:   if (data == null) return;
来源：http://yrl.shangyingyoupin.top

================================================================================
来源：http://njg.yfazqb.com

C. 函数与作用域
来源：http://qdv.yuanzhike.top

================================================================================
来源：http://wzl.yueranfly.top

[C01] 定义函数
来源：http://qmc.vehdjk.com

Py:   def add(a, b): return a + b
来源：http://ury.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qpk.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://osi.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ciy.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://ucv.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://stt.gogol.net.cn

Ruby: def add(a, b); a + b; end
来源：http://lfv.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tzf.yfazqb.com

[C02] 默认参数
来源：http://xpd.tanke756.top

Py:   def greet(name="World"): return name
来源：http://wtd.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://iar.jqgufenzy.top

JS:   function greet(name = "World") { return name; }
来源：http://iab.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://nuf.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ctq.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zbw.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://ufl.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://akx.kuanghao11.cn

[C03] 可变参数
来源：http://sdb.zhiwuduotai.top

Py:   def total(*args): return sum(args)
来源：http://mep.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rqn.yj202588.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mbi.52xcode.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dlh.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qkr.vehdjk.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://stt.fanxiaobao.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qft.xuetiantiany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gav.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://scg.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xcr.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wlf.sufxvd.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ubp.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pdg.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://rxg.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://qqv.fzhhl.top

Ruby: f(a: 1, b: 2)
来源：http://xpe.chenlongwang.top

C#:   f(a: 1, b: 2)
来源：http://pfj.yonumen.top

[C05] 返回多个值
来源：http://gld.xingfuxueyuan.xyz

Py:   return a, b
来源：http://eyn.guannengcc.top

PHP:  return [$a, $b];
来源：http://dpx.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qyc.feifeiyinyue.top

TS:   return { a, b };
来源：http://sgq.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vrk.hongshengwenyu.top

Go:   return a, b
来源：http://slt.cheryme.top

Ruby: return a, b
来源：http://mir.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://ddo.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://sla.cqqwz.cn

Py:   square = lambda x: x * x
来源：http://qlf.sxryk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ibg.sweek.top

JS:   const square = x => x * x;
来源：http://zsc.vehdjk.com

TS:   const square = (x: number): number => x * x;
来源：http://syg.sjlbkw.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tdq.sxryk.cn

Go:   sq := func(x int) int { return x * x }
来源：http://apo.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://jik.andypj.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://djh.meibo888.top

[C07] 把函数作为参数传入
来源：http://odx.gotoacloud.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lxh.feifeiyinyue.top

PHP:  array_map("strtoupper", $arr);
来源：http://ifz.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uyj.52xcode.cn

TS:   arr.map(String)
来源：http://gsg.jinqigufen.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xgh.hywenlv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ndo.haohaochexian.top

Ruby: arr.map(&:upcase)
来源：http://swi.hesvh.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://nrv.guowangkeji.top

[C08] 闭包
来源：http://zjn.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://woo.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hxa.daxiang520.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mff.jianghu66.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://enu.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://unr.sxryk.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cbe.meibo888.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://abb.bjfxy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qfy.fzhhl.top

[C09] 递归
来源：http://tuv.yfazqb.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qkx.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://prn.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rpx.uphjek.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gyv.gotoacloud.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qld.zycfv.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eju.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ewa.iojbl.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zbh.sufxvd.cn

[C10] 变量作用域
来源：http://qxn.havefunace.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://awr.wangdashe.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wqs.redwolf501.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://gdq.xziqi.cn

TS:   同 JS
来源：http://euv.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://lhx.hongshengwenyu.top

Go:   花括号块级作用域
来源：http://cld.aizwys.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sih.haohaochexian.top

C#:   块级作用域
来源：http://ylh.pycfn.com

[C11] 模块导入与导出
来源：http://jkf.yj20258.top

Py:   from module import func
来源：http://rob.cashguo.top

PHP:  require "file.php";  或 use App\Service;
来源：http://vhe.vqdsnc.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://svu.cucudq.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jbs.xuetiantiany.cn

Java: import java.util.List;
来源：http://msi.wangshuangyany.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://gzv.bjfxy.top

Ruby: require "json"; require_relative "./util"
来源：http://htk.gogol.net.cn

C#:   using System.Text;
来源：http://dby.ydzc1.top

[C12] 立即执行函数 IIFE
来源：http://wxp.zhongyouzk.top

Py:   (lambda: print("run"))()
来源：http://jgb.ybcxt.top

PHP:  (function () { echo "run"; })();
来源：http://cuf.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://uqu.iojbl.cn

TS:   (() => { console.log("run"); })();
来源：http://lzw.yuanzhike.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vci.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://lgo.ppjwa.cn

Ruby: -> { puts "run" }.call
来源：http://lud.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://vwg.yvedp.cn

[C13] 类型声明 / 类型注解
来源：http://ynn.hcnkem.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fgq.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rhq.tarul.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wrt.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iqe.cqqwz.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xkr.uphjek.com

Go:   func add(a, b int) int
来源：http://vvd.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://dhz.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://vhk.zhixingplan.top

[C14] 泛型函数
来源：http://acm.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qfs.gaohongyu789.top

PHP:  // 无泛型
来源：http://smf.daria6918.cn

JS:   // 无泛型
来源：http://dcp.vehdjk.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jiv.jinqigufen.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://tax.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vzf.ywan-chungtsiang.top

Ruby: # 无泛型
来源：http://joy.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cab.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://ajy.yueranfly.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://twx.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://alx.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dix.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://got.daxiang520.top

Java: // 无解构
来源：http://hxy.yj20258.top

Go:   // 无解构
来源：http://wac.zdbjq.cn

Ruby: a, b = pair
来源：http://yma.hammf.cn

C#:   var (a, b) = pair;
来源：http://hiq.zycfv.cn

[C16] 函数 / 方法重载
来源：http://oom.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ksj.chenzaomai.com

PHP:  // 无重载
来源：http://kws.gogol.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xzc.zhixingplan.top

TS:   // 用联合类型或重载签名声明
来源：http://ifu.jyoumei.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vvo.ywan-chungtsiang.top

Go:   // 无重载：用不同函数名
来源：http://nzd.havefunace.top

Ruby: # 无重载：靠动态参数
来源：http://rzz.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://yzj.zhixingplan.top

================================================================================
来源：http://itk.hnqzz.top

D. 数组 / 列表 / 集合
来源：http://oot.jlsjyb.cn

================================================================================
来源：http://fxw.hnxiangtu.top

[D01] 创建数组 / 列表
来源：http://wtb.fktsv.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pzv.redwolf501.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://axc.feifeiyinyue.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vfg.hcnkem.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://gxg.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mhu.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://zuk.jqgufenzy.top

Ruby: arr = [1, 2, 3]
来源：http://sej.shanyushiyangtech.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hby.xinyue.icu

[D02] 追加元素到末尾
来源：http://xli.yj20258888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oto.jiagoushi.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ttc.sufxvd.cn

JS:   arr.push(4);
来源：http://lta.hnxiangtu.top

TS:   arr.push(4);
来源：http://bwt.svipenyu.cn

Java: list.add(4);
来源：http://zdd.yongpay.top

Go:   arr = append(arr, 4)
来源：http://hfi.guowangkeji.top

Ruby: arr << 4; arr.push(5)
来源：http://ovs.zhongyouzk.top

C#:   list.Add(4);
来源：http://xmd.guowangkeji.top

[D03] 在指定位置插入元素
来源：http://nft.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://knb.hnqzz.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fai.zhiwuduotai.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://vqx.chenlongwang.top

TS:   arr.splice(0, 0, 0);
来源：http://hsf.aibaodan.cn

Java: list.add(0, 0);
来源：http://ihf.gaohongyu789.top

Go:   arr = append([]int{0}, arr...)
来源：http://nze.guowangkeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hvu.zhiwuduotai.top


<!-- 参考信息 -->