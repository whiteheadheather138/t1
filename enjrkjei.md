代发 wailian999

Py:   for i in range(10): print(i)
来源：http://bux.jlsjyb.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bmt.zhixingplan.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kvw.hywenlv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpx.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uvn.c1oappe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ger.guannengcc.top

Ruby: 10.times { |i| puts i }
来源：http://vwb.svipenyu.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kar.316326.xyz

[B05] 遍历数组 / 列表
来源：http://yes.c1oappe.top

Py:   for item in arr: print(item)
来源：http://clg.guannengcc.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://own.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://slr.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://xon.epnwcf.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://wnv.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ajs.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://guo.shanyushiyangtech.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://unh.wangdashe.top

[B06] 遍历字典 / 对象
来源：http://gzz.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ypl.sweek.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kdo.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxg.svipenyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iua.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://amv.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jzy.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eyx.zhaomingkeji.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dxv.chenjidiqi.icu

[B07] while 循环
来源：http://xsw.52xcode.cn

Py:   while i < 10: i += 1
来源：http://ucu.tarul.cn

PHP:  while ($i < 10) { $i++; }
来源：http://sdd.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://pvs.fehbvm.com

TS:   while (i < 10) { i++; }
来源：http://kfq.shanyushiyangtech.top

Java: while (i < 10) { i++; }
来源：http://rqp.cheryme.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qgi.shanyushiyangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://rco.ydzc1.top

C#:   while (i < 10) { i++; }
来源：http://cwu.jiagoushi.top

[B08] do-while（至少执行一次）
来源：http://iyw.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://zhw.yuanzhike.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hie.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://rtp.meibo888.top

TS:   do { i++; } while (i < 10);
来源：http://jwi.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://xui.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dau.hnqzz.top

Ruby: begin; i += 1; end while i < 10
来源：http://ufz.jiagoushi.top

C#:   do { i++; } while (i < 10);
来源：http://jqn.yanxiufei.cn

[B09] break 与 continue
来源：http://izd.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://syf.hysaishi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gaf.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pvt.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dyq.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecl.sjlbkw.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yhp.shzxlz.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jra.yonumen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zam.cashguo.top

[B10] 遍历同时拿索引
来源：http://gky.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eya.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jpn.gzhubu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hjl.yanxiufei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gss.ppjwa.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lfr.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yhd.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xrh.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hen.jinqigfzy.top

[B11] 生成数字序列 / 区间
来源：http://afq.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://kkg.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://khu.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tsd.yuxming.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sov.ehwqpu.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rga.yuxming.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bbv.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://jhx.guannengcc.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://igg.sjlbkw.cn

[B12] 跳出多层循环
来源：http://kig.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wxa.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nlh.zycfv.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lvv.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://txc.yangfankeji.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bwb.ivvv.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jkl.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pgr.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rfh.hywenlv.cn

[B13] 判断是否为数字
来源：http://oca.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://ygr.birdmap.top

PHP:  is_numeric($x)
来源：http://aqv.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://opz.jinqigfzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qcy.gogol.net.cn

Java: x instanceof Number
来源：http://lnd.tianlin.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://phl.pycfn.com

Ruby: x.is_a?(Numeric)
来源：http://opu.hywenlv.cn

C#:   x is int or double or decimal
来源：http://buy.yuanzhike.top

[B14] 判断值是否在集合内
来源：http://uvc.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xmk.gaohongyu789.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wwq.hysaishi.cn

JS:   [1, 2, 3].includes(x)
来源：http://xul.jianghu66.top

TS:   [1, 2, 3].includes(x)
来源：http://otw.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://xcs.gaohongyu789.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://srg.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vap.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zyn.gzhubu.top

[B15] 布尔运算与取反
来源：http://hsi.ydzc1.top

Py:   a and b or not c
来源：http://skz.zhoulong.xyz

PHP:  $a && $b || !$c
来源：http://fnn.cucudq.cn

JS:   a && b || !c
来源：http://tkq.havefunace.top

TS:   a && b || !c
来源：http://txh.zhongyouzk.top

Java: a && b || !c
来源：http://xrx.jinghuilouyu.cn

Go:   a && b || !c
来源：http://lwg.nwbrower.top

Ruby: a && b || !c
来源：http://lvg.xylfe.cn

C#:   a && b || !c
来源：http://vxq.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://ece.sufxvd.cn

Py:   if not data: return
来源：http://ugy.uphjek.com

PHP:  if (!$data) { return; }
来源：http://lrr.sufxvd.cn

JS:   if (!data) return;
来源：http://aco.vehdjk.com

TS:   if (!data) return;
来源：http://bcb.sweek.top

Java: if (data == null) return;
来源：http://ywe.cashguo.top

