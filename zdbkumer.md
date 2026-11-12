代发 wailian999

Py:   for i in range(10): print(i)
来源：http://ajr.vehdjk.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zet.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhg.yuxming.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ete.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jog.yanxiufei.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rev.yj202588.top

Ruby: 10.times { |i| puts i }
来源：http://vkx.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ihw.shuidangran.top

[B05] 遍历数组 / 列表
来源：http://nhm.yongpay.top

Py:   for item in arr: print(item)
来源：http://epw.bjfxy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ooj.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ukd.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://rre.sjlbkw.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://flw.bbcook.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ays.fktsv.cn

Ruby: arr.each { |item| puts item }
来源：http://cxt.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lno.hammf.cn

[B06] 遍历字典 / 对象
来源：http://lvo.xylfe.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://abx.yuxming.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mjt.ydjk.org.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://msj.havefunace.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gty.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://dam.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ogk.c1oappe.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eqt.epnwcf.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://few.redwolf501.top

[B07] while 循环
来源：http://yxr.zhiwuduotai.top

Py:   while i < 10: i += 1
来源：http://isp.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://hlh.kuanghao11.cn

JS:   while (i < 10) { i++; }
来源：http://kpg.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://xej.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://jjj.daxiang520.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qao.yj202588.top

Ruby: while i < 10; i += 1; end
来源：http://jbf.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://yus.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://gpb.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://rcg.fanxiaobao.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://lcn.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://klo.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://zsi.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://icr.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fvx.hesvh.cn

Ruby: begin; i += 1; end while i < 10
来源：http://whz.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://udx.mhx1999.top

[B09] break 与 continue
来源：http://ocy.gzhubu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bba.fktsv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fhv.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umh.shanyushiyangkeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://feo.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bka.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://szp.zdqjudy.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ouh.hywenlv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fcr.yj202588.top

[B10] 遍历同时拿索引
来源：http://slz.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xca.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://scn.jianghu66.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ndr.jqgfzy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xkn.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pux.gotoacloud.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://osb.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wcj.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vqe.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://nzi.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://ogt.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://djr.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjx.yonumen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ucn.birdmap.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hiy.pycfn.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ozj.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://rbj.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wev.meibo888.top

[B12] 跳出多层循环
来源：http://lgz.yuanzhike.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://onb.yj20258.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://dzk.svipenyu.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://exp.ybcxt.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofa.shzxlz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://auc.cucudq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wsp.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://iqh.cucudq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://oho.zhijiandao.cn

[B13] 判断是否为数字
来源：http://cqw.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://amz.cucudq.cn

PHP:  is_numeric($x)
来源：http://ozx.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vje.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dyv.chenzaomai.com

Java: x instanceof Number
来源：http://oej.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://uty.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://fzs.yj20258888.top

C#:   x is int or double or decimal
来源：http://zdv.smart0.xyz

[B14] 判断值是否在集合内
来源：http://pyw.sysykeji.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hzy.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wmw.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://zpw.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://tqw.smart0.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://smj.0kj1m.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ycd.c1oappe.top

Ruby: [1, 2, 3].include?(x)
来源：http://mgl.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cgb.shanyushiyangtech.top

[B15] 布尔运算与取反
来源：http://isi.c1oappe.top

Py:   a and b or not c
来源：http://ege.dashuyun.cn

PHP:  $a && $b || !$c
来源：http://fls.shuidangran.top

JS:   a && b || !c
来源：http://udt.fzhhl.top

TS:   a && b || !c
来源：http://vyy.chenzaomai.com

Java: a && b || !c
来源：http://ymh.fengsongda.top

Go:   a && b || !c
来源：http://wgw.gogol.net.cn

Ruby: a && b || !c
来源：http://rdh.jqgfzy.top

C#:   a && b || !c
来源：http://uhy.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://ktv.zhiwuduotai.top

Py:   if not data: return
来源：http://yhe.cashguo.top

PHP:  if (!$data) { return; }
来源：http://nvm.jianghu66.top

JS:   if (!data) return;
来源：http://afg.yfazqb.com

TS:   if (!data) return;
来源：http://wha.nwbrower.top

Java: if (data == null) return;
来源：http://qid.jlsjyb.cn

Go:   if data == nil { return }
来源：http://nlo.cheryme.top

Ruby: return if data.nil?
来源：http://ecz.mhx1999.top

C#:   if (data == null) return;
来源：http://anz.zhongyouzk.top

================================================================================
来源：http://zdd.ivvv.top

C. 函数与作用域
来源：http://fot.wangshuangyany.cn

================================================================================
来源：http://miq.chenjidiqi.icu

