代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://ad.zhonguo7118.cn

[B06] 遍历字典 / 对象
来源：https://xt.zhonguo8118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://en.zhonguo1118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://iw.zhonguo8118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://ku.zhonguo3118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://df.zhonguo8118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://bc.zhonguo8118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ck.zhonguo7118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://me.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://dm.zhonguo1118.cn

[B07] while 循环
来源：https://km.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://qh.zhonguo7118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://eb.zhonguo7118.cn

JS:   while (i < 10) { i++; }
来源：https://zg.zhonguo8118.cn

TS:   while (i < 10) { i++; }
来源：https://hg.zhonguo5118.cn

Java: while (i < 10) { i++; }
来源：https://iv.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://ku.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://it.zhonguo5118.cn

C#:   while (i < 10) { i++; }
来源：https://kt.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://sl.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://oz.zhonguo4118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://fa.zhonguo3118.cn

JS:   do { i++; } while (i < 10);
来源：https://ay.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://xk.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://vc.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://rj.zhonguo2118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://mr.zhonguo1118.cn

C#:   do { i++; } while (i < 10);
来源：https://jh.zhonguo2118.cn

[B09] break 与 continue
来源：https://ck.zhonguo7118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://vt.zhonguo4118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ak.zhonguo4118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://vj.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://gg.zhonguo2118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://qc.zhonguo6118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://sf.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://qx.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ch.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://ue.zhonguo5118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://qk.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://lp.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://nt.zhonguo2118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ta.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://br.zhonguo6118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://om.zhonguo6118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://fa.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://qw.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://nk.zhonguo3118.cn

Py:   list(range(0, 10, 2))
来源：https://ny.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://vh.zhonguo8118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://cr.zhonguo6118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://na.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://nb.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://tv.zhonguo3118.cn

Ruby: (0...10).step(2).to_a
来源：https://pq.zhonguo7118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://wz.zhonguo5118.cn

[B12] 跳出多层循环
来源：https://jp.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://dv.zhonguo8118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://du.zhonguo3118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://dk.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://nv.zhonguo5118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://rx.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ci.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://pp.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://fz.zhonguo5118.cn

[B13] 判断是否为数字
来源：https://vc.zhonguo7118.cn

Py:   isinstance(x, (int, float))
来源：https://eq.zhonguo5118.cn

PHP:  is_numeric($x)
来源：https://rx.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://qw.zhonguo6118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://th.zhonguo4118.cn

Java: x instanceof Number
来源：https://zs.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://eg.zhonguo8118.cn

Ruby: x.is_a?(Numeric)
来源：https://zx.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://jb.zhonguo5118.cn

[B14] 判断值是否在集合内
来源：https://lh.zhonguo5118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://nu.zhonguo3118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ol.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ix.zhonguo1118.cn

TS:   [1, 2, 3].includes(x)
来源：https://mg.zhonguo5118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://ct.zhonguo6118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://dv.zhonguo8118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://bq.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://zm.zhonguo6118.cn

[B15] 布尔运算与取反
来源：https://lr.zhonguo4118.cn

Py:   a and b or not c
来源：https://te.zhonguo7118.cn

PHP:  $a && $b || !$c
来源：https://qc.zhonguo4118.cn

JS:   a && b || !c
来源：https://iv.zhonguo8118.cn

TS:   a && b || !c
来源：https://fj.zhonguo8118.cn

Java: a && b || !c
来源：https://fc.zhonguo8118.cn

Go:   a && b || !c
来源：https://tl.zhonguo2118.cn

Ruby: a && b || !c
来源：https://uq.zhonguo8118.cn

C#:   a && b || !c
来源：https://in.zhonguo8118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://qd.zhonguo3118.cn

Py:   if not data: return
来源：https://ra.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://uj.zhonguo2118.cn

JS:   if (!data) return;
来源：https://iw.zhonguo2118.cn

TS:   if (!data) return;
来源：https://gw.zhonguo4118.cn

Java: if (data == null) return;
来源：https://nn.zhonguo2118.cn

Go:   if data == nil { return }
来源：https://mz.zhonguo1118.cn

Ruby: return if data.nil?
来源：https://ls.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://ir.zhonguo5118.cn

================================================================================
来源：https://jp.zhonguo6118.cn

C. 函数与作用域
来源：https://kl.zhonguo3118.cn

================================================================================
来源：https://ef.zhonguo5118.cn

