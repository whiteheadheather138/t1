代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gea.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fsu.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzu.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ang.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://apm.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tes.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ltc.zhixingplan.top

[B04] for 计数循环
来源：http://vgc.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://eub.yangfankeji.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://snc.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tvy.hfpthk.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ukz.svipenyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kya.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://psi.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://tie.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://syl.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://gnv.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://iex.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tkt.gaohongyu789.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nsc.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mkx.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iew.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dlc.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://uzz.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dfp.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://dfx.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uxd.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gik.sysykeji.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kbe.daxiang520.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://emn.zhaomingkeji.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hkl.daxiang520.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zru.shuidangran.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://asp.tian-w.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://akc.hnxiangtu.top

[B07] while 循环
来源：http://fsm.xingfuxueyuan.xyz

Py:   while i < 10: i += 1
来源：http://oey.yfazqb.com

PHP:  while ($i < 10) { $i++; }
来源：http://etb.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://aee.cqqwz.cn

TS:   while (i < 10) { i++; }
来源：http://bks.hnqzz.top

Java: while (i < 10) { i++; }
来源：http://mrt.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ucy.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://tam.jianghu66.top

C#:   while (i < 10) { i++; }
来源：http://xnp.hongshengwenyu.top

[B08] do-while（至少执行一次）
来源：http://xai.hysaishi.cn

Py:   # 无 do-while：用 while True + break
来源：http://xxa.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hgx.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://afy.smart0.xyz

TS:   do { i++; } while (i < 10);
来源：http://kvy.52xcode.cn

Java: do { i++; } while (i < 10);
来源：http://zqk.dianchejie.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ndf.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vpy.zhiwuduotai.top

C#:   do { i++; } while (i < 10);
来源：http://nod.hnxiangtu.top

[B09] break 与 continue
来源：http://ihj.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://spv.gotoacloud.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rvh.jiagoushi.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gfl.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rhg.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jzz.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uhv.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mmh.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zbl.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://nxp.gotoacloud.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://awr.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zyt.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tzu.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wno.quarkkingdee.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xhd.nanxuanxn.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mow.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://isg.cashguo.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sah.guannengcc.top

[B11] 生成数字序列 / 区间
来源：http://iwd.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://uni.zycfv.cn

PHP:  range(0, 10, 2);
来源：http://erm.dianchejie.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nzz.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://obz.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ipj.havefunace.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ojv.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://del.nwbrower.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kuk.xinyue.icu

[B12] 跳出多层循环
来源：http://qxx.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://usg.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://bty.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ymz.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://aso.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dxb.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fyq.xuanzx.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ssw.fktsv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vkx.wangdashe.top

[B13] 判断是否为数字
来源：http://jdu.uphjek.com

Py:   isinstance(x, (int, float))
来源：http://dxz.cdnleiting.top

PHP:  is_numeric($x)
来源：http://cez.chenlongwang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jck.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hlv.bjfxy.top

Java: x instanceof Number
来源：http://sws.ywan-chungtsiang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ijx.aizwys.cn

Ruby: x.is_a?(Numeric)
来源：http://wah.chenzaomai.com

C#:   x is int or double or decimal
来源：http://mui.havefunace.top

[B14] 判断值是否在集合内
来源：http://ylu.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cjj.zhixingplan.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://htz.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://pxp.fktsv.cn

TS:   [1, 2, 3].includes(x)
来源：http://jlv.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://bgo.sxryk.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qxw.tianlin.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://ekr.meibo888.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nip.guannengcc.top

[B15] 布尔运算与取反
来源：http://sqe.snrcjt.cn

Py:   a and b or not c
来源：http://veo.jlsjyb.cn

PHP:  $a && $b || !$c
来源：http://uwt.jinqigfzy.top

JS:   a && b || !c
来源：http://gzp.jiagoushi.top

TS:   a && b || !c
来源：http://llw.mhx1999.top

Java: a && b || !c
来源：http://cod.vqdsnc.cn

Go:   a && b || !c
来源：http://xwr.meibo888.top

Ruby: a && b || !c
来源：http://ojq.0kj1m.cn

C#:   a && b || !c
来源：http://bib.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://pid.snrcjt.cn

Py:   if not data: return
来源：http://waf.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://qma.vqdsnc.cn

JS:   if (!data) return;
来源：http://iwd.shzxlz.cn

TS:   if (!data) return;
来源：http://akw.zhiwuduotai.top

Java: if (data == null) return;
来源：http://rdl.9152youxi.cn

Go:   if data == nil { return }
来源：http://otq.hysaishi.cn

Ruby: return if data.nil?
来源：http://cya.zdbjq.cn

