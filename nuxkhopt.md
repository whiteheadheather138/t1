代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://atv.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rmi.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://una.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ttx.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xxb.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qqr.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ztj.cdnleiting.top

[B04] for 计数循环
来源：http://vjx.bbcook.cn

Py:   for i in range(10): print(i)
来源：http://svk.gzhubu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://evn.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ymk.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dhr.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qif.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nfl.yj20258888.top

Ruby: 10.times { |i| puts i }
来源：http://zqs.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hzf.tanke756.top

[B05] 遍历数组 / 列表
来源：http://rrx.kuanghao11.cn

Py:   for item in arr: print(item)
来源：http://cez.pycfn.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ltg.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://urf.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lvo.shanyushiyangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ezp.nwbrower.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qyb.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://zuv.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ybf.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://gez.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://bjz.cucudq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ucw.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ccz.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hdb.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://coo.ybcxt.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xgo.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zkv.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tkt.cqqwz.cn

[B07] while 循环
来源：http://aac.uphjek.com

Py:   while i < 10: i += 1
来源：http://wuh.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://efe.fzhhl.top

JS:   while (i < 10) { i++; }
来源：http://xoo.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://yqc.sufxvd.cn

Java: while (i < 10) { i++; }
来源：http://kbd.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nst.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://fnl.hnxiangtu.top

C#:   while (i < 10) { i++; }
来源：http://xci.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://xbb.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://orx.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vor.guannengcc.top

JS:   do { i++; } while (i < 10);
来源：http://jqp.wangshuangyany.cn

TS:   do { i++; } while (i < 10);
来源：http://lbl.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://mod.jiagoushi.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xnf.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://vpm.zdqjudy.top

C#:   do { i++; } while (i < 10);
来源：http://omq.redwolf501.top

[B09] break 与 continue
来源：http://lbx.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://thv.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zjj.shanyushiyangtech.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qoa.xuanzx.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pee.jqgufenzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttu.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://scn.52xcode.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://aew.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://scb.yongpay.top

[B10] 遍历同时拿索引
来源：http://ape.sweek.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgb.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfp.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lyd.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jmr.chenlongwang.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kgc.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://son.yj202588.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hok.jinqigufen.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hzb.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://biy.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://fml.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://fzo.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avp.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kwm.yuxming.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://udp.hammf.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dkt.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://vex.fengsongda.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zse.cqqwz.cn

[B12] 跳出多层循环
来源：http://kot.snrcjt.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ajd.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tus.yangfankeji.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofx.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://drd.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ica.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://glo.zdqjudy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wwv.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ltf.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://jxi.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://qxb.yj20258.top

PHP:  is_numeric($x)
来源：http://mgv.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bko.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wdv.daxiang520.top

Java: x instanceof Number
来源：http://yfn.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://iay.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://gam.jyoumei.cn

C#:   x is int or double or decimal
来源：http://ndg.fengsongda.top

[B14] 判断值是否在集合内
来源：http://erl.pycfn.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fiu.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tiq.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://yrb.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://peq.cheryme.top

Java: List.of(1, 2, 3).contains(x)
来源：http://lym.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://amn.hnqzz.top

Ruby: [1, 2, 3].include?(x)
来源：http://gmd.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://usu.pycfn.com

[B15] 布尔运算与取反
来源：http://fhy.xylfe.cn

Py:   a and b or not c
来源：http://fqs.tian-w.cn

PHP:  $a && $b || !$c
来源：http://fum.chenzaomai.com

JS:   a && b || !c
来源：http://hei.xziqi.cn

TS:   a && b || !c
来源：http://bhc.cqqwz.cn

Java: a && b || !c
来源：http://ysq.yfazqb.com

Go:   a && b || !c
来源：http://qor.nanxinkj.top

Ruby: a && b || !c
来源：http://ogi.ppjwa.cn

C#:   a && b || !c
来源：http://cyv.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://ivg.cdnleiting.top

Py:   if not data: return
来源：http://inu.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://kib.gaohongyu789.top

JS:   if (!data) return;
来源：http://mpc.aizwys.cn

TS:   if (!data) return;
来源：http://pfw.bjfxy.top

Java: if (data == null) return;
来源：http://ufg.xuetiantiany.cn

Go:   if data == nil { return }
来源：http://pzd.kuanghao11.cn

Ruby: return if data.nil?
来源：http://gur.zhijiandao.cn

