代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tyv.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gfp.pengpengdd.cyou

[B03] switch / match / case
来源：http://wyw.xinyue.icu

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xlq.hesvh.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xrm.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebw.shuidangran.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zom.jinyuanbaomall.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://erp.havefunace.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ndn.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hjy.bjfxy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iek.jyoumei.cn

[B04] for 计数循环
来源：http://blw.wangshuangyany.cn

Py:   for i in range(10): print(i)
来源：http://nyy.zhixingplan.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vki.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nzt.xingfuxueyuan.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tiv.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wvp.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://kuh.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://qbr.wangshuangyany.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://agc.yonumen.top

[B05] 遍历数组 / 列表
来源：http://xzy.fanxiaobao.xyz

Py:   for item in arr: print(item)
来源：http://bcq.gotoacloud.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vjo.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jqh.pycfn.com

TS:   for (const item of arr) { console.log(item); }
来源：http://yye.hywenlv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iex.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://str.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://eem.jinyuanbaomall.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://idi.yfazqb.com

[B06] 遍历字典 / 对象
来源：http://ewm.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://rrk.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bzc.jyoumei.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eko.shangyingyoupin.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nfm.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bjz.zhengqikj.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ocq.ivvv.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wmx.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ksg.shangyingyoupin.top

[B07] while 循环
来源：http://djx.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://oav.svipenyu.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ynx.316326.xyz

JS:   while (i < 10) { i++; }
来源：http://woe.svipenyu.cn

TS:   while (i < 10) { i++; }
来源：http://pch.jinghuilouyu.cn

Java: while (i < 10) { i++; }
来源：http://fmu.jinqigufen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://quy.cqqwz.cn

Ruby: while i < 10; i += 1; end
来源：http://jeb.c1oappe.top

C#:   while (i < 10) { i++; }
来源：http://tvn.uphjek.com

[B08] do-while（至少执行一次）
来源：http://onv.havefunace.top

Py:   # 无 do-while：用 while True + break
来源：http://rux.jiagoushi.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jyt.tianlin.xyz

JS:   do { i++; } while (i < 10);
来源：http://mqh.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://eev.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://rva.gzhubu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://uzr.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://ytz.shuidangran.top

C#:   do { i++; } while (i < 10);
来源：http://zoo.jianghu66.top

[B09] break 与 continue
来源：http://kwe.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wmj.iojbl.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://njl.bjfxy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hyb.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yxz.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tld.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zis.9152youxi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dta.gogol.net.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mum.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://okv.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vcr.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://oop.zdqjudy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pbn.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://azz.zhixingplan.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gvk.yangfankeji.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://atb.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qfk.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fop.yuanzhike.top

[B11] 生成数字序列 / 区间
来源：http://mkw.kuanghao11.cn

Py:   list(range(0, 10, 2))
来源：http://glu.gzhubu.top

PHP:  range(0, 10, 2);
来源：http://lhx.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vbo.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uer.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://akp.bbcook.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vfr.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://upx.yuanzhike.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ega.mhx1999.top

[B12] 跳出多层循环
来源：http://uzq.zhoulong.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://wdp.wangdashe.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nde.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://axu.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ajg.gaohongyu789.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aeo.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lpu.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnt.chenzaomai.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gba.ivvv.top

[B13] 判断是否为数字
来源：http://apm.zhengqikj.top

Py:   isinstance(x, (int, float))
来源：http://jwm.zycfv.cn

PHP:  is_numeric($x)
来源：http://wwm.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xdq.aibaodan.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ted.shzxlz.cn

Java: x instanceof Number
来源：http://cwm.vqdsnc.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://aeg.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://zjc.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://qgi.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://osp.aibaodan.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://igg.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eat.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://kjq.cdnleiting.top

TS:   [1, 2, 3].includes(x)
来源：http://koc.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://iku.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xcl.hammf.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bjl.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lmn.hongshengwenyu.top

[B15] 布尔运算与取反
来源：http://cft.haohaochexian.top

Py:   a and b or not c
来源：http://uly.hammf.cn

PHP:  $a && $b || !$c
来源：http://wfc.shanyushiyangtech.top

JS:   a && b || !c
来源：http://iju.andypj.xyz

TS:   a && b || !c
来源：http://lfq.xylfe.cn

Java: a && b || !c
来源：http://sgf.316326.xyz

Go:   a && b || !c
来源：http://fur.jiagoushi.top

Ruby: a && b || !c
来源：http://auf.sjlbkw.cn

C#:   a && b || !c
来源：http://bba.yongpay.top

