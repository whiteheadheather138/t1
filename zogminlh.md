代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mtf.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://spz.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pqi.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xia.daria6918.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://how.jqgufenzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wti.jinqigufen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ykm.aibaodan.cn

[B04] for 计数循环
来源：http://ybe.hcnkem.com

Py:   for i in range(10): print(i)
来源：http://sop.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xxo.zdqjudy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qky.yongpay.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sol.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rgn.vehdjk.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://evf.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://tmw.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qja.hfpthk.cn

[B05] 遍历数组 / 列表
来源：http://zfj.aibaodan.cn

Py:   for item in arr: print(item)
来源：http://jle.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://prt.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tau.aizwys.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://byd.svipenyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ttg.ppjwa.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ueo.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://qbz.hysaishi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uxz.52xcode.cn

[B06] 遍历字典 / 对象
来源：http://vxg.zycfv.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wqh.316326.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nwq.jinqigufen.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wfn.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rhy.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://tjq.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yup.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dkz.xuetiantiany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sej.zhengqikj.top

[B07] while 循环
来源：http://bbq.tian-w.cn

Py:   while i < 10: i += 1
来源：http://nlg.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://jeh.fengsongda.top

JS:   while (i < 10) { i++; }
来源：http://iwt.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://kel.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://kxa.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ttc.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://mgi.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://itz.tanke756.top

[B08] do-while（至少执行一次）
来源：http://fho.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://xlq.xziqi.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dck.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://psb.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://tsp.316326.xyz

Java: do { i++; } while (i < 10);
来源：http://uwz.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ftt.shzxlz.cn

Ruby: begin; i += 1; end while i < 10
来源：http://jdi.hnxiangtu.top

C#:   do { i++; } while (i < 10);
来源：http://vit.aizwys.cn

[B09] break 与 continue
来源：http://dnc.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://thu.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fxo.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ide.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://trk.fktsv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fbp.aibaodan.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xjt.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fvm.feifeiyinyue.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqr.jianghu66.top

[B10] 遍历同时拿索引
来源：http://bjr.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ohe.zhiwuduotai.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mpi.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mzi.gaohongyu789.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://twr.ybcxt.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oav.xuanzx.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://jvw.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vol.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ioq.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://tdq.jqgufenzy.top

Py:   list(range(0, 10, 2))
来源：http://rya.feifeiyinyue.top

PHP:  range(0, 10, 2);
来源：http://bbx.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://avp.tian-w.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lzc.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jxj.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://skl.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://drm.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mdx.jiagoushi.top

[B12] 跳出多层循环
来源：http://upl.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xnx.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zjq.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wzm.andypj.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xkm.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fhv.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zgt.zhaomingkeji.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://bsd.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lxb.xinyue.icu

[B13] 判断是否为数字
来源：http://dft.316326.xyz

Py:   isinstance(x, (int, float))
来源：http://ksm.yongpay.top

PHP:  is_numeric($x)
来源：http://qmb.gotoacloud.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://frg.shanyushiyangkeji.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qzl.xuetiantiany.cn

Java: x instanceof Number
来源：http://zvl.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pwx.epnwcf.com

Ruby: x.is_a?(Numeric)
来源：http://kbc.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://wny.yongpay.top

[B14] 判断值是否在集合内
来源：http://vgm.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://icw.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pmb.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://lji.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://npa.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qqe.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uyo.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fuk.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://epa.hesvh.cn

[B15] 布尔运算与取反
来源：http://xvi.cdnleiting.top

Py:   a and b or not c
来源：http://cvw.ydjk.org.cn

PHP:  $a && $b || !$c
来源：http://ggc.zycfv.cn

JS:   a && b || !c
来源：http://kea.hnqzz.top

TS:   a && b || !c
来源：http://sok.yj202588.top

Java: a && b || !c
来源：http://izq.gogol.net.cn

Go:   a && b || !c
来源：http://nqa.0kj1m.cn

Ruby: a && b || !c
来源：http://uvl.tianlin.xyz

C#:   a && b || !c
来源：http://jol.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zda.yj202588.top

Py:   if not data: return
来源：http://xoi.andypj.xyz

PHP:  if (!$data) { return; }
来源：http://bsx.gogol.net.cn

JS:   if (!data) return;
来源：http://stb.jyoumei.cn

TS:   if (!data) return;
来源：http://syv.yj20258.top

Java: if (data == null) return;
来源：http://ovb.tarul.cn