C#:   if (data == null) return;
来源：http://txj.yj202588.top

================================================================================
来源：http://gfk.dianchejie.cn

C. 函数与作用域
来源：http://rdg.nanxuanxn.top

================================================================================
来源：http://seu.jianghu66.top

[C01] 定义函数
来源：http://cpz.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://tvk.gogol.net.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ueu.chenlongwang.top

JS:   function add(a, b) { return a + b; }
来源：http://urc.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iwx.vehdjk.com

Java: static int add(int a, int b) { return a + b; }
来源：http://obk.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://sct.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://vzx.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wlo.gogol.net.cn

[C02] 默认参数
来源：http://hxn.52xcode.cn

Py:   def greet(name="World"): return name
来源：http://ukv.jiagoushi.top

PHP:  function greet($name = "World") { return $name; }
来源：http://joe.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://quz.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://bjv.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dyu.sxryk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zse.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://xab.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://rop.zhijiandao.cn

[C03] 可变参数
来源：http://wql.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://omd.hongshengwenyu.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zmc.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mkm.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zmg.sufxvd.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://reg.ybcxt.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bft.ydjk.org.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nja.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pqi.zhongyouzk.top

[C04] 命名参数 / 关键字参数
来源：http://kic.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://biv.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://haz.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://trp.52xcode.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zqn.xingfuxueyuan.xyz

Java: // 无：用 Builder 模式或 record
来源：http://qgf.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://rso.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://pce.haohaochexian.top

C#:   f(a: 1, b: 2)
来源：http://uho.haohaochexian.top

[C05] 返回多个值
来源：http://rol.xylfe.cn

Py:   return a, b
来源：http://gru.hysaishi.cn

PHP:  return [$a, $b];
来源：http://kfn.hfpthk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://hrc.fzhhl.top

TS:   return { a, b };
来源：http://mrs.xziqi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://huw.yfazqb.com

Go:   return a, b
来源：http://xxr.shangyingyoupin.top

Ruby: return a, b
来源：http://tbz.gogol.net.cn

C#:   return (a, b);              // ValueTuple
来源：http://peo.hfpthk.cn

[C06] 匿名函数 / lambda
来源：http://avc.xinyue.icu

Py:   square = lambda x: x * x
来源：http://rjs.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://muy.hfpthk.cn

JS:   const square = x => x * x;
来源：http://yaa.andypj.xyz

TS:   const square = (x: number): number => x * x;
来源：http://cat.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ytm.zhoulong.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://wpq.redwolf501.top

Ruby: square = ->(x) { x * x }
来源：http://xaq.c1oappe.top

C#:   Func<int, int> square = x => x * x;
来源：http://bhn.zhoulong.xyz

[C07] 把函数作为参数传入
来源：http://xws.zhijiandao.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mgp.yuxming.cn

PHP:  array_map("strtoupper", $arr);
来源：http://hfp.zycfv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zbf.sxryk.cn

TS:   arr.map(String)
来源：http://pak.xuetiantiany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mpr.xuetiantiany.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://alm.zhixingplan.top

Ruby: arr.map(&:upcase)
来源：http://cvw.fengsongda.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gft.guannengcc.top

[C08] 闭包
来源：http://vny.hnqzz.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jjt.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hdy.ydjk.org.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xnp.cdnleiting.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bbc.hywenlv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yjz.jqgufenzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dte.xuetiantiany.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rmp.ybcxt.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ckq.tanke756.top

[C09] 递归
来源：http://amx.bbcook.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cgy.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://cyy.yuxming.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://joc.jinqigufen.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ble.zhixingplan.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://icc.mhx1999.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zsp.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://dmb.haohaochexian.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uzs.zhiwuduotai.top

[C10] 变量作用域
来源：http://fjz.sjlbkw.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qvo.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ege.vehdjk.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bne.c1oappe.top

TS:   同 JS
来源：http://wnd.xinyue.icu

Java: 方法内为块级作用域
来源：http://oeo.ydjk.org.cn

Go:   花括号块级作用域
来源：http://zza.daxiang520.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tkc.sxryk.cn

C#:   块级作用域
来源：http://cdm.tarul.cn

[C11] 模块导入与导出
来源：http://upl.daxiang520.top

Py:   from module import func
来源：http://tpx.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://dom.xylfe.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hma.fktsv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://muv.mhx1999.top

