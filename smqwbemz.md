代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tyg.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://biq.fanxiaobao.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jiz.meibo888.top

[B04] for 计数循环
来源：http://tnc.pengpengdd.cyou

Py:   for i in range(10): print(i)
来源：http://rdq.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bvz.meibo888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://byf.gotoacloud.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://atj.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qxy.feifeiyinyue.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rsh.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://ktb.ppjwa.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qxh.snrcjt.cn

[B05] 遍历数组 / 列表
来源：http://rcd.hcnkem.com

Py:   for item in arr: print(item)
来源：http://jnu.hnxiangtu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gxw.zycfv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yhp.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mba.zdqjudy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ewd.ctjpmb.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mwx.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://ezb.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gaa.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://jbi.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://eod.jlsjyb.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ivk.yuxming.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ttz.ctjpmb.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wld.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uxc.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nyq.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://iay.jyoumei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pmz.ctjpmb.com

[B07] while 循环
来源：http://lys.nanxuanxn.top

Py:   while i < 10: i += 1
来源：http://pmg.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bmw.ctjpmb.com

JS:   while (i < 10) { i++; }
来源：http://ogw.c1oappe.top

TS:   while (i < 10) { i++; }
来源：http://wvr.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://mbx.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ila.316326.xyz

Ruby: while i < 10; i += 1; end
来源：http://zjp.zhixingplan.top

C#:   while (i < 10) { i++; }
来源：http://geq.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://hpn.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://eoo.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sca.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://wlc.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://roe.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://ymq.zdqjudy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gpx.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://uss.jinqigufen.top

C#:   do { i++; } while (i < 10);
来源：http://cte.dashuyun.cn

[B09] break 与 continue
来源：http://yjy.ppjwa.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qse.shzxlz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://iqj.zhaomingkeji.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qff.cashguo.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fnk.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hau.fanxiaobao.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sxi.chenjidiqi.icu

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pyg.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtg.andypj.xyz

[B10] 遍历同时拿索引
来源：http://uvv.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fof.xziqi.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zra.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://avk.birdmap.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ebf.jinqigufen.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hft.ydzc1.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sae.yj20258888.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cnn.shzxlz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://otm.hesvh.cn

[B11] 生成数字序列 / 区间
来源：http://jlr.gogol.net.cn

Py:   list(range(0, 10, 2))
来源：http://iaf.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://ztx.yuxming.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssm.hfpthk.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rwu.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bwa.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vid.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://xza.ydjk.org.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://loz.ivvv.top

[B12] 跳出多层循环
来源：http://vqx.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://zgh.feifeiyinyue.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ioh.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://eit.chenlongwang.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ibw.xylfe.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://prb.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hda.yangfankeji.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nkq.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tqd.fktsv.cn

[B13] 判断是否为数字
来源：http://ile.ydzc1.top

Py:   isinstance(x, (int, float))
来源：http://ejb.yueranfly.top

PHP:  is_numeric($x)
来源：http://lbh.hammf.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nfx.zhijiandao.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ubd.yvedp.cn

Java: x instanceof Number
来源：http://gpq.nwbrower.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bso.cheryme.top

Ruby: x.is_a?(Numeric)
来源：http://unt.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://wvi.shanyushiyangtech.top

[B14] 判断值是否在集合内
来源：http://ssm.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgr.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yrk.shanyushiyangtech.top

JS:   [1, 2, 3].includes(x)
来源：http://bru.316326.xyz

TS:   [1, 2, 3].includes(x)
来源：http://fmi.hywenlv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sxv.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lur.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qyy.quarkkingdee.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vek.sysykeji.top

[B15] 布尔运算与取反
来源：http://gvq.daria6918.cn

Py:   a and b or not c
来源：http://lrw.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://wrk.uphjek.com

JS:   a && b || !c
来源：http://ufh.cheryme.top

TS:   a && b || !c
来源：http://uug.jlsjyb.cn

Java: a && b || !c
来源：http://hvn.nanxinkj.top

Go:   a && b || !c
来源：http://zsd.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://eua.yongpay.top

C#:   a && b || !c
来源：http://bzt.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://hom.xziqi.cn

Py:   if not data: return
来源：http://qzw.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://myu.aizwys.cn

JS:   if (!data) return;
来源：http://yil.jlsjyb.cn

TS:   if (!data) return;
来源：http://fdb.9152youxi.cn

Java: if (data == null) return;
来源：http://ifc.snrcjt.cn

