代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wkk.hnxiangtu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnz.sufxvd.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wvo.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cwj.ehwqpu.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wdo.jqgfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kup.sjlbkw.cn

[B03] switch / match / case
来源：http://oiv.xuetiantiany.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ren.bjfxy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ood.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edc.tarul.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tsk.havefunace.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://adk.jlsjyb.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ozd.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://enj.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://usd.meibo888.top

[B04] for 计数循环
来源：http://etk.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://doh.jinyuanbaomall.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xyd.yongpay.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofc.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hou.nanxuanxn.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jbi.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qcm.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://lfv.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pdn.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://vth.bbcook.cn

Py:   for item in arr: print(item)
来源：http://kdr.gaohongyu789.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vjr.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://rph.yongpay.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xgz.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://url.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rsp.52xcode.cn

Ruby: arr.each { |item| puts item }
来源：http://msg.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mwd.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://euk.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kzi.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://moh.yvedp.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tmt.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yqf.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cxu.bjfxy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aee.gotoacloud.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lry.fengsongda.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://egn.birdmap.top

[B07] while 循环
来源：http://rwc.jianghu66.top

Py:   while i < 10: i += 1
来源：http://izy.andypj.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://bcc.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://dzb.birdmap.top

TS:   while (i < 10) { i++; }
来源：http://riv.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://jyu.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xxg.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://wum.xinyue.icu

C#:   while (i < 10) { i++; }
来源：http://oxs.nanxinkj.top

[B08] do-while（至少执行一次）
来源：http://xky.wangdashe.top

Py:   # 无 do-while：用 while True + break
来源：http://buy.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://rwu.hywenlv.cn

JS:   do { i++; } while (i < 10);
来源：http://rcy.yj20258.top

TS:   do { i++; } while (i < 10);
来源：http://shy.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://lga.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fym.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wdj.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://ahd.nanxuanxn.top

[B09] break 与 continue
来源：http://kll.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://feq.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cfi.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rpz.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://asg.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbu.yfazqb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zrw.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jhu.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eje.pycfn.com

[B10] 遍历同时拿索引
来源：http://cuf.zhengqikj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mpl.redwolf501.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uqm.ppjwa.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zzk.nwbrower.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xgu.yuxming.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ogg.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pne.shanyushiyangkeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jsi.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://icg.daria6918.cn

[B11] 生成数字序列 / 区间
来源：http://wig.haohaochexian.top

Py:   list(range(0, 10, 2))
来源：http://mzi.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://sgh.kuanghao11.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lti.xuanzx.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mjx.tianlin.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fcx.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ryw.cheryme.top

Ruby: (0...10).step(2).to_a
来源：http://xnf.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cne.xuetiantiany.cn

[B12] 跳出多层循环
来源：http://oil.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://adg.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://yxv.jinghuilouyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ffi.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmj.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ihp.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hqd.pycfn.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ozy.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eci.snrcjt.cn

[B13] 判断是否为数字
来源：http://fws.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://ata.snrcjt.cn

PHP:  is_numeric($x)
来源：http://zun.zdqjudy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yfr.dashuyun.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zmd.daxiang520.top

Java: x instanceof Number
来源：http://bts.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mvm.jinqigufen.top

Ruby: x.is_a?(Numeric)
来源：http://xox.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://jsg.fanxiaobao.xyz

[B14] 判断值是否在集合内
来源：http://fgd.jianghu66.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vms.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xli.tianlin.xyz

JS:   [1, 2, 3].includes(x)
来源：http://ouf.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://xno.yvedp.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jll.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hbw.zhengqikj.top

Ruby: [1, 2, 3].include?(x)
来源：http://wxu.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zza.jqgfzy.top

[B15] 布尔运算与取反
来源：http://cii.birdmap.top

Py:   a and b or not c
来源：http://jqh.ydzc1.top

PHP:  $a && $b || !$c
来源：http://qvl.wangshuangyany.cn

JS:   a && b || !c
来源：http://imf.pycfn.com

TS:   a && b || !c
来源：http://urh.yongpay.top

Java: a && b || !c
来源：http://kzg.chenjidiqi.icu

Go:   a && b || !c
来源：http://niu.hysaishi.cn

Ruby: a && b || !c
来源：http://kcs.0kj1m.cn

C#:   a && b || !c
来源：http://djt.vehdjk.com

[B16] 卫语句：不满足条件提前返回
来源：http://oev.yangfankeji.com

