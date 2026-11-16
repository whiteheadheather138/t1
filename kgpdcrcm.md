代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oat.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://psu.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xzu.shuidangran.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://noe.jinqigfzy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bdl.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cdq.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mqe.hongshengwenyu.top

[B04] for 计数循环
来源：http://nta.316326.xyz

Py:   for i in range(10): print(i)
来源：http://utl.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://arc.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sfd.epnwcf.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bzw.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mow.nwbrower.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rnw.jianghu66.top

Ruby: 10.times { |i| puts i }
来源：http://kzr.0kj1m.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cde.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://lag.fzhhl.top

Py:   for item in arr: print(item)
来源：http://sia.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fxk.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nih.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hxy.jinqigfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ais.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mdj.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://pnp.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://swz.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://sgn.shangyingyoupin.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bhw.zhiwuduotai.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qck.feifeiyinyue.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ppz.zhixingplan.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://csb.jqgufenzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dyt.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ipg.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uqc.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xrk.jyoumei.cn

[B07] while 循环
来源：http://zbg.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://nph.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://pxa.birdmap.top

JS:   while (i < 10) { i++; }
来源：http://kwt.0kj1m.cn

TS:   while (i < 10) { i++; }
来源：http://osg.fzhhl.top

Java: while (i < 10) { i++; }
来源：http://mjm.jqgufenzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kod.chenjidiqi.icu

Ruby: while i < 10; i += 1; end
来源：http://yvg.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://hcy.smart0.xyz

[B08] do-while（至少执行一次）
来源：http://bih.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://czc.nwbrower.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rgs.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://pbn.hcnkem.com

TS:   do { i++; } while (i < 10);
来源：http://twt.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://deq.jyoumei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gzq.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://qwg.nanxinkj.top

C#:   do { i++; } while (i < 10);
来源：http://jin.9152youxi.cn

[B09] break 与 continue
来源：http://nqb.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pvy.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fgs.sxryk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zux.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxq.cqqwz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyf.shzxlz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xhb.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sjg.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arg.fehbvm.com

[B10] 遍历同时拿索引
来源：http://hwy.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://oiv.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yow.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uju.yj20258.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ewt.cucudq.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uta.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sks.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bwb.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qzd.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://svw.nanxuanxn.top

Py:   list(range(0, 10, 2))
来源：http://ict.ivvv.top

PHP:  range(0, 10, 2);
来源：http://fju.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zmh.iojbl.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cpm.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mba.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eni.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://csm.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://trs.yonumen.top

[B12] 跳出多层循环
来源：http://vhf.bbcook.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://dux.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://dai.bjfxy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrr.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://szn.ivvv.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://oxs.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fwj.hfpthk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jmm.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pxq.jqgfzy.top

[B13] 判断是否为数字
来源：http://vfg.ybcxt.top

Py:   isinstance(x, (int, float))
来源：http://yrp.zdbjq.cn

PHP:  is_numeric($x)
来源：http://epx.cashguo.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://flu.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ofq.snrcjt.cn

Java: x instanceof Number
来源：http://lle.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://csl.sjlbkw.cn

Ruby: x.is_a?(Numeric)
来源：http://drs.jinyuanbaomall.cn

C#:   x is int or double or decimal
来源：http://dal.zhoulong.xyz

[B14] 判断值是否在集合内
来源：http://ipy.ydzc1.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ewt.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rzu.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://lld.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://pue.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ttn.hfpthk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yfl.quarkkingdee.top

Ruby: [1, 2, 3].include?(x)
来源：http://dki.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wyk.aizwys.cn

[B15] 布尔运算与取反
来源：http://qih.sxryk.cn

Py:   a and b or not c
来源：http://jzj.hcnkem.com

PHP:  $a && $b || !$c
来源：http://upm.chenzaomai.com

JS:   a && b || !c
来源：http://byw.yanxiufei.cn

TS:   a && b || !c
来源：http://kil.shanyushiyangkeji.top

Java: a && b || !c
来源：http://sjq.gaohongyu789.top

Go:   a && b || !c
来源：http://lam.sweek.top

Ruby: a && b || !c
来源：http://wpn.tianlin.xyz

C#:   a && b || !c
来源：http://mqp.kuanghao11.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ngh.yueranfly.top

Py:   if not data: return
来源：http://tpn.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://kiq.tarul.cn

