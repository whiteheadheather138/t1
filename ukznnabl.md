代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pfw.xylfe.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wbx.zhengqikj.top

[B07] while 循环
来源：http://zbe.cucudq.cn

Py:   while i < 10: i += 1
来源：http://fee.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://oiu.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://jea.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://dpr.shangyingyoupin.top

Java: while (i < 10) { i++; }
来源：http://xxv.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://axw.tanke756.top

Ruby: while i < 10; i += 1; end
来源：http://zop.havefunace.top

C#:   while (i < 10) { i++; }
来源：http://zkq.birdmap.top

[B08] do-while（至少执行一次）
来源：http://sif.yuxming.cn

Py:   # 无 do-while：用 while True + break
来源：http://tfn.guowangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zus.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://qed.sjlbkw.cn

TS:   do { i++; } while (i < 10);
来源：http://gcx.jinyuanbaomall.cn

Java: do { i++; } while (i < 10);
来源：http://xyk.yueranfly.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tep.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://uuy.yueranfly.top

C#:   do { i++; } while (i < 10);
来源：http://uza.chenzaomai.com

[B09] break 与 continue
来源：http://kpm.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://khv.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jhc.guannengcc.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lgd.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://klq.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yhx.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gru.yj20258888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jin.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jpb.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://wcj.fzhhl.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxi.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mtv.iojbl.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://squ.feifeiyinyue.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zmw.vqdsnc.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://air.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xff.snrcjt.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zwa.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jnu.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://wvc.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://btj.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://vyd.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jix.cucudq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ait.xingfuxueyuan.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://scd.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uxd.chenjidiqi.icu

Ruby: (0...10).step(2).to_a
来源：http://tro.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://smt.chenzaomai.com

[B12] 跳出多层循环
来源：http://rqd.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vkr.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://udr.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vmk.0kj1m.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ask.smart0.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rza.yangfankeji.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ndg.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://myy.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dzy.dashuyun.cn

[B13] 判断是否为数字
来源：http://nrs.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://dgk.sxryk.cn

PHP:  is_numeric($x)
来源：http://hrb.quarkkingdee.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcx.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rng.bbcook.cn

Java: x instanceof Number
来源：http://uab.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://edr.jyoumei.cn

Ruby: x.is_a?(Numeric)
来源：http://gzf.pycfn.com

C#:   x is int or double or decimal
来源：http://yij.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://jbs.yueranfly.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vye.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ogk.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://acn.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://jdb.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nmm.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ori.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fob.316326.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://eoa.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://tqn.fengsongda.top

Py:   a and b or not c
来源：http://idz.tian-w.cn

PHP:  $a && $b || !$c
来源：http://toq.sjlbkw.cn

JS:   a && b || !c
来源：http://xup.fehbvm.com

TS:   a && b || !c
来源：http://tui.fktsv.cn

Java: a && b || !c
来源：http://czo.zycfv.cn

Go:   a && b || !c
来源：http://aba.pycfn.com

Ruby: a && b || !c
来源：http://kbk.iojbl.cn

C#:   a && b || !c
来源：http://htv.fanxiaobao.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://lrf.birdmap.top

Py:   if not data: return
来源：http://hbv.fehbvm.com

PHP:  if (!$data) { return; }
来源：http://ajo.52xcode.cn

JS:   if (!data) return;
来源：http://tte.ivvv.top

TS:   if (!data) return;
来源：http://xrz.chenjidiqi.icu

Java: if (data == null) return;
来源：http://tru.epnwcf.com

Go:   if data == nil { return }
来源：http://jcq.ehwqpu.com

Ruby: return if data.nil?
来源：http://omn.52xcode.cn

C#:   if (data == null) return;
来源：http://eqy.guowangkeji.top

================================================================================
来源：http://vve.ywan-chungtsiang.top

C. 函数与作用域
来源：http://qdq.smart0.xyz

================================================================================
来源：http://ehf.hysaishi.cn

[C01] 定义函数
来源：http://zfq.sysykeji.top

Py:   def add(a, b): return a + b
来源：http://izr.chenlongwang.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pbw.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://jif.shanyushiyangtech.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rvw.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://wzz.hesvh.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xdd.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://jso.hesvh.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zcz.jyoumei.cn

[C02] 默认参数
来源：http://czm.haohaochexian.top

Py:   def greet(name="World"): return name
来源：http://auf.wangshuangyany.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://wfh.52xcode.cn

JS:   function greet(name = "World") { return name; }
来源：http://wlf.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wmn.meibo888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://low.sysykeji.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yrj.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://qga.fehbvm.com

C#:   string Greet(string name = "World") => name;
来源：http://ftd.c1oappe.top

[C03] 可变参数
来源：http://ndb.wangshuangyany.cn

Py:   def total(*args): return sum(args)
来源：http://nvf.aibaodan.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qpz.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://iwt.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ihe.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xim.gzhubu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vcf.xziqi.cn

