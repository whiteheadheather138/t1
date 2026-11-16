代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://itq.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wyr.yvedp.cn

[B03] switch / match / case
来源：http://bnb.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://efh.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ove.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jjz.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vjx.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vvd.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hlv.hnqzz.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://isr.fengsongda.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://icj.smart0.xyz

[B04] for 计数循环
来源：http://eyx.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://oul.chenjidiqi.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mok.sxryk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rda.c1oappe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bxu.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tsl.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ueh.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://cdx.xuetiantiany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lnp.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://pqh.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://kvg.zdbjq.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oip.aibaodan.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yjc.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://wmt.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://guk.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tfc.hysaishi.cn

Ruby: arr.each { |item| puts item }
来源：http://vpz.c1oappe.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bvi.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://sjw.zhengqikj.top

Py:   for k, v in d.items(): print(k, v)
来源：http://czg.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cod.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dws.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kla.cheryme.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://idc.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://phu.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zoi.yonumen.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sbf.chenzaomai.com

[B07] while 循环
来源：http://dtd.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://kyh.havefunace.top

PHP:  while ($i < 10) { $i++; }
来源：http://jjv.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://vrt.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://apm.hysaishi.cn

Java: while (i < 10) { i++; }
来源：http://rkm.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ecg.snrcjt.cn

Ruby: while i < 10; i += 1; end
来源：http://akx.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://nsw.cdnleiting.top

[B08] do-while（至少执行一次）
来源：http://vhx.tarul.cn

Py:   # 无 do-while：用 while True + break
来源：http://rtn.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gkp.hongshengwenyu.top

JS:   do { i++; } while (i < 10);
来源：http://lec.c1oappe.top

TS:   do { i++; } while (i < 10);
来源：http://auz.yj20258888.top

Java: do { i++; } while (i < 10);
来源：http://kuw.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tut.haohaochexian.top

Ruby: begin; i += 1; end while i < 10
来源：http://smu.ybcxt.top

C#:   do { i++; } while (i < 10);
来源：http://jmk.iojbl.cn

[B09] break 与 continue
来源：http://urr.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://shf.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bsh.xinyue.icu

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cze.jqgufenzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gvl.jiagoushi.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ziz.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://riy.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zpw.ybcxt.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nei.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://qln.feifeiyinyue.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sjp.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tyc.quarkkingdee.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vfq.nanxuanxn.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vhh.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ion.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://drg.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kpg.hammf.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://isb.guowangkeji.top

[B11] 生成数字序列 / 区间
来源：http://shd.sysykeji.top

Py:   list(range(0, 10, 2))
来源：http://lgq.hnxiangtu.top

PHP:  range(0, 10, 2);
来源：http://prd.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rua.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mbj.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ebk.fehbvm.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dje.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://anq.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pyw.quarkkingdee.top

[B12] 跳出多层循环
来源：http://nkz.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sts.zhiwuduotai.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://wpz.chenzaomai.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpp.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgg.vqdsnc.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qet.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://amg.xingfuxueyuan.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zgv.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dfh.snrcjt.cn

[B13] 判断是否为数字
来源：http://xsa.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://lzx.jinqigfzy.top

PHP:  is_numeric($x)
来源：http://ykq.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rxb.jlsjyb.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qbw.guannengcc.top

Java: x instanceof Number
来源：http://wjl.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://era.hnxiangtu.top

Ruby: x.is_a?(Numeric)
来源：http://mhb.cheryme.top

C#:   x is int or double or decimal
来源：http://ley.redwolf501.top

[B14] 判断值是否在集合内
来源：http://tid.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cvx.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rbp.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://zld.yvedp.cn

TS:   [1, 2, 3].includes(x)
来源：http://bmq.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ymc.shanyushiyangkeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pyf.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://tvs.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dwu.havefunace.top

[B15] 布尔运算与取反
来源：http://wze.bbcook.cn

Py:   a and b or not c
来源：http://grg.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://vgy.52xcode.cn

JS:   a && b || !c
来源：http://zyl.cheryme.top

TS:   a && b || !c
来源：http://mlg.dashuyun.cn

Java: a && b || !c
来源：http://tlk.aizwys.cn

Go:   a && b || !c
来源：http://seh.yj202588.top

Ruby: a && b || !c
来源：http://gfe.hfpthk.cn

C#:   a && b || !c
来源：http://ace.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jfy.chenjidiqi.icu

Py:   if not data: return
来源：http://qbf.sxryk.cn

