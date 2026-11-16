代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rkv.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kyc.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://its.chenzaomai.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pqs.sjlbkw.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bhm.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nfx.52xcode.cn

[B03] switch / match / case
来源：http://mov.gotoacloud.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cab.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dje.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eun.feifeiyinyue.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyo.mhx1999.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://moi.zhijiandao.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qaz.hongshengwenyu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kbi.guowangkeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bit.jinqigfzy.top

[B04] for 计数循环
来源：http://gdo.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://mbe.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zlw.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sxt.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://inz.vehdjk.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rdy.sysykeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cbt.gogol.net.cn

Ruby: 10.times { |i| puts i }
来源：http://cxs.hfpthk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ywd.yongpay.top

[B05] 遍历数组 / 列表
来源：http://yae.bjfxy.top

Py:   for item in arr: print(item)
来源：http://tir.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://btq.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://cis.yangfankeji.com

TS:   for (const item of arr) { console.log(item); }
来源：http://fdn.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://wjj.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zey.yongpay.top

Ruby: arr.each { |item| puts item }
来源：http://rlj.shuidangran.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sef.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://wkb.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ntv.haohaochexian.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xfl.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wat.ydjk.org.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jiz.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zkw.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://dpu.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xlx.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uyx.yuxming.cn

[B07] while 循环
来源：http://qhn.yangfankeji.com

Py:   while i < 10: i += 1
来源：http://saq.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://evi.chenzaomai.com

JS:   while (i < 10) { i++; }
来源：http://nkc.yuanzhike.top

TS:   while (i < 10) { i++; }
来源：http://ikr.daxiang520.top

Java: while (i < 10) { i++; }
来源：http://zep.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bcp.yonumen.top

Ruby: while i < 10; i += 1; end
来源：http://ggh.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://oqt.fengsongda.top

[B08] do-while（至少执行一次）
来源：http://sts.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://rvu.hnqzz.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xxz.ctjpmb.com

JS:   do { i++; } while (i < 10);
来源：http://kaj.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://tyb.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://kfn.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://obk.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://dsn.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://osh.zhongyouzk.top

[B09] break 与 continue
来源：http://gxp.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bpr.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kfu.jinghuilouyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yrn.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vdr.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzo.hesvh.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jba.tanke756.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ika.bbcook.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uel.jqgfzy.top

[B10] 遍历同时拿索引
来源：http://ncq.hesvh.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cup.sysykeji.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wbc.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wxi.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cfd.pycfn.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://saf.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lki.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mdv.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pmd.yuxming.cn

[B11] 生成数字序列 / 区间
来源：http://pml.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://uts.cashguo.top

PHP:  range(0, 10, 2);
来源：http://itt.yj20258888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fuj.yj20258.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://swo.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lhr.zhiwuduotai.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xkg.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://rku.yvedp.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ppi.jlsjyb.cn

[B12] 跳出多层循环
来源：http://ivx.yueranfly.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fce.jinqigufen.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://hyq.xuetiantiany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uhl.zhaomingkeji.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ede.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://owv.andypj.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yty.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tft.wangdashe.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://auu.tian-w.cn

[B13] 判断是否为数字
来源：http://gad.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://rqv.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://son.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://igx.cqqwz.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eao.hesvh.cn

Java: x instanceof Number
来源：http://jmw.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pbb.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://jms.nanxinkj.top

C#:   x is int or double or decimal
来源：http://zpe.wangdashe.top

[B14] 判断值是否在集合内
来源：http://ars.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fie.bbcook.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tyo.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://bpl.smart0.xyz

TS:   [1, 2, 3].includes(x)
来源：http://sfk.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fak.zycfv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jmc.gaohongyu789.top

Ruby: [1, 2, 3].include?(x)
来源：http://uue.9152youxi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nnm.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://oip.dashuyun.cn

Py:   a and b or not c
来源：http://rnp.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://mhc.fanxiaobao.xyz

JS:   a && b || !c
来源：http://xuz.dianchejie.cn

TS:   a && b || !c
来源：http://ecm.ydzc1.top

Java: a && b || !c
来源：http://jgn.chenjidiqi.icu

Go:   a && b || !c
来源：http://ayz.nanxinkj.top

Ruby: a && b || !c
来源：http://gtu.52xcode.cn

C#:   a && b || !c
来源：http://kpe.zdqjudy.top

