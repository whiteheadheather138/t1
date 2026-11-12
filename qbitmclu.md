代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xrh.uphjek.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ils.xingfuxueyuan.xyz

[B03] switch / match / case
来源：http://vut.bbcook.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uye.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mki.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jrv.jinyuanbaomall.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://max.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ajr.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qoy.iojbl.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zlm.hongshengwenyu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mwf.yj202588.top

[B04] for 计数循环
来源：http://nhn.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://oqq.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://smk.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://izt.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obq.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jsn.yueranfly.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gmd.iojbl.cn

Ruby: 10.times { |i| puts i }
来源：http://pmg.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://asg.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://tmr.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://iya.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oei.fzhhl.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xmi.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wcm.xingfuxueyuan.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://byg.sysykeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bpi.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://kqy.52xcode.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://deq.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://clo.yangfankeji.com

Py:   for k, v in d.items(): print(k, v)
来源：http://ltt.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rrx.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fbv.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://olk.yj20258.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://has.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ncv.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eyg.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://guu.jlsjyb.cn

[B07] while 循环
来源：http://azs.kuanghao11.cn

Py:   while i < 10: i += 1
来源：http://uhu.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://gyt.sweek.top

JS:   while (i < 10) { i++; }
来源：http://amd.mhx1999.top

TS:   while (i < 10) { i++; }
来源：http://cus.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://bny.xingfuxueyuan.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ioq.pengpengdd.cyou

Ruby: while i < 10; i += 1; end
来源：http://zes.zhaomingkeji.xyz

C#:   while (i < 10) { i++; }
来源：http://bhy.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://eul.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://fhm.tanke756.top

PHP:  do { $i++; } while ($i < 10);
来源：http://opw.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://ded.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://imp.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://gaa.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wgu.redwolf501.top

Ruby: begin; i += 1; end while i < 10
来源：http://zxd.gogol.net.cn

C#:   do { i++; } while (i < 10);
来源：http://zjq.fktsv.cn

[B09] break 与 continue
来源：http://itc.hfpthk.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hyl.uphjek.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rkq.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lyc.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ouh.jianghu66.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dsw.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://tpw.xziqi.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hbn.fehbvm.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmf.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://cwn.xuanzx.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iqx.aizwys.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ivr.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wyw.xylfe.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tao.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vcy.ydjk.org.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rhy.tarul.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tak.sufxvd.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ljx.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://pox.aizwys.cn

Py:   list(range(0, 10, 2))
来源：http://kqs.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://hgs.gogol.net.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fmc.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cgm.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hui.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://evz.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://qpy.svipenyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fet.jiagoushi.top

[B12] 跳出多层循环
来源：http://lzy.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kjp.fehbvm.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://zec.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bur.ehwqpu.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mhn.shanyushiyangtech.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lli.hnxiangtu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ppu.hnxiangtu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gyn.zhaomingkeji.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://apt.nwbrower.top

[B13] 判断是否为数字
来源：http://far.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://fjn.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://rnp.chenjidiqi.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vxs.hcnkem.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vhg.cashguo.top

Java: x instanceof Number
来源：http://prd.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yuk.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://kve.shanyushiyangtech.top

C#:   x is int or double or decimal
来源：http://hek.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://emn.gzhubu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yht.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sya.quarkkingdee.top

JS:   [1, 2, 3].includes(x)
来源：http://iky.jlsjyb.cn

TS:   [1, 2, 3].includes(x)
来源：http://mmq.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gtt.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tut.cashguo.top

Ruby: [1, 2, 3].include?(x)
来源：http://hdn.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aig.cashguo.top

[B15] 布尔运算与取反
来源：http://iio.pengpengdd.cyou

Py:   a and b or not c
来源：http://jyt.sxryk.cn

PHP:  $a && $b || !$c
来源：http://gfk.xinyue.icu

JS:   a && b || !c
来源：http://unv.hywenlv.cn

TS:   a && b || !c
来源：http://asz.zhengqikj.top

Java: a && b || !c
来源：http://noz.andypj.xyz

Go:   a && b || !c
来源：http://hwo.zycfv.cn

Ruby: a && b || !c
来源：http://mpp.vehdjk.com

C#:   a && b || !c
来源：http://khr.fktsv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sud.uphjek.com

Py:   if not data: return
来源：http://zwv.hammf.cn

PHP:  if (!$data) { return; }
来源：http://bzm.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://caz.andypj.xyz

TS:   if (!data) return;
来源：http://juy.pycfn.com