[C01] 定义函数
来源：https://kq.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://lk.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://zm.zhonguo2118.cn

JS:   function add(a, b) { return a + b; }
来源：https://ui.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://gv.zhonguo5118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://zg.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://fz.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://qj.zhonguo2118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://zo.zhonguo7118.cn

[C02] 默认参数
来源：https://yz.zhonguo4118.cn

Py:   def greet(name="World"): return name
来源：https://ys.zhonguo4118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://lf.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://pw.zhonguo2118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://os.zhonguo6118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://dz.zhonguo7118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://em.zhonguo7118.cn

Ruby: def greet(name = "World") = name
来源：https://qr.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://me.zhonguo1118.cn

[C03] 可变参数
来源：https://ku.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://ub.zhonguo5118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://kx.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://hk.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ix.zhonguo3118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://mt.zhonguo1118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://hx.zhonguo6118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://bp.zhonguo2118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://ma.zhonguo2118.cn

[C04] 命名参数 / 关键字参数
来源：https://ao.zhonguo1118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://oh.zhonguo3118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://ck.zhonguo3118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://wa.zhonguo8118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://mh.zhonguo3118.cn

Java: // 无：用 Builder 模式或 record
来源：https://jl.zhonguo5118.cn

Go:   // 无：用配置结构体参数
来源：https://kr.zhonguo4118.cn

Ruby: f(a: 1, b: 2)
来源：https://vf.zhonguo6118.cn

C#:   f(a: 1, b: 2)
来源：https://co.zhonguo2118.cn

[C05] 返回多个值
来源：https://vg.zhonguo7118.cn

Py:   return a, b
来源：https://kq.zhonguo8118.cn

PHP:  return [$a, $b];
来源：https://zp.zhonguo2118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://ju.zhonguo5118.cn

TS:   return { a, b };
来源：https://bf.zhonguo6118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://xc.zhonguo6118.cn

Go:   return a, b
来源：https://ej.zhonguo4118.cn

Ruby: return a, b
来源：https://ya.zhonguo2118.cn

C#:   return (a, b);              // ValueTuple
来源：https://uy.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://iv.zhonguo7118.cn

Py:   square = lambda x: x * x
来源：https://co.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://de.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://af.zhonguo1118.cn

TS:   const square = (x: number): number => x * x;
来源：https://nt.zhonguo3118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://ik.zhonguo1118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://tl.zhonguo3118.cn

Ruby: square = ->(x) { x * x }
来源：https://eo.zhonguo3118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://ru.zhonguo4118.cn

[C07] 把函数作为参数传入
来源：https://jj.zhonguo7118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://rt.zhonguo7118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://qw.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://oy.zhonguo4118.cn

TS:   arr.map(String)
来源：https://ww.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://tg.zhonguo6118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://fh.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://vg.zhonguo8118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://qd.zhonguo7118.cn

[C08] 闭包
来源：https://lk.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://dx.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://wu.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://pc.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://bi.zhonguo6118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://ww.zhonguo4118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://kn.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ld.zhonguo7118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://oe.zhonguo2118.cn

[C09] 递归
来源：https://uj.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ag.zhonguo7118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://tm.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://vb.zhonguo3118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ir.zhonguo1118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://dp.zhonguo8118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://gs.zhonguo7118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ut.zhonguo3118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://cq.zhonguo2118.cn

[C10] 变量作用域
来源：https://uw.zhonguo1118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://vy.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://cd.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://zp.zhonguo6118.cn

TS:   同 JS
来源：https://cm.zhonguo8118.cn

Java: 方法内为块级作用域
来源：https://zl.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://tg.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://yz.zhonguo3118.cn

C#:   块级作用域
来源：https://qn.zhonguo6118.cn

[C11] 模块导入与导出
来源：https://sj.zhonguo6118.cn

Py:   from module import func
来源：https://cm.zhonguo1118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://av.zhonguo7118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://at.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://ry.zhonguo1118.cn

Java: import java.util.List;
来源：https://xz.zhonguo7118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://th.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://zl.zhonguo2118.cn

C#:   using System.Text;
来源：https://op.zhonguo7118.cn

[C12] 立即执行函数 IIFE
来源：https://ag.zhonguo5118.cn

Py:   (lambda: print("run"))()
来源：https://rz.zhonguo8118.cn

PHP:  (function () { echo "run"; })();
来源：https://wh.zhonguo5118.cn