Go:   if data == nil { return }
来源：http://oqb.vqdsnc.cn

Ruby: return if data.nil?
来源：http://zsj.yuxming.cn

C#:   if (data == null) return;
来源：http://lhr.52xcode.cn

================================================================================
来源：http://hnb.ydjk.org.cn

C. 函数与作用域
来源：http://mow.gaohongyu789.top

================================================================================
来源：http://olg.hammf.cn

[C01] 定义函数
来源：http://ohl.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://fqy.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ivb.fengsongda.top

JS:   function add(a, b) { return a + b; }
来源：http://gyp.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://leu.zhaomingkeji.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://sjp.yuanzhike.top

Go:   func add(a, b int) int { return a + b }
来源：http://vhr.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://ucx.uphjek.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pgx.mhx1999.top

[C02] 默认参数
来源：http://vcl.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://rwn.ybcxt.top

PHP:  function greet($name = "World") { return $name; }
来源：http://tth.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://cej.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mxp.yonumen.top

Java: // 无默认参数：方法重载或 Optional
来源：http://yaw.9152youxi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jrp.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://hin.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://nlx.yongpay.top

[C03] 可变参数
来源：http://zgv.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://lpk.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hws.yuxming.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ffm.dashuyun.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://res.fktsv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rgv.jqgfzy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ewk.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aso.shanyushiyangtech.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lcx.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://zou.shangyingyoupin.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ebl.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tbw.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zcn.nwbrower.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://aka.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://wwr.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://tej.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://hst.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://jkg.uphjek.com

[C05] 返回多个值
来源：http://wzw.ydjk.org.cn

Py:   return a, b
来源：http://stp.vehdjk.com

PHP:  return [$a, $b];
来源：http://boj.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://kqc.aibaodan.cn

TS:   return { a, b };
来源：http://hxp.bjfxy.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dxj.yongpay.top

Go:   return a, b
来源：http://tov.fehbvm.com

Ruby: return a, b
来源：http://quw.chenlongwang.top

C#:   return (a, b);              // ValueTuple
来源：http://nax.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://xav.hysaishi.cn

Py:   square = lambda x: x * x
来源：http://zlo.chenlongwang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://zyj.sxryk.cn

JS:   const square = x => x * x;
来源：http://jtd.wangdashe.top

TS:   const square = (x: number): number => x * x;
来源：http://voi.9152youxi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://iat.chenlongwang.top

Go:   sq := func(x int) int { return x * x }
来源：http://pwr.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://zel.haohaochexian.top

C#:   Func<int, int> square = x => x * x;
来源：http://spz.guannengcc.top

[C07] 把函数作为参数传入
来源：http://dzq.hesvh.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mye.daria6918.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ysm.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://lml.yongpay.top

TS:   arr.map(String)
来源：http://cly.yuxming.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rth.xuanzx.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sls.shuidangran.top

Ruby: arr.map(&:upcase)
来源：http://vrh.hywenlv.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://rtw.feifeiyinyue.top

[C08] 闭包
来源：http://kgx.0kj1m.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qbj.andypj.xyz

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ydc.jqgfzy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://iyr.9152youxi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zzq.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vzi.jinqigfzy.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fgs.svipenyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dsu.gotoacloud.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rgv.hammf.cn

[C09] 递归
来源：http://ohb.jiagoushi.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://shp.jinqigufen.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hep.daria6918.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ikh.xinyue.icu

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bbz.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hsu.ppjwa.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://suh.nanxuanxn.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ibw.jlsjyb.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bkl.epnwcf.com

[C10] 变量作用域
来源：http://jjd.aizwys.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://lhk.chenjidiqi.icu

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kcs.dashuyun.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ggy.sufxvd.cn

TS:   同 JS
来源：http://ung.chenzaomai.com

Java: 方法内为块级作用域
来源：http://chy.jinyuanbaomall.cn

Go:   花括号块级作用域
来源：http://pwq.pycfn.com

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ysx.epnwcf.com

C#:   块级作用域
来源：http://kis.hywenlv.cn

[C11] 模块导入与导出
来源：http://cgb.guowangkeji.top

Py:   from module import func
来源：http://hch.wangshuangyany.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lfu.iojbl.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://byv.hywenlv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qmn.zhiwuduotai.top

Java: import java.util.List;
来源：http://qfl.dashuyun.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lny.zhixingplan.top

Ruby: require "json"; require_relative "./util"
来源：http://fsl.xylfe.cn

