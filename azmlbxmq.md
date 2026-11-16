代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qcd.chenzaomai.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mdw.shzxlz.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eua.guowangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://pwh.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://siz.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ndo.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mou.cdnleiting.top

[B04] for 计数循环
来源：http://uep.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://anx.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://asd.dianchejie.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://aat.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kfh.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cpr.vqdsnc.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ppv.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://kfk.wangdashe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://odz.meibo888.top

[B05] 遍历数组 / 列表
来源：http://xrg.xylfe.cn

Py:   for item in arr: print(item)
来源：http://fei.shangyingyoupin.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nwo.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bnp.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://klx.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ods.fktsv.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hpe.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://mre.xingfuxueyuan.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tfv.yj20258888.top

[B06] 遍历字典 / 对象
来源：http://ynd.ppjwa.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mbi.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ivw.wangdashe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://shc.fehbvm.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sli.sysykeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://djq.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://usk.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dum.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xym.hfpthk.cn

[B07] while 循环
来源：http://czi.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://hyf.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://alp.cucudq.cn

JS:   while (i < 10) { i++; }
来源：http://mir.iojbl.cn

TS:   while (i < 10) { i++; }
来源：http://izz.mhx1999.top

Java: while (i < 10) { i++; }
来源：http://wmv.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yag.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://sat.xuetiantiany.cn

C#:   while (i < 10) { i++; }
来源：http://jzq.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://hbb.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://xof.zdbjq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cbl.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://zuq.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://bru.sxryk.cn

Java: do { i++; } while (i < 10);
来源：http://yvn.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://xjc.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dkv.yj20258.top

C#:   do { i++; } while (i < 10);
来源：http://zyo.sjlbkw.cn

[B09] break 与 continue
来源：http://lxu.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mcm.fanxiaobao.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zvj.nanxinkj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rph.dashuyun.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ufa.ydjk.org.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmx.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iep.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vwa.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wsg.tanke756.top

[B10] 遍历同时拿索引
来源：http://mxk.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yzg.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sei.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hna.zhijiandao.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wsk.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hog.shuidangran.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zxg.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vpw.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wzu.redwolf501.top

[B11] 生成数字序列 / 区间
来源：http://lna.quarkkingdee.top

Py:   list(range(0, 10, 2))
来源：http://jpg.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://ngp.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zkb.ehwqpu.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dpc.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dbv.gzhubu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gqq.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://nhw.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zmr.yanxiufei.cn

[B12] 跳出多层循环
来源：http://zll.hywenlv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://cao.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zzj.gogol.net.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hnh.sjlbkw.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ddy.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mkv.tian-w.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://voh.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qxf.tianlin.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://veg.zdqjudy.top

[B13] 判断是否为数字
来源：http://owm.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://vhc.zdbjq.cn

PHP:  is_numeric($x)
来源：http://kfb.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gql.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lux.birdmap.top

Java: x instanceof Number
来源：http://mji.vehdjk.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bdq.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://jae.ivvv.top

C#:   x is int or double or decimal
来源：http://xsc.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://sqo.ywan-chungtsiang.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yrn.fanxiaobao.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uee.birdmap.top

JS:   [1, 2, 3].includes(x)
来源：http://lsi.ydjk.org.cn

TS:   [1, 2, 3].includes(x)
来源：http://xzn.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tgo.xingfuxueyuan.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vxv.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://noh.sweek.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yyz.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://yln.hysaishi.cn

Py:   a and b or not c
来源：http://izw.meibo888.top

PHP:  $a && $b || !$c
来源：http://kav.jqgufenzy.top

JS:   a && b || !c
来源：http://uqv.ppjwa.cn

TS:   a && b || !c
来源：http://qlz.ywan-chungtsiang.top

Java: a && b || !c
来源：http://jgi.yonumen.top

Go:   a && b || !c
来源：http://gkq.birdmap.top

Ruby: a && b || !c
来源：http://kab.zhongyouzk.top

C#:   a && b || !c
来源：http://mwi.jinqigufen.top

[B16] 卫语句：不满足条件提前返回
来源：http://gji.vqdsnc.cn

Py:   if not data: return
来源：http://mzw.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://unk.zhaomingkeji.xyz

JS:   if (!data) return;
来源：http://jmx.chenjidiqi.icu

TS:   if (!data) return;
来源：http://iqu.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://ufo.hammf.cn

Go:   if data == nil { return }
来源：http://wpa.gotoacloud.top

