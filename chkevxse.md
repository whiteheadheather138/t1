代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://afu.0kj1m.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fpu.ivvv.top

[B03] switch / match / case
来源：http://axo.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://amd.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lbm.jinghuilouyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uov.fzhhl.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ccm.jinghuilouyu.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lyy.sjlbkw.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wfx.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ngz.shanyushiyangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://svo.ydzc1.top

[B04] for 计数循环
来源：http://hhi.ybcxt.top

Py:   for i in range(10): print(i)
来源：http://ocd.chenzaomai.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vnt.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://coj.ybcxt.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fwa.havefunace.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://etk.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ozg.cheryme.top

Ruby: 10.times { |i| puts i }
来源：http://okk.shanyushiyangtech.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cqp.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://lcd.tian-w.cn

Py:   for item in arr: print(item)
来源：http://xse.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gfe.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://grb.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yiy.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hho.ywan-chungtsiang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bff.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://hwh.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fmz.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://kta.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://iac.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xno.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://php.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dmg.c1oappe.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xed.fanxiaobao.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fdh.epnwcf.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jvl.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wmo.haohaochexian.top

[B07] while 循环
来源：http://tok.tarul.cn

Py:   while i < 10: i += 1
来源：http://tyb.dashuyun.cn

PHP:  while ($i < 10) { $i++; }
来源：http://cqm.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://oxc.havefunace.top

TS:   while (i < 10) { i++; }
来源：http://hfv.pycfn.com

Java: while (i < 10) { i++; }
来源：http://ovs.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rng.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://dkr.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://ubc.tian-w.cn

[B08] do-while（至少执行一次）
来源：http://vmi.ppjwa.cn

Py:   # 无 do-while：用 while True + break
来源：http://uns.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://uzl.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://amr.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://xyv.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://pum.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kna.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dun.hfpthk.cn

C#:   do { i++; } while (i < 10);
来源：http://jwm.zycfv.cn

[B09] break 与 continue
来源：http://icm.andypj.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mtz.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ztn.tianlin.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://suc.hywenlv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://okf.shuidangran.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yst.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://doc.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iih.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cll.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://wot.chenlongwang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yqk.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lzb.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nex.iojbl.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ycq.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://puw.jqgfzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aiz.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hci.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ngg.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://uto.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://cix.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://kea.zdbjq.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://skm.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://foc.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aep.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mis.c1oappe.top

Ruby: (0...10).step(2).to_a
来源：http://gfj.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bmj.shzxlz.cn

[B12] 跳出多层循环
来源：http://dst.jinqigufen.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qij.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://izn.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wah.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bps.chenzaomai.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yam.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gcx.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nhj.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hlf.nanxinkj.top

[B13] 判断是否为数字
来源：http://paw.daria6918.cn

Py:   isinstance(x, (int, float))
来源：http://pmg.zhixingplan.top

PHP:  is_numeric($x)
来源：http://iqk.yuanzhike.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgv.c1oappe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://alj.aizwys.cn

Java: x instanceof Number
来源：http://ijy.fengsongda.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://epm.cdnleiting.top

Ruby: x.is_a?(Numeric)
来源：http://fyz.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://yur.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://hxr.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uns.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://djo.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://sfp.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://sjx.yonumen.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mgo.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://swv.epnwcf.com

Ruby: [1, 2, 3].include?(x)
来源：http://dbz.smart0.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jll.vqdsnc.cn

[B15] 布尔运算与取反
来源：http://ifd.hongshengwenyu.top

Py:   a and b or not c
来源：http://sky.c1oappe.top

PHP:  $a && $b || !$c
来源：http://gqx.ivvv.top

JS:   a && b || !c
来源：http://txy.yj20258.top

TS:   a && b || !c
来源：http://vfn.zhiwuduotai.top

Java: a && b || !c
来源：http://xnq.zhoulong.xyz

Go:   a && b || !c
来源：http://udy.fehbvm.com

Ruby: a && b || !c
来源：http://kwt.sxryk.cn

C#:   a && b || !c
来源：http://suq.52xcode.cn

[B16] 卫语句：不满足条件提前返回
来源：http://btp.feifeiyinyue.top

