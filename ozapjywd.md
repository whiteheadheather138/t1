代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kpk.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vpo.svipenyu.cn

[B03] switch / match / case
来源：http://wiv.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xfr.yongpay.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://luy.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bed.daxiang520.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wug.ivvv.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rfh.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nch.fanxiaobao.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ooy.mhx1999.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tkq.feifeiyinyue.top

[B04] for 计数循环
来源：http://pru.9152youxi.cn

Py:   for i in range(10): print(i)
来源：http://kds.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dxw.cashguo.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lwq.cdnleiting.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nbo.ehwqpu.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hht.shzxlz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ref.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://qzi.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wwz.yvedp.cn

[B05] 遍历数组 / 列表
来源：http://ibf.hammf.cn

Py:   for item in arr: print(item)
来源：http://rge.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://pxj.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://cjt.tian-w.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lab.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gnh.hongshengwenyu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gjl.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://ndt.daria6918.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pwv.havefunace.top

[B06] 遍历字典 / 对象
来源：http://djp.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://bli.yj202588.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vjc.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xoi.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlq.tarul.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hkm.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zfh.zhixingplan.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mwq.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cmi.epnwcf.com

[B07] while 循环
来源：http://uns.nanxinkj.top

Py:   while i < 10: i += 1
来源：http://aji.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://hjy.hammf.cn

JS:   while (i < 10) { i++; }
来源：http://rks.shanyushiyangtech.top

TS:   while (i < 10) { i++; }
来源：http://ymw.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://ydk.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rwv.shanyushiyangtech.top

Ruby: while i < 10; i += 1; end
来源：http://mdt.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://yza.yj20258.top

[B08] do-while（至少执行一次）
来源：http://hfv.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://eec.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kvc.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://uqn.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://vmk.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://zva.hcnkem.com

Go:   for { i++; if i >= 10 { break } }
来源：http://chg.yj20258888.top

Ruby: begin; i += 1; end while i < 10
来源：http://htt.hcnkem.com

C#:   do { i++; } while (i < 10);
来源：http://mlp.feifeiyinyue.top

[B09] break 与 continue
来源：http://zve.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://sti.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kos.pycfn.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plo.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttx.svipenyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svt.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zuy.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wos.yvedp.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xbj.sweek.top

[B10] 遍历同时拿索引
来源：http://ndp.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bse.shanyushiyangkeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qbw.yvedp.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fbt.0kj1m.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kez.bjfxy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bef.jlsjyb.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ebe.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://taw.hfpthk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ukd.hnqzz.top

[B11] 生成数字序列 / 区间
来源：http://tmd.jyoumei.cn

Py:   list(range(0, 10, 2))
来源：http://nwj.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://brg.xingfuxueyuan.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxz.chenjidiqi.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xgx.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tlk.smart0.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mhe.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://rpj.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eau.tanke756.top

[B12] 跳出多层循环
来源：http://ddq.aizwys.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://sde.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ert.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bdr.shzxlz.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://enj.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzk.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ejx.xylfe.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gch.aibaodan.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bxg.0kj1m.cn

[B13] 判断是否为数字
来源：http://nsp.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://yga.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://kot.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://suq.hongshengwenyu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uee.jianghu66.top

Java: x instanceof Number
来源：http://cxk.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cxn.uphjek.com

Ruby: x.is_a?(Numeric)
来源：http://ejd.chenzaomai.com

C#:   x is int or double or decimal
来源：http://vlt.smart0.xyz

[B14] 判断值是否在集合内
来源：http://ufo.uphjek.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tyo.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vgj.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://lok.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://ikz.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://psi.zhongyouzk.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://snd.xingfuxueyuan.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://azm.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vfn.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://shy.tianlin.xyz

Py:   a and b or not c
来源：http://oeg.yj20258.top

PHP:  $a && $b || !$c
来源：http://pxu.hnqzz.top

JS:   a && b || !c
来源：http://ths.wangdashe.top

TS:   a && b || !c
来源：http://dbj.tarul.cn

Java: a && b || !c
来源：http://owu.zhengqikj.top

Go:   a && b || !c
来源：http://jds.cucudq.cn

Ruby: a && b || !c
来源：http://sce.yuxming.cn

C#:   a && b || !c
来源：http://ovf.quarkkingdee.top

[B16] 卫语句：不满足条件提前返回
来源：http://vub.haohaochexian.top

Py:   if not data: return
来源：http://zcq.pycfn.com

PHP:  if (!$data) { return; }
来源：http://tsv.ybcxt.top

