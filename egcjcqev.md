代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ydt.jlsjyb.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ptx.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sgh.fanxiaobao.xyz

[B04] for 计数循环
来源：http://sul.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://fbi.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eif.jinqigufen.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dwh.zhongyouzk.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cph.zdqjudy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ezl.zhengqikj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qys.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://eyg.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rvm.316326.xyz

[B05] 遍历数组 / 列表
来源：http://fyz.zdqjudy.top

Py:   for item in arr: print(item)
来源：http://dwy.xuanzx.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://msl.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://inr.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ngj.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cib.epnwcf.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://prs.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://xpa.yvedp.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uud.kuanghao11.cn

[B06] 遍历字典 / 对象
来源：http://oqa.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ofl.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jvv.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dqv.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://grl.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://byi.smart0.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tss.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lhk.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eqb.yfazqb.com

[B07] while 循环
来源：http://jqi.shanyushiyangkeji.top

Py:   while i < 10: i += 1
来源：http://vps.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gug.cashguo.top

JS:   while (i < 10) { i++; }
来源：http://vpa.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://tgc.yj20258.top

Java: while (i < 10) { i++; }
来源：http://bla.chenlongwang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tad.shzxlz.cn

Ruby: while i < 10; i += 1; end
来源：http://fol.pengpengdd.cyou

C#:   while (i < 10) { i++; }
来源：http://uwv.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://xkp.aibaodan.cn

Py:   # 无 do-while：用 while True + break
来源：http://ngy.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wqp.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://nrw.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://rwj.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://mno.gogol.net.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wex.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://pnt.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://oyn.0kj1m.cn

[B09] break 与 continue
来源：http://pcj.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cxs.meibo888.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://isl.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozo.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://inh.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://usb.hysaishi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://phj.xingfuxueyuan.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ssd.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ldz.cdnleiting.top

[B10] 遍历同时拿索引
来源：http://qmu.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgg.gzhubu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eoj.haohaochexian.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jcg.yj20258888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://squ.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://egh.ppjwa.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://kxn.sjlbkw.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://btu.ydjk.org.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xtb.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://dft.redwolf501.top

Py:   list(range(0, 10, 2))
来源：http://nsv.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://sog.smart0.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bul.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yyv.ppjwa.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uaf.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nus.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://xeb.vehdjk.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lpt.shuidangran.top

[B12] 跳出多层循环
来源：http://syn.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://laz.hysaishi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tub.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oul.xinyue.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lcp.wangshuangyany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cla.shangyingyoupin.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ydn.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wmc.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axp.vehdjk.com

[B13] 判断是否为数字
来源：http://kcz.zhoulong.xyz

Py:   isinstance(x, (int, float))
来源：http://rip.zycfv.cn

PHP:  is_numeric($x)
来源：http://hqm.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dmm.ybcxt.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yje.uphjek.com

Java: x instanceof Number
来源：http://mef.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dtt.fehbvm.com

Ruby: x.is_a?(Numeric)
来源：http://dkh.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://llw.cheryme.top

[B14] 判断值是否在集合内
来源：http://oyl.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vam.smart0.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hgc.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://rom.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://iup.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ggm.ppjwa.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blw.yj202588.top

Ruby: [1, 2, 3].include?(x)
来源：http://dcc.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jbu.nwbrower.top

[B15] 布尔运算与取反
来源：http://ujl.hesvh.cn

Py:   a and b or not c
来源：http://pzy.cdnleiting.top

PHP:  $a && $b || !$c
来源：http://koy.chenlongwang.top

JS:   a && b || !c
来源：http://wjh.ydzc1.top

TS:   a && b || !c
来源：http://osf.shzxlz.cn

Java: a && b || !c
来源：http://gvj.bbcook.cn

Go:   a && b || !c
来源：http://teg.tian-w.cn

Ruby: a && b || !c
来源：http://iij.jqgfzy.top

C#:   a && b || !c
来源：http://ukr.hnqzz.top

[B16] 卫语句：不满足条件提前返回
来源：http://slg.hnqzz.top

Py:   if not data: return
来源：http://ddg.xingfuxueyuan.xyz

PHP:  if (!$data) { return; }
来源：http://joi.havefunace.top

JS:   if (!data) return;
来源：http://khm.feifeiyinyue.top

TS:   if (!data) return;
来源：http://yis.316326.xyz

Java: if (data == null) return;
来源：http://bsd.tianlin.xyz

Go:   if data == nil { return }
来源：http://rea.nanxinkj.top

Ruby: return if data.nil?
来源：http://dzv.uphjek.com

C#:   if (data == null) return;
来源：http://gly.tarul.cn

================================================================================
来源：http://orn.gogol.net.cn

