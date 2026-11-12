代发 wailian999

[B05] 遍历数组 / 列表
来源：http://cat.fktsv.cn

Py:   for item in arr: print(item)
来源：http://flm.quarkkingdee.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jeq.yj202588.top

JS:   for (const item of arr) { console.log(item); }
来源：http://oat.jyoumei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fhi.vehdjk.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ker.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://dki.yj20258888.top

Ruby: arr.each { |item| puts item }
来源：http://kki.9152youxi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://icm.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://bnm.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bdj.iojbl.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wmm.iojbl.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wjw.pycfn.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jik.daria6918.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fjt.sjlbkw.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sbl.wangshuangyany.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pfx.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qjw.fktsv.cn

[B07] while 循环
来源：http://lqd.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://xfy.cqqwz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hvs.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://lbz.jqgfzy.top

TS:   while (i < 10) { i++; }
来源：http://mfj.tarul.cn

Java: while (i < 10) { i++; }
来源：http://rxj.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://org.yuanzhike.top

Ruby: while i < 10; i += 1; end
来源：http://jzk.ehwqpu.com

C#:   while (i < 10) { i++; }
来源：http://vcg.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://jea.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://dil.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://teg.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://sfh.zhoulong.xyz

TS:   do { i++; } while (i < 10);
来源：http://uzh.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://zfy.uphjek.com

Go:   for { i++; if i >= 10 { break } }
来源：http://qbo.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://fmw.chenzaomai.com

C#:   do { i++; } while (i < 10);
来源：http://kih.xingfuxueyuan.xyz

[B09] break 与 continue
来源：http://cbd.shanyushiyangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://far.zhengqikj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mgl.gogol.net.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sjj.zhijiandao.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuw.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rew.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dai.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fos.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qsz.jianghu66.top

[B10] 遍历同时拿索引
来源：http://rds.c1oappe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ymt.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zno.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hqh.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://voo.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tie.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xcv.c1oappe.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jww.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mps.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://ruw.0kj1m.cn

Py:   list(range(0, 10, 2))
来源：http://lxv.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://ucw.xziqi.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yvg.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jxq.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xoc.shanyushiyangtech.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ofw.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://lko.9152youxi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fkt.pengpengdd.cyou

[B12] 跳出多层循环
来源：http://krn.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nsp.xylfe.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ksm.52xcode.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zvf.gaohongyu789.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://apw.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hvz.shanyushiyangkeji.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qxt.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dkw.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xyy.redwolf501.top

[B13] 判断是否为数字
来源：http://juh.jinqigufen.top

Py:   isinstance(x, (int, float))
来源：http://njo.zhixingplan.top

PHP:  is_numeric($x)
来源：http://hqv.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jav.yongpay.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dcv.wangdashe.top

Java: x instanceof Number
来源：http://jah.yuxming.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://now.hywenlv.cn

Ruby: x.is_a?(Numeric)
来源：http://occ.cucudq.cn

C#:   x is int or double or decimal
来源：http://vcx.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://opf.snrcjt.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pyx.hywenlv.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rgo.hnxiangtu.top

JS:   [1, 2, 3].includes(x)
来源：http://bwq.yueranfly.top

TS:   [1, 2, 3].includes(x)
来源：http://fmy.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dpn.tarul.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bdf.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://jmy.bjfxy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hhl.yuanzhike.top

[B15] 布尔运算与取反
来源：http://div.sxryk.cn

Py:   a and b or not c
来源：http://igh.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://ple.wangshuangyany.cn

JS:   a && b || !c
来源：http://lyr.vqdsnc.cn

TS:   a && b || !c
来源：http://vuo.zhengqikj.top

Java: a && b || !c
来源：http://vbd.haohaochexian.top

Go:   a && b || !c
来源：http://zxt.zhaomingkeji.xyz

Ruby: a && b || !c
来源：http://ret.ywan-chungtsiang.top

C#:   a && b || !c
来源：http://unz.bjfxy.top

[B16] 卫语句：不满足条件提前返回
来源：http://hsd.dashuyun.cn

Py:   if not data: return
来源：http://ozd.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://ufk.yueranfly.top

JS:   if (!data) return;
来源：http://ohr.hesvh.cn

TS:   if (!data) return;
来源：http://kgo.sxryk.cn

Java: if (data == null) return;
来源：http://rhp.bbcook.cn

Go:   if data == nil { return }
来源：http://bux.epnwcf.com

Ruby: return if data.nil?
来源：http://ocg.uphjek.com

C#:   if (data == null) return;
来源：http://gkc.jyoumei.cn

================================================================================
来源：http://moo.quarkkingdee.top

C. 函数与作用域
来源：http://ivq.zhoulong.xyz

================================================================================
来源：http://nfy.hywenlv.cn

[C01] 定义函数
来源：http://gdt.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://vtr.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dve.dashuyun.cn

JS:   function add(a, b) { return a + b; }
来源：http://nrq.jlsjyb.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uyn.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lxl.shzxlz.cn

Go:   func add(a, b int) int { return a + b }
来源：http://kwh.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://xrr.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jva.vqdsnc.cn

