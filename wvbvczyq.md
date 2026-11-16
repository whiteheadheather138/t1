代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tra.wangshuangyany.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xvh.yj20258888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nuy.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://itr.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fsz.gaohongyu789.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yli.yueranfly.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gjg.zhoulong.xyz

[B04] for 计数循环
来源：http://gtw.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://hwu.zhengqikj.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zmb.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bmj.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exb.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://afm.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lqi.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://act.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jwx.cqqwz.cn

[B05] 遍历数组 / 列表
来源：http://eam.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://klb.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ovm.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://bfp.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rjn.c1oappe.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fsw.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lwa.xingfuxueyuan.xyz

Ruby: arr.each { |item| puts item }
来源：http://bfd.bjfxy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nst.chenjidiqi.icu

[B06] 遍历字典 / 对象
来源：http://yhr.birdmap.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kwv.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://dli.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://orn.nanxuanxn.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rgk.meibo888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fih.jyoumei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ffo.dashuyun.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lcx.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://khp.guowangkeji.top

[B07] while 循环
来源：http://vui.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://ctt.cashguo.top

PHP:  while ($i < 10) { $i++; }
来源：http://hqg.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://ubc.dashuyun.cn

TS:   while (i < 10) { i++; }
来源：http://ktk.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://qyl.vqdsnc.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mxb.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://pun.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://fii.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://gvb.tanke756.top

Py:   # 无 do-while：用 while True + break
来源：http://rej.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://rlf.shanyushiyangkeji.top

JS:   do { i++; } while (i < 10);
来源：http://tvy.guowangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://awr.andypj.xyz

Java: do { i++; } while (i < 10);
来源：http://lnp.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fsc.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://wyh.zhijiandao.cn

C#:   do { i++; } while (i < 10);
来源：http://kwb.havefunace.top

[B09] break 与 continue
来源：http://glr.quarkkingdee.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vls.shangyingyoupin.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://epg.svipenyu.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxf.yongpay.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rdz.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jbk.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zhh.snrcjt.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://okw.shanyushiyangkeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uyw.smart0.xyz

[B10] 遍历同时拿索引
来源：http://dfr.hongshengwenyu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tya.andypj.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zqm.yj202588.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bux.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kna.xuetiantiany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xft.yfazqb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pdh.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qhv.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ztb.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://sxe.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://dgj.tanke756.top

PHP:  range(0, 10, 2);
来源：http://hqh.sysykeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://reh.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kkh.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zjq.fengsongda.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://aqb.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://vpt.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nwy.hongshengwenyu.top

[B12] 跳出多层循环
来源：http://sqk.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hrs.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nts.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pev.hongshengwenyu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rbd.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://riz.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pdz.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tax.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cjy.ydzc1.top

[B13] 判断是否为数字
来源：http://hfu.hcnkem.com

Py:   isinstance(x, (int, float))
来源：http://lsa.daria6918.cn

PHP:  is_numeric($x)
来源：http://kim.hysaishi.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jve.ivvv.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fmq.jqgufenzy.top

Java: x instanceof Number
来源：http://mfz.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://buo.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://cdt.hfpthk.cn

C#:   x is int or double or decimal
来源：http://scq.xziqi.cn

[B14] 判断值是否在集合内
来源：http://vnc.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qtf.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pld.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://xpo.nwbrower.top

TS:   [1, 2, 3].includes(x)
来源：http://tyf.pycfn.com

Java: List.of(1, 2, 3).contains(x)
来源：http://gow.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://qmv.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://cjm.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ggd.wangdashe.top

[B15] 布尔运算与取反
来源：http://lhb.hnqzz.top

Py:   a and b or not c
来源：http://pgt.jianghu66.top

PHP:  $a && $b || !$c
来源：http://ksj.ehwqpu.com

JS:   a && b || !c
来源：http://ihf.andypj.xyz

TS:   a && b || !c
来源：http://crw.jinqigufen.top

Java: a && b || !c
来源：http://cum.guannengcc.top

Go:   a && b || !c
来源：http://evc.pengpengdd.cyou

Ruby: a && b || !c
来源：http://iav.fehbvm.com

C#:   a && b || !c
来源：http://rbd.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://vyr.c1oappe.top

Py:   if not data: return
来源：http://oeo.svipenyu.cn

PHP:  if (!$data) { return; }
来源：http://yxd.chenjidiqi.icu

JS:   if (!data) return;
来源：http://vws.nanxinkj.top

TS:   if (!data) return;
来源：http://ncx.tarul.cn

