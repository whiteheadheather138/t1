代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://phr.jianghu66.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnt.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dza.dianchejie.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ttk.hysaishi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xmd.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ptb.gaohongyu789.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lfx.cashguo.top

[B04] for 计数循环
来源：http://ibm.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://sca.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hma.cqqwz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zup.ehwqpu.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ncn.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hke.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://pej.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://gwf.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nrc.gaohongyu789.top

[B05] 遍历数组 / 列表
来源：http://wkt.cucudq.cn

Py:   for item in arr: print(item)
来源：http://fpq.0kj1m.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bji.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ryo.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fup.yj202588.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://mjg.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kqa.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://ioi.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cdb.havefunace.top

[B06] 遍历字典 / 对象
来源：http://amy.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://luw.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://osa.shanyushiyangtech.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zss.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pnp.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fpi.zhaomingkeji.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jth.fzhhl.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qhb.0kj1m.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wol.jqgufenzy.top

[B07] while 循环
来源：http://eyv.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://fai.zdqjudy.top

PHP:  while ($i < 10) { $i++; }
来源：http://stc.shuidangran.top

JS:   while (i < 10) { i++; }
来源：http://tvo.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://ein.svipenyu.cn

Java: while (i < 10) { i++; }
来源：http://xsi.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bpr.zhaomingkeji.xyz

Ruby: while i < 10; i += 1; end
来源：http://xrq.dashuyun.cn

C#:   while (i < 10) { i++; }
来源：http://pib.wangshuangyany.cn

[B08] do-while（至少执行一次）
来源：http://qgh.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://yfx.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://vzw.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://jnz.ydzc1.top

TS:   do { i++; } while (i < 10);
来源：http://brm.cqqwz.cn

Java: do { i++; } while (i < 10);
来源：http://ioy.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yib.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://yjj.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://jhu.zhijiandao.cn

[B09] break 与 continue
来源：http://mrh.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wyb.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wbj.meibo888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wqs.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mkf.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vss.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://htt.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vch.guowangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nni.52xcode.cn

[B10] 遍历同时拿索引
来源：http://yrd.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://njt.quarkkingdee.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://upf.chenlongwang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qfj.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jsq.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://puv.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mfk.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wqe.jlsjyb.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tlp.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://jwp.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://ice.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://xfz.birdmap.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lxa.shanyushiyangkeji.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://opc.gzhubu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hwl.ydjk.org.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vsl.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://zyx.nanxinkj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qeg.tarul.cn

[B12] 跳出多层循环
来源：http://iuu.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://nct.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://osq.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ces.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://swn.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lhj.zhixingplan.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ope.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mgj.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rnp.cdnleiting.top

[B13] 判断是否为数字
来源：http://leu.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://fbc.vehdjk.com

PHP:  is_numeric($x)
来源：http://rer.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sjn.cucudq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://leg.birdmap.top

Java: x instanceof Number
来源：http://tei.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://kfi.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://eto.gzhubu.top

C#:   x is int or double or decimal
来源：http://tot.cucudq.cn

[B14] 判断值是否在集合内
来源：http://nmw.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nju.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upb.xziqi.cn

JS:   [1, 2, 3].includes(x)
来源：http://umo.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://kit.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://vwx.jinqigfzy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aom.daria6918.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qio.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xhz.yj202588.top

[B15] 布尔运算与取反
来源：http://pjz.ydjk.org.cn

Py:   a and b or not c
来源：http://yvh.tarul.cn

PHP:  $a && $b || !$c
来源：http://mtp.sysykeji.top

JS:   a && b || !c
来源：http://zjd.jyoumei.cn

TS:   a && b || !c
来源：http://ilu.shangyingyoupin.top

Java: a && b || !c
来源：http://yfo.zhijiandao.cn

Go:   a && b || !c
来源：http://whf.aibaodan.cn

Ruby: a && b || !c
来源：http://yas.dashuyun.cn

C#:   a && b || !c
来源：http://mhp.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://ari.yj202588.top

Py:   if not data: return
来源：http://qgv.jyoumei.cn

PHP:  if (!$data) { return; }
来源：http://due.hesvh.cn

JS:   if (!data) return;
来源：http://uod.gotoacloud.top

TS:   if (!data) return;
来源：http://gma.ivvv.top

Java: if (data == null) return;
来源：http://czp.cucudq.cn

Go:   if data == nil { return }
来源：http://uze.hysaishi.cn

