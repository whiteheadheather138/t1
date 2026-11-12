代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uii.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mri.vehdjk.com

[B03] switch / match / case
来源：http://hjm.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kyn.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vpe.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tom.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://irk.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ato.iojbl.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jez.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zro.sweek.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pyk.epnwcf.com

[B04] for 计数循环
来源：http://any.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://gxf.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://obe.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yhe.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hwg.gaohongyu789.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://omb.jinghuilouyu.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ucv.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://xzo.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://htz.tian-w.cn

[B05] 遍历数组 / 列表
来源：http://lqb.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://fpy.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hgp.jinqigfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ewp.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://plc.nwbrower.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kay.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://saj.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://mup.ydzc1.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rhk.cheryme.top

[B06] 遍历字典 / 对象
来源：http://jdv.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pqi.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ewe.fanxiaobao.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xly.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wyc.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://elu.tian-w.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jih.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pkv.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lcv.andypj.xyz

[B07] while 循环
来源：http://vgz.tarul.cn

Py:   while i < 10: i += 1
来源：http://aby.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://llx.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://zfi.jqgufenzy.top

TS:   while (i < 10) { i++; }
来源：http://rzp.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://nvs.jinyuanbaomall.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sgg.hcnkem.com

Ruby: while i < 10; i += 1; end
来源：http://lpt.zhiwuduotai.top

C#:   while (i < 10) { i++; }
来源：http://pvj.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://iwr.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://vax.hysaishi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xrm.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://klu.quarkkingdee.top

TS:   do { i++; } while (i < 10);
来源：http://vnu.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://nqk.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dvv.gaohongyu789.top

Ruby: begin; i += 1; end while i < 10
来源：http://kci.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://lmr.jyoumei.cn

[B09] break 与 continue
来源：http://nhs.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kxb.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fpv.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xqx.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uiw.gogol.net.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsp.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqf.zhijiandao.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lez.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wka.kuanghao11.cn

[B10] 遍历同时拿索引
来源：http://obz.yonumen.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://abi.nanxuanxn.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wdu.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ioi.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mrb.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rol.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://chy.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://usp.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://oqo.aibaodan.cn

[B11] 生成数字序列 / 区间
来源：http://hmg.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://oqr.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://cuk.zhongyouzk.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://win.andypj.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhe.hysaishi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mhz.tianlin.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rht.yanxiufei.cn

Ruby: (0...10).step(2).to_a
来源：http://myt.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wub.guannengcc.top

[B12] 跳出多层循环
来源：http://nlm.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://zou.dashuyun.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zbb.fanxiaobao.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ggs.cashguo.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ido.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://stx.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bvx.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lgu.jiagoushi.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eym.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://ybu.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://rsy.fzhhl.top

PHP:  is_numeric($x)
来源：http://fgi.haohaochexian.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qob.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ecj.tarul.cn

Java: x instanceof Number
来源：http://yqg.redwolf501.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ncj.nwbrower.top

Ruby: x.is_a?(Numeric)
来源：http://jbm.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://uns.yj20258.top

[B14] 判断值是否在集合内
来源：http://lrp.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ben.nanxuanxn.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://epq.xylfe.cn

JS:   [1, 2, 3].includes(x)
来源：http://ngn.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://cfe.aibaodan.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://udh.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ubr.andypj.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://mac.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tpl.cucudq.cn

[B15] 布尔运算与取反
来源：http://utn.yvedp.cn

Py:   a and b or not c
来源：http://joo.sufxvd.cn

PHP:  $a && $b || !$c
来源：http://xab.ybcxt.top

JS:   a && b || !c
来源：http://iyu.yfazqb.com

TS:   a && b || !c
来源：http://vsc.yangfankeji.com

Java: a && b || !c
来源：http://zbu.daxiang520.top

Go:   a && b || !c
来源：http://lio.jyoumei.cn

Ruby: a && b || !c
来源：http://see.cucudq.cn

C#:   a && b || !c
来源：http://ldu.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://jhh.nanxinkj.top

Py:   if not data: return
来源：http://efm.pycfn.com

PHP:  if (!$data) { return; }
来源：http://lgu.mhx1999.top

JS:   if (!data) return;
来源：http://lro.cashguo.top

TS:   if (!data) return;
来源：http://cjd.hesvh.cn