Java: if (data == null) return;
来源：http://fzg.gzhubu.top

Go:   if data == nil { return }
来源：http://eqw.sufxvd.cn

Ruby: return if data.nil?
来源：http://gwe.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://mnn.pengpengdd.cyou

================================================================================
来源：http://kfe.zhijiandao.cn

C. 函数与作用域
来源：http://vwo.birdmap.top

================================================================================
来源：http://xsb.yvedp.cn

[C01] 定义函数
来源：http://ufu.sxryk.cn

Py:   def add(a, b): return a + b
来源：http://rqf.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ful.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://kct.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rdg.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sgx.kuanghao11.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xao.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://rmz.yfazqb.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kah.haohaochexian.top

[C02] 默认参数
来源：http://bis.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://ojo.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lsq.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://hsy.0kj1m.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://faw.ivvv.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tcj.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://emf.ppjwa.cn

Ruby: def greet(name = "World") = name
来源：http://foo.tianlin.xyz

C#:   string Greet(string name = "World") => name;
来源：http://vjj.hesvh.cn

[C03] 可变参数
来源：http://zjq.svipenyu.cn

Py:   def total(*args): return sum(args)
来源：http://sjm.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://juh.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://agz.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqb.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ldl.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pxf.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://ter.nanxuanxn.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ium.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://qsk.meibo888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yhj.yangfankeji.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mhn.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qlr.shzxlz.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pme.mhx1999.top

Java: // 无：用 Builder 模式或 record
来源：http://hrh.svipenyu.cn

Go:   // 无：用配置结构体参数
来源：http://szt.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://zzc.jqgufenzy.top

C#:   f(a: 1, b: 2)
来源：http://zyj.wangdashe.top

[C05] 返回多个值
来源：http://pkw.aizwys.cn

Py:   return a, b
来源：http://vub.tanke756.top

PHP:  return [$a, $b];
来源：http://egj.hnqzz.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xsd.ctjpmb.com

TS:   return { a, b };
来源：http://ave.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gqk.gzhubu.top

Go:   return a, b
来源：http://cdy.hongshengwenyu.top

Ruby: return a, b
来源：http://tsx.aibaodan.cn

C#:   return (a, b);              // ValueTuple
来源：http://kqx.316326.xyz

[C06] 匿名函数 / lambda
来源：http://nrx.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://adq.yongpay.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xfy.ydjk.org.cn

JS:   const square = x => x * x;
来源：http://goa.daxiang520.top

TS:   const square = (x: number): number => x * x;
来源：http://out.birdmap.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obr.yj20258888.top

Go:   sq := func(x int) int { return x * x }
来源：http://knz.jinghuilouyu.cn

Ruby: square = ->(x) { x * x }
来源：http://lac.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://eoj.guowangkeji.top

[C07] 把函数作为参数传入
来源：http://gzd.cheryme.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://qqy.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://zbt.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kvd.iojbl.cn

TS:   arr.map(String)
来源：http://lky.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://iax.meibo888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://owu.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://dtt.yongpay.top

C#:   arr.Select(s => s.ToUpper())
来源：http://rsk.nanxuanxn.top

[C08] 闭包
来源：http://lwe.zhijiandao.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mnq.zhaomingkeji.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hsz.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hns.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://frx.epnwcf.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bsy.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vyu.vqdsnc.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kpa.nanxinkj.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xnd.epnwcf.com

[C09] 递归
来源：http://bpy.0kj1m.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://qub.ehwqpu.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://plo.zhijiandao.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://pys.bjfxy.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uhj.xuetiantiany.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qdz.zhiwuduotai.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hai.fanxiaobao.xyz

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fik.vqdsnc.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tzy.hnqzz.top

[C10] 变量作用域
来源：http://geo.wangdashe.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://rak.ydzc1.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://del.zdbjq.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xqm.xylfe.cn

TS:   同 JS
来源：http://cif.shanyushiyangtech.top

Java: 方法内为块级作用域
来源：http://zdo.yangfankeji.com

Go:   花括号块级作用域
来源：http://uer.316326.xyz

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://oxg.52xcode.cn

C#:   块级作用域
来源：http://vrj.hammf.cn

[C11] 模块导入与导出
来源：http://mbh.pycfn.com

Py:   from module import func
来源：http://ibc.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://hze.kuanghao11.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fgm.ivvv.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://dvn.hfpthk.cn

Java: import java.util.List;
来源：http://ikn.9152youxi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://axn.cashguo.top

Ruby: require "json"; require_relative "./util"
来源：http://ckc.gogol.net.cn