Go:   if data == nil { return }
来源：http://xpz.zhaomingkeji.xyz

Ruby: return if data.nil?
来源：http://iuy.andypj.xyz

C#:   if (data == null) return;
来源：http://pew.hesvh.cn

================================================================================
来源：http://xjt.zhiwuduotai.top

C. 函数与作用域
来源：http://byc.zdqjudy.top

================================================================================
来源：http://yer.c1oappe.top

[C01] 定义函数
来源：http://lsx.yueranfly.top

Py:   def add(a, b): return a + b
来源：http://lxq.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zkd.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://muo.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ciy.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://srw.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://hls.aibaodan.cn

Ruby: def add(a, b); a + b; end
来源：http://yhq.jinqigufen.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://lou.wangdashe.top

[C02] 默认参数
来源：http://atj.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://nrs.zdbjq.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dce.cheryme.top

JS:   function greet(name = "World") { return name; }
来源：http://fmr.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mdm.uphjek.com

Java: // 无默认参数：方法重载或 Optional
来源：http://ksu.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ikc.daria6918.cn

Ruby: def greet(name = "World") = name
来源：http://tmj.ydzc1.top

C#:   string Greet(string name = "World") => name;
来源：http://qwc.havefunace.top

[C03] 可变参数
来源：http://pwx.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://kex.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tes.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qyk.chenjidiqi.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xtg.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qlo.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qol.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://uoc.9152youxi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jte.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://zee.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gdy.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mmn.sjlbkw.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lyo.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ykh.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://chs.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://bsb.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://jwp.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://boq.hnqzz.top

[C05] 返回多个值
来源：http://iju.vehdjk.com

Py:   return a, b
来源：http://pun.wangshuangyany.cn

PHP:  return [$a, $b];
来源：http://wko.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://ucw.uphjek.com

TS:   return { a, b };
来源：http://hwm.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jxa.guowangkeji.top

Go:   return a, b
来源：http://mhz.ydjk.org.cn

Ruby: return a, b
来源：http://cba.yueranfly.top

C#:   return (a, b);              // ValueTuple
来源：http://rsx.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://zag.havefunace.top

Py:   square = lambda x: x * x
来源：http://mys.aizwys.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fvz.nwbrower.top

JS:   const square = x => x * x;
来源：http://liw.hfpthk.cn

TS:   const square = (x: number): number => x * x;
来源：http://pkr.smart0.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ndn.yongpay.top

Go:   sq := func(x int) int { return x * x }
来源：http://awj.shangyingyoupin.top

Ruby: square = ->(x) { x * x }
来源：http://eyg.nanxuanxn.top

C#:   Func<int, int> square = x => x * x;
来源：http://duc.hfpthk.cn

[C07] 把函数作为参数传入
来源：http://isq.ydzc1.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ylh.c1oappe.top

PHP:  array_map("strtoupper", $arr);
来源：http://tqr.ydzc1.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xqq.xuetiantiany.cn

TS:   arr.map(String)
来源：http://zpu.shuidangran.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://oqn.hcnkem.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dzy.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://ixf.zdqjudy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ihp.gaohongyu789.top

[C08] 闭包
来源：http://uty.ctjpmb.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://cfd.nanxuanxn.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kch.yfazqb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://xsc.yangfankeji.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://krd.nwbrower.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uad.shzxlz.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wem.cqqwz.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zek.gaohongyu789.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oey.yonumen.top

[C09] 递归
来源：http://pdb.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nou.yuxming.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vtu.yangfankeji.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xid.yj202588.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lzh.jqgfzy.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://amv.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://quc.nanxinkj.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://emq.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tgp.yonumen.top

[C10] 变量作用域
来源：http://xcn.zhengqikj.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://kgz.hongshengwenyu.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://djf.sysykeji.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tih.yj202588.top

TS:   同 JS
来源：http://uid.316326.xyz

Java: 方法内为块级作用域
来源：http://yyd.jinqigfzy.top

Go:   花括号块级作用域
来源：http://ixc.hfpthk.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cop.hnxiangtu.top

C#:   块级作用域
来源：http://beb.fehbvm.com

[C11] 模块导入与导出
来源：http://dtx.yuxming.cn

Py:   from module import func
来源：http://kjs.cdnleiting.top

PHP:  require "file.php";  或 use App\Service;
来源：http://ien.jinyuanbaomall.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ywg.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dwm.sxryk.cn

Java: import java.util.List;
来源：http://ucp.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lcv.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://osj.zhengqikj.top