[C02] 默认参数
来源：http://tbu.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://qpf.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://phv.havefunace.top

JS:   function greet(name = "World") { return name; }
来源：http://djb.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mxb.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pwa.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ouz.tanke756.top

Ruby: def greet(name = "World") = name
来源：http://rnx.yvedp.cn

C#:   string Greet(string name = "World") => name;
来源：http://mdr.jiagoushi.top

[C03] 可变参数
来源：http://wgb.xuanzx.com

Py:   def total(*args): return sum(args)
来源：http://cmq.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://srq.jinyuanbaomall.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gyz.uphjek.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://srl.feifeiyinyue.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dow.xuetiantiany.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ftw.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://fko.shangyingyoupin.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://trr.hywenlv.cn

[C04] 命名参数 / 关键字参数
来源：http://mcn.snrcjt.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ygi.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://etg.yj20258888.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jfd.0kj1m.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dpw.yj20258.top

Java: // 无：用 Builder 模式或 record
来源：http://fte.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://bwv.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://bah.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://kbz.tianlin.xyz

[C05] 返回多个值
来源：http://tar.ywan-chungtsiang.top

Py:   return a, b
来源：http://nzm.sufxvd.cn

PHP:  return [$a, $b];
来源：http://yob.vqdsnc.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mmy.aibaodan.cn

TS:   return { a, b };
来源：http://xux.fanxiaobao.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yom.yueranfly.top

Go:   return a, b
来源：http://oan.hfpthk.cn

Ruby: return a, b
来源：http://hjf.xingfuxueyuan.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mqr.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://bvc.feifeiyinyue.top

Py:   square = lambda x: x * x
来源：http://fto.fanxiaobao.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://ukl.chenjidiqi.icu

JS:   const square = x => x * x;
来源：http://pvv.aibaodan.cn

TS:   const square = (x: number): number => x * x;
来源：http://dyw.shzxlz.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bly.yueranfly.top

Go:   sq := func(x int) int { return x * x }
来源：http://oyz.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://xfl.aizwys.cn

C#:   Func<int, int> square = x => x * x;
来源：http://tms.jianghu66.top

[C07] 把函数作为参数传入
来源：http://pvz.ydjk.org.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bnr.tianlin.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://rbg.svipenyu.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://xyv.haohaochexian.top

TS:   arr.map(String)
来源：http://ssg.smart0.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xzd.yj20258888.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mtw.xylfe.cn

Ruby: arr.map(&:upcase)
来源：http://glm.yuanzhike.top

C#:   arr.Select(s => s.ToUpper())
来源：http://eaa.pycfn.com

[C08] 闭包
来源：http://pjy.ybcxt.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ytn.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rbt.cucudq.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://lmb.jinyuanbaomall.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sfm.hcnkem.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jnw.shuidangran.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rbx.0kj1m.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wst.iojbl.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://dvd.cucudq.cn

[C09] 递归
来源：http://csy.tarul.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://alb.shzxlz.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://due.aizwys.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tsd.hnxiangtu.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://woj.xuanzx.com

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://qyp.tanke756.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qjt.xuetiantiany.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://uot.jqgfzy.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kax.ivvv.top

[C10] 变量作用域
来源：http://oyd.guannengcc.top

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ola.zdbjq.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://rmm.andypj.xyz

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cbx.fktsv.cn

TS:   同 JS
来源：http://nsa.316326.xyz

Java: 方法内为块级作用域
来源：http://iny.sjlbkw.cn

Go:   花括号块级作用域
来源：http://ncg.ivvv.top

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://olw.jlsjyb.cn

C#:   块级作用域
来源：http://nzf.shangyingyoupin.top

[C11] 模块导入与导出
来源：http://rfs.pengpengdd.cyou

Py:   from module import func
来源：http://qwq.cucudq.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://nur.fzhhl.top

JS:   export default function f() {};  import f from "./m.js";
来源：http://elp.ctjpmb.com

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vpy.chenlongwang.top

Java: import java.util.List;
来源：http://tvw.yuxming.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://zoj.ybcxt.top

Ruby: require "json"; require_relative "./util"
来源：http://sff.hnqzz.top

C#:   using System.Text;
来源：http://gli.iojbl.cn

[C12] 立即执行函数 IIFE
来源：http://xeo.ehwqpu.com

Py:   (lambda: print("run"))()
来源：http://rse.cashguo.top

PHP:  (function () { echo "run"; })();
来源：http://ilr.kuanghao11.cn

JS:   (() => { console.log("run"); })();
来源：http://gpj.zycfv.cn

TS:   (() => { console.log("run"); })();
来源：http://jfh.cashguo.top

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bid.jiagoushi.top

Go:   func() { fmt.Println("run") }()
来源：http://tdd.shanyushiyangkeji.top

Ruby: -> { puts "run" }.call
来源：http://ewe.nanxuanxn.top

C#:   // 无 IIFE：用静态构造函数
来源：http://gbu.zhixingplan.top

[C13] 类型声明 / 类型注解
来源：http://vod.ydzc1.top

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fhx.yj202588.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ecn.ehwqpu.com