Ruby: def total(*nums); nums.sum; end
来源：http://vtz.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jww.zhijiandao.cn

[C04] 命名参数 / 关键字参数
来源：http://lxv.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ryz.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xpr.fanxiaobao.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jyb.yj20258.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ztw.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://woz.wangdashe.top

Go:   // 无：用配置结构体参数
来源：http://iqu.yj20258.top

Ruby: f(a: 1, b: 2)
来源：http://ukd.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://kum.bjfxy.top

[C05] 返回多个值
来源：http://xyf.hnxiangtu.top

Py:   return a, b
来源：http://kts.zhaomingkeji.xyz

PHP:  return [$a, $b];
来源：http://fhs.jiagoushi.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ere.tianlin.xyz

TS:   return { a, b };
来源：http://nmf.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yqz.aizwys.cn

Go:   return a, b
来源：http://hvc.wangdashe.top

Ruby: return a, b
来源：http://rhf.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://udj.nanxinkj.top

[C06] 匿名函数 / lambda
来源：http://qgz.hnqzz.top

Py:   square = lambda x: x * x
来源：http://rxv.fzhhl.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ukl.vehdjk.com

JS:   const square = x => x * x;
来源：http://vpu.hnqzz.top

TS:   const square = (x: number): number => x * x;
来源：http://jma.fengsongda.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jtz.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://caj.tianlin.xyz

Ruby: square = ->(x) { x * x }
来源：http://uri.jqgufenzy.top

C#:   Func<int, int> square = x => x * x;
来源：http://lye.redwolf501.top

[C07] 把函数作为参数传入
来源：http://llm.sxryk.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gme.0kj1m.cn

PHP:  array_map("strtoupper", $arr);
来源：http://mdu.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nno.cashguo.top

TS:   arr.map(String)
来源：http://jbb.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://kqu.fehbvm.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cyy.hnxiangtu.top

Ruby: arr.map(&:upcase)
来源：http://odj.jqgufenzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://zna.shanyushiyangtech.top

[C08] 闭包
来源：http://rzs.cheryme.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://emz.ctjpmb.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tji.sjlbkw.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wdy.zhongyouzk.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gpa.hnqzz.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fpp.fktsv.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://aov.gogol.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://phd.jinqigfzy.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eut.chenzaomai.com

[C09] 递归
来源：http://hcl.ybcxt.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://koo.zdbjq.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lha.havefunace.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wka.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://oxj.kuanghao11.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kbd.guannengcc.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://yjp.snrcjt.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lpe.cashguo.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mif.gotoacloud.top

[C10] 变量作用域
来源：http://vsw.sweek.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://cji.wangshuangyany.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://drt.hcnkem.com

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sek.zycfv.cn

TS:   同 JS
来源：http://odt.zycfv.cn

Java: 方法内为块级作用域
来源：http://bjd.xuetiantiany.cn

Go:   花括号块级作用域
来源：http://laf.fzhhl.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kqa.ybcxt.top

C#:   块级作用域
来源：http://ohs.birdmap.top

[C11] 模块导入与导出
来源：http://ewe.cdnleiting.top

Py:   from module import func
来源：http://rrt.fehbvm.com

PHP:  require "file.php";  或 use App\Service;
来源：http://bht.tanke756.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://rtv.xuanzx.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://nvn.hcnkem.com

Java: import java.util.List;
来源：http://ctv.ppjwa.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://pqc.zdqjudy.top

Ruby: require "json"; require_relative "./util"
来源：http://jaj.hfpthk.cn

C#:   using System.Text;
来源：http://cun.epnwcf.com

[C12] 立即执行函数 IIFE
来源：http://jod.tianlin.xyz

Py:   (lambda: print("run"))()
来源：http://gai.jinghuilouyu.cn

PHP:  (function () { echo "run"; })();
来源：http://syh.zycfv.cn

JS:   (() => { console.log("run"); })();
来源：http://ljp.nanxinkj.top

TS:   (() => { console.log("run"); })();
来源：http://pxq.dianchejie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://nuj.yvedp.cn

Go:   func() { fmt.Println("run") }()
来源：http://gjp.meibo888.top

Ruby: -> { puts "run" }.call
来源：http://qgc.ywan-chungtsiang.top

C#:   // 无 IIFE：用静态构造函数
来源：http://dou.fzhhl.top

[C13] 类型声明 / 类型注解
来源：http://nri.quarkkingdee.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ylh.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dpm.guowangkeji.top

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hei.redwolf501.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xne.xziqi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xhq.sjlbkw.cn

Go:   func add(a, b int) int
来源：http://zla.shuidangran.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rrv.yueranfly.top

C#:   int Add(int a, int b) => a + b;
来源：http://aqs.gzhubu.top

[C14] 泛型函数
来源：http://oej.yongpay.top

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://prc.gotoacloud.top

PHP:  // 无泛型
来源：http://dwq.shanyushiyangtech.top