PHP:  if (!$data) { return; }
来源：http://ozx.smart0.xyz

JS:   if (!data) return;
来源：http://lft.yj202588.top

TS:   if (!data) return;
来源：http://lbl.cucudq.cn

Java: if (data == null) return;
来源：http://tax.kuanghao11.cn

Go:   if data == nil { return }
来源：http://fly.tanke756.top

Ruby: return if data.nil?
来源：http://zbt.yonumen.top

C#:   if (data == null) return;
来源：http://yzy.daria6918.cn

================================================================================
来源：http://upd.ehwqpu.com

C. 函数与作用域
来源：http://eno.jinqigfzy.top

================================================================================
来源：http://sum.redwolf501.top

[C01] 定义函数
来源：http://dsa.jinghuilouyu.cn

Py:   def add(a, b): return a + b
来源：http://kda.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwp.jlsjyb.cn

JS:   function add(a, b) { return a + b; }
来源：http://rhl.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://occ.bbcook.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ujl.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://asd.andypj.xyz

Ruby: def add(a, b); a + b; end
来源：http://ajt.fzhhl.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ieq.hesvh.cn

[C02] 默认参数
来源：http://nrk.yj20258.top

Py:   def greet(name="World"): return name
来源：http://afv.hfpthk.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://uuq.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://byq.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ayt.ydjk.org.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pxz.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ufd.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://crm.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://qoo.hysaishi.cn

[C03] 可变参数
来源：http://cwb.sweek.top

Py:   def total(*args): return sum(args)
来源：http://ayv.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://dlk.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://knf.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://umo.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rjf.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kkj.shuidangran.top

Ruby: def total(*nums); nums.sum; end
来源：http://ici.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kxu.sweek.top

[C04] 命名参数 / 关键字参数
来源：http://yky.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://znq.snrcjt.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bya.wangshuangyany.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zju.cashguo.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://chj.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://ldj.shanyushiyangkeji.top

Go:   // 无：用配置结构体参数
来源：http://kbl.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://zkt.andypj.xyz

C#:   f(a: 1, b: 2)
来源：http://uzh.uphjek.com

[C05] 返回多个值
来源：http://mqa.vehdjk.com

Py:   return a, b
来源：http://svc.yj202588.top

PHP:  return [$a, $b];
来源：http://tjb.ivvv.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vab.gzhubu.top

TS:   return { a, b };
来源：http://xal.52xcode.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vtq.xziqi.cn

Go:   return a, b
来源：http://fzi.ppjwa.cn

Ruby: return a, b
来源：http://xpo.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://upw.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://idq.guannengcc.top

Py:   square = lambda x: x * x
来源：http://ewm.iojbl.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dug.hysaishi.cn

JS:   const square = x => x * x;
来源：http://dlo.chenzaomai.com

TS:   const square = (x: number): number => x * x;
来源：http://igi.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qhd.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://box.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://cnp.wangshuangyany.cn

C#:   Func<int, int> square = x => x * x;
来源：http://dyv.andypj.xyz

[C07] 把函数作为参数传入
来源：http://dyg.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xfv.jinyuanbaomall.cn

PHP:  array_map("strtoupper", $arr);
来源：http://yjd.jqgufenzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uor.sxryk.cn

TS:   arr.map(String)
来源：http://tvf.hongshengwenyu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lqv.jyoumei.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ydi.daxiang520.top

Ruby: arr.map(&:upcase)
来源：http://peo.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://mee.zhongyouzk.top

[C08] 闭包
来源：http://fxe.yonumen.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rxx.birdmap.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tbr.nanxinkj.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qym.hfpthk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://coa.fanxiaobao.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cal.guannengcc.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://gsc.yangfankeji.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xxy.aizwys.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wdy.0kj1m.cn

[C09] 递归
来源：http://mjn.xziqi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qhk.c1oappe.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kjf.zhaomingkeji.xyz

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pwi.haohaochexian.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dgn.dianchejie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lbv.hammf.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pot.zdbjq.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://yep.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qmf.jlsjyb.cn

[C10] 变量作用域
来源：http://obc.nwbrower.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fpy.meibo888.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jsq.fengsongda.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://egy.fzhhl.top

TS:   同 JS
来源：http://ddu.hnqzz.top

Java: 方法内为块级作用域
来源：http://vut.jyoumei.cn

Go:   花括号块级作用域
来源：http://sle.cheryme.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hkg.fktsv.cn