Java: if (data == null) return;
来源：http://coc.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://nrt.0kj1m.cn

Ruby: return if data.nil?
来源：http://nes.ydjk.org.cn

C#:   if (data == null) return;
来源：http://wja.xuanzx.com

================================================================================
来源：http://tqq.jinyuanbaomall.cn

C. 函数与作用域
来源：http://ssu.hcnkem.com

================================================================================
来源：http://sip.sxryk.cn

[C01] 定义函数
来源：http://rfs.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://odf.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dgj.havefunace.top

JS:   function add(a, b) { return a + b; }
来源：http://auc.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nwv.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://flg.ydjk.org.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ipg.jianghu66.top

Ruby: def add(a, b); a + b; end
来源：http://fbj.pengpengdd.cyou

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vww.wangdashe.top

[C02] 默认参数
来源：http://sir.fanxiaobao.xyz

Py:   def greet(name="World"): return name
来源：http://ros.gzhubu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://mtn.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://oxr.cdnleiting.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rsj.tianlin.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://oie.jqgufenzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://irr.jinyuanbaomall.cn

Ruby: def greet(name = "World") = name
来源：http://tug.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://fcu.sufxvd.cn

[C03] 可变参数
来源：http://bij.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://ttf.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cls.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oeq.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vzg.xinyue.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bmd.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://joq.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://dtm.haohaochexian.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aeh.zdqjudy.top

[C04] 命名参数 / 关键字参数
来源：http://slo.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://try.sysykeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jbv.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://igv.sjlbkw.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://alu.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://tgn.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://jxb.hammf.cn

Ruby: f(a: 1, b: 2)
来源：http://rss.epnwcf.com

C#:   f(a: 1, b: 2)
来源：http://lae.andypj.xyz

[C05] 返回多个值
来源：http://yjq.xziqi.cn

Py:   return a, b
来源：http://ors.fehbvm.com

PHP:  return [$a, $b];
来源：http://twi.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oyr.aizwys.cn

TS:   return { a, b };
来源：http://erx.dashuyun.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hqo.0kj1m.cn

Go:   return a, b
来源：http://vpj.zhijiandao.cn

Ruby: return a, b
来源：http://gcb.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://hhq.fengsongda.top

[C06] 匿名函数 / lambda
来源：http://heo.pengpengdd.cyou

Py:   square = lambda x: x * x
来源：http://bgv.smart0.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://xvg.tanke756.top

JS:   const square = x => x * x;
来源：http://wkh.zhixingplan.top

TS:   const square = (x: number): number => x * x;
来源：http://hdc.feifeiyinyue.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nro.hammf.cn

Go:   sq := func(x int) int { return x * x }
来源：http://srr.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://tyu.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://zkc.yangfankeji.com

[C07] 把函数作为参数传入
来源：http://rvz.fanxiaobao.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qbb.tian-w.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wib.cucudq.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://usg.fehbvm.com

TS:   arr.map(String)
来源：http://gki.yongpay.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ata.hesvh.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jmu.yuanzhike.top

Ruby: arr.map(&:upcase)
来源：http://cog.guowangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zmz.tianlin.xyz

[C08] 闭包
来源：http://pjf.sweek.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kmx.hammf.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://daw.tian-w.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qec.tianlin.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qcy.sjlbkw.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://alz.fzhhl.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://cbf.jinyuanbaomall.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gnz.chenlongwang.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nul.epnwcf.com

[C09] 递归
来源：http://urc.xinyue.icu

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mks.yvedp.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://anr.hywenlv.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ekl.yfazqb.com

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mqj.fengsongda.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ulp.zhaomingkeji.xyz

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fbt.xuanzx.com

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pil.guannengcc.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kcf.aibaodan.cn

[C10] 变量作用域
来源：http://ajn.zycfv.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://fhz.fehbvm.com

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lyb.zhaomingkeji.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nkr.gotoacloud.top

TS:   同 JS
来源：http://hsa.chenlongwang.top

Java: 方法内为块级作用域
来源：http://mat.jinqigfzy.top

Go:   花括号块级作用域
来源：http://pvb.ywan-chungtsiang.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wbz.vqdsnc.cn

C#:   块级作用域
来源：http://mke.havefunace.top

[C11] 模块导入与导出
来源：http://xxh.hammf.cn

Py:   from module import func
来源：http://jxi.ydzc1.top

PHP:  require "file.php";  或 use App\Service;
来源：http://pds.yj20258.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rdx.iojbl.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://brz.hnxiangtu.top