Java: if (data == null) return;
来源：http://brt.zycfv.cn

Go:   if data == nil { return }
来源：http://aoz.hywenlv.cn

Ruby: return if data.nil?
来源：http://bec.sufxvd.cn

C#:   if (data == null) return;
来源：http://zuv.ctjpmb.com

================================================================================
来源：http://tnx.zhijiandao.cn

C. 函数与作用域
来源：http://cuf.haohaochexian.top

================================================================================
来源：http://fzl.pycfn.com

[C01] 定义函数
来源：http://ztv.bjfxy.top

Py:   def add(a, b): return a + b
来源：http://hzj.yanxiufei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yku.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://orl.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xas.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://wsx.cucudq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://zhd.daria6918.cn

Ruby: def add(a, b); a + b; end
来源：http://kzz.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fiz.cashguo.top

[C02] 默认参数
来源：http://jds.cucudq.cn

Py:   def greet(name="World"): return name
来源：http://tcr.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://sgg.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://edw.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://btu.daxiang520.top

Java: // 无默认参数：方法重载或 Optional
来源：http://iev.zdqjudy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vex.bbcook.cn

Ruby: def greet(name = "World") = name
来源：http://yig.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://xnc.iojbl.cn

[C03] 可变参数
来源：http://atf.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://idl.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://rvn.c1oappe.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lkf.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrg.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://yob.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://dwz.dianchejie.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lwf.kuanghao11.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zcd.yj20258.top

[C04] 命名参数 / 关键字参数
来源：http://bve.0kj1m.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eth.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rha.yvedp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://amu.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qni.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://qxs.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://njz.sysykeji.top

Ruby: f(a: 1, b: 2)
来源：http://wgb.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://vvq.yj20258.top

[C05] 返回多个值
来源：http://dmy.ctjpmb.com

Py:   return a, b
来源：http://ucx.sweek.top

PHP:  return [$a, $b];
来源：http://ncj.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://fgv.cashguo.top

TS:   return { a, b };
来源：http://opj.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cei.sjlbkw.cn

Go:   return a, b
来源：http://clo.mhx1999.top

Ruby: return a, b
来源：http://hod.yanxiufei.cn

C#:   return (a, b);              // ValueTuple
来源：http://yel.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://ncm.yonumen.top

Py:   square = lambda x: x * x
来源：http://pqx.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://veq.svipenyu.cn

JS:   const square = x => x * x;
来源：http://plu.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://obr.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hze.9152youxi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://drb.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://rni.shanyushiyangkeji.top

C#:   Func<int, int> square = x => x * x;
来源：http://dqo.guannengcc.top

[C07] 把函数作为参数传入
来源：http://cef.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ooj.uphjek.com

PHP:  array_map("strtoupper", $arr);
来源：http://hfd.jyoumei.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://egv.hywenlv.cn

TS:   arr.map(String)
来源：http://fxk.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://jzr.jqgufenzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qhi.zhongyouzk.top

Ruby: arr.map(&:upcase)
来源：http://hbv.gzhubu.top

C#:   arr.Select(s => s.ToUpper())
来源：http://ioi.gaohongyu789.top

[C08] 闭包
来源：http://sah.hywenlv.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://teo.fehbvm.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://irt.zhongyouzk.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vsb.sxryk.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ufh.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bbm.hysaishi.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ihh.cashguo.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fte.yangfankeji.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://msa.bbcook.cn

[C09] 递归
来源：http://dqk.gotoacloud.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hcg.zhoulong.xyz

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fdv.fehbvm.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rzq.cdnleiting.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iyu.sufxvd.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://eip.hesvh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://giu.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zzw.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://nxf.zycfv.cn

[C10] 变量作用域
来源：http://plm.cucudq.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vtc.xuetiantiany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://eei.sjlbkw.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://klq.smart0.xyz

TS:   同 JS
来源：http://vso.yangfankeji.com

Java: 方法内为块级作用域
来源：http://qpp.yfazqb.com

Go:   花括号块级作用域
来源：http://pvs.zhengqikj.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://led.pengpengdd.cyou

C#:   块级作用域
来源：http://yxq.xinyue.icu

[C11] 模块导入与导出
来源：http://vxw.meibo888.top

Py:   from module import func
来源：http://trx.9152youxi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://tms.cqqwz.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sta.havefunace.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xcb.fehbvm.com

