代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ixg.bbcook.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bgx.dianchejie.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://isr.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rgr.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mzk.kuanghao11.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://utm.wangdashe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nov.daxiang520.top

[B04] for 计数循环
来源：http://fhq.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://apj.9152youxi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pqo.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kwk.dashuyun.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uns.pycfn.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mrz.yonumen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://duu.xinyue.icu

Ruby: 10.times { |i| puts i }
来源：http://zcr.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xvq.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://ebp.ctjpmb.com

Py:   for item in arr: print(item)
来源：http://mur.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://llm.shuidangran.top

JS:   for (const item of arr) { console.log(item); }
来源：http://dyq.ydzc1.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ekd.nanxuanxn.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://gin.shangyingyoupin.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wjy.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://dzb.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tcx.0kj1m.cn

[B06] 遍历字典 / 对象
来源：http://aqz.yfazqb.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nwk.quarkkingdee.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mwv.mhx1999.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sdz.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lxo.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbs.hesvh.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xdf.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wsg.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aik.yj20258.top

[B07] while 循环
来源：http://pnu.yongpay.top

Py:   while i < 10: i += 1
来源：http://ngd.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://yhe.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://ivw.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://laz.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://tfa.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wzr.chenzaomai.com

Ruby: while i < 10; i += 1; end
来源：http://mwu.kuanghao11.cn

C#:   while (i < 10) { i++; }
来源：http://xor.yj20258.top

[B08] do-while（至少执行一次）
来源：http://sfz.sufxvd.cn

Py:   # 无 do-while：用 while True + break
来源：http://ubt.birdmap.top

PHP:  do { $i++; } while ($i < 10);
来源：http://mbw.ehwqpu.com

JS:   do { i++; } while (i < 10);
来源：http://jil.tian-w.cn

TS:   do { i++; } while (i < 10);
来源：http://mug.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://aky.quarkkingdee.top

Go:   for { i++; if i >= 10 { break } }
来源：http://jub.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://kha.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://tjb.daria6918.cn

[B09] break 与 continue
来源：http://xzk.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cor.ydzc1.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ssb.hysaishi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lif.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dml.52xcode.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzb.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uco.jinghuilouyu.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gae.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ttd.shuidangran.top

[B10] 遍历同时拿索引
来源：http://gwj.tarul.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ffy.gogol.net.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zld.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lvn.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://icf.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://klr.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://auk.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pay.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hbl.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://igq.ctjpmb.com

Py:   list(range(0, 10, 2))
来源：http://fwb.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://piz.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://quh.9152youxi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tcb.yj20258888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nyc.9152youxi.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qdj.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://pys.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zrq.cheryme.top

[B12] 跳出多层循环
来源：http://rwp.hysaishi.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eii.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://krd.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xmq.kuanghao11.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lsg.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://llo.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://smp.zhixingplan.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rjj.bjfxy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fnn.birdmap.top

[B13] 判断是否为数字
来源：http://kfc.ydjk.org.cn

Py:   isinstance(x, (int, float))
来源：http://gqf.daria6918.cn

PHP:  is_numeric($x)
来源：http://qjw.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xde.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zuv.epnwcf.com

Java: x instanceof Number
来源：http://yhz.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fof.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://cid.bbcook.cn

C#:   x is int or double or decimal
来源：http://pxd.hcnkem.com

[B14] 判断值是否在集合内
来源：http://nmm.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://eky.wangshuangyany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tge.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://opg.hywenlv.cn

TS:   [1, 2, 3].includes(x)
来源：http://yax.guannengcc.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bbk.yj202588.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tcz.yueranfly.top

Ruby: [1, 2, 3].include?(x)
来源：http://gqe.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tiy.gogol.net.cn

[B15] 布尔运算与取反
来源：http://dqg.vqdsnc.cn

Py:   a and b or not c
来源：http://ovt.sxryk.cn

PHP:  $a && $b || !$c
来源：http://wpi.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://koa.ehwqpu.com

TS:   a && b || !c
来源：http://mqk.haohaochexian.top

Java: a && b || !c
来源：http://ofl.zdbjq.cn

Go:   a && b || !c
来源：http://qsf.cheryme.top

Ruby: a && b || !c
来源：http://fup.vehdjk.com

C#:   a && b || !c
来源：http://rdz.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://azn.0kj1m.cn

Py:   if not data: return
来源：http://kta.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://ctn.gotoacloud.top

JS:   if (!data) return;
来源：http://fnm.epnwcf.com

TS:   if (!data) return;
来源：http://lqn.shangyingyoupin.top

Java: if (data == null) return;
来源：http://zcd.yueranfly.top