C#:   if (data == null) return;
来源：http://myg.hesvh.cn

================================================================================
来源：http://mgn.zhongyouzk.top

C. 函数与作用域
来源：http://okt.yuanzhike.top

================================================================================
来源：http://nhj.pengpengdd.cyou

[C01] 定义函数
来源：http://mdg.nanxuanxn.top

Py:   def add(a, b): return a + b
来源：http://ajw.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fif.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://hch.52xcode.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://txp.yangfankeji.com

Java: static int add(int a, int b) { return a + b; }
来源：http://cby.ehwqpu.com

Go:   func add(a, b int) int { return a + b }
来源：http://dpe.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://yhv.tarul.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://elr.zhiwuduotai.top

[C02] 默认参数
来源：http://akr.kuanghao11.cn

Py:   def greet(name="World"): return name
来源：http://ulk.ivvv.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xvl.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://tbz.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://xfa.c1oappe.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qhs.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kga.jinghuilouyu.cn

Ruby: def greet(name = "World") = name
来源：http://sqb.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://znw.jqgfzy.top

[C03] 可变参数
来源：http://ils.xuetiantiany.cn

Py:   def total(*args): return sum(args)
来源：http://aji.bbcook.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ykm.zhengqikj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aze.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gww.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nnp.yuxming.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yka.smart0.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://qgo.shzxlz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zmt.yongpay.top

[C04] 命名参数 / 关键字参数
来源：http://trq.gzhubu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xkm.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tuf.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tbu.hnqzz.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jwv.havefunace.top

Java: // 无：用 Builder 模式或 record
来源：http://gpv.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://hbx.nanxuanxn.top

Ruby: f(a: 1, b: 2)
来源：http://eaf.jlsjyb.cn

C#:   f(a: 1, b: 2)
来源：http://nec.dashuyun.cn

[C05] 返回多个值
来源：http://vlu.jinqigfzy.top

Py:   return a, b
来源：http://mmq.cashguo.top

PHP:  return [$a, $b];
来源：http://rup.xuetiantiany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yuy.shzxlz.cn

TS:   return { a, b };
来源：http://iar.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://btx.epnwcf.com

Go:   return a, b
来源：http://njg.yvedp.cn

Ruby: return a, b
来源：http://jms.fengsongda.top

C#:   return (a, b);              // ValueTuple
来源：http://jmr.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://oml.xziqi.cn

Py:   square = lambda x: x * x
来源：http://vmu.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://esp.jinqigfzy.top

JS:   const square = x => x * x;
来源：http://kan.shanyushiyangkeji.top

TS:   const square = (x: number): number => x * x;
来源：http://goc.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ikw.cdnleiting.top

Go:   sq := func(x int) int { return x * x }
来源：http://wng.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://gcj.xuanzx.com

C#:   Func<int, int> square = x => x * x;
来源：http://wcn.xuanzx.com

[C07] 把函数作为参数传入
来源：http://vjq.yonumen.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rpm.gzhubu.top

PHP:  array_map("strtoupper", $arr);
来源：http://asj.shangyingyoupin.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vkt.gotoacloud.top

TS:   arr.map(String)
来源：http://hop.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tmz.xingfuxueyuan.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vwi.cqqwz.cn

Ruby: arr.map(&:upcase)
来源：http://vjd.jianghu66.top

C#:   arr.Select(s => s.ToUpper())
来源：http://bkq.yonumen.top

[C08] 闭包
来源：http://kdd.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dhi.chenlongwang.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yea.zhaomingkeji.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://esh.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ttk.jinqigufen.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wqz.shanyushiyangkeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://sgz.birdmap.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rwz.jinghuilouyu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ovi.tarul.cn

[C09] 递归
来源：http://bvp.yonumen.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hwt.sxryk.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://eud.gaohongyu789.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lge.gotoacloud.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dcs.ivvv.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gnv.bbcook.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://noc.aizwys.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qin.gogol.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jfc.wangdashe.top

[C10] 变量作用域
来源：http://ulo.tarul.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://gdf.jqgfzy.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://zmh.meibo888.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://jyf.gogol.net.cn

TS:   同 JS
来源：http://ybn.hcnkem.com

Java: 方法内为块级作用域
来源：http://mhg.meibo888.top

Go:   花括号块级作用域
来源：http://bbi.chenjidiqi.icu

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ivn.ivvv.top

C#:   块级作用域
来源：http://nsh.jianghu66.top

[C11] 模块导入与导出
来源：http://kzg.hywenlv.cn

Py:   from module import func
来源：http://wpw.shzxlz.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://vba.zhiwuduotai.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rqn.ywan-chungtsiang.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vvw.yangfankeji.com