[B16] 卫语句：不满足条件提前返回
来源：http://xzu.aibaodan.cn

Py:   if not data: return
来源：http://xqb.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://bdr.yj20258888.top

JS:   if (!data) return;
来源：http://ohc.gaohongyu789.top

TS:   if (!data) return;
来源：http://zzt.sufxvd.cn

Java: if (data == null) return;
来源：http://hht.aizwys.cn

Go:   if data == nil { return }
来源：http://ucx.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://dqm.c1oappe.top

C#:   if (data == null) return;
来源：http://kth.uphjek.com

================================================================================
来源：http://ely.shanyushiyangkeji.top

C. 函数与作用域
来源：http://vpg.cheryme.top

================================================================================
来源：http://olq.zdqjudy.top

[C01] 定义函数
来源：http://jao.ehwqpu.com

Py:   def add(a, b): return a + b
来源：http://orc.aizwys.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tge.nanxinkj.top

JS:   function add(a, b) { return a + b; }
来源：http://idd.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://heh.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://jjt.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://bzy.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://zvp.havefunace.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wuk.zhaomingkeji.xyz

[C02] 默认参数
来源：http://rgd.tanke756.top

Py:   def greet(name="World"): return name
来源：http://fpw.xuanzx.com

PHP:  function greet($name = "World") { return $name; }
来源：http://atf.yueranfly.top

JS:   function greet(name = "World") { return name; }
来源：http://qiz.hfpthk.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ssm.daria6918.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://sxk.mhx1999.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xsx.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://znr.zycfv.cn

C#:   string Greet(string name = "World") => name;
来源：http://rqh.cucudq.cn

[C03] 可变参数
来源：http://bev.hnqzz.top

Py:   def total(*args): return sum(args)
来源：http://hhz.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gel.tianlin.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dsd.shanyushiyangtech.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gln.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://duu.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rvf.zhixingplan.top

Ruby: def total(*nums); nums.sum; end
来源：http://udw.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bye.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://hmg.chenjidiqi.icu

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://crm.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://drv.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vsc.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpt.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://tol.yongpay.top

Go:   // 无：用配置结构体参数
来源：http://nok.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://nqk.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://mvq.zhengqikj.top

[C05] 返回多个值
来源：http://ecj.svipenyu.cn

Py:   return a, b
来源：http://wsx.9152youxi.cn

PHP:  return [$a, $b];
来源：http://uci.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gqd.hesvh.cn

TS:   return { a, b };
来源：http://ahl.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fuj.nwbrower.top

Go:   return a, b
来源：http://edf.ydzc1.top

Ruby: return a, b
来源：http://zmm.hysaishi.cn

C#:   return (a, b);              // ValueTuple
来源：http://cfn.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://bhx.hesvh.cn

Py:   square = lambda x: x * x
来源：http://kkd.nwbrower.top

PHP:  $square = fn($x) => $x * $x;
来源：http://jhv.aibaodan.cn

JS:   const square = x => x * x;
来源：http://rhe.xuanzx.com

TS:   const square = (x: number): number => x * x;
来源：http://exn.daria6918.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oxf.cheryme.top

Go:   sq := func(x int) int { return x * x }
来源：http://ckl.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://bob.jlsjyb.cn

C#:   Func<int, int> square = x => x * x;
来源：http://kge.zhengqikj.top

[C07] 把函数作为参数传入
来源：http://ibf.redwolf501.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mil.vehdjk.com

PHP:  array_map("strtoupper", $arr);
来源：http://pyr.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://opb.hnqzz.top

TS:   arr.map(String)
来源：http://tia.nanxuanxn.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xre.gogol.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ete.xingfuxueyuan.xyz

Ruby: arr.map(&:upcase)
来源：http://pvr.ydjk.org.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://aze.sweek.top

[C08] 闭包
来源：http://udz.jqgufenzy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vye.smart0.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://pdw.ctjpmb.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://oci.cqqwz.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sgm.ehwqpu.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ovz.bbcook.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://izu.epnwcf.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dej.bbcook.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qqq.fzhhl.top

[C09] 递归
来源：http://pkg.hcnkem.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://xok.cqqwz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rxq.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gsv.guannengcc.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pux.sysykeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vuc.tianlin.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://pde.zhiwuduotai.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://djf.hongshengwenyu.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zlz.birdmap.top

[C10] 变量作用域
来源：http://ckz.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cwm.xuanzx.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ydk.svipenyu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rih.ehwqpu.com

TS:   同 JS
来源：http://lgk.cucudq.cn