[B16] 卫语句：不满足条件提前返回
来源：http://eem.shzxlz.cn

Py:   if not data: return
来源：http://qwx.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://zjl.wangshuangyany.cn

JS:   if (!data) return;
来源：http://bjj.tanke756.top

TS:   if (!data) return;
来源：http://otp.havefunace.top

Java: if (data == null) return;
来源：http://fvk.chenjidiqi.icu

Go:   if data == nil { return }
来源：http://mhq.gogol.net.cn

Ruby: return if data.nil?
来源：http://ond.hywenlv.cn

C#:   if (data == null) return;
来源：http://gix.cashguo.top

================================================================================
来源：http://xsv.epnwcf.com

C. 函数与作用域
来源：http://gyz.feifeiyinyue.top

================================================================================
来源：http://kfa.jqgfzy.top

[C01] 定义函数
来源：http://qah.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://yvc.gzhubu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://lcn.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://ctz.snrcjt.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qeb.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://dpk.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://urs.feifeiyinyue.top

Ruby: def add(a, b); a + b; end
来源：http://jcq.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pua.hnqzz.top

[C02] 默认参数
来源：http://odc.yanxiufei.cn

Py:   def greet(name="World"): return name
来源：http://hao.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kkc.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://rbu.bjfxy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lul.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rjx.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fqt.shangyingyoupin.top

Ruby: def greet(name = "World") = name
来源：http://frl.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://nzy.yuanzhike.top

[C03] 可变参数
来源：http://fxo.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://rqf.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zft.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zka.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxw.ppjwa.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wrk.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://owl.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aye.wangdashe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dql.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://aci.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://szk.cucudq.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aro.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ige.xuanzx.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mmv.xziqi.cn

Java: // 无：用 Builder 模式或 record
来源：http://zzj.shanyushiyangtech.top

Go:   // 无：用配置结构体参数
来源：http://djh.sweek.top

Ruby: f(a: 1, b: 2)
来源：http://ucf.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://uro.jlsjyb.cn

[C05] 返回多个值
来源：http://mbw.feifeiyinyue.top

Py:   return a, b
来源：http://fjf.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://ssa.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ote.tian-w.cn

TS:   return { a, b };
来源：http://iqd.havefunace.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://imq.zycfv.cn

Go:   return a, b
来源：http://pbb.haohaochexian.top

Ruby: return a, b
来源：http://how.cqqwz.cn

C#:   return (a, b);              // ValueTuple
来源：http://hww.xinyue.icu

[C06] 匿名函数 / lambda
来源：http://zeq.wangdashe.top

Py:   square = lambda x: x * x
来源：http://mkw.gogol.net.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fhj.hywenlv.cn

JS:   const square = x => x * x;
来源：http://pav.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://jmc.aizwys.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pfa.fzhhl.top

Go:   sq := func(x int) int { return x * x }
来源：http://jkj.zhengqikj.top

Ruby: square = ->(x) { x * x }
来源：http://bbo.mhx1999.top

C#:   Func<int, int> square = x => x * x;
来源：http://eqb.yueranfly.top

[C07] 把函数作为参数传入
来源：http://mvz.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://cle.zdqjudy.top

PHP:  array_map("strtoupper", $arr);
来源：http://hum.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://coz.cucudq.cn

TS:   arr.map(String)
来源：http://cyh.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iwm.tianlin.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mbs.redwolf501.top

Ruby: arr.map(&:upcase)
来源：http://kys.dianchejie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://kxt.tarul.cn

[C08] 闭包
来源：http://taf.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://rxv.shanyushiyangtech.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jmk.redwolf501.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dcs.fehbvm.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bmh.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sdn.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hdn.sufxvd.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qeq.sxryk.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://vmd.zhoulong.xyz

[C09] 递归
来源：http://nzq.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xkv.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://foh.yfazqb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dwi.aizwys.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ojx.xziqi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gre.feifeiyinyue.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://zqi.epnwcf.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mcz.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://vcj.daxiang520.top

[C10] 变量作用域
来源：http://jhi.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://btr.ctjpmb.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fac.zhijiandao.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qbc.chenjidiqi.icu

TS:   同 JS
来源：http://aqw.yanxiufei.cn

Java: 方法内为块级作用域
来源：http://bxh.ehwqpu.com