JS:   if (!data) return;
来源：http://etv.iojbl.cn

TS:   if (!data) return;
来源：http://lki.yongpay.top

Java: if (data == null) return;
来源：http://ozj.zhengqikj.top

Go:   if data == nil { return }
来源：http://jzv.xingfuxueyuan.xyz

Ruby: return if data.nil?
来源：http://xym.jinqigufen.top

C#:   if (data == null) return;
来源：http://jju.chenjidiqi.icu

================================================================================
来源：http://pck.cqqwz.cn

C. 函数与作用域
来源：http://oit.vehdjk.com

================================================================================
来源：http://qwr.yfazqb.com

[C01] 定义函数
来源：http://dwu.shanyushiyangtech.top

Py:   def add(a, b): return a + b
来源：http://gay.sxryk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cfi.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://dgx.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jdb.yfazqb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://wka.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jgk.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://aek.ctjpmb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eld.cdnleiting.top

[C02] 默认参数
来源：http://jlu.aizwys.cn

Py:   def greet(name="World"): return name
来源：http://ndn.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://cqe.smart0.xyz

JS:   function greet(name = "World") { return name; }
来源：http://zbc.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tjr.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://obs.xuetiantiany.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xad.kuanghao11.cn

Ruby: def greet(name = "World") = name
来源：http://ohu.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://oew.havefunace.top

[C03] 可变参数
来源：http://glt.aizwys.cn

Py:   def total(*args): return sum(args)
来源：http://jjx.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zse.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ppi.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypu.hesvh.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oso.zdqjudy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://klz.52xcode.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vdr.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://evm.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://tjl.birdmap.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://oik.shanyushiyangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://yhl.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lrf.meibo888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://cer.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://sgc.meibo888.top

Go:   // 无：用配置结构体参数
来源：http://wro.haohaochexian.top

Ruby: f(a: 1, b: 2)
来源：http://mth.yueranfly.top

C#:   f(a: 1, b: 2)
来源：http://xhe.cqqwz.cn

[C05] 返回多个值
来源：http://kpt.shuidangran.top

Py:   return a, b
来源：http://bau.jqgfzy.top

PHP:  return [$a, $b];
来源：http://fxa.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wlg.ydzc1.top

TS:   return { a, b };
来源：http://oew.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vkw.cucudq.cn

Go:   return a, b
来源：http://jhr.hongshengwenyu.top

Ruby: return a, b
来源：http://ejp.jinqigfzy.top

C#:   return (a, b);              // ValueTuple
来源：http://awl.chenlongwang.top

[C06] 匿名函数 / lambda
来源：http://dip.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://mws.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://mjo.hnqzz.top

JS:   const square = x => x * x;
来源：http://alm.svipenyu.cn

TS:   const square = (x: number): number => x * x;
来源：http://xgt.bbcook.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ofe.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://bjd.yonumen.top

Ruby: square = ->(x) { x * x }
来源：http://cnb.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://kgp.sufxvd.cn

[C07] 把函数作为参数传入
来源：http://kyn.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lrk.tanke756.top

PHP:  array_map("strtoupper", $arr);
来源：http://uuk.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xkh.jinqigufen.top

TS:   arr.map(String)
来源：http://eor.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://fta.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wje.bbcook.cn

Ruby: arr.map(&:upcase)
来源：http://eri.fktsv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aru.gotoacloud.top

[C08] 闭包
来源：http://jze.yangfankeji.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://del.daria6918.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ejs.quarkkingdee.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cdx.dianchejie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://uwl.jiagoushi.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uik.cucudq.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dzz.zdbjq.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://che.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zrx.zhoulong.xyz

[C09] 递归
来源：http://knt.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://czk.nwbrower.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ben.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iag.tian-w.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nyt.ctjpmb.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tsw.jianghu66.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hsz.dashuyun.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jrf.yanxiufei.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qrf.shanyushiyangkeji.top

[C10] 变量作用域
来源：http://ueb.tianlin.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gcg.epnwcf.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zda.zhixingplan.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sev.daria6918.cn

TS:   同 JS
来源：http://vdg.shanyushiyangkeji.top

Java: 方法内为块级作用域
来源：http://rei.ctjpmb.com

Go:   花括号块级作用域
来源：http://czp.jiagoushi.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qyt.epnwcf.com

C#:   块级作用域
来源：http://wdd.tian-w.cn

[C11] 模块导入与导出
来源：http://fed.xziqi.cn