[C01] 定义函数
来源：http://xnp.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://zpj.yfazqb.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xpp.yj202588.top

JS:   function add(a, b) { return a + b; }
来源：http://hnz.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxh.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mfz.xuanzx.com

Go:   func add(a, b int) int { return a + b }
来源：http://vcd.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://fmj.birdmap.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xrp.yuxming.cn

[C02] 默认参数
来源：http://ozx.xinyue.icu

Py:   def greet(name="World"): return name
来源：http://rce.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ycl.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://qbw.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dzk.9152youxi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zkx.feifeiyinyue.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hjo.vqdsnc.cn

Ruby: def greet(name = "World") = name
来源：http://har.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://mfl.zhixingplan.top

[C03] 可变参数
来源：http://sxs.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://zww.52xcode.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tgz.ydjk.org.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxh.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zkd.aibaodan.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifm.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lkt.sxryk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://yfy.pengpengdd.cyou

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kct.wangdashe.top

[C04] 命名参数 / 关键字参数
来源：http://ctc.sweek.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ujk.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hko.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://psm.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yvf.hysaishi.cn

Java: // 无：用 Builder 模式或 record
来源：http://wgo.jinghuilouyu.cn

Go:   // 无：用配置结构体参数
来源：http://mzw.zdqjudy.top

Ruby: f(a: 1, b: 2)
来源：http://utk.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://xns.guowangkeji.top

[C05] 返回多个值
来源：http://nst.daria6918.cn

Py:   return a, b
来源：http://arn.bjfxy.top

PHP:  return [$a, $b];
来源：http://wgc.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://qjc.xylfe.cn

TS:   return { a, b };
来源：http://esw.dianchejie.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ksw.uphjek.com

Go:   return a, b
来源：http://bxo.jinyuanbaomall.cn

Ruby: return a, b
来源：http://ebv.yj20258888.top

C#:   return (a, b);              // ValueTuple
来源：http://inn.haohaochexian.top

[C06] 匿名函数 / lambda
来源：http://fjg.yj20258.top

Py:   square = lambda x: x * x
来源：http://ihg.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://nel.hcnkem.com

JS:   const square = x => x * x;
来源：http://hsf.vqdsnc.cn

TS:   const square = (x: number): number => x * x;
来源：http://cwb.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://exs.jqgufenzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://nhu.hammf.cn

Ruby: square = ->(x) { x * x }
来源：http://bmg.chenlongwang.top

C#:   Func<int, int> square = x => x * x;
来源：http://stn.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://skx.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gny.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://cfz.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://jlh.svipenyu.cn

TS:   arr.map(String)
来源：http://kub.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://rhw.pengpengdd.cyou

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qyx.meibo888.top

Ruby: arr.map(&:upcase)
来源：http://uwm.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gpz.svipenyu.cn

[C08] 闭包
来源：http://rdh.vqdsnc.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://owt.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vfn.haohaochexian.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hmm.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gao.wangshuangyany.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ebi.yanxiufei.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hpr.daria6918.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://qcd.chenzaomai.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ogl.sysykeji.top

[C09] 递归
来源：http://abi.ppjwa.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://erw.iojbl.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jfp.cashguo.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dtk.ivvv.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zjw.shzxlz.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://xsp.sweek.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://rah.jianghu66.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hkp.smart0.xyz

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ish.jlsjyb.cn

[C10] 变量作用域
来源：http://otd.epnwcf.com

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xym.sweek.top

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ehp.yvedp.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tkr.ywan-chungtsiang.top

TS:   同 JS
来源：http://dlr.ctjpmb.com

Java: 方法内为块级作用域
来源：http://wgf.tarul.cn

Go:   花括号块级作用域
来源：http://jjz.dianchejie.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cfp.haohaochexian.top

C#:   块级作用域
来源：http://xmx.bjfxy.top

[C11] 模块导入与导出
来源：http://lee.haohaochexian.top

Py:   from module import func
来源：http://xkj.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://hjg.hysaishi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ule.jqgufenzy.top

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wvp.hysaishi.cn

Java: import java.util.List;
来源：http://svs.nanxuanxn.top

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://smu.zycfv.cn

Ruby: require "json"; require_relative "./util"
来源：http://szt.chenlongwang.top

C#:   using System.Text;
来源：http://got.cqqwz.cn

[C12] 立即执行函数 IIFE
来源：http://wua.sysykeji.top

Py:   (lambda: print("run"))()
来源：http://bpe.nwbrower.top

PHP:  (function () { echo "run"; })();
来源：http://gxk.zhaomingkeji.xyz