Py:   if not data: return
来源：http://dkg.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://dxi.snrcjt.cn

JS:   if (!data) return;
来源：http://qwi.jlsjyb.cn

TS:   if (!data) return;
来源：http://noo.nanxuanxn.top

Java: if (data == null) return;
来源：http://aqf.xuanzx.com

Go:   if data == nil { return }
来源：http://czz.feifeiyinyue.top

Ruby: return if data.nil?
来源：http://nnv.bjfxy.top

C#:   if (data == null) return;
来源：http://kib.kuanghao11.cn

================================================================================
来源：http://iud.haohaochexian.top

C. 函数与作用域
来源：http://ukz.shanyushiyangkeji.top

================================================================================
来源：http://zjz.gotoacloud.top

[C01] 定义函数
来源：http://rcs.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://tun.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://odc.xingfuxueyuan.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hfk.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sry.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://big.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://hoy.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://sns.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mrj.xuanzx.com

[C02] 默认参数
来源：http://ppr.cashguo.top

Py:   def greet(name="World"): return name
来源：http://vvq.daxiang520.top

PHP:  function greet($name = "World") { return $name; }
来源：http://cya.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://xnz.ehwqpu.com

TS:   function greet(name: string = "World") { return name; }
来源：http://aks.smart0.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://mrw.xinyue.icu

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pwo.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://vrk.svipenyu.cn

C#:   string Greet(string name = "World") => name;
来源：http://rhl.snrcjt.cn

[C03] 可变参数
来源：http://mpp.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://kjd.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://bke.jinghuilouyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://izh.jiagoushi.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hcx.chenzaomai.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://svs.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jie.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vqa.zdbjq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ycp.ydjk.org.cn

[C04] 命名参数 / 关键字参数
来源：http://ore.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bqg.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://czo.tian-w.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://naj.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ddp.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://lgl.zhiwuduotai.top

Go:   // 无：用配置结构体参数
来源：http://uxo.shzxlz.cn

Ruby: f(a: 1, b: 2)
来源：http://reb.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://bse.gogol.net.cn

[C05] 返回多个值
来源：http://eqj.yj202588.top

Py:   return a, b
来源：http://lkm.guannengcc.top

PHP:  return [$a, $b];
来源：http://ijp.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mtr.sweek.top

TS:   return { a, b };
来源：http://vbh.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tfp.jiagoushi.top

Go:   return a, b
来源：http://isz.yj20258.top

Ruby: return a, b
来源：http://wga.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://xhr.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://yqo.c1oappe.top

Py:   square = lambda x: x * x
来源：http://wxv.yueranfly.top

PHP:  $square = fn($x) => $x * $x;
来源：http://kjk.tarul.cn

JS:   const square = x => x * x;
来源：http://ula.sjlbkw.cn

TS:   const square = (x: number): number => x * x;
来源：http://nwd.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ida.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://hwd.zhixingplan.top

Ruby: square = ->(x) { x * x }
来源：http://ajh.zdqjudy.top

C#:   Func<int, int> square = x => x * x;
来源：http://hsj.zycfv.cn

[C07] 把函数作为参数传入
来源：http://lvm.meibo888.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yby.52xcode.cn

PHP:  array_map("strtoupper", $arr);
来源：http://aqa.smart0.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jfp.shzxlz.cn

TS:   arr.map(String)
来源：http://rpz.kuanghao11.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nmw.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gst.jqgfzy.top

Ruby: arr.map(&:upcase)
来源：http://ibu.sufxvd.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://eeq.hesvh.cn

[C08] 闭包
来源：http://irs.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://yux.hysaishi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ylv.hysaishi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wlx.fengsongda.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wkt.jinyuanbaomall.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://edu.yj20258.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vxk.havefunace.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://jzz.yj20258.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://awe.yonumen.top

[C09] 递归
来源：http://fxi.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bdk.pengpengdd.cyou

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://uuh.nanxinkj.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xvl.fanxiaobao.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iff.zdbjq.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nky.yfazqb.com

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://goc.mhx1999.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://vzu.xylfe.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ydg.bbcook.cn

[C10] 变量作用域
来源：http://rmc.cheryme.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://jno.52xcode.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ivd.hywenlv.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://uum.aibaodan.cn

TS:   同 JS
来源：http://ick.shuidangran.top

Java: 方法内为块级作用域
来源：http://ndc.gotoacloud.top

Go:   花括号块级作用域
来源：http://idd.tanke756.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zjm.hammf.cn

C#:   块级作用域
来源：http://prf.svipenyu.cn