JS:   (() => { console.log("run"); })();
来源：https://wb.zhonguo4118.cn

TS:   (() => { console.log("run"); })();
来源：https://qp.zhonguo3118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://gm.zhonguo6118.cn

Go:   func() { fmt.Println("run") }()
来源：https://wx.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://eh.zhonguo8118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://mr.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://pz.zhonguo7118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://bp.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://lz.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://pf.zhonguo4118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://af.zhonguo5118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://tt.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://wo.zhonguo7118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://dl.zhonguo2118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://dy.zhonguo1118.cn

[C14] 泛型函数
来源：https://ze.zhonguo4118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ax.zhonguo5118.cn

PHP:  // 无泛型
来源：https://bw.zhonguo3118.cn

JS:   // 无泛型
来源：https://tt.zhonguo5118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://uj.zhonguo5118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://et.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://qr.zhonguo8118.cn

Ruby: # 无泛型
来源：https://lv.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://wn.zhonguo7118.cn

[C15] 解构 / 展开参数
来源：https://ep.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://zn.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://cm.zhonguo6118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://da.zhonguo1118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://qm.zhonguo3118.cn

Java: // 无解构
来源：https://vg.zhonguo6118.cn

Go:   // 无解构
来源：https://zr.zhonguo6118.cn

Ruby: a, b = pair
来源：https://ik.zhonguo2118.cn

C#:   var (a, b) = pair;
来源：https://kb.zhonguo8118.cn

[C16] 函数 / 方法重载
来源：https://fo.zhonguo1118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://gf.zhonguo4118.cn

PHP:  // 无重载
来源：https://lr.zhonguo3118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://sz.zhonguo6118.cn

TS:   // 用联合类型或重载签名声明
来源：https://mz.zhonguo2118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://vw.zhonguo6118.cn

Go:   // 无重载：用不同函数名
来源：https://wz.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://of.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jy.zhonguo6118.cn

================================================================================
来源：https://mm.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://ww.zhonguo3118.cn

================================================================================
来源：https://qm.zhonguo4118.cn

[D01] 创建数组 / 列表
来源：https://xd.zhonguo5118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://dn.zhonguo8118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://lv.zhonguo7118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://il.zhonguo3118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://ac.zhonguo7118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://gr.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://yk.zhonguo6118.cn

Ruby: arr = [1, 2, 3]
来源：https://ok.zhonguo5118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://fp.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://nc.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://ui.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://pq.zhonguo5118.cn

JS:   arr.push(4);
来源：https://kn.zhonguo6118.cn

TS:   arr.push(4);
来源：https://yj.zhonguo7118.cn

Java: list.add(4);
来源：https://pn.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://bg.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://oj.zhonguo2118.cn

C#:   list.Add(4);
来源：https://ea.zhonguo3118.cn

[D03] 在指定位置插入元素
来源：https://jc.zhonguo2118.cn

Py:   arr.insert(0, 0)
来源：https://dz.zhonguo4118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://qd.zhonguo2118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://iw.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://cy.zhonguo4118.cn

Java: list.add(0, 0);
来源：https://zh.zhonguo3118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://gj.zhonguo6118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://mz.zhonguo7118.cn

C#:   list.Insert(0, 0);
来源：https://gq.zhonguo4118.cn

[D04] 删除元素
来源：https://hl.zhonguo7118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://nx.zhonguo8118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://wz.zhonguo6118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://bv.zhonguo5118.cn

TS:   arr.splice(0, 1);
来源：https://sv.zhonguo2118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://iy.zhonguo7118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://kl.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://uh.zhonguo1118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://ih.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://dj.zhonguo8118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ml.zhonguo3118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://yg.zhonguo3118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://pv.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ru.zhonguo4118.cn

Java: list.get(0); list.set(0, 9);
来源：https://xj.zhonguo3118.cn

Go:   arr[0]; arr[0] = 9
来源：https://tu.zhonguo1118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://ej.zhonguo3118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://zk.zhonguo8118.cn

[D06] 数组长度
来源：https://nb.zhonguo6118.cn

Py:   len(arr)
来源：https://yu.zhonguo8118.cn

PHP:  count($arr);
来源：https://zm.zhonguo2118.cn

JS:   arr.length
来源：https://qj.zhonguo2118.cn

TS:   arr.length
来源：https://qi.zhonguo5118.cn


<!-- 参考信息 -->