Py:   from module import func
来源：http://ixi.tanke756.top

PHP:  require "file.php";  或 use App\Service;
来源：http://sks.zdqjudy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://jxw.hnqzz.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ozc.cucudq.cn

Java: import java.util.List;
来源：http://vme.sysykeji.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jxc.ywan-chungtsiang.top

Ruby: require "json"; require_relative "./util"
来源：http://zik.redwolf501.top

C#:   using System.Text;
来源：http://ohc.cheryme.top

[C12] 立即执行函数 IIFE
来源：http://qre.iojbl.cn

Py:   (lambda: print("run"))()
来源：http://nay.hesvh.cn

PHP:  (function () { echo "run"; })();
来源：http://uil.chenjidiqi.icu

JS:   (() => { console.log("run"); })();
来源：http://obk.yfazqb.com

TS:   (() => { console.log("run"); })();
来源：http://bwt.52xcode.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://sxz.ivvv.top

Go:   func() { fmt.Println("run") }()
来源：http://bha.gaohongyu789.top

Ruby: -> { puts "run" }.call
来源：http://ngt.yuanzhike.top

C#:   // 无 IIFE：用静态构造函数
来源：http://tgp.nanxuanxn.top

[C13] 类型声明 / 类型注解
来源：http://tyy.yvedp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jjp.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rnr.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xdv.wangdashe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vej.tanke756.top

Java: int add(int a, int b) { return a + b; }
来源：http://icq.gzhubu.top

Go:   func add(a, b int) int
来源：http://dhn.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://zwb.mhx1999.top

C#:   int Add(int a, int b) => a + b;
来源：http://neq.daria6918.cn

[C14] 泛型函数
来源：http://eai.bjfxy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://smq.zycfv.cn

PHP:  // 无泛型
来源：http://aiz.zycfv.cn

JS:   // 无泛型
来源：http://ccc.quarkkingdee.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yzy.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://bxi.hnqzz.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rrw.cdnleiting.top

Ruby: # 无泛型
来源：http://roo.jqgfzy.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://clp.daria6918.cn

[C15] 解构 / 展开参数
来源：http://dex.yanxiufei.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xkb.gotoacloud.top

PHP:  [$a, $b] = $pair;
来源：http://ibl.fktsv.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gie.zhaomingkeji.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gyg.nwbrower.top

Java: // 无解构
来源：http://vdb.sxryk.cn

Go:   // 无解构
来源：http://fsj.xziqi.cn

Ruby: a, b = pair
来源：http://sox.sweek.top

C#:   var (a, b) = pair;
来源：http://niz.zhixingplan.top

[C16] 函数 / 方法重载
来源：http://lvg.zycfv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xkl.gogol.net.cn

PHP:  // 无重载
来源：http://gwk.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://yqo.jinqigfzy.top

TS:   // 用联合类型或重载签名声明
来源：http://who.fzhhl.top

Java: void f(int a) {}  void f(String a) {}
来源：http://lxl.hcnkem.com

Go:   // 无重载：用不同函数名
来源：http://nai.jyoumei.cn

Ruby: # 无重载：靠动态参数
来源：http://yhb.ydzc1.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://pro.yongpay.top

================================================================================
来源：http://nld.yueranfly.top

D. 数组 / 列表 / 集合
来源：http://xwt.jlsjyb.cn

================================================================================
来源：http://xdk.dashuyun.cn

[D01] 创建数组 / 列表
来源：http://aop.nanxuanxn.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dud.shanyushiyangkeji.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tkh.fktsv.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jmg.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://miu.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://juz.ywan-chungtsiang.top

Go:   arr := []int{1, 2, 3}
来源：http://ktb.aibaodan.cn

Ruby: arr = [1, 2, 3]
来源：http://bbz.xingfuxueyuan.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://aij.sjlbkw.cn

[D02] 追加元素到末尾
来源：http://stl.hywenlv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bvr.jinqigufen.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ptl.jinghuilouyu.cn

JS:   arr.push(4);
来源：http://jfp.fehbvm.com

TS:   arr.push(4);
来源：http://nrz.jinghuilouyu.cn

Java: list.add(4);
来源：http://hdc.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://aum.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://gxt.hysaishi.cn

C#:   list.Add(4);
来源：http://mun.sweek.top

[D03] 在指定位置插入元素
来源：http://rls.xziqi.cn

Py:   arr.insert(0, 0)
来源：http://xjg.xinyue.icu

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://nlw.gogol.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fkr.mhx1999.top


<!-- 参考信息 -->