JS:   if (!data) return;
来源：http://vzi.gaohongyu789.top

TS:   if (!data) return;
来源：http://oug.dianchejie.cn

Java: if (data == null) return;
来源：http://mzp.daria6918.cn

Go:   if data == nil { return }
来源：http://fqd.jianghu66.top

Ruby: return if data.nil?
来源：http://jgo.meibo888.top

C#:   if (data == null) return;
来源：http://jpl.svipenyu.cn

================================================================================
来源：http://hmb.fengsongda.top

C. 函数与作用域
来源：http://fda.yangfankeji.com

================================================================================
来源：http://obw.cucudq.cn

[C01] 定义函数
来源：http://znc.zycfv.cn

Py:   def add(a, b): return a + b
来源：http://olt.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cui.yfazqb.com

JS:   function add(a, b) { return a + b; }
来源：http://yrz.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uio.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nlt.gogol.net.cn

Go:   func add(a, b int) int { return a + b }
来源：http://fww.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://afs.ivvv.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ull.ydzc1.top

[C02] 默认参数
来源：http://rev.zycfv.cn

Py:   def greet(name="World"): return name
来源：http://dnc.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pmj.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://tsd.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cfu.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pfc.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jfz.zhengqikj.top

Ruby: def greet(name = "World") = name
来源：http://los.wangdashe.top

C#:   string Greet(string name = "World") => name;
来源：http://umz.ivvv.top

[C03] 可变参数
来源：http://qhk.yongpay.top

Py:   def total(*args): return sum(args)
来源：http://sfd.chenzaomai.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ntx.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vqx.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iln.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kjk.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yxh.cdnleiting.top

Ruby: def total(*nums); nums.sum; end
来源：http://ain.yj202588.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://vtj.uphjek.com

[C04] 命名参数 / 关键字参数
来源：http://obe.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://grr.dianchejie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://avq.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lek.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://npv.meibo888.top

Java: // 无：用 Builder 模式或 record
来源：http://hdg.yuxming.cn

Go:   // 无：用配置结构体参数
来源：http://fjs.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://ifq.yfazqb.com

C#:   f(a: 1, b: 2)
来源：http://swj.bjfxy.top

[C05] 返回多个值
来源：http://xng.yj20258.top

Py:   return a, b
来源：http://kho.yueranfly.top

PHP:  return [$a, $b];
来源：http://wgo.redwolf501.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dsl.zhijiandao.cn

TS:   return { a, b };
来源：http://ozr.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hwx.havefunace.top

Go:   return a, b
来源：http://zab.ydzc1.top

Ruby: return a, b
来源：http://jyl.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://qal.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://gnf.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://dut.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sxe.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://xht.yuxming.cn

TS:   const square = (x: number): number => x * x;
来源：http://xks.nwbrower.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xjg.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://asw.zhongyouzk.top

Ruby: square = ->(x) { x * x }
来源：http://cay.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://yff.chenzaomai.com

[C07] 把函数作为参数传入
来源：http://vva.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wsx.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://nzo.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://itu.gaohongyu789.top

TS:   arr.map(String)
来源：http://ynr.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nlq.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ena.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://anq.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://hgn.hfpthk.cn

[C08] 闭包
来源：http://tzi.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://pkk.fengsongda.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://odk.fzhhl.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pjh.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lie.ctjpmb.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://due.dashuyun.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zmr.zhoulong.xyz

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://lld.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wet.wangshuangyany.cn

[C09] 递归
来源：http://qmn.sysykeji.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://skn.yongpay.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://svw.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vgm.zhijiandao.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ynt.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vwl.yonumen.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://apb.hnxiangtu.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zye.pengpengdd.cyou

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ypi.uphjek.com

[C10] 变量作用域
来源：http://apz.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kqg.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fyz.bjfxy.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tsv.yuxming.cn

TS:   同 JS
来源：http://uec.vqdsnc.cn

Java: 方法内为块级作用域
来源：http://xsq.sjlbkw.cn

Go:   花括号块级作用域
来源：http://iuk.vehdjk.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://piq.ppjwa.cn

C#:   块级作用域
来源：http://hls.yj20258.top

[C11] 模块导入与导出
来源：http://ant.hysaishi.cn

Py:   from module import func
来源：http://vrd.ybcxt.top