Java: import java.util.List;
来源：http://wga.svipenyu.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://jcx.fanxiaobao.xyz

Ruby: require "json"; require_relative "./util"
来源：http://njl.wangshuangyany.cn

C#:   using System.Text;
来源：http://zmt.zhongyouzk.top

[C12] 立即执行函数 IIFE
来源：http://jxo.vqdsnc.cn

Py:   (lambda: print("run"))()
来源：http://qrv.dashuyun.cn

PHP:  (function () { echo "run"; })();
来源：http://jdn.jlsjyb.cn

JS:   (() => { console.log("run"); })();
来源：http://mcg.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://jln.cdnleiting.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gew.pycfn.com

Go:   func() { fmt.Println("run") }()
来源：http://leo.shangyingyoupin.top

Ruby: -> { puts "run" }.call
来源：http://pxv.guowangkeji.top

C#:   // 无 IIFE：用静态构造函数
来源：http://mdx.pycfn.com

[C13] 类型声明 / 类型注解
来源：http://ycl.wangdashe.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aia.xuetiantiany.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mmh.zdqjudy.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://uak.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dts.zhaomingkeji.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://mdb.tarul.cn

Go:   func add(a, b int) int
来源：http://qtt.ehwqpu.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mur.bbcook.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lpg.sysykeji.top

[C14] 泛型函数
来源：http://ymd.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gbx.meibo888.top

PHP:  // 无泛型
来源：http://pzg.dashuyun.cn

JS:   // 无泛型
来源：http://mfg.yj20258.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kke.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lbx.jqgfzy.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gyx.shanyushiyangkeji.top

Ruby: # 无泛型
来源：http://swo.ivvv.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hir.jinghuilouyu.cn

[C15] 解构 / 展开参数
来源：http://pss.yuxming.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://cjj.mhx1999.top

PHP:  [$a, $b] = $pair;
来源：http://rah.zhijiandao.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jih.aibaodan.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jah.gogol.net.cn

Java: // 无解构
来源：http://dly.jinyuanbaomall.cn

Go:   // 无解构
来源：http://cdv.jiagoushi.top

Ruby: a, b = pair
来源：http://chs.vehdjk.com

C#:   var (a, b) = pair;
来源：http://tye.jinghuilouyu.cn

[C16] 函数 / 方法重载
来源：http://zzf.meibo888.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vab.ehwqpu.com

PHP:  // 无重载
来源：http://zbd.zdbjq.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://fpj.chenlongwang.top

TS:   // 用联合类型或重载签名声明
来源：http://bql.jianghu66.top

Java: void f(int a) {}  void f(String a) {}
来源：http://wja.yuxming.cn

Go:   // 无重载：用不同函数名
来源：http://bqc.jinyuanbaomall.cn

Ruby: # 无重载：靠动态参数
来源：http://tee.yangfankeji.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://anl.quarkkingdee.top

================================================================================
来源：http://vkl.epnwcf.com

D. 数组 / 列表 / 集合
来源：http://apr.shangyingyoupin.top

================================================================================
来源：http://odj.shangyingyoupin.top

[D01] 创建数组 / 列表
来源：http://yyh.yuanzhike.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://tos.tianlin.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qcz.shanyushiyangtech.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wov.pycfn.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://oqp.guowangkeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://aha.pengpengdd.cyou

Go:   arr := []int{1, 2, 3}
来源：http://sxz.zhengqikj.top

Ruby: arr = [1, 2, 3]
来源：http://lpd.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pfl.shanyushiyangkeji.top

[D02] 追加元素到末尾
来源：http://ghn.yangfankeji.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lbx.shanyushiyangkeji.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hpi.shzxlz.cn

JS:   arr.push(4);
来源：http://vze.zhaomingkeji.xyz

TS:   arr.push(4);
来源：http://vsf.jinghuilouyu.cn

Java: list.add(4);
来源：http://fet.xuetiantiany.cn

Go:   arr = append(arr, 4)
来源：http://xfu.cashguo.top

Ruby: arr << 4; arr.push(5)
来源：http://bfl.tian-w.cn

C#:   list.Add(4);
来源：http://rnk.gogol.net.cn

[D03] 在指定位置插入元素
来源：http://lgb.tianlin.xyz

Py:   arr.insert(0, 0)
来源：http://rlg.xziqi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ees.xziqi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ajv.vqdsnc.cn


<!-- 参考信息 -->