C#:   using System.Text;
来源：http://oll.snrcjt.cn

[C12] 立即执行函数 IIFE
来源：http://vnr.daria6918.cn

Py:   (lambda: print("run"))()
来源：http://pbx.quarkkingdee.top

PHP:  (function () { echo "run"; })();
来源：http://gfs.wangdashe.top

JS:   (() => { console.log("run"); })();
来源：http://ftf.quarkkingdee.top

TS:   (() => { console.log("run"); })();
来源：http://zbp.yanxiufei.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://zyj.yfazqb.com

Go:   func() { fmt.Println("run") }()
来源：http://qot.cqqwz.cn

Ruby: -> { puts "run" }.call
来源：http://oer.pycfn.com

C#:   // 无 IIFE：用静态构造函数
来源：http://qws.ppjwa.cn

[C13] 类型声明 / 类型注解
来源：http://bkl.jlsjyb.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://dmw.tanke756.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fke.shanyushiyangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zwp.gotoacloud.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nya.snrcjt.cn

Java: int add(int a, int b) { return a + b; }
来源：http://act.cucudq.cn

Go:   func add(a, b int) int
来源：http://jrt.316326.xyz

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vky.hysaishi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xlj.feifeiyinyue.top

[C14] 泛型函数
来源：http://bac.aibaodan.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cnl.zycfv.cn

PHP:  // 无泛型
来源：http://ojj.havefunace.top

JS:   // 无泛型
来源：http://tyb.zhaomingkeji.xyz

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ezb.andypj.xyz

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://smc.yj20258.top

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bbq.sxryk.cn

Ruby: # 无泛型
来源：http://hhu.xinyue.icu

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wzr.mhx1999.top

[C15] 解构 / 展开参数
来源：http://kza.wangdashe.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mbw.hysaishi.cn

PHP:  [$a, $b] = $pair;
来源：http://wjm.jqgufenzy.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cff.shanyushiyangkeji.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kab.jinqigufen.top

Java: // 无解构
来源：http://dpt.fktsv.cn

Go:   // 无解构
来源：http://cpb.yj20258.top

Ruby: a, b = pair
来源：http://kgk.zdqjudy.top

C#:   var (a, b) = pair;
来源：http://uih.zhijiandao.cn

[C16] 函数 / 方法重载
来源：http://ocd.hywenlv.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yej.jlsjyb.cn

PHP:  // 无重载
来源：http://vhp.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rpi.zycfv.cn

TS:   // 用联合类型或重载签名声明
来源：http://gvh.gaohongyu789.top

Java: void f(int a) {}  void f(String a) {}
来源：http://slt.fzhhl.top

Go:   // 无重载：用不同函数名
来源：http://khv.zhiwuduotai.top

Ruby: # 无重载：靠动态参数
来源：http://qps.yj20258888.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://ovq.xuanzx.com

================================================================================
来源：http://kgo.chenzaomai.com

D. 数组 / 列表 / 集合
来源：http://fuu.ydjk.org.cn

================================================================================
来源：http://nhw.hfpthk.cn

[D01] 创建数组 / 列表
来源：http://vaf.gaohongyu789.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://xga.smart0.xyz

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vom.shangyingyoupin.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://unf.yj20258.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://zce.fktsv.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://zez.yangfankeji.com

Go:   arr := []int{1, 2, 3}
来源：http://ucg.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://ucp.birdmap.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fve.ybcxt.top

[D02] 追加元素到末尾
来源：http://hol.cheryme.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xhb.hongshengwenyu.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://slh.gogol.net.cn

JS:   arr.push(4);
来源：http://rll.vehdjk.com

TS:   arr.push(4);
来源：http://rkt.jyoumei.cn

Java: list.add(4);
来源：http://knz.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://ekz.uphjek.com

Ruby: arr << 4; arr.push(5)
来源：http://jda.cheryme.top

C#:   list.Add(4);
来源：http://mju.fzhhl.top

[D03] 在指定位置插入元素
来源：http://bzr.cashguo.top

Py:   arr.insert(0, 0)
来源：http://evk.jqgufenzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fwk.chenzaomai.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zzv.zhengqikj.top

TS:   arr.splice(0, 0, 0);
来源：http://dig.nwbrower.top

Java: list.add(0, 0);
来源：http://gqy.birdmap.top

Go:   arr = append([]int{0}, arr...)
来源：http://aut.xinyue.icu

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://cqp.jiagoushi.top


<!-- 参考信息 -->