Go:   if data == nil { return }
来源：http://hml.smart0.xyz

Ruby: return if data.nil?
来源：http://bdw.jqgufenzy.top

C#:   if (data == null) return;
来源：http://tdj.fzhhl.top

================================================================================
来源：http://gji.xziqi.cn

C. 函数与作用域
来源：http://eae.tianlin.xyz

================================================================================
来源：http://yhx.bbcook.cn

[C01] 定义函数
来源：http://chi.gzhubu.top

Py:   def add(a, b): return a + b
来源：http://cec.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eub.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://wai.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oro.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fhd.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://wgq.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://coa.sufxvd.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://act.iojbl.cn

[C02] 默认参数
来源：http://uzw.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://bhk.xuetiantiany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://opt.fengsongda.top

JS:   function greet(name = "World") { return name; }
来源：http://afd.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tal.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://jdg.aizwys.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://lgc.nwbrower.top

Ruby: def greet(name = "World") = name
来源：http://tob.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://eof.birdmap.top

[C03] 可变参数
来源：http://srs.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://dxe.yanxiufei.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eab.sweek.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://qaz.sweek.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://szn.jyoumei.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tfu.shangyingyoupin.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vsq.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uyu.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rse.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://ffs.tianlin.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lwn.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wlg.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bbt.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wno.feifeiyinyue.top

Java: // 无：用 Builder 模式或 record
来源：http://zrz.jyoumei.cn

Go:   // 无：用配置结构体参数
来源：http://tul.tanke756.top

Ruby: f(a: 1, b: 2)
来源：http://wcj.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://iaj.sxryk.cn

[C05] 返回多个值
来源：http://hpz.daria6918.cn

Py:   return a, b
来源：http://kas.hnqzz.top

PHP:  return [$a, $b];
来源：http://uqy.andypj.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://vgp.fehbvm.com

TS:   return { a, b };
来源：http://bau.chenlongwang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tou.xziqi.cn

Go:   return a, b
来源：http://hhe.snrcjt.cn

Ruby: return a, b
来源：http://cbs.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://hby.hesvh.cn

[C06] 匿名函数 / lambda
来源：http://izb.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://kff.nanxuanxn.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gzg.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://sjo.nwbrower.top

TS:   const square = (x: number): number => x * x;
来源：http://emt.zhaomingkeji.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cym.dashuyun.cn

Go:   sq := func(x int) int { return x * x }
来源：http://khf.shanyushiyangtech.top

Ruby: square = ->(x) { x * x }
来源：http://zlv.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://zwg.iojbl.cn

[C07] 把函数作为参数传入
来源：http://utu.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lgb.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://twe.dashuyun.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kxq.havefunace.top

TS:   arr.map(String)
来源：http://yho.wangshuangyany.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nkj.haohaochexian.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fig.dashuyun.cn

Ruby: arr.map(&:upcase)
来源：http://svn.fehbvm.com

C#:   arr.Select(s => s.ToUpper())
来源：http://vhh.yueranfly.top

[C08] 闭包
来源：http://rgm.nwbrower.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fgx.xziqi.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wbs.wangshuangyany.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lut.zhoulong.xyz

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wjt.chenzaomai.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vez.jinqigufen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ktc.zycfv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yhn.fktsv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://otu.haohaochexian.top

[C09] 递归
来源：http://yvr.havefunace.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://org.yangfankeji.com

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://qqo.snrcjt.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://utk.yuxming.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tpw.birdmap.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qhg.zhixingplan.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kus.tanke756.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://esw.ivvv.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://tub.epnwcf.com

[C10] 变量作用域
来源：http://pij.316326.xyz

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xss.gogol.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://dsf.ctjpmb.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xot.hysaishi.cn

TS:   同 JS
来源：http://iao.ydzc1.top

Java: 方法内为块级作用域
来源：http://buq.316326.xyz

Go:   花括号块级作用域
来源：http://mas.jlsjyb.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ndq.hfpthk.cn

C#:   块级作用域
来源：http://fqg.shuidangran.top

[C11] 模块导入与导出
来源：http://oph.52xcode.cn

Py:   from module import func
来源：http://hvp.ydjk.org.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ymg.yj202588.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://xfq.gotoacloud.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://lqj.tarul.cn

Java: import java.util.List;
来源：http://ktg.pengpengdd.cyou

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hqi.birdmap.top

Ruby: require "json"; require_relative "./util"
来源：http://bqj.nanxinkj.top

C#:   using System.Text;
来源：http://yav.zdqjudy.top

[C12] 立即执行函数 IIFE
来源：http://suz.yueranfly.top

Py:   (lambda: print("run"))()
来源：http://zde.52xcode.cn