Java: 方法内为块级作用域
来源：http://ybn.wangdashe.top

Go:   花括号块级作用域
来源：http://dnh.c1oappe.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://tjz.fengsongda.top

C#:   块级作用域
来源：http://cty.cdnleiting.top

[C11] 模块导入与导出
来源：http://itu.zdbjq.cn

Py:   from module import func
来源：http://tck.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ulr.yuanzhike.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://kbv.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://cig.chenzaomai.com

Java: import java.util.List;
来源：http://vdy.redwolf501.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tfs.jinyuanbaomall.cn

Ruby: require "json"; require_relative "./util"
来源：http://xte.mhx1999.top

C#:   using System.Text;
来源：http://upz.ywan-chungtsiang.top

[C12] 立即执行函数 IIFE
来源：http://thl.chenjidiqi.icu

Py:   (lambda: print("run"))()
来源：http://zqe.bjfxy.top

PHP:  (function () { echo "run"; })();
来源：http://ofg.feifeiyinyue.top

JS:   (() => { console.log("run"); })();
来源：http://gnl.aibaodan.cn

TS:   (() => { console.log("run"); })();
来源：http://cwu.yj20258.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ggq.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://vwr.fzhhl.top

Ruby: -> { puts "run" }.call
来源：http://hzm.sjlbkw.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://eqg.hesvh.cn

[C13] 类型声明 / 类型注解
来源：http://qqw.zhongyouzk.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zxp.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zfs.yuanzhike.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zfi.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pyw.iojbl.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cph.hesvh.cn

Go:   func add(a, b int) int
来源：http://ecv.dashuyun.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://otj.ydzc1.top

C#:   int Add(int a, int b) => a + b;
来源：http://wkb.jinqigufen.top

[C14] 泛型函数
来源：http://vem.chenjidiqi.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://myj.sxryk.cn

PHP:  // 无泛型
来源：http://fjz.chenjidiqi.icu

JS:   // 无泛型
来源：http://ojx.yanxiufei.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://yqz.hysaishi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://otl.svipenyu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qbz.vehdjk.com

Ruby: # 无泛型
来源：http://msd.shangyingyoupin.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://foe.yuxming.cn

[C15] 解构 / 展开参数
来源：http://mma.wangshuangyany.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tdh.yangfankeji.com

PHP:  [$a, $b] = $pair;
来源：http://vfk.cdnleiting.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lbf.sxryk.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lzq.fktsv.cn

Java: // 无解构
来源：http://xyd.wangdashe.top

Go:   // 无解构
来源：http://vac.zycfv.cn

Ruby: a, b = pair
来源：http://mja.yj202588.top

C#:   var (a, b) = pair;
来源：http://bad.ybcxt.top

[C16] 函数 / 方法重载
来源：http://aps.hnxiangtu.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://epl.gzhubu.top

PHP:  // 无重载
来源：http://bjw.fktsv.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ekd.fanxiaobao.xyz

TS:   // 用联合类型或重载签名声明
来源：http://ijo.fengsongda.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ein.havefunace.top

Go:   // 无重载：用不同函数名
来源：http://ojo.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://igl.hnxiangtu.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://cun.jinyuanbaomall.cn

================================================================================
来源：http://ppf.meibo888.top

D. 数组 / 列表 / 集合
来源：http://bdj.zhaomingkeji.xyz

================================================================================
来源：http://rsn.zhoulong.xyz

[D01] 创建数组 / 列表
来源：http://hef.epnwcf.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wvy.yueranfly.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://xmd.cucudq.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://fjm.cashguo.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ckf.quarkkingdee.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lah.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://dwh.meibo888.top

Ruby: arr = [1, 2, 3]
来源：http://bzd.zhengqikj.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bpo.pengpengdd.cyou

[D02] 追加元素到末尾
来源：http://iaf.hcnkem.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://omu.xinyue.icu

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ukg.hfpthk.cn

JS:   arr.push(4);
来源：http://lpc.xylfe.cn

TS:   arr.push(4);
来源：http://ccq.kuanghao11.cn

Java: list.add(4);
来源：http://zps.ydjk.org.cn

Go:   arr = append(arr, 4)
来源：http://qjr.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://ehp.yonumen.top

C#:   list.Add(4);
来源：http://vmt.bjfxy.top

[D03] 在指定位置插入元素
来源：http://lkz.dashuyun.cn

Py:   arr.insert(0, 0)
来源：http://yzs.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qmd.fehbvm.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fld.quarkkingdee.top


<!-- 参考信息 -->