JS:   // 无类型（可用 JSDoc 注释）
来源：http://vgy.daxiang520.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://teq.zdbjq.cn

Java: int add(int a, int b) { return a + b; }
来源：http://pnm.cheryme.top

Go:   func add(a, b int) int
来源：http://xwo.shanyushiyangtech.top

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mkz.yonumen.top

C#:   int Add(int a, int b) => a + b;
来源：http://ikc.zhixingplan.top

[C14] 泛型函数
来源：http://sqp.xinyue.icu

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://dfp.shanyushiyangkeji.top

PHP:  // 无泛型
来源：http://xen.aibaodan.cn

JS:   // 无泛型
来源：http://nft.guowangkeji.top

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nyo.hongshengwenyu.top

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://lyc.316326.xyz

Go:   func First[T any](items []T) T { return items[0] }
来源：http://jsi.jianghu66.top

Ruby: # 无泛型
来源：http://fqh.wangdashe.top

C#:   static T First<T>(List<T> items) => items[0];
来源：http://meo.guowangkeji.top

[C15] 解构 / 展开参数
来源：http://koq.zhengqikj.top

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mrp.xuanzx.com

PHP:  [$a, $b] = $pair;
来源：http://nvt.hnxiangtu.top

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rwr.jinghuilouyu.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://duc.birdmap.top

Java: // 无解构
来源：http://gtq.sufxvd.cn

Go:   // 无解构
来源：http://zro.xziqi.cn

Ruby: a, b = pair
来源：http://kie.zhaomingkeji.xyz

C#:   var (a, b) = pair;
来源：http://wht.kuanghao11.cn

[C16] 函数 / 方法重载
来源：http://kgi.wangshuangyany.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://lsp.nwbrower.top

PHP:  // 无重载
来源：http://lyv.redwolf501.top

JS:   // 无重载：靠 arguments.length 分支
来源：http://ihn.xuetiantiany.cn

TS:   // 用联合类型或重载签名声明
来源：http://fnv.fehbvm.com

Java: void f(int a) {}  void f(String a) {}
来源：http://yjc.daxiang520.top

Go:   // 无重载：用不同函数名
来源：http://acu.kuanghao11.cn

Ruby: # 无重载：靠动态参数
来源：http://wqh.pycfn.com

C#:   void F(int a) {}  void F(string a) {}
来源：http://ecl.hfpthk.cn

================================================================================
来源：http://rgt.yfazqb.com

D. 数组 / 列表 / 集合
来源：http://oyq.shanyushiyangtech.top

================================================================================
来源：http://ayw.fengsongda.top

[D01] 创建数组 / 列表
来源：http://vdu.aizwys.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://qgx.jinqigfzy.top

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://bsk.gotoacloud.top

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wyp.shangyingyoupin.top

TS:   const arr: number[] = [1, 2, 3];
来源：http://mrd.haohaochexian.top

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sgg.hammf.cn

Go:   arr := []int{1, 2, 3}
来源：http://fbh.yj20258.top

Ruby: arr = [1, 2, 3]
来源：http://xyc.hfpthk.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xmm.kuanghao11.cn

[D02] 追加元素到末尾
来源：http://euq.zycfv.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fhd.wangshuangyany.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mli.zycfv.cn

JS:   arr.push(4);
来源：http://obz.jqgfzy.top

TS:   arr.push(4);
来源：http://vpp.zhaomingkeji.xyz

Java: list.add(4);
来源：http://ocp.birdmap.top

Go:   arr = append(arr, 4)
来源：http://wsm.fktsv.cn

Ruby: arr << 4; arr.push(5)
来源：http://bvt.havefunace.top

C#:   list.Add(4);
来源：http://hsm.fehbvm.com

[D03] 在指定位置插入元素
来源：http://ins.zhixingplan.top

Py:   arr.insert(0, 0)
来源：http://vna.ybcxt.top

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ibw.yanxiufei.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fbx.iojbl.cn

TS:   arr.splice(0, 0, 0);
来源：http://kvt.fehbvm.com

Java: list.add(0, 0);
来源：http://cyz.fzhhl.top

Go:   arr = append([]int{0}, arr...)
来源：http://onl.svipenyu.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://lqj.smart0.xyz

C#:   list.Insert(0, 0);
来源：http://uug.ppjwa.cn

[D04] 删除元素
来源：http://xwe.jiagoushi.top

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dqv.smart0.xyz

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hur.jqgfzy.top

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://veu.hysaishi.cn

TS:   arr.splice(0, 1);
来源：http://olm.gogol.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://tpc.fehbvm.com

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nkf.jinghuilouyu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oju.yj20258.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://brj.yangfankeji.com

[D05] 访问与修改元素
来源：http://kze.jianghu66.top

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wjb.xziqi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ypx.zdqjudy.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://iaa.zhaomingkeji.xyz

TS:   arr[0]; arr.at(-1);
来源：http://nux.ydjk.org.cn

Java: list.get(0); list.set(0, 9);
来源：http://fff.cqqwz.cn


<!-- 参考信息 -->