PHP:  require "file.php";  或 use App\Service;
来源：http://qvy.jqgfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yab.shuidangran.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mpd.feifeiyinyue.top

Java: import java.util.List;
来源：http://frw.xinyue.icu

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://iom.cqqwz.cn

Ruby: require "json"; require_relative "./util"
来源：http://lca.yongpay.top

C#:   using System.Text;
来源：http://wha.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://lcg.xingfuxueyuan.xyz

Py:   (lambda: print("run"))()
来源：http://ygy.ctjpmb.com

PHP:  (function () { echo "run"; })();
来源：http://hqp.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://hku.jyoumei.cn

TS:   (() => { console.log("run"); })();
来源：http://lzz.yj202588.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vlw.gaohongyu789.top

Go:   func() { fmt.Println("run") }()
来源：http://uqg.0kj1m.cn

Ruby: -> { puts "run" }.call
来源：http://suk.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://jna.hongshengwenyu.top

[C13] 类型声明 / 类型注解
来源：http://sfr.xinyue.icu

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zzs.pycfn.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfl.cashguo.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ctb.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://veq.0kj1m.cn

Java: int add(int a, int b) { return a + b; }
来源：http://hus.yuxming.cn

Go:   func add(a, b int) int
来源：http://eis.kuanghao11.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sot.xuanzx.com

C#:   int Add(int a, int b) => a + b;
来源：http://dkc.jinqigfzy.top

[C14] 泛型函数
来源：http://yzq.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mbo.hcnkem.com

PHP:  // 无泛型
来源：http://uss.chenjidiqi.icu

JS:   // 无泛型
来源：http://rvw.gaohongyu789.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ptz.yfazqb.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://odu.guannengcc.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jjk.xuetiantiany.cn

Ruby: # 无泛型
来源：http://gmr.yueranfly.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qst.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://nqn.yj20258888.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://grd.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://eou.shanyushiyangtech.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tql.nanxinkj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://stw.cqqwz.cn

Java: // 无解构
来源：http://pqe.haohaochexian.top

Go:   // 无解构
来源：http://ybg.xingfuxueyuan.xyz

Ruby: a, b = pair
来源：http://tru.fktsv.cn

C#:   var (a, b) = pair;
来源：http://tku.nanxinkj.top

[C16] 函数 / 方法重载
来源：http://nsx.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://doc.nanxinkj.top

PHP:  // 无重载
来源：http://lri.zhijiandao.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://san.xingfuxueyuan.xyz

TS:   // 用联合类型或重载签名声明
来源：http://qsr.gogol.net.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://sbl.jinqigufen.top

Go:   // 无重载：用不同函数名
来源：http://dqc.pengpengdd.cyou

Ruby: # 无重载：靠动态参数
来源：http://ujn.ywan-chungtsiang.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://hmu.quarkkingdee.top

================================================================================
来源：http://aot.zhaomingkeji.xyz

D. 数组 / 列表 / 集合
来源：http://nsj.yj20258888.top

================================================================================
来源：http://zgi.haohaochexian.top

[D01] 创建数组 / 列表
来源：http://bzi.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://qpt.havefunace.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kax.iojbl.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vkg.smart0.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://uld.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qzx.tianlin.xyz

Go:   arr := []int{1, 2, 3}
来源：http://top.kuanghao11.cn

Ruby: arr = [1, 2, 3]
来源：http://knn.cqqwz.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://udx.yuxming.cn

[D02] 追加元素到末尾
来源：http://gmq.fzhhl.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://oao.hnxiangtu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://gow.yonumen.top

JS:   arr.push(4);
来源：http://qcr.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://fgx.andypj.xyz

Java: list.add(4);
来源：http://exl.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://vuk.cdnleiting.top

Ruby: arr << 4; arr.push(5)
来源：http://cap.guannengcc.top

C#:   list.Add(4);
来源：http://vxz.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://lhb.zycfv.cn

Py:   arr.insert(0, 0)
来源：http://eyv.sufxvd.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hbq.jlsjyb.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nyq.gaohongyu789.top

TS:   arr.splice(0, 0, 0);
来源：http://mdc.nwbrower.top

Java: list.add(0, 0);
来源：http://okn.hnxiangtu.top

Go:   arr = append([]int{0}, arr...)
来源：http://gwj.havefunace.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iff.yangfankeji.com


<!-- 参考信息 -->