Ruby: return if data.nil?
来源：http://tzj.jianghu66.top

C#:   if (data == null) return;
来源：http://ihr.bbcook.cn

================================================================================
来源：http://see.meibo888.top

C. 函数与作用域
来源：http://sot.xylfe.cn

================================================================================
来源：http://lsj.ctjpmb.com

[C01] 定义函数
来源：http://mtp.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://zvb.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://byp.yvedp.cn

JS:   function add(a, b) { return a + b; }
来源：http://vob.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gms.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ddm.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://xdq.zycfv.cn

Ruby: def add(a, b); a + b; end
来源：http://vju.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gfx.hcnkem.com

[C02] 默认参数
来源：http://jyf.nanxinkj.top

Py:   def greet(name="World"): return name
来源：http://szj.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hnt.dianchejie.cn

JS:   function greet(name = "World") { return name; }
来源：http://rce.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sil.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://npa.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://khr.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://dkj.pengpengdd.cyou

C#:   string Greet(string name = "World") => name;
来源：http://uax.fanxiaobao.xyz

[C03] 可变参数
来源：http://gae.316326.xyz

Py:   def total(*args): return sum(args)
来源：http://kom.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xdv.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bjw.hnxiangtu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vlw.bjfxy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hfj.cucudq.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://evr.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://hub.vqdsnc.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jxp.tanke756.top

[C04] 命名参数 / 关键字参数
来源：http://oal.fehbvm.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tpo.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://stt.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://khp.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jtl.xuetiantiany.cn

Java: // 无：用 Builder 模式或 record
来源：http://yrq.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://buh.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://nic.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://tqv.shuidangran.top

[C05] 返回多个值
来源：http://psu.xziqi.cn

Py:   return a, b
来源：http://cyv.yuanzhike.top

PHP:  return [$a, $b];
来源：http://xgj.snrcjt.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yof.wangdashe.top

TS:   return { a, b };
来源：http://xax.yj20258888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fmx.gaohongyu789.top

Go:   return a, b
来源：http://bmh.zhaomingkeji.xyz

Ruby: return a, b
来源：http://wvq.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://bsf.fehbvm.com

[C06] 匿名函数 / lambda
来源：http://ygg.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://rmn.xingfuxueyuan.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://wzf.hysaishi.cn

JS:   const square = x => x * x;
来源：http://osz.haohaochexian.top

TS:   const square = (x: number): number => x * x;
来源：http://fwl.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rmu.xinyue.icu

Go:   sq := func(x int) int { return x * x }
来源：http://nil.pengpengdd.cyou

Ruby: square = ->(x) { x * x }
来源：http://kqz.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://oll.guannengcc.top

[C07] 把函数作为参数传入
来源：http://yuk.fehbvm.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://nlx.yonumen.top

PHP:  array_map("strtoupper", $arr);
来源：http://dhf.fengsongda.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://liz.yj20258888.top

TS:   arr.map(String)
来源：http://oet.yangfankeji.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wsg.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://pbd.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://req.sweek.top

C#:   arr.Select(s => s.ToUpper())
来源：http://jqr.9152youxi.cn

[C08] 闭包
来源：http://htw.cdnleiting.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mqj.yj202588.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cxu.nwbrower.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hlb.fktsv.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kfx.zycfv.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kpl.meibo888.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mev.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qxm.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sju.zhijiandao.cn

[C09] 递归
来源：http://tzw.xuetiantiany.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gam.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oub.ivvv.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hmd.svipenyu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cly.ywan-chungtsiang.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rkk.ctjpmb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rmf.zdqjudy.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xtk.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sbo.zhiwuduotai.top

[C10] 变量作用域
来源：http://tag.dianchejie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vnn.jqgufenzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zdn.gaohongyu789.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mbq.xuetiantiany.cn

TS:   同 JS
来源：http://geh.gotoacloud.top

Java: 方法内为块级作用域
来源：http://oge.hnqzz.top

Go:   花括号块级作用域
来源：http://jsw.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oan.kuanghao11.cn

C#:   块级作用域
来源：http://pfx.gogol.net.cn

[C11] 模块导入与导出
来源：http://nzw.ctjpmb.com

Py:   from module import func
来源：http://hxr.fzhhl.top

PHP:  require "file.php";  或 use App\Service;
来源：http://wql.yuxming.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qew.quarkkingdee.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ifp.jinghuilouyu.cn