C. 函数与作用域
来源：http://mtl.yvedp.cn

================================================================================
来源：http://akn.xuanzx.com

[C01] 定义函数
来源：http://npf.meibo888.top

Py:   def add(a, b): return a + b
来源：http://qsa.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ikx.yj20258888.top

JS:   function add(a, b) { return a + b; }
来源：http://ume.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wgd.havefunace.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pvf.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://erm.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://rny.zhongyouzk.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fuf.andypj.xyz

[C02] 默认参数
来源：http://wvz.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://haz.uphjek.com

PHP:  function greet($name = "World") { return $name; }
来源：http://uuz.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://fqq.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zxq.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rlf.zdbjq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xqx.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://box.xylfe.cn

C#:   string Greet(string name = "World") => name;
来源：http://ppm.fzhhl.top

[C03] 可变参数
来源：http://csm.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://gcx.bjfxy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fnj.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lfq.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dmx.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nxl.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ygo.daria6918.cn

Ruby: def total(*nums); nums.sum; end
来源：http://tja.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://avx.52xcode.cn

[C04] 命名参数 / 关键字参数
来源：http://lqg.jqgufenzy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kof.uphjek.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://esf.mhx1999.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mwi.wangshuangyany.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pti.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://lna.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://mgd.cheryme.top

Ruby: f(a: 1, b: 2)
来源：http://wbm.chenjidiqi.icu

C#:   f(a: 1, b: 2)
来源：http://jye.jiagoushi.top

[C05] 返回多个值
来源：http://opv.meibo888.top

Py:   return a, b
来源：http://aaz.jianghu66.top

PHP:  return [$a, $b];
来源：http://alr.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://frl.sysykeji.top

TS:   return { a, b };
来源：http://fzf.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cgg.daxiang520.top

Go:   return a, b
来源：http://aet.gaohongyu789.top

Ruby: return a, b
来源：http://iio.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://lab.hcnkem.com

[C06] 匿名函数 / lambda
来源：http://ojk.wangdashe.top

Py:   square = lambda x: x * x
来源：http://iui.316326.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://qrl.hammf.cn

JS:   const square = x => x * x;
来源：http://oif.shangyingyoupin.top

TS:   const square = (x: number): number => x * x;
来源：http://elj.dashuyun.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ftz.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://wuy.havefunace.top

Ruby: square = ->(x) { x * x }
来源：http://hvv.jiagoushi.top

C#:   Func<int, int> square = x => x * x;
来源：http://iiy.jiagoushi.top

[C07] 把函数作为参数传入
来源：http://tod.zhiwuduotai.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ndy.xuetiantiany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mbq.xziqi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mzm.jlsjyb.cn

TS:   arr.map(String)
来源：http://qtr.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uwe.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vpf.smart0.xyz

Ruby: arr.map(&:upcase)
来源：http://kky.52xcode.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pea.vehdjk.com

[C08] 闭包
来源：http://fyk.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ijl.feifeiyinyue.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://kgk.yonumen.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jsl.yfazqb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://acq.jyoumei.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tpy.havefunace.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zos.hammf.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cjn.zdbjq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pte.jiagoushi.top

[C09] 递归
来源：http://dch.aibaodan.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ddv.sysykeji.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kej.ctjpmb.com

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qvb.zycfv.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://uqg.daria6918.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qdu.gotoacloud.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jss.cdnleiting.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://kqr.tian-w.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hkz.yuxming.cn

[C10] 变量作用域
来源：http://wrm.haohaochexian.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hmy.guannengcc.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xps.quarkkingdee.top

JS:   let/const 块级作用域，var 函数级作用域
来源：http://joe.aibaodan.cn

TS:   同 JS
来源：http://mry.jqgufenzy.top

Java: 方法内为块级作用域
来源：http://xut.c1oappe.top

Go:   花括号块级作用域
来源：http://beo.yongpay.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://dte.sufxvd.cn

C#:   块级作用域
来源：http://qay.9152youxi.cn

[C11] 模块导入与导出
来源：http://pcw.tian-w.cn

Py:   from module import func
来源：http://bqf.xuanzx.com

PHP:  require "file.php";  或 use App\Service;
来源：http://ett.sufxvd.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fpw.guowangkeji.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ajw.shzxlz.cn

Java: import java.util.List;
来源：http://lzb.ydjk.org.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://fpy.ivvv.top

Ruby: require "json"; require_relative "./util"
来源：http://yck.guowangkeji.top

C#:   using System.Text;
来源：http://xmi.hnxiangtu.top

[C12] 立即执行函数 IIFE
来源：http://cbh.shuidangran.top

Py:   (lambda: print("run"))()
来源：http://wjb.shuidangran.top