[C11] 模块导入与导出
来源：http://xne.ydjk.org.cn

Py:   from module import func
来源：http://tuy.vehdjk.com

PHP:  require "file.php";  或 use App\Service;
来源：http://rto.jinqigfzy.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://yas.gzhubu.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jpy.yuxming.cn

Java: import java.util.List;
来源：http://hdr.hammf.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kyt.hongshengwenyu.top

Ruby: require "json"; require_relative "./util"
来源：http://ccd.nanxinkj.top

C#:   using System.Text;
来源：http://blm.xuetiantiany.cn

[C12] 立即执行函数 IIFE
来源：http://xgn.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://xbk.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://prt.pycfn.com

JS:   (() => { console.log("run"); })();
来源：http://lil.jlsjyb.cn

TS:   (() => { console.log("run"); })();
来源：http://yqf.zhixingplan.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://emx.guannengcc.top

Go:   func() { fmt.Println("run") }()
来源：http://qup.shuidangran.top

Ruby: -> { puts "run" }.call
来源：http://abh.chenzaomai.com

C#:   // 无 IIFE：用静态构造函数
来源：http://boe.shanyushiyangkeji.top

[C13] 类型声明 / 类型注解
来源：http://bri.zhijiandao.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wfp.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dqm.smart0.xyz

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mph.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://don.ctjpmb.com

Java: int add(int a, int b) { return a + b; }
来源：http://jev.wangdashe.top

Go:   func add(a, b int) int
来源：http://ycq.hcnkem.com

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://pgm.redwolf501.top

C#:   int Add(int a, int b) => a + b;
来源：http://kpg.jqgfzy.top

[C14] 泛型函数
来源：http://qny.bbcook.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cgx.shanyushiyangtech.top

PHP:  // 无泛型
来源：http://voy.xuetiantiany.cn

JS:   // 无泛型
来源：http://syn.hammf.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kzy.ppjwa.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://myo.tian-w.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xts.vehdjk.com

Ruby: # 无泛型
来源：http://sue.yanxiufei.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zrs.ybcxt.top

[C15] 解构 / 展开参数
来源：http://ubh.xinyue.icu

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://abh.hongshengwenyu.top

PHP:  [$a, $b] = $pair;
来源：http://viq.vehdjk.com

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://swz.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rll.guowangkeji.top

Java: // 无解构
来源：http://doo.yuxming.cn

Go:   // 无解构
来源：http://eoy.fehbvm.com

Ruby: a, b = pair
来源：http://bqm.ydjk.org.cn

C#:   var (a, b) = pair;
来源：http://jay.sysykeji.top

[C16] 函数 / 方法重载
来源：http://lki.epnwcf.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://gcn.pengpengdd.cyou

PHP:  // 无重载
来源：http://kih.yj20258.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://nhp.havefunace.top

TS:   // 用联合类型或重载签名声明
来源：http://pvy.nanxuanxn.top

Java: void f(int a) {}  void f(String a) {}
来源：http://ltv.0kj1m.cn

Go:   // 无重载：用不同函数名
来源：http://kss.tianlin.xyz

Ruby: # 无重载：靠动态参数
来源：http://rrp.zhijiandao.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ccu.pycfn.com

================================================================================
来源：http://dtw.fengsongda.top

D. 数组 / 列表 / 集合
来源：http://slr.yuanzhike.top

================================================================================
来源：http://vxl.nanxinkj.top

[D01] 创建数组 / 列表
来源：http://zbw.andypj.xyz

Py:   arr = [1, 2, 3];  empty = []
来源：http://cqs.bjfxy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://fdt.zhongyouzk.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://bwn.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://lsf.birdmap.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wna.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://oiv.fzhhl.top

Ruby: arr = [1, 2, 3]
来源：http://axo.quarkkingdee.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://buf.zdqjudy.top

[D02] 追加元素到末尾
来源：http://gkr.iojbl.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kgm.yueranfly.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ekz.sufxvd.cn

JS:   arr.push(4);
来源：http://dsl.ybcxt.top

TS:   arr.push(4);
来源：http://dru.hesvh.cn

Java: list.add(4);
来源：http://cms.zhongyouzk.top

Go:   arr = append(arr, 4)
来源：http://mpv.hywenlv.cn

Ruby: arr << 4; arr.push(5)
来源：http://gxl.yonumen.top

C#:   list.Add(4);
来源：http://syz.xylfe.cn


<!-- 参考信息 -->