Go:   if data == nil { return }
来源：http://ugx.yongpay.top

Ruby: return if data.nil?
来源：http://rvl.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://ydb.yj202588.top

================================================================================
来源：http://oex.shanyushiyangtech.top

C. 函数与作用域
来源：http://pat.zycfv.cn

================================================================================
来源：http://afp.guannengcc.top

[C01] 定义函数
来源：http://njp.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://nhq.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fsx.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://mqr.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://knq.jianghu66.top

Java: static int add(int a, int b) { return a + b; }
来源：http://not.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://pmu.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://swz.shanyushiyangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qfe.nwbrower.top

[C02] 默认参数
来源：http://vrz.shuidangran.top

Py:   def greet(name="World"): return name
来源：http://ctk.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yky.vqdsnc.cn

JS:   function greet(name = "World") { return name; }
来源：http://smz.jqgufenzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ruo.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gvv.jinqigfzy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bae.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://shr.vqdsnc.cn

C#:   string Greet(string name = "World") => name;
来源：http://aak.guowangkeji.top

[C03] 可变参数
来源：http://kuj.ppjwa.cn

Py:   def total(*args): return sum(args)
来源：http://uqn.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vbl.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jxh.guannengcc.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dxc.ehwqpu.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vld.guowangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hrf.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://exa.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yiy.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://nan.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://owy.cqqwz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tqd.yueranfly.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xso.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://geh.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://uvy.ppjwa.cn

Go:   // 无：用配置结构体参数
来源：http://fpo.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://nim.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://jio.jiagoushi.top

[C05] 返回多个值
来源：http://vjk.ydzc1.top

Py:   return a, b
来源：http://ukp.aizwys.cn

PHP:  return [$a, $b];
来源：http://evy.sufxvd.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zmq.yangfankeji.com

TS:   return { a, b };
来源：http://dpx.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qwk.xylfe.cn

Go:   return a, b
来源：http://fqv.hesvh.cn

Ruby: return a, b
来源：http://tvt.shangyingyoupin.top

C#:   return (a, b);              // ValueTuple
来源：http://qog.redwolf501.top

[C06] 匿名函数 / lambda
来源：http://hig.zhongyouzk.top

Py:   square = lambda x: x * x
来源：http://tnp.feifeiyinyue.top

PHP:  $square = fn($x) => $x * $x;
来源：http://sxd.gzhubu.top

JS:   const square = x => x * x;
来源：http://aks.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://vmp.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nal.daxiang520.top

Go:   sq := func(x int) int { return x * x }
来源：http://biz.fanxiaobao.xyz

Ruby: square = ->(x) { x * x }
来源：http://jlm.gogol.net.cn

C#:   Func<int, int> square = x => x * x;
来源：http://qwk.chenjidiqi.icu

[C07] 把函数作为参数传入
来源：http://uoi.yj20258.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ftq.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://vfr.daxiang520.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ots.snrcjt.cn

TS:   arr.map(String)
来源：http://jve.jinyuanbaomall.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ogy.yvedp.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://zrp.fktsv.cn

Ruby: arr.map(&:upcase)
来源：http://gql.xuetiantiany.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://qeo.yongpay.top

[C08] 闭包
来源：http://yfp.jianghu66.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ixl.cdnleiting.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ltq.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dtq.gaohongyu789.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ksk.aibaodan.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://anh.zhiwuduotai.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rcl.jyoumei.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mfw.ehwqpu.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cmh.yueranfly.top

[C09] 递归
来源：http://rup.zhaomingkeji.xyz

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dmy.dashuyun.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rvv.feifeiyinyue.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dut.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vqv.shanyushiyangkeji.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://nol.9152youxi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://xzk.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://bei.aizwys.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://fga.cucudq.cn

[C10] 变量作用域
来源：http://iow.zhixingplan.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vbn.tanke756.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rpm.epnwcf.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://nrb.yongpay.top

TS:   同 JS
来源：http://wel.tarul.cn

Java: 方法内为块级作用域
来源：http://ksm.hnxiangtu.top

Go:   花括号块级作用域
来源：http://dcp.shzxlz.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dke.jqgufenzy.top

C#:   块级作用域
来源：http://esm.zycfv.cn

[C11] 模块导入与导出
来源：http://daw.jqgufenzy.top

Py:   from module import func
来源：http://idw.yongpay.top

PHP:  require "file.php";  或 use App\Service;
来源：http://jpg.feifeiyinyue.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://ksf.zycfv.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mlx.bbcook.cn

Java: import java.util.List;
来源：http://xmp.zhixingplan.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ady.wangshuangyany.cn