Java: import java.util.List;
来源：http://yus.guannengcc.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vby.0kj1m.cn

Ruby: require "json"; require_relative "./util"
来源：http://ffv.sysykeji.top

C#:   using System.Text;
来源：http://qnp.sufxvd.cn

[C12] 立即执行函数 IIFE
来源：http://pqt.gzhubu.top

Py:   (lambda: print("run"))()
来源：http://kxt.fktsv.cn

PHP:  (function () { echo "run"; })();
来源：http://fus.nanxinkj.top

JS:   (() => { console.log("run"); })();
来源：http://skq.fzhhl.top

TS:   (() => { console.log("run"); })();
来源：http://qaj.fehbvm.com

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://kae.zdbjq.cn

Go:   func() { fmt.Println("run") }()
来源：http://xbw.tianlin.xyz

Ruby: -> { puts "run" }.call
来源：http://grh.dianchejie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://omq.zycfv.cn

[C13] 类型声明 / 类型注解
来源：http://knf.bbcook.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://moq.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zca.ppjwa.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rzw.guowangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tsx.zhijiandao.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fwo.xinyue.icu

Go:   func add(a, b int) int
来源：http://zda.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://aoz.fzhhl.top

C#:   int Add(int a, int b) => a + b;
来源：http://fhs.yueranfly.top

[C14] 泛型函数
来源：http://psl.sxryk.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://szm.birdmap.top

PHP:  // 无泛型
来源：http://ync.daxiang520.top

JS:   // 无泛型
来源：http://slm.kuanghao11.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ixr.nwbrower.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://klx.daxiang520.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://qxu.jinqigfzy.top

Ruby: # 无泛型
来源：http://drn.xuanzx.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dou.chenzaomai.com

[C15] 解构 / 展开参数
来源：http://bhw.guannengcc.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dzk.ybcxt.top

PHP:  [$a, $b] = $pair;
来源：http://fvq.pengpengdd.cyou

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://odi.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ieq.hysaishi.cn

Java: // 无解构
来源：http://yxz.jinyuanbaomall.cn

Go:   // 无解构
来源：http://zwn.yangfankeji.com

Ruby: a, b = pair
来源：http://kju.zhijiandao.cn

C#:   var (a, b) = pair;
来源：http://afe.zhengqikj.top

[C16] 函数 / 方法重载
来源：http://gtr.wangdashe.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://dmj.havefunace.top

PHP:  // 无重载
来源：http://yda.cqqwz.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lpt.ybcxt.top

TS:   // 用联合类型或重载签名声明
来源：http://mrj.jlsjyb.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vzz.cashguo.top

Go:   // 无重载：用不同函数名
来源：http://yfz.daxiang520.top

Ruby: # 无重载：靠动态参数
来源：http://cgs.yueranfly.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://jjn.yfazqb.com

================================================================================
来源：http://jer.jqgufenzy.top

D. 数组 / 列表 / 集合
来源：http://nzu.sweek.top

================================================================================
来源：http://qdh.yangfankeji.com

[D01] 创建数组 / 列表
来源：http://hrt.fehbvm.com

Py:   arr = [1, 2, 3];  empty = []
来源：http://wyy.yvedp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://voz.guowangkeji.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ktf.cheryme.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://doz.ybcxt.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hjc.jiagoushi.top

Go:   arr := []int{1, 2, 3}
来源：http://chb.havefunace.top

Ruby: arr = [1, 2, 3]
来源：http://mqz.kuanghao11.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kra.nwbrower.top

[D02] 追加元素到末尾
来源：http://haz.zhixingplan.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://cgi.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cyl.ehwqpu.com

JS:   arr.push(4);
来源：http://fyq.sxryk.cn

TS:   arr.push(4);
来源：http://vej.shuidangran.top

Java: list.add(4);
来源：http://zei.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://pfh.yfazqb.com

Ruby: arr << 4; arr.push(5)
来源：http://eql.wangshuangyany.cn

C#:   list.Add(4);
来源：http://xlr.ybcxt.top

[D03] 在指定位置插入元素
来源：http://bta.fanxiaobao.xyz

Py:   arr.insert(0, 0)
来源：http://len.zhoulong.xyz

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ygx.xylfe.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mvh.quarkkingdee.top


<!-- 参考信息 -->