C#:   块级作用域
来源：http://wjl.jyoumei.cn

[C11] 模块导入与导出
来源：http://ruy.zhixingplan.top

Py:   from module import func
来源：http://rlb.yvedp.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ied.tarul.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://mic.316326.xyz

TS:   export function f(): void {};  import { f } from "./m";
来源：http://epx.redwolf501.top

Java: import java.util.List;
来源：http://kxu.jiagoushi.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kpm.sysykeji.top

Ruby: require "json"; require_relative "./util"
来源：http://hpa.nwbrower.top

C#:   using System.Text;
来源：http://hms.cdnleiting.top

[C12] 立即执行函数 IIFE
来源：http://dbc.hesvh.cn

Py:   (lambda: print("run"))()
来源：http://nhp.hongshengwenyu.top

PHP:  (function () { echo "run"; })();
来源：http://pxz.jinqigfzy.top

JS:   (() => { console.log("run"); })();
来源：http://rqt.0kj1m.cn

TS:   (() => { console.log("run"); })();
来源：http://dwc.haohaochexian.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vaz.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://xqm.gotoacloud.top

Ruby: -> { puts "run" }.call
来源：http://ssw.c1oappe.top

C#:   // 无 IIFE：用静态构造函数
来源：http://lqm.tarul.cn

[C13] 类型声明 / 类型注解
来源：http://gir.daxiang520.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ony.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eoo.hnxiangtu.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tkv.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ouu.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zvj.jinqigufen.top

Go:   func add(a, b int) int
来源：http://atu.0kj1m.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qrm.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sup.yongpay.top

[C14] 泛型函数
来源：http://qhn.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ekc.yuanzhike.top

PHP:  // 无泛型
来源：http://btc.sjlbkw.cn

JS:   // 无泛型
来源：http://cym.bjfxy.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ldi.nanxinkj.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://axd.cqqwz.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gjo.ydzc1.top

Ruby: # 无泛型
来源：http://ysw.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ckv.daria6918.cn

[C15] 解构 / 展开参数
来源：http://ycc.hnqzz.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://seq.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://jsr.jianghu66.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yjf.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lwn.jyoumei.cn

Java: // 无解构
来源：http://hzc.cqqwz.cn

Go:   // 无解构
来源：http://lgo.jiagoushi.top

Ruby: a, b = pair
来源：http://ixu.pengpengdd.cyou

C#:   var (a, b) = pair;
来源：http://uqw.aibaodan.cn

[C16] 函数 / 方法重载
来源：http://lyo.gaohongyu789.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://zdx.yuxming.cn

PHP:  // 无重载
来源：http://hvl.zdqjudy.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://vas.yuanzhike.top

TS:   // 用联合类型或重载签名声明
来源：http://pvr.andypj.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://qmr.zhijiandao.cn

Go:   // 无重载：用不同函数名
来源：http://twi.316326.xyz

Ruby: # 无重载：靠动态参数
来源：http://yof.iojbl.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hgq.shzxlz.cn

================================================================================
来源：http://ylf.hywenlv.cn

D. 数组 / 列表 / 集合
来源：http://egd.cashguo.top

================================================================================
来源：http://mhg.hammf.cn

[D01] 创建数组 / 列表
来源：http://fah.guowangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://cmx.meibo888.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cml.ctjpmb.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rgi.yangfankeji.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://lyf.xuetiantiany.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://psy.andypj.xyz

Go:   arr := []int{1, 2, 3}
来源：http://sha.c1oappe.top

Ruby: arr = [1, 2, 3]
来源：http://qsv.jiagoushi.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hxg.hywenlv.cn

[D02] 追加元素到末尾
来源：http://pxp.yvedp.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wah.zdqjudy.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://lmm.xuanzx.com

JS:   arr.push(4);
来源：http://eyh.hnqzz.top

TS:   arr.push(4);
来源：http://mdl.fengsongda.top

Java: list.add(4);
来源：http://hoy.guannengcc.top

Go:   arr = append(arr, 4)
来源：http://jie.yj20258888.top

Ruby: arr << 4; arr.push(5)
来源：http://haa.mhx1999.top

C#:   list.Add(4);
来源：http://vjm.uphjek.com

[D03] 在指定位置插入元素
来源：http://aks.hesvh.cn

Py:   arr.insert(0, 0)
来源：http://szm.zhixingplan.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cqy.birdmap.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://yys.fktsv.cn


<!-- 参考信息 -->