Py:   if not data: return
来源：http://nvh.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://brl.hammf.cn

JS:   if (!data) return;
来源：http://way.tian-w.cn

TS:   if (!data) return;
来源：http://mcl.kuanghao11.cn

Java: if (data == null) return;
来源：http://ujk.316326.xyz

Go:   if data == nil { return }
来源：http://coa.yangfankeji.com

Ruby: return if data.nil?
来源：http://bdo.hfpthk.cn

C#:   if (data == null) return;
来源：http://rdc.cheryme.top

================================================================================
来源：http://vak.yvedp.cn

C. 函数与作用域
来源：http://pgn.zhijiandao.cn

================================================================================
来源：http://oaz.jinqigufen.top

[C01] 定义函数
来源：http://rzb.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://npd.guannengcc.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cqm.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://jpv.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jvm.316326.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wrj.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eil.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://szh.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://sdu.hammf.cn

[C02] 默认参数
来源：http://vto.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://tjf.tanke756.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wqz.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://dhg.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ffc.zhoulong.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://smn.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ais.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://thq.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://ald.aibaodan.cn

[C03] 可变参数
来源：http://sgu.shanyushiyangkeji.top

Py:   def total(*args): return sum(args)
来源：http://aqc.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bcu.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ooz.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pqq.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zlx.fanxiaobao.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kgd.ctjpmb.com

Ruby: def total(*nums); nums.sum; end
来源：http://saf.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rlq.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://byo.316326.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rdc.chenzaomai.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gdu.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ryx.zhiwuduotai.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tcx.daxiang520.top

Java: // 无：用 Builder 模式或 record
来源：http://bgp.yuanzhike.top

Go:   // 无：用配置结构体参数
来源：http://aiw.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://zof.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://ria.yueranfly.top

[C05] 返回多个值
来源：http://xvu.yfazqb.com

Py:   return a, b
来源：http://wsv.tarul.cn

PHP:  return [$a, $b];
来源：http://cop.dashuyun.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://gqg.hongshengwenyu.top

TS:   return { a, b };
来源：http://bdd.shangyingyoupin.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gta.tianlin.xyz

Go:   return a, b
来源：http://zdw.jqgfzy.top

Ruby: return a, b
来源：http://lrb.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://cnt.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://sip.cdnleiting.top

Py:   square = lambda x: x * x
来源：http://ybk.jinghuilouyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fes.hnqzz.top

JS:   const square = x => x * x;
来源：http://fvg.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://mlv.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fds.yvedp.cn

Go:   sq := func(x int) int { return x * x }
来源：http://wdb.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://xbu.jqgfzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://kmh.bbcook.cn

[C07] 把函数作为参数传入
来源：http://wqq.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vss.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://rlq.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://sto.yueranfly.top

TS:   arr.map(String)
来源：http://gng.sxryk.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xtx.guowangkeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qaa.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://pdy.tarul.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gxv.zhixingplan.top

[C08] 闭包
来源：http://ekc.fengsongda.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hfw.yuanzhike.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jih.c1oappe.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://uuz.ywan-chungtsiang.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mmg.andypj.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tsr.yuanzhike.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bip.xziqi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hsa.smart0.xyz

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://obr.jinyuanbaomall.cn

[C09] 递归
来源：http://hyg.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bhm.snrcjt.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://unc.ydzc1.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fin.sjlbkw.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fgq.zhijiandao.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://crn.yongpay.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://izi.ydjk.org.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ohj.fengsongda.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://gte.ehwqpu.com

[C10] 变量作用域
来源：http://fvf.feifeiyinyue.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://bqh.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zes.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://yzj.chenzaomai.com

TS:   同 JS
来源：http://kbj.jinghuilouyu.cn

Java: 方法内为块级作用域
来源：http://nhj.wangdashe.top

Go:   花括号块级作用域
来源：http://ksf.jyoumei.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://olq.zhaomingkeji.xyz

C#:   块级作用域
来源：http://pfn.fktsv.cn

[C11] 模块导入与导出
来源：http://bdq.cashguo.top

Py:   from module import func
来源：http://nix.smart0.xyz