C#:   using System.Text;
来源：http://anj.daria6918.cn

[C12] 立即执行函数 IIFE
来源：http://gnk.shangyingyoupin.top

Py:   (lambda: print("run"))()
来源：http://cxz.chenlongwang.top

PHP:  (function () { echo "run"; })();
来源：http://sur.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://cgx.vehdjk.com

TS:   (() => { console.log("run"); })();
来源：http://bgf.nwbrower.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qzs.jinqigufen.top

Go:   func() { fmt.Println("run") }()
来源：http://qxy.guannengcc.top

Ruby: -> { puts "run" }.call
来源：http://yiq.hywenlv.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cly.yanxiufei.cn

[C13] 类型声明 / 类型注解
来源：http://dgb.xziqi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pgn.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gji.jqgufenzy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://otj.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xpz.vqdsnc.cn

Java: int add(int a, int b) { return a + b; }
来源：http://odg.vqdsnc.cn

Go:   func add(a, b int) int
来源：http://idh.xuanzx.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://jbh.9152youxi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://qtl.chenlongwang.top

[C14] 泛型函数
来源：http://tzf.yuxming.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://isk.zhongyouzk.top

PHP:  // 无泛型
来源：http://hqi.aizwys.cn

JS:   // 无泛型
来源：http://ryn.sysykeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jvk.chenlongwang.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://jow.hywenlv.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://kgw.quarkkingdee.top

Ruby: # 无泛型
来源：http://hsx.svipenyu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://boa.gaohongyu789.top

[C15] 解构 / 展开参数
来源：http://aoy.xuetiantiany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jgm.zhoulong.xyz

PHP:  [$a, $b] = $pair;
来源：http://bgi.gaohongyu789.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nfo.haohaochexian.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kxz.yonumen.top

Java: // 无解构
来源：http://wft.pengpengdd.cyou

Go:   // 无解构
来源：http://atb.cucudq.cn

Ruby: a, b = pair
来源：http://ztm.zhengqikj.top

C#:   var (a, b) = pair;
来源：http://gho.aizwys.cn

[C16] 函数 / 方法重载
来源：http://gnv.ehwqpu.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hju.meibo888.top

PHP:  // 无重载
来源：http://ybp.snrcjt.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qzq.ydjk.org.cn

TS:   // 用联合类型或重载签名声明
来源：http://kxx.aibaodan.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://qpm.pengpengdd.cyou

Go:   // 无重载：用不同函数名
来源：http://tcd.dashuyun.cn

Ruby: # 无重载：靠动态参数
来源：http://vws.xinyue.icu

C#:   void F(int a) {}  void F(string a) {}
来源：http://fsj.xuetiantiany.cn

================================================================================
来源：http://for.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://hou.svipenyu.cn

================================================================================
来源：http://gfm.hnqzz.top

[D01] 创建数组 / 列表
来源：http://fuq.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://tuc.hywenlv.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://eln.gzhubu.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bjv.birdmap.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://gke.zhoulong.xyz

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ozs.feifeiyinyue.top

Go:   arr := []int{1, 2, 3}
来源：http://unc.fanxiaobao.xyz

Ruby: arr = [1, 2, 3]
来源：http://rqu.fktsv.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pmx.zhengqikj.top

[D02] 追加元素到末尾
来源：http://tgu.epnwcf.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fir.yuxming.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jie.tarul.cn

JS:   arr.push(4);
来源：http://jjk.sufxvd.cn

TS:   arr.push(4);
来源：http://qlm.svipenyu.cn

Java: list.add(4);
来源：http://enf.nwbrower.top

Go:   arr = append(arr, 4)
来源：http://won.daxiang520.top

Ruby: arr << 4; arr.push(5)
来源：http://sie.tianlin.xyz

C#:   list.Add(4);
来源：http://okt.pycfn.com

[D03] 在指定位置插入元素
来源：http://sbo.fktsv.cn

Py:   arr.insert(0, 0)
来源：http://gzk.zhijiandao.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tpr.dashuyun.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://coj.sjlbkw.cn

TS:   arr.splice(0, 0, 0);
来源：http://aod.vqdsnc.cn

Java: list.add(0, 0);
来源：http://yru.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://jlz.ivvv.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iii.sweek.top

C#:   list.Insert(0, 0);
来源：http://smq.cqqwz.cn

[D04] 删除元素
来源：http://yvx.jqgufenzy.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kxe.yuanzhike.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zsu.tian-w.cn


<!-- 参考信息 -->