Java: import java.util.List;
来源：http://ijb.gotoacloud.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uvz.daxiang520.top

Ruby: require "json"; require_relative "./util"
来源：http://cxv.kuanghao11.cn

C#:   using System.Text;
来源：http://txg.hfpthk.cn

[C12] 立即执行函数 IIFE
来源：http://cmk.52xcode.cn

Py:   (lambda: print("run"))()
来源：http://jke.xuetiantiany.cn

PHP:  (function () { echo "run"; })();
来源：http://cmi.yj202588.top

JS:   (() => { console.log("run"); })();
来源：http://cwp.jinyuanbaomall.cn

TS:   (() => { console.log("run"); })();
来源：http://mku.hesvh.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uig.haohaochexian.top

Go:   func() { fmt.Println("run") }()
来源：http://szi.dianchejie.cn

Ruby: -> { puts "run" }.call
来源：http://xby.havefunace.top

C#:   // 无 IIFE：用静态构造函数
来源：http://fye.zhoulong.xyz

[C13] 类型声明 / 类型注解
来源：http://eic.guannengcc.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cyc.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dak.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yvi.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xaf.chenjidiqi.icu

Java: int add(int a, int b) { return a + b; }
来源：http://fsf.ywan-chungtsiang.top

Go:   func add(a, b int) int
来源：http://jwe.xuetiantiany.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ixg.shanyushiyangtech.top

C#:   int Add(int a, int b) => a + b;
来源：http://gfo.gzhubu.top

[C14] 泛型函数
来源：http://xcx.haohaochexian.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gyb.bjfxy.top

PHP:  // 无泛型
来源：http://zue.hongshengwenyu.top

JS:   // 无泛型
来源：http://ssu.hongshengwenyu.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://oim.kuanghao11.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ncf.zhijiandao.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xre.svipenyu.cn

Ruby: # 无泛型
来源：http://vyx.vqdsnc.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://smj.fzhhl.top

[C15] 解构 / 展开参数
来源：http://opi.yangfankeji.com

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://fni.sjlbkw.cn

PHP:  [$a, $b] = $pair;
来源：http://ecd.guannengcc.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qyf.zhengqikj.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://prq.nanxuanxn.top

Java: // 无解构
来源：http://qbd.yongpay.top

Go:   // 无解构
来源：http://dsu.zhengqikj.top

Ruby: a, b = pair
来源：http://nyf.sjlbkw.cn

C#:   var (a, b) = pair;
来源：http://tys.bjfxy.top

[C16] 函数 / 方法重载
来源：http://hgc.uphjek.com

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jsk.dianchejie.cn

PHP:  // 无重载
来源：http://ift.yonumen.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://dgs.zhoulong.xyz

TS:   // 用联合类型或重载签名声明
来源：http://eyz.xziqi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xbl.nwbrower.top

Go:   // 无重载：用不同函数名
来源：http://com.feifeiyinyue.top

Ruby: # 无重载：靠动态参数
来源：http://gbk.shanyushiyangtech.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://mrt.316326.xyz

================================================================================
来源：http://mpj.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://tja.xuetiantiany.cn

================================================================================
来源：http://iqi.tanke756.top

[D01] 创建数组 / 列表
来源：http://goo.cqqwz.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ehg.shanyushiyangtech.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tum.andypj.xyz

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lxv.yueranfly.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://snh.fehbvm.com

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ycc.yfazqb.com

Go:   arr := []int{1, 2, 3}
来源：http://vfh.xziqi.cn

Ruby: arr = [1, 2, 3]
来源：http://ole.hammf.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tpl.fanxiaobao.xyz

[D02] 追加元素到末尾
来源：http://fwz.sjlbkw.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jqi.shzxlz.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nwo.xylfe.cn

JS:   arr.push(4);
来源：http://lyq.uphjek.com

TS:   arr.push(4);
来源：http://baj.yuanzhike.top

Java: list.add(4);
来源：http://ifh.zhengqikj.top

Go:   arr = append(arr, 4)
来源：http://ghs.cheryme.top

Ruby: arr << 4; arr.push(5)
来源：http://guu.yangfankeji.com

C#:   list.Add(4);
来源：http://koz.shzxlz.cn

[D03] 在指定位置插入元素
来源：http://ozo.dianchejie.cn

Py:   arr.insert(0, 0)
来源：http://hgf.wangshuangyany.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mve.hongshengwenyu.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://icx.shangyingyoupin.top

TS:   arr.splice(0, 0, 0);
来源：http://sdl.tian-w.cn

Java: list.add(0, 0);
来源：http://ifc.ydjk.org.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zsd.hysaishi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aiv.0kj1m.cn


<!-- 参考信息 -->