Go:   花括号块级作用域
来源：http://vrz.fanxiaobao.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dbz.xinyue.icu

C#:   块级作用域
来源：http://edl.cashguo.top

[C11] 模块导入与导出
来源：http://zam.jlsjyb.cn

Py:   from module import func
来源：http://sxs.jyoumei.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ide.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://npq.cqqwz.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://unu.c1oappe.top

Java: import java.util.List;
来源：http://kdz.tianlin.xyz

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ydo.ctjpmb.com

Ruby: require "json"; require_relative "./util"
来源：http://rju.dashuyun.cn

C#:   using System.Text;
来源：http://jip.0kj1m.cn

[C12] 立即执行函数 IIFE
来源：http://hbj.jqgfzy.top

Py:   (lambda: print("run"))()
来源：http://ajo.mhx1999.top

PHP:  (function () { echo "run"; })();
来源：http://zpl.ydzc1.top

JS:   (() => { console.log("run"); })();
来源：http://ome.wangshuangyany.cn

TS:   (() => { console.log("run"); })();
来源：http://zld.0kj1m.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xgh.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://itm.jqgufenzy.top

Ruby: -> { puts "run" }.call
来源：http://zzn.yvedp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://pbi.316326.xyz

[C13] 类型声明 / 类型注解
来源：http://fmw.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cmy.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fuk.iojbl.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ags.yvedp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtw.dianchejie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://zmi.0kj1m.cn

Go:   func add(a, b int) int
来源：http://tbp.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mjr.daria6918.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ryp.yfazqb.com

[C14] 泛型函数
来源：http://wfx.zhoulong.xyz

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hoh.hfpthk.cn

PHP:  // 无泛型
来源：http://ust.fktsv.cn

JS:   // 无泛型
来源：http://dny.fktsv.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://obs.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://icf.pengpengdd.cyou

Go:   func First[T any](items []T) T { return items[0] }
来源：http://oqb.quarkkingdee.top

Ruby: # 无泛型
来源：http://orv.zhiwuduotai.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bed.jiagoushi.top

[C15] 解构 / 展开参数
来源：http://xag.redwolf501.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dqk.tarul.cn

PHP:  [$a, $b] = $pair;
来源：http://aba.ybcxt.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://czi.guowangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://obz.hnxiangtu.top

Java: // 无解构
来源：http://qmv.havefunace.top

Go:   // 无解构
来源：http://cae.chenjidiqi.icu

Ruby: a, b = pair
来源：http://ewk.xinyue.icu

C#:   var (a, b) = pair;
来源：http://fhn.cqqwz.cn

[C16] 函数 / 方法重载
来源：http://kwu.jyoumei.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pyg.jianghu66.top

PHP:  // 无重载
来源：http://iqm.316326.xyz

JS:   // 无重载：靠 arguments.length 分支
来源：http://hnw.fktsv.cn

TS:   // 用联合类型或重载签名声明
来源：http://afp.ydjk.org.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://gfx.yj20258888.top

Go:   // 无重载：用不同函数名
来源：http://ddw.uphjek.com

Ruby: # 无重载：靠动态参数
来源：http://cfl.meibo888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ezk.ybcxt.top

================================================================================
来源：http://sfm.cdnleiting.top

D. 数组 / 列表 / 集合
来源：http://zsl.tarul.cn

================================================================================
来源：http://kic.sysykeji.top

[D01] 创建数组 / 列表
来源：http://yza.hcnkem.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://ovx.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://txg.xylfe.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hki.snrcjt.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ejz.ehwqpu.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://xou.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://art.guowangkeji.top

Ruby: arr = [1, 2, 3]
来源：http://sef.meibo888.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ehu.hnqzz.top

[D02] 追加元素到末尾
来源：http://pmm.tian-w.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yej.yj20258.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://knj.gaohongyu789.top

JS:   arr.push(4);
来源：http://tuz.tian-w.cn

TS:   arr.push(4);
来源：http://wjr.shzxlz.cn

Java: list.add(4);
来源：http://mvk.xylfe.cn

Go:   arr = append(arr, 4)
来源：http://cix.ywan-chungtsiang.top

Ruby: arr << 4; arr.push(5)
来源：http://ckc.fktsv.cn

C#:   list.Add(4);
来源：http://xcm.yj20258.top


<!-- 参考信息 -->