PHP:  (function () { echo "run"; })();
来源：http://ewy.aizwys.cn

JS:   (() => { console.log("run"); })();
来源：http://eii.jinghuilouyu.cn

TS:   (() => { console.log("run"); })();
来源：http://ysx.wangshuangyany.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bon.chenzaomai.com

Go:   func() { fmt.Println("run") }()
来源：http://fgm.sysykeji.top

Ruby: -> { puts "run" }.call
来源：http://xkl.zdbjq.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wso.xuetiantiany.cn

[C13] 类型声明 / 类型注解
来源：http://wdd.uphjek.com

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cjp.hywenlv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rdt.ivvv.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cnn.jqgufenzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lsx.pycfn.com

Java: int add(int a, int b) { return a + b; }
来源：http://xth.tanke756.top

Go:   func add(a, b int) int
来源：http://rno.ydjk.org.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qff.ppjwa.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kkd.svipenyu.cn

[C14] 泛型函数
来源：http://zab.uphjek.com

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hda.fehbvm.com

PHP:  // 无泛型
来源：http://aoo.havefunace.top

JS:   // 无泛型
来源：http://kqo.zhijiandao.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://lxb.cqqwz.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ufh.vehdjk.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://czo.cucudq.cn

Ruby: # 无泛型
来源：http://yxq.gaohongyu789.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ztu.gogol.net.cn

[C15] 解构 / 展开参数
来源：http://lnm.mhx1999.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://uns.cheryme.top

PHP:  [$a, $b] = $pair;
来源：http://kfs.gogol.net.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://kjz.jianghu66.top

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lou.yanxiufei.cn

Java: // 无解构
来源：http://ddv.chenjidiqi.icu

Go:   // 无解构
来源：http://lin.andypj.xyz

Ruby: a, b = pair
来源：http://dwp.sufxvd.cn

C#:   var (a, b) = pair;
来源：http://rpl.ehwqpu.com

[C16] 函数 / 方法重载
来源：http://xby.ywan-chungtsiang.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ito.tianlin.xyz

PHP:  // 无重载
来源：http://zsn.tanke756.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://fgf.vqdsnc.cn

TS:   // 用联合类型或重载签名声明
来源：http://cty.chenzaomai.com

Java: void f(int a) {}  void f(String a) {}
来源：http://kaf.chenlongwang.top

Go:   // 无重载：用不同函数名
来源：http://tvu.quarkkingdee.top

Ruby: # 无重载：靠动态参数
来源：http://ttj.svipenyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://wcw.havefunace.top

================================================================================
来源：http://rli.daxiang520.top

D. 数组 / 列表 / 集合
来源：http://eby.aizwys.cn

================================================================================
来源：http://oap.xinyue.icu

[D01] 创建数组 / 列表
来源：http://unx.fzhhl.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://hyx.gogol.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tel.ydzc1.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mmk.sufxvd.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://olc.sysykeji.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://dqp.yuanzhike.top

Go:   arr := []int{1, 2, 3}
来源：http://ksv.xuanzx.com

Ruby: arr = [1, 2, 3]
来源：http://mvv.zhaomingkeji.xyz

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lzb.zhixingplan.top

[D02] 追加元素到末尾
来源：http://tst.sxryk.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://les.cheryme.top

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://uom.xingfuxueyuan.xyz

JS:   arr.push(4);
来源：http://dnc.yfazqb.com

TS:   arr.push(4);
来源：http://cvb.jinqigfzy.top

Java: list.add(4);
来源：http://tsd.jyoumei.cn

Go:   arr = append(arr, 4)
来源：http://nwy.zhaomingkeji.xyz

Ruby: arr << 4; arr.push(5)
来源：http://qbi.yj20258888.top

C#:   list.Add(4);
来源：http://kub.tianlin.xyz

[D03] 在指定位置插入元素
来源：http://qeu.yangfankeji.com

Py:   arr.insert(0, 0)
来源：http://plb.fzhhl.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ure.gotoacloud.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qyk.xylfe.cn

TS:   arr.splice(0, 0, 0);
来源：http://klv.shanyushiyangkeji.top

Java: list.add(0, 0);
来源：http://hfy.fanxiaobao.xyz

Go:   arr = append([]int{0}, arr...)
来源：http://vgg.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kys.sweek.top

C#:   list.Insert(0, 0);
来源：http://jas.fzhhl.top

[D04] 删除元素
来源：http://ygs.fzhhl.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://knl.jinqigfzy.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ijv.yongpay.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://kjp.jyoumei.cn

TS:   arr.splice(0, 1);
来源：http://zku.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tcz.gzhubu.top

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zdi.smart0.xyz


<!-- 参考信息 -->