Java: import java.util.List;
来源：http://kwb.daxiang520.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zxg.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://blt.yuxming.cn

C#:   using System.Text;
来源：http://vip.yongpay.top

[C12] 立即执行函数 IIFE
来源：http://zwq.jyoumei.cn

Py:   (lambda: print("run"))()
来源：http://wez.zhiwuduotai.top

PHP:  (function () { echo "run"; })();
来源：http://cfy.9152youxi.cn

JS:   (() => { console.log("run"); })();
来源：http://tls.gzhubu.top

TS:   (() => { console.log("run"); })();
来源：http://hgi.9152youxi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ugy.andypj.xyz

Go:   func() { fmt.Println("run") }()
来源：http://hgt.jianghu66.top

Ruby: -> { puts "run" }.call
来源：http://tka.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bzv.bjfxy.top

[C13] 类型声明 / 类型注解
来源：http://ysq.havefunace.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pth.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lvo.sweek.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://nse.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rhp.guannengcc.top

Java: int add(int a, int b) { return a + b; }
来源：http://duj.hfpthk.cn

Go:   func add(a, b int) int
来源：http://duw.chenjidiqi.icu

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ymx.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cee.yvedp.cn

[C14] 泛型函数
来源：http://jcp.dashuyun.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://efr.yonumen.top

PHP:  // 无泛型
来源：http://svm.cheryme.top

JS:   // 无泛型
来源：http://syu.feifeiyinyue.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gjt.zhiwuduotai.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://inm.ywan-chungtsiang.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://otm.yueranfly.top

Ruby: # 无泛型
来源：http://wwd.ehwqpu.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qzj.hysaishi.cn

[C15] 解构 / 展开参数
来源：http://mbx.tian-w.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wke.meibo888.top

PHP:  [$a, $b] = $pair;
来源：http://bna.c1oappe.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tgm.epnwcf.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://abw.cashguo.top

Java: // 无解构
来源：http://tuw.hfpthk.cn

Go:   // 无解构
来源：http://hlj.birdmap.top

Ruby: a, b = pair
来源：http://mah.cdnleiting.top

C#:   var (a, b) = pair;
来源：http://onz.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://lgc.gogol.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ufl.52xcode.cn

PHP:  // 无重载
来源：http://ktw.xuanzx.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://wxz.haohaochexian.top

TS:   // 用联合类型或重载签名声明
来源：http://qcm.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://aga.xingfuxueyuan.xyz

Go:   // 无重载：用不同函数名
来源：http://xid.jinqigufen.top

Ruby: # 无重载：靠动态参数
来源：http://elf.ppjwa.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://adz.snrcjt.cn

================================================================================
来源：http://ugx.gogol.net.cn

D. 数组 / 列表 / 集合
来源：http://dje.jinghuilouyu.cn

================================================================================
来源：http://bhj.iojbl.cn

[D01] 创建数组 / 列表
来源：http://kcr.zhengqikj.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://pis.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://udb.yanxiufei.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bhe.xuetiantiany.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bii.yuxming.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gbm.hnqzz.top

Go:   arr := []int{1, 2, 3}
来源：http://wys.zhoulong.xyz

Ruby: arr = [1, 2, 3]
来源：http://xhq.havefunace.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://whk.yuanzhike.top

[D02] 追加元素到末尾
来源：http://sgl.daria6918.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://afw.dianchejie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xdg.ywan-chungtsiang.top

JS:   arr.push(4);
来源：http://dwx.meibo888.top

TS:   arr.push(4);
来源：http://zoz.yj202588.top

Java: list.add(4);
来源：http://nfq.yj202588.top

Go:   arr = append(arr, 4)
来源：http://ggk.tianlin.xyz

Ruby: arr << 4; arr.push(5)
来源：http://miy.havefunace.top

C#:   list.Add(4);
来源：http://wmj.yongpay.top

[D03] 在指定位置插入元素
来源：http://sxi.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://xje.snrcjt.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ylf.mhx1999.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ten.svipenyu.cn

TS:   arr.splice(0, 0, 0);
来源：http://oxl.cheryme.top

Java: list.add(0, 0);
来源：http://ucn.yangfankeji.com

Go:   arr = append([]int{0}, arr...)
来源：http://omr.hongshengwenyu.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bsr.mhx1999.top


<!-- 参考信息 -->