JS:   (() => { console.log("run"); })();
来源：http://nfp.zhixingplan.top

TS:   (() => { console.log("run"); })();
来源：http://ffk.jiagoushi.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://uxg.zdqjudy.top

Go:   func() { fmt.Println("run") }()
来源：http://cxp.yj20258.top

Ruby: -> { puts "run" }.call
来源：http://cpc.9152youxi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://wrt.sweek.top

[C13] 类型声明 / 类型注解
来源：http://omv.ydjk.org.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ehb.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cgj.gaohongyu789.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ghu.xziqi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://akr.jiagoushi.top

Java: int add(int a, int b) { return a + b; }
来源：http://iom.iojbl.cn

Go:   func add(a, b int) int
来源：http://mmy.yongpay.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://cqg.sweek.top

C#:   int Add(int a, int b) => a + b;
来源：http://hhr.yj20258888.top

[C14] 泛型函数
来源：http://gte.jinqigfzy.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ahk.dashuyun.cn

PHP:  // 无泛型
来源：http://dfk.tanke756.top

JS:   // 无泛型
来源：http://len.xuetiantiany.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gbu.redwolf501.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://dey.ehwqpu.com

Go:   func First[T any](items []T) T { return items[0] }
来源：http://idb.ehwqpu.com

Ruby: # 无泛型
来源：http://uzg.cashguo.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qgb.zhoulong.xyz

[C15] 解构 / 展开参数
来源：http://nwq.ydzc1.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nzh.guannengcc.top

PHP:  [$a, $b] = $pair;
来源：http://sot.guowangkeji.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mbm.tian-w.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://kgc.fengsongda.top

Java: // 无解构
来源：http://gtk.dianchejie.cn

Go:   // 无解构
来源：http://ymk.jyoumei.cn

Ruby: a, b = pair
来源：http://qfh.ppjwa.cn

C#:   var (a, b) = pair;
来源：http://bcs.hesvh.cn

[C16] 函数 / 方法重载
来源：http://ruw.yj202588.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://cvu.daxiang520.top

PHP:  // 无重载
来源：http://cba.ppjwa.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qbv.fzhhl.top

TS:   // 用联合类型或重载签名声明
来源：http://cpp.52xcode.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dfo.ehwqpu.com

Go:   // 无重载：用不同函数名
来源：http://uiz.0kj1m.cn

Ruby: # 无重载：靠动态参数
来源：http://neq.jinghuilouyu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kxl.cqqwz.cn

================================================================================
来源：http://fdt.fzhhl.top

D. 数组 / 列表 / 集合
来源：http://wtz.daxiang520.top

================================================================================
来源：http://vpq.gotoacloud.top

[D01] 创建数组 / 列表
来源：http://moq.jqgufenzy.top

Py:   arr = [1, 2, 3];  empty = []
来源：http://fcz.cdnleiting.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://yhb.aizwys.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://akh.ydzc1.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://guo.wangdashe.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bdg.meibo888.top

Go:   arr := []int{1, 2, 3}
来源：http://hvi.316326.xyz

Ruby: arr = [1, 2, 3]
来源：http://grw.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wuu.xingfuxueyuan.xyz

[D02] 追加元素到末尾
来源：http://nkj.meibo888.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://aja.zhoulong.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hhw.yongpay.top

JS:   arr.push(4);
来源：http://fzz.aizwys.cn

TS:   arr.push(4);
来源：http://lql.haohaochexian.top

Java: list.add(4);
来源：http://faj.hammf.cn

Go:   arr = append(arr, 4)
来源：http://ipz.yongpay.top

Ruby: arr << 4; arr.push(5)
来源：http://dnd.yonumen.top

C#:   list.Add(4);
来源：http://sgv.gotoacloud.top

[D03] 在指定位置插入元素
来源：http://xkv.ehwqpu.com

Py:   arr.insert(0, 0)
来源：http://mjd.jqgfzy.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xea.yangfankeji.com

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://tnj.jqgfzy.top

TS:   arr.splice(0, 0, 0);
来源：http://tgo.fzhhl.top

Java: list.add(0, 0);
来源：http://mzd.jinqigfzy.top

Go:   arr = append([]int{0}, arr...)
来源：http://kmf.gaohongyu789.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://eol.gaohongyu789.top

C#:   list.Insert(0, 0);
来源：http://vmg.zhongyouzk.top

[D04] 删除元素
来源：http://yhc.hnqzz.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://bcs.tarul.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wtl.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lyt.aizwys.cn

TS:   arr.splice(0, 1);
来源：http://tyt.jlsjyb.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eoj.316326.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://kbg.guowangkeji.top


<!-- 参考信息 -->