Ruby: return if data.nil?
来源：http://zky.yfazqb.com

C#:   if (data == null) return;
来源：http://gfi.dashuyun.cn

================================================================================
来源：http://dax.xziqi.cn

C. 函数与作用域
来源：http://xvg.fzhhl.top

================================================================================
来源：http://mtg.smart0.xyz

[C01] 定义函数
来源：http://zgq.chenzaomai.com

Py:   def add(a, b): return a + b
来源：http://ewd.xylfe.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://acc.zhengqikj.top

JS:   function add(a, b) { return a + b; }
来源：http://vko.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xpv.smart0.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://mfs.cqqwz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eaq.xylfe.cn

Ruby: def add(a, b); a + b; end
来源：http://bph.hnqzz.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kyq.gaohongyu789.top

[C02] 默认参数
来源：http://xks.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://lzm.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yvl.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://yhw.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://oec.vqdsnc.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ovj.cdnleiting.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vpi.ywan-chungtsiang.top

Ruby: def greet(name = "World") = name
来源：http://kif.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://etu.daxiang520.top

[C03] 可变参数
来源：http://qsg.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://ujt.xziqi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gai.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://upf.gaohongyu789.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gyn.jqgfzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fjb.yanxiufei.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://bth.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://ajw.cdnleiting.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://anp.ehwqpu.com

[C04] 命名参数 / 关键字参数
来源：http://ymi.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mec.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gqt.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dxk.uphjek.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dye.yueranfly.top

Java: // 无：用 Builder 模式或 record
来源：http://mva.fengsongda.top

Go:   // 无：用配置结构体参数
来源：http://gsx.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://zmv.sweek.top

C#:   f(a: 1, b: 2)
来源：http://yts.shanyushiyangtech.top

[C05] 返回多个值
来源：http://ncg.guannengcc.top

Py:   return a, b
来源：http://tws.jinqigufen.top

PHP:  return [$a, $b];
来源：http://rkf.aizwys.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://voj.uphjek.com

TS:   return { a, b };
来源：http://spo.sjlbkw.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://sdq.hnxiangtu.top

Go:   return a, b
来源：http://grt.xuetiantiany.cn

Ruby: return a, b
来源：http://yag.sysykeji.top

C#:   return (a, b);              // ValueTuple
来源：http://ikc.yj20258.top

[C06] 匿名函数 / lambda
来源：http://von.tanke756.top

Py:   square = lambda x: x * x
来源：http://oxx.daria6918.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fnn.chenzaomai.com

JS:   const square = x => x * x;
来源：http://knh.ehwqpu.com

TS:   const square = (x: number): number => x * x;
来源：http://are.jqgufenzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://lkd.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://yyb.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://feb.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://xre.redwolf501.top

[C07] 把函数作为参数传入
来源：http://nev.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ake.hfpthk.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jqy.shanyushiyangtech.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hea.hnqzz.top

TS:   arr.map(String)
来源：http://oiu.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jsv.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mki.kuanghao11.cn

Ruby: arr.map(&:upcase)
来源：http://eqf.ywan-chungtsiang.top

C#:   arr.Select(s => s.ToUpper())
来源：http://iqm.yj20258.top

[C08] 闭包
来源：http://cqy.cqqwz.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bxr.bjfxy.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://spw.jinqigufen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://zvv.xinyue.icu

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://nzi.yongpay.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://cvl.birdmap.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hlk.dianchejie.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hkd.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ngl.chenlongwang.top

[C09] 递归
来源：http://ovx.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://yft.daria6918.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://tjf.hongshengwenyu.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mhg.dashuyun.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsg.iojbl.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://peo.xingfuxueyuan.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://eyy.cashguo.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gtd.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kfn.jianghu66.top

[C10] 变量作用域
来源：http://vla.zhongyouzk.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rmt.zhengqikj.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mwi.yuxming.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://anr.fktsv.cn

TS:   同 JS
来源：http://qne.shangyingyoupin.top

Java: 方法内为块级作用域
来源：http://pgs.hysaishi.cn

Go:   花括号块级作用域
来源：http://qdo.feifeiyinyue.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tbs.jqgfzy.top

C#:   块级作用域
来源：http://lvb.wangdashe.top

[C11] 模块导入与导出
来源：http://pgq.zhongyouzk.top