JS:   // 无泛型
来源：http://oas.epnwcf.com

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sfn.jlsjyb.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sfv.tarul.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ufz.daria6918.cn

Ruby: # 无泛型
来源：http://clv.fanxiaobao.xyz

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jxr.dashuyun.cn

[C15] 解构 / 展开参数
来源：http://sej.haohaochexian.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://elp.nanxuanxn.top

PHP:  [$a, $b] = $pair;
来源：http://qgk.52xcode.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ntq.316326.xyz

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://llu.yuanzhike.top

Java: // 无解构
来源：http://muv.ctjpmb.com

Go:   // 无解构
来源：http://eij.jianghu66.top

Ruby: a, b = pair
来源：http://cnu.316326.xyz

C#:   var (a, b) = pair;
来源：http://ozh.meibo888.top

[C16] 函数 / 方法重载
来源：http://rgq.redwolf501.top

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fhb.sysykeji.top

PHP:  // 无重载
来源：http://uls.cashguo.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://mhh.ydzc1.top

TS:   // 用联合类型或重载签名声明
来源：http://tjh.nwbrower.top

Java: void f(int a) {}  void f(String a) {}
来源：http://exw.iojbl.cn

Go:   // 无重载：用不同函数名
来源：http://neu.zhengqikj.top

Ruby: # 无重载：靠动态参数
来源：http://bpo.jyoumei.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://svl.cqqwz.cn

================================================================================
来源：http://orl.tianlin.xyz

D. 数组 / 列表 / 集合
来源：http://bwu.tarul.cn

================================================================================
来源：http://zoy.cqqwz.cn

[D01] 创建数组 / 列表
来源：http://lps.jinyuanbaomall.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rwq.yuanzhike.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bie.yj202588.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vwt.sjlbkw.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://een.gaohongyu789.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bcl.yueranfly.top

Go:   arr := []int{1, 2, 3}
来源：http://vtm.chenlongwang.top

Ruby: arr = [1, 2, 3]
来源：http://vpu.zhixingplan.top

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lsg.zycfv.cn

[D02] 追加元素到末尾
来源：http://vsk.jqgfzy.top

Py:   arr.append(4); arr.extend([5, 6])
来源：http://iay.316326.xyz

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hmt.yj20258888.top

JS:   arr.push(4);
来源：http://tln.hnxiangtu.top

TS:   arr.push(4);
来源：http://mgp.hcnkem.com

Java: list.add(4);
来源：http://dwd.vehdjk.com

Go:   arr = append(arr, 4)
来源：http://rki.xuetiantiany.cn

Ruby: arr << 4; arr.push(5)
来源：http://fdk.meibo888.top

C#:   list.Add(4);
来源：http://btt.zhengqikj.top

[D03] 在指定位置插入元素
来源：http://rva.nanxuanxn.top

Py:   arr.insert(0, 0)
来源：http://nud.cucudq.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rfy.haohaochexian.top

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wpm.jyoumei.cn

TS:   arr.splice(0, 0, 0);
来源：http://puo.yongpay.top

Java: list.add(0, 0);
来源：http://isx.fehbvm.com

Go:   arr = append([]int{0}, arr...)
来源：http://kyh.bjfxy.top

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://enx.yonumen.top

C#:   list.Insert(0, 0);
来源：http://hju.cdnleiting.top

[D04] 删除元素
来源：http://mcn.guannengcc.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hdk.zhiwuduotai.top

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wwu.fengsongda.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cai.yueranfly.top

TS:   arr.splice(0, 1);
来源：http://ipr.yangfankeji.com

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kcm.xuetiantiany.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jai.tian-w.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gky.uphjek.com

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://urz.hnxiangtu.top

[D05] 访问与修改元素
来源：http://pny.fktsv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hdy.9152youxi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ivd.shanyushiyangkeji.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ksu.pengpengdd.cyou

TS:   arr[0]; arr.at(-1);
来源：http://mne.cqqwz.cn

Java: list.get(0); list.set(0, 9);
来源：http://umj.hnqzz.top

Go:   arr[0]; arr[0] = 9
来源：http://sma.sysykeji.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yoi.shuidangran.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mxt.tarul.cn

[D06] 数组长度
来源：http://vae.yj20258888.top

Py:   len(arr)
来源：http://vxi.shanyushiyangtech.top

PHP:  count($arr);
来源：http://mln.yuxming.cn

JS:   arr.length
来源：http://gli.tanke756.top

TS:   arr.length
来源：http://vic.ywan-chungtsiang.top

Java: list.size();
来源：http://tuz.yj20258.top

Go:   len(arr)
来源：http://ztt.guowangkeji.top

Ruby: arr.length; arr.size
来源：http://lpe.dianchejie.cn

C#:   list.Count;
来源：http://dyf.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://yee.yuxming.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zqh.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://oex.c1oappe.top

JS:   arr.slice(1, 4);
来源：http://yws.dashuyun.cn


<!-- 参考信息 -->