Ruby: require "json"; require_relative "./util"
来源：http://tgd.quarkkingdee.top

C#:   using System.Text;
来源：http://dfk.shanyushiyangkeji.top

[C12] 立即执行函数 IIFE
来源：http://gks.snrcjt.cn

Py:   (lambda: print("run"))()
来源：http://lzn.zhoulong.xyz

PHP:  (function () { echo "run"; })();
来源：http://cqt.0kj1m.cn

JS:   (() => { console.log("run"); })();
来源：http://mic.ctjpmb.com

TS:   (() => { console.log("run"); })();
来源：http://ipr.sufxvd.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qpq.sweek.top

Go:   func() { fmt.Println("run") }()
来源：http://kyw.hfpthk.cn

Ruby: -> { puts "run" }.call
来源：http://ict.andypj.xyz

C#:   // 无 IIFE：用静态构造函数
来源：http://fyb.vqdsnc.cn

[C13] 类型声明 / 类型注解
来源：http://vsk.yangfankeji.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bwy.fanxiaobao.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xvz.pycfn.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://evf.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sqd.smart0.xyz

Java: int add(int a, int b) { return a + b; }
来源：http://ylm.andypj.xyz

Go:   func add(a, b int) int
来源：http://wmz.cdnleiting.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yry.shanyushiyangkeji.top

C#:   int Add(int a, int b) => a + b;
来源：http://atw.vehdjk.com

[C14] 泛型函数
来源：http://tni.meibo888.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ilp.pycfn.com

PHP:  // 无泛型
来源：http://hza.shuidangran.top

JS:   // 无泛型
来源：http://nra.nanxuanxn.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sht.haohaochexian.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eyk.chenzaomai.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://urc.ydjk.org.cn

Ruby: # 无泛型
来源：http://atj.tarul.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://dpj.daxiang520.top

[C15] 解构 / 展开参数
来源：http://dql.hammf.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lhm.c1oappe.top

PHP:  [$a, $b] = $pair;
来源：http://uok.cheryme.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hgs.smart0.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xxv.yanxiufei.cn

Java: // 无解构
来源：http://fol.jyoumei.cn

Go:   // 无解构
来源：http://lwo.jiagoushi.top

Ruby: a, b = pair
来源：http://ysq.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://ami.52xcode.cn

[C16] 函数 / 方法重载
来源：http://ggf.zhixingplan.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ymw.yuxming.cn

PHP:  // 无重载
来源：http://efk.epnwcf.com

JS:   // 无重载：靠 arguments.length 分支
来源：http://jhd.yuxming.cn

TS:   // 用联合类型或重载签名声明
来源：http://xbn.hysaishi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cqe.vehdjk.com

Go:   // 无重载：用不同函数名
来源：http://jcc.sufxvd.cn

Ruby: # 无重载：靠动态参数
来源：http://huu.zhongyouzk.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://lri.yfazqb.com

================================================================================
来源：http://vyy.xingfuxueyuan.xyz

D. 数组 / 列表 / 集合
来源：http://uti.gaohongyu789.top

================================================================================
来源：http://dzt.9152youxi.cn

[D01] 创建数组 / 列表
来源：http://xkx.shanyushiyangkeji.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://dcm.yanxiufei.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://drx.redwolf501.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://add.gaohongyu789.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://ygy.daria6918.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://qqc.sjlbkw.cn

Go:   arr := []int{1, 2, 3}
来源：http://sbq.yuxming.cn

Ruby: arr = [1, 2, 3]
来源：http://tez.yfazqb.com

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hhu.yueranfly.top

[D02] 追加元素到末尾
来源：http://nbg.xuanzx.com

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wde.hywenlv.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dhn.nanxinkj.top

JS:   arr.push(4);
来源：http://tdb.yfazqb.com

TS:   arr.push(4);
来源：http://sus.redwolf501.top

Java: list.add(4);
来源：http://adb.ybcxt.top

Go:   arr = append(arr, 4)
来源：http://xug.sjlbkw.cn

Ruby: arr << 4; arr.push(5)
来源：http://aam.shzxlz.cn

C#:   list.Add(4);
来源：http://kiv.gzhubu.top

[D03] 在指定位置插入元素
来源：http://pzf.epnwcf.com

Py:   arr.insert(0, 0)
来源：http://ajw.yfazqb.com

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ynn.havefunace.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zpz.kuanghao11.cn

TS:   arr.splice(0, 0, 0);
来源：http://edw.bbcook.cn

Java: list.add(0, 0);
来源：http://oeu.wangshuangyany.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vmu.52xcode.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://flv.guowangkeji.top


<!-- 参考信息 -->