PHP:  (function () { echo "run"; })();
来源：http://lvr.vehdjk.com

JS:   (() => { console.log("run"); })();
来源：http://ggy.chenzaomai.com

TS:   (() => { console.log("run"); })();
来源：http://dbm.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://dwe.hesvh.cn

Go:   func() { fmt.Println("run") }()
来源：http://xry.shanyushiyangtech.top

Ruby: -> { puts "run" }.call
来源：http://xqv.xziqi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qed.jinghuilouyu.cn

[C13] 类型声明 / 类型注解
来源：http://yqg.hesvh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://evj.xziqi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wtz.yonumen.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://yae.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pud.zhixingplan.top

Java: int add(int a, int b) { return a + b; }
来源：http://fjb.meibo888.top

Go:   func add(a, b int) int
来源：http://onw.zycfv.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ufd.svipenyu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://dgb.redwolf501.top

[C14] 泛型函数
来源：http://mzr.jyoumei.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://thq.fanxiaobao.xyz

PHP:  // 无泛型
来源：http://udc.fzhhl.top

JS:   // 无泛型
来源：http://hrq.ehwqpu.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zzy.wangshuangyany.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cux.epnwcf.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gxc.vehdjk.com

Ruby: # 无泛型
来源：http://klf.hcnkem.com

C#:   static T First<T>(List<T> items) => items[0];
来源：http://krm.shanyushiyangkeji.top

[C15] 解构 / 展开参数
来源：http://udx.gotoacloud.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mrq.jqgfzy.top

PHP:  [$a, $b] = $pair;
来源：http://yba.yj20258888.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vya.hesvh.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://gti.xylfe.cn

Java: // 无解构
来源：http://mwk.snrcjt.cn

Go:   // 无解构
来源：http://epp.hysaishi.cn

Ruby: a, b = pair
来源：http://csi.yfazqb.com

C#:   var (a, b) = pair;
来源：http://kwo.gotoacloud.top

[C16] 函数 / 方法重载
来源：http://hhw.nanxinkj.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ifq.bjfxy.top

PHP:  // 无重载
来源：http://rhx.aizwys.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rsh.smart0.xyz

TS:   // 用联合类型或重载签名声明
来源：http://wsr.jinyuanbaomall.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wgm.tian-w.cn

Go:   // 无重载：用不同函数名
来源：http://mgd.cheryme.top

Ruby: # 无重载：靠动态参数
来源：http://jpe.guannengcc.top

C#:   void F(int a) {}  void F(string a) {}
来源：http://gnv.52xcode.cn

================================================================================
来源：http://wfo.dianchejie.cn

D. 数组 / 列表 / 集合
来源：http://gvd.snrcjt.cn

================================================================================
来源：http://yrv.0kj1m.cn

[D01] 创建数组 / 列表
来源：http://njp.pengpengdd.cyou

Py:   arr = [1, 2, 3];  empty = []
来源：http://oxl.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kwd.pengpengdd.cyou

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ncm.yfazqb.com

TS:   const arr: number[] = [1, 2, 3];
来源：http://shf.jianghu66.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ypf.zdqjudy.top

Go:   arr := []int{1, 2, 3}
来源：http://vov.sxryk.cn

Ruby: arr = [1, 2, 3]
来源：http://fcs.xylfe.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wgz.meibo888.top

[D02] 追加元素到末尾
来源：http://tdx.yuxming.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nnf.zhijiandao.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zox.iojbl.cn

JS:   arr.push(4);
来源：http://xzd.zhongyouzk.top

TS:   arr.push(4);
来源：http://wps.meibo888.top

Java: list.add(4);
来源：http://lnx.fengsongda.top

Go:   arr = append(arr, 4)
来源：http://vns.jinqigufen.top

Ruby: arr << 4; arr.push(5)
来源：http://vjs.0kj1m.cn

C#:   list.Add(4);
来源：http://gxr.hywenlv.cn

[D03] 在指定位置插入元素
来源：http://nod.haohaochexian.top

Py:   arr.insert(0, 0)
来源：http://nrt.shangyingyoupin.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ikm.tianlin.xyz

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://izk.hcnkem.com

TS:   arr.splice(0, 0, 0);
来源：http://ccl.yongpay.top

Java: list.add(0, 0);
来源：http://hmr.shzxlz.cn

Go:   arr = append([]int{0}, arr...)
来源：http://mey.cheryme.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://drj.jlsjyb.cn

C#:   list.Insert(0, 0);
来源：http://bgy.meibo888.top

[D04] 删除元素
来源：http://sqx.zhijiandao.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hot.jinghuilouyu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xsv.9152youxi.cn


<!-- 参考信息 -->