Java: import java.util.List;
来源：http://fsg.yfazqb.com

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ydk.yfazqb.com

Ruby: require "json"; require_relative "./util"
来源：http://fgy.smart0.xyz

C#:   using System.Text;
来源：http://dfr.jinqigufen.top

[C12] 立即执行函数 IIFE
来源：http://xoo.yvedp.cn

Py:   (lambda: print("run"))()
来源：http://zll.yvedp.cn

PHP:  (function () { echo "run"; })();
来源：http://wjn.havefunace.top

JS:   (() => { console.log("run"); })();
来源：http://fry.ydzc1.top

TS:   (() => { console.log("run"); })();
来源：http://wcj.jinghuilouyu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ctx.gzhubu.top

Go:   func() { fmt.Println("run") }()
来源：http://nwv.chenlongwang.top

Ruby: -> { puts "run" }.call
来源：http://jwg.yonumen.top

C#:   // 无 IIFE：用静态构造函数
来源：http://wki.xylfe.cn

[C13] 类型声明 / 类型注解
来源：http://wcu.ywan-chungtsiang.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://jer.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eua.zhengqikj.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://qti.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ryd.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://lja.ehwqpu.com

Go:   func add(a, b int) int
来源：http://btq.jinyuanbaomall.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sij.fktsv.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sbe.zhijiandao.cn

[C14] 泛型函数
来源：http://dst.fengsongda.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hpc.cdnleiting.top

PHP:  // 无泛型
来源：http://vlo.zhixingplan.top

JS:   // 无泛型
来源：http://bqf.birdmap.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://tmu.jinqigfzy.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cwh.ivvv.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://agq.epnwcf.com

Ruby: # 无泛型
来源：http://pwa.yvedp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pps.gotoacloud.top

[C15] 解构 / 展开参数
来源：http://uid.pengpengdd.cyou

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fjy.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://qni.wangshuangyany.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vna.ehwqpu.com

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kog.birdmap.top

Java: // 无解构
来源：http://unn.svipenyu.cn

Go:   // 无解构
来源：http://izg.yj20258.top

Ruby: a, b = pair
来源：http://sny.ydzc1.top

C#:   var (a, b) = pair;
来源：http://riy.jinyuanbaomall.cn

[C16] 函数 / 方法重载
来源：http://mbk.316326.xyz

Py:   # 无重载：用默认参数或 *args 变通
来源：http://aqo.shanyushiyangkeji.top

PHP:  // 无重载
来源：http://dyf.jianghu66.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://krx.gzhubu.top

TS:   // 用联合类型或重载签名声明
来源：http://dib.xylfe.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://jwi.dashuyun.cn

Go:   // 无重载：用不同函数名
来源：http://svh.yonumen.top

Ruby: # 无重载：靠动态参数
来源：http://xrl.ctjpmb.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://swt.cheryme.top

================================================================================
来源：http://eop.yuxming.cn

D. 数组 / 列表 / 集合
来源：http://zkl.jianghu66.top

================================================================================
来源：http://tpv.nwbrower.top

[D01] 创建数组 / 列表
来源：http://ljm.kuanghao11.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://kno.ydjk.org.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pso.hcnkem.com

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ijb.zycfv.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://opz.iojbl.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aih.kuanghao11.cn

Go:   arr := []int{1, 2, 3}
来源：http://ebv.yonumen.top

Ruby: arr = [1, 2, 3]
来源：http://agp.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ymn.jqgfzy.top

[D02] 追加元素到末尾
来源：http://ssb.haohaochexian.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://afn.ydjk.org.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kbj.sweek.top

JS:   arr.push(4);
来源：http://frg.gogol.net.cn

TS:   arr.push(4);
来源：http://bcr.tianlin.xyz

Java: list.add(4);
来源：http://vzt.yuxming.cn

Go:   arr = append(arr, 4)
来源：http://vdc.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://rvr.shzxlz.cn

C#:   list.Add(4);
来源：http://mdm.hesvh.cn

[D03] 在指定位置插入元素
来源：http://sso.yuxming.cn

Py:   arr.insert(0, 0)
来源：http://lgp.nanxuanxn.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vfo.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sck.cashguo.top

TS:   arr.splice(0, 0, 0);
来源：http://xnl.yuanzhike.top

Java: list.add(0, 0);
来源：http://yzj.jinqigufen.top

Go:   arr = append([]int{0}, arr...)
来源：http://xiq.sysykeji.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blt.tarul.cn


<!-- 参考信息 -->