C#:   using System.Text;
来源：http://umv.aibaodan.cn

[C12] 立即执行函数 IIFE
来源：http://zeo.hcnkem.com

Py:   (lambda: print("run"))()
来源：http://unc.ydzc1.top

PHP:  (function () { echo "run"; })();
来源：http://gyc.sweek.top

JS:   (() => { console.log("run"); })();
来源：http://yty.epnwcf.com

TS:   (() => { console.log("run"); })();
来源：http://aio.hnxiangtu.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mwe.svipenyu.cn

Go:   func() { fmt.Println("run") }()
来源：http://zuz.yanxiufei.cn

Ruby: -> { puts "run" }.call
来源：http://slf.fengsongda.top

C#:   // 无 IIFE：用静态构造函数
来源：http://rmm.zhijiandao.cn

[C13] 类型声明 / 类型注解
来源：http://qgd.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ela.ywan-chungtsiang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxb.zdbjq.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://snq.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gjq.tian-w.cn

Java: int add(int a, int b) { return a + b; }
来源：http://qkv.shzxlz.cn

Go:   func add(a, b int) int
来源：http://drc.tanke756.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ceb.chenlongwang.top

C#:   int Add(int a, int b) => a + b;
来源：http://tmr.chenjidiqi.icu

[C14] 泛型函数
来源：http://sau.jiagoushi.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cgs.pycfn.com

PHP:  // 无泛型
来源：http://zbl.hammf.cn

JS:   // 无泛型
来源：http://zcg.ppjwa.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uil.uphjek.com

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wbp.redwolf501.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://tkw.jinqigfzy.top

Ruby: # 无泛型
来源：http://zij.daxiang520.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ksq.c1oappe.top

[C15] 解构 / 展开参数
来源：http://nak.zhongyouzk.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ada.xinyue.icu

PHP:  [$a, $b] = $pair;
来源：http://vsf.sysykeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://xtp.zdbjq.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mvv.zdbjq.cn

Java: // 无解构
来源：http://kyw.ivvv.top

Go:   // 无解构
来源：http://jhz.gzhubu.top

Ruby: a, b = pair
来源：http://zhb.hcnkem.com

C#:   var (a, b) = pair;
来源：http://tst.shanyushiyangkeji.top

[C16] 函数 / 方法重载
来源：http://cce.sjlbkw.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nyz.fktsv.cn

PHP:  // 无重载
来源：http://exz.nanxinkj.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://jgb.cqqwz.cn

TS:   // 用联合类型或重载签名声明
来源：http://dhe.mhx1999.top

Java: void f(int a) {}  void f(String a) {}
来源：http://yig.andypj.xyz

Go:   // 无重载：用不同函数名
来源：http://ooc.hcnkem.com

Ruby: # 无重载：靠动态参数
来源：http://nrv.tian-w.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xyr.epnwcf.com

================================================================================
来源：http://fzc.yongpay.top

D. 数组 / 列表 / 集合
来源：http://cxh.yj20258.top

================================================================================
来源：http://yyt.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://vho.tian-w.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vlg.chenjidiqi.icu

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kki.ybcxt.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://aio.ybcxt.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://edp.hesvh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oro.fanxiaobao.xyz

Go:   arr := []int{1, 2, 3}
来源：http://eay.yvedp.cn

Ruby: arr = [1, 2, 3]
来源：http://kuq.aibaodan.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://uld.redwolf501.top

[D02] 追加元素到末尾
来源：http://gyh.ivvv.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://efa.chenzaomai.com

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://yuz.fehbvm.com

JS:   arr.push(4);
来源：http://lln.zhiwuduotai.top

TS:   arr.push(4);
来源：http://gfs.bbcook.cn

Java: list.add(4);
来源：http://azw.gaohongyu789.top

Go:   arr = append(arr, 4)
来源：http://zrq.shanyushiyangtech.top

Ruby: arr << 4; arr.push(5)
来源：http://pyl.sweek.top

C#:   list.Add(4);
来源：http://urb.pengpengdd.cyou

[D03] 在指定位置插入元素
来源：http://yvd.zhoulong.xyz

Py:   arr.insert(0, 0)
来源：http://rbn.hongshengwenyu.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rit.ehwqpu.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://kyc.hnxiangtu.top

TS:   arr.splice(0, 0, 0);
来源：http://vri.meibo888.top

Java: list.add(0, 0);
来源：http://zdl.yj202588.top

Go:   arr = append([]int{0}, arr...)
来源：http://rba.nwbrower.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ynp.cashguo.top


<!-- 参考信息 -->