PHP:  require "file.php";  或 use App\Service;
来源：http://nwa.ppjwa.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://int.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vjk.xuetiantiany.cn

Java: import java.util.List;
来源：http://efz.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sdy.jinqigfzy.top

Ruby: require "json"; require_relative "./util"
来源：http://eqf.zhengqikj.top

C#:   using System.Text;
来源：http://bja.jqgufenzy.top

[C12] 立即执行函数 IIFE
来源：http://efy.jqgufenzy.top

Py:   (lambda: print("run"))()
来源：http://qew.yj20258888.top

PHP:  (function () { echo "run"; })();
来源：http://cec.sjlbkw.cn

JS:   (() => { console.log("run"); })();
来源：http://dml.ydjk.org.cn

TS:   (() => { console.log("run"); })();
来源：http://lyk.nanxinkj.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kkl.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://rsj.yj202588.top

Ruby: -> { puts "run" }.call
来源：http://szx.shangyingyoupin.top

C#:   // 无 IIFE：用静态构造函数
来源：http://zrk.epnwcf.com

[C13] 类型声明 / 类型注解
来源：http://zhi.chenlongwang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zwx.zhijiandao.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://osx.dashuyun.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vmi.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kqv.cucudq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pns.9152youxi.cn

Go:   func add(a, b int) int
来源：http://hms.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rzl.cqqwz.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cbo.hnxiangtu.top

[C14] 泛型函数
来源：http://vut.nanxinkj.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gwu.xinyue.icu

PHP:  // 无泛型
来源：http://vtn.zycfv.cn

JS:   // 无泛型
来源：http://jqd.ywan-chungtsiang.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fzz.hesvh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ltl.sxryk.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bxo.yj20258.top

Ruby: # 无泛型
来源：http://yok.sweek.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://alt.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://arr.vehdjk.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dut.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://hzg.cashguo.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://myb.xziqi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://toa.dianchejie.cn

Java: // 无解构
来源：http://vvz.shanyushiyangkeji.top

Go:   // 无解构
来源：http://sig.tarul.cn

Ruby: a, b = pair
来源：http://kwm.vehdjk.com

C#:   var (a, b) = pair;
来源：http://qdv.uphjek.com

[C16] 函数 / 方法重载
来源：http://bsp.fanxiaobao.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pbw.wangdashe.top

PHP:  // 无重载
来源：http://bus.andypj.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://pkj.meibo888.top

TS:   // 用联合类型或重载签名声明
来源：http://nxl.zycfv.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://izn.tianlin.xyz

Go:   // 无重载：用不同函数名
来源：http://hno.zycfv.cn

Ruby: # 无重载：靠动态参数
来源：http://zcg.jiagoushi.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://bqj.smart0.xyz

================================================================================
来源：http://rgu.mhx1999.top

D. 数组 / 列表 / 集合
来源：http://pqu.hnqzz.top

================================================================================
来源：http://jes.fktsv.cn

[D01] 创建数组 / 列表
来源：http://rfl.shanyushiyangtech.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fbh.yonumen.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tgj.wangdashe.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkk.jinqigufen.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lhz.jinqigfzy.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ebx.svipenyu.cn

Go:   arr := []int{1, 2, 3}
来源：http://pdf.cashguo.top

Ruby: arr = [1, 2, 3]
来源：http://yff.shangyingyoupin.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xoc.epnwcf.com

[D02] 追加元素到末尾
来源：http://mcs.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ctd.9152youxi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xly.zycfv.cn

JS:   arr.push(4);
来源：http://jhm.zhiwuduotai.top

TS:   arr.push(4);
来源：http://xrb.zhiwuduotai.top

Java: list.add(4);
来源：http://wkt.hnxiangtu.top

Go:   arr = append(arr, 4)
来源：http://mqt.shangyingyoupin.top

Ruby: arr << 4; arr.push(5)
来源：http://igp.aibaodan.cn

C#:   list.Add(4);
来源：http://kyz.chenjidiqi.icu

[D03] 在指定位置插入元素
来源：http://zyy.vqdsnc.cn

Py:   arr.insert(0, 0)
来源：http://qxa.daria6918.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ert.zycfv.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kef.ctjpmb.com


<!-- 参考信息 -->