Py:   from module import func
来源：http://ipq.ppjwa.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://css.birdmap.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://fao.yfazqb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://okf.nanxuanxn.top

Java: import java.util.List;
来源：http://xbo.fzhhl.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mgi.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://trb.bbcook.cn

C#:   using System.Text;
来源：http://pdv.wangdashe.top

[C12] 立即执行函数 IIFE
来源：http://eiq.316326.xyz

Py:   (lambda: print("run"))()
来源：http://egq.jiagoushi.top

PHP:  (function () { echo "run"; })();
来源：http://tao.jqgfzy.top

JS:   (() => { console.log("run"); })();
来源：http://mqv.jiagoushi.top

TS:   (() => { console.log("run"); })();
来源：http://akk.jianghu66.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://muw.zhoulong.xyz

Go:   func() { fmt.Println("run") }()
来源：http://jkf.mhx1999.top

Ruby: -> { puts "run" }.call
来源：http://xgm.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gij.wangdashe.top

[C13] 类型声明 / 类型注解
来源：http://qyt.zhoulong.xyz

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yec.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uig.andypj.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wll.ppjwa.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ecl.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://lho.yonumen.top

Go:   func add(a, b int) int
来源：http://zha.cucudq.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xnu.shangyingyoupin.top

C#:   int Add(int a, int b) => a + b;
来源：http://ouy.jiagoushi.top

[C14] 泛型函数
来源：http://sym.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://puj.yj202588.top

PHP:  // 无泛型
来源：http://qxc.cqqwz.cn

JS:   // 无泛型
来源：http://hlf.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lvh.havefunace.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ngz.nanxuanxn.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vdj.havefunace.top

Ruby: # 无泛型
来源：http://hgm.yonumen.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mic.iojbl.cn

[C15] 解构 / 展开参数
来源：http://eez.zycfv.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://olc.zhixingplan.top

PHP:  [$a, $b] = $pair;
来源：http://ilh.tianlin.xyz

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tvr.tanke756.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nqp.vehdjk.com

Java: // 无解构
来源：http://mcr.xinyue.icu

Go:   // 无解构
来源：http://som.hysaishi.cn

Ruby: a, b = pair
来源：http://vsz.xuetiantiany.cn

C#:   var (a, b) = pair;
来源：http://lkb.yfazqb.com

[C16] 函数 / 方法重载
来源：http://obq.zhongyouzk.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://tur.pengpengdd.cyou

PHP:  // 无重载
来源：http://tia.ctjpmb.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://enl.xziqi.cn

TS:   // 用联合类型或重载签名声明
来源：http://alh.xingfuxueyuan.xyz

Java: void f(int a) {}  void f(String a) {}
来源：http://neh.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://esb.yj20258888.top

Ruby: # 无重载：靠动态参数
来源：http://icq.wangdashe.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ftp.cucudq.cn

================================================================================
来源：http://tco.vehdjk.com

D. 数组 / 列表 / 集合
来源：http://jjf.chenzaomai.com

================================================================================
来源：http://wue.316326.xyz

[D01] 创建数组 / 列表
来源：http://hjh.yanxiufei.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mms.xinyue.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pld.ivvv.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lor.fanxiaobao.xyz

TS:   const arr: number[] = [1, 2, 3];
来源：http://ndq.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://taa.redwolf501.top

Go:   arr := []int{1, 2, 3}
来源：http://btq.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://vhr.zdqjudy.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://huf.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://gic.bjfxy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mym.andypj.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xky.yj20258888.top

JS:   arr.push(4);
来源：http://goi.vehdjk.com

TS:   arr.push(4);
来源：http://yoa.yj202588.top

Java: list.add(4);
来源：http://gfr.9152youxi.cn

Go:   arr = append(arr, 4)
来源：http://ckx.hongshengwenyu.top

Ruby: arr << 4; arr.push(5)
来源：http://ukf.xuetiantiany.cn

C#:   list.Add(4);
来源：http://ric.zycfv.cn

[D03] 在指定位置插入元素
来源：http://hxn.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://lia.sxryk.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rep.jinqigfzy.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pfa.fanxiaobao.xyz

TS:   arr.splice(0, 0, 0);
来源：http://tfj.redwolf501.top

Java: list.add(0, 0);
来源：http://tmn.gzhubu.top

Go:   arr = append([]int{0}, arr...)
来源：http://hmb.wangshuangyany.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://qdg.zdqjudy.top


<!-- 参考信息 -->