代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://wo.zhonguo1118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://jt.zhonguo5118.cn

[B07] while 循环
来源：https://ep.zhonguo6118.cn

Py:   while i < 10: i += 1
来源：https://lx.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://ho.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://qe.zhonguo7118.cn

TS:   while (i < 10) { i++; }
来源：https://ai.zhonguo6118.cn

Java: while (i < 10) { i++; }
来源：https://hv.zhonguo7118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://ba.zhonguo2118.cn

Ruby: while i < 10; i += 1; end
来源：https://vi.zhonguo5118.cn

C#:   while (i < 10) { i++; }
来源：https://sp.zhonguo4118.cn

[B08] do-while（至少执行一次）
来源：https://mi.zhonguo3118.cn

Py:   # 无 do-while：用 while True + break
来源：https://ko.zhonguo6118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://of.zhonguo1118.cn

JS:   do { i++; } while (i < 10);
来源：https://rw.zhonguo7118.cn

TS:   do { i++; } while (i < 10);
来源：https://qp.zhonguo6118.cn

Java: do { i++; } while (i < 10);
来源：https://tz.zhonguo3118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://zk.zhonguo1118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://oi.zhonguo5118.cn

C#:   do { i++; } while (i < 10);
来源：https://ac.zhonguo3118.cn

[B09] break 与 continue
来源：https://jm.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://ac.zhonguo2118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://ll.zhonguo8118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://mh.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ys.zhonguo1118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://xd.zhonguo2118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://qt.zhonguo7118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://cj.zhonguo7118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://tt.zhonguo1118.cn

[B10] 遍历同时拿索引
来源：https://wf.zhonguo7118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://pd.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://pp.zhonguo7118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://hl.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://xa.zhonguo6118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://dq.zhonguo7118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ka.zhonguo2118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://fj.zhonguo3118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://zv.zhonguo8118.cn

[B11] 生成数字序列 / 区间
来源：https://fx.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://mm.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://hd.zhonguo3118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://lv.zhonguo8118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://jr.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://oi.zhonguo2118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://yi.zhonguo3118.cn

Ruby: (0...10).step(2).to_a
来源：https://ux.zhonguo3118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://gw.zhonguo4118.cn

[B12] 跳出多层循环
来源：https://mr.zhonguo3118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://ce.zhonguo3118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://kn.zhonguo1118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://pq.zhonguo4118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://wi.zhonguo7118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://oa.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://pd.zhonguo1118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://dq.zhonguo6118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://uw.zhonguo5118.cn

[B13] 判断是否为数字
来源：https://ep.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://ij.zhonguo1118.cn

PHP:  is_numeric($x)
来源：https://yk.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ej.zhonguo2118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://db.zhonguo8118.cn

Java: x instanceof Number
来源：https://dq.zhonguo8118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ai.zhonguo8118.cn

Ruby: x.is_a?(Numeric)
来源：https://bt.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://xf.zhonguo8118.cn

[B14] 判断值是否在集合内
来源：https://iw.zhonguo7118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://sx.zhonguo1118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://df.zhonguo4118.cn

JS:   [1, 2, 3].includes(x)
来源：https://vc.zhonguo4118.cn

TS:   [1, 2, 3].includes(x)
来源：https://wp.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://em.zhonguo5118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://qn.zhonguo3118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://vf.zhonguo6118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://as.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://wk.zhonguo4118.cn

Py:   a and b or not c
来源：https://ar.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://xq.zhonguo2118.cn

JS:   a && b || !c
来源：https://yz.zhonguo3118.cn

TS:   a && b || !c
来源：https://gd.zhonguo8118.cn

Java: a && b || !c
来源：https://ya.zhonguo3118.cn

Go:   a && b || !c
来源：https://kd.zhonguo5118.cn

Ruby: a && b || !c
来源：https://py.zhonguo6118.cn

C#:   a && b || !c
来源：https://tv.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://is.zhonguo7118.cn

Py:   if not data: return
来源：https://ce.zhonguo7118.cn

PHP:  if (!$data) { return; }
来源：https://zl.zhonguo1118.cn

JS:   if (!data) return;
来源：https://qo.zhonguo7118.cn

TS:   if (!data) return;
来源：https://kg.zhonguo7118.cn

Java: if (data == null) return;
来源：https://io.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://ok.zhonguo3118.cn

Ruby: return if data.nil?
来源：https://mn.zhonguo5118.cn

C#:   if (data == null) return;
来源：https://ei.zhonguo6118.cn

================================================================================
来源：https://ul.zhonguo5118.cn

C. 函数与作用域
来源：https://wj.zhonguo3118.cn

================================================================================
来源：https://eq.zhonguo8118.cn

[C01] 定义函数
来源：https://uy.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://of.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://hc.zhonguo8118.cn

JS:   function add(a, b) { return a + b; }
来源：https://lw.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://zo.zhonguo7118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://sr.zhonguo1118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://li.zhonguo5118.cn

Ruby: def add(a, b); a + b; end
来源：https://ha.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://pq.zhonguo5118.cn

[C02] 默认参数
来源：https://vh.zhonguo8118.cn

Py:   def greet(name="World"): return name
来源：https://qh.zhonguo5118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://ir.zhonguo3118.cn

JS:   function greet(name = "World") { return name; }
来源：https://xw.zhonguo8118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://cx.zhonguo5118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://br.zhonguo6118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://an.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://xu.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://ts.zhonguo7118.cn

[C03] 可变参数
来源：https://nj.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://bi.zhonguo1118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://ut.zhonguo7118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://yi.zhonguo1118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ln.zhonguo5118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://zk.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://px.zhonguo4118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://vf.zhonguo6118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://zu.zhonguo1118.cn

[C04] 命名参数 / 关键字参数
来源：https://wy.zhonguo1118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ai.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://lm.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://rc.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://jl.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://go.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://hc.zhonguo7118.cn

Ruby: f(a: 1, b: 2)
来源：https://yc.zhonguo4118.cn

C#:   f(a: 1, b: 2)
来源：https://wm.zhonguo3118.cn

[C05] 返回多个值
来源：https://rf.zhonguo5118.cn

Py:   return a, b
来源：https://hc.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://ji.zhonguo6118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://zc.zhonguo7118.cn

TS:   return { a, b };
来源：https://qv.zhonguo2118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ap.zhonguo1118.cn

Go:   return a, b
来源：https://iw.zhonguo3118.cn

Ruby: return a, b
来源：https://nw.zhonguo4118.cn

C#:   return (a, b);              // ValueTuple
来源：https://bg.zhonguo2118.cn

[C06] 匿名函数 / lambda
来源：https://xr.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://hz.zhonguo8118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://cg.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://bo.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ay.zhonguo8118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://la.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://lb.zhonguo4118.cn

Ruby: square = ->(x) { x * x }
来源：https://dq.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://yq.zhonguo6118.cn

[C07] 把函数作为参数传入
来源：https://gb.zhonguo5118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://gy.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://mp.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://mg.zhonguo5118.cn

TS:   arr.map(String)
来源：https://py.zhonguo1118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://ag.zhonguo8118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://fu.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://sn.zhonguo3118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ao.zhonguo3118.cn

[C08] 闭包
来源：https://uh.zhonguo5118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://cm.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://vr.zhonguo4118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://rh.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://zp.zhonguo2118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://ha.zhonguo6118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://eu.zhonguo5118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://av.zhonguo8118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://ve.zhonguo5118.cn

[C09] 递归
来源：https://zr.zhonguo7118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ks.zhonguo2118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://aj.zhonguo5118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://jb.zhonguo3118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://gp.zhonguo3118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://zf.zhonguo1118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://jh.zhonguo3118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://qo.zhonguo1118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://fk.zhonguo6118.cn

[C10] 变量作用域
来源：https://nv.zhonguo2118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://zo.zhonguo7118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ax.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://pm.zhonguo4118.cn

TS:   同 JS
来源：https://im.zhonguo5118.cn

Java: 方法内为块级作用域
来源：https://qi.zhonguo1118.cn

Go:   花括号块级作用域
来源：https://pp.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://cg.zhonguo7118.cn

C#:   块级作用域
来源：https://wv.zhonguo8118.cn

[C11] 模块导入与导出
来源：https://hz.zhonguo1118.cn

Py:   from module import func
来源：https://kc.zhonguo3118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://yu.zhonguo5118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://df.zhonguo7118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://nz.zhonguo3118.cn

Java: import java.util.List;
来源：https://fz.zhonguo3118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://na.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://ia.zhonguo6118.cn

C#:   using System.Text;
来源：https://ph.zhonguo1118.cn

[C12] 立即执行函数 IIFE
来源：https://ci.zhonguo8118.cn

Py:   (lambda: print("run"))()
来源：https://zb.zhonguo3118.cn

PHP:  (function () { echo "run"; })();
来源：https://sf.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://xb.zhonguo5118.cn

TS:   (() => { console.log("run"); })();
来源：https://nf.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://un.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://sb.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://rq.zhonguo7118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://vc.zhonguo1118.cn

[C13] 类型声明 / 类型注解
来源：https://jv.zhonguo3118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ws.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ks.zhonguo7118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://hf.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ug.zhonguo4118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://xp.zhonguo6118.cn

Go:   func add(a, b int) int
来源：https://gu.zhonguo4118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ur.zhonguo4118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://qu.zhonguo8118.cn

[C14] 泛型函数
来源：https://sn.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://gv.zhonguo3118.cn

PHP:  // 无泛型
来源：https://ay.zhonguo6118.cn

JS:   // 无泛型
来源：https://gm.zhonguo6118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://ub.zhonguo5118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://ty.zhonguo4118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://iz.zhonguo5118.cn

Ruby: # 无泛型
来源：https://iw.zhonguo3118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://wh.zhonguo1118.cn

[C15] 解构 / 展开参数
来源：https://nf.zhonguo1118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://vh.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://ft.zhonguo2118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://ft.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://mf.zhonguo8118.cn

Java: // 无解构
来源：https://xf.zhonguo4118.cn

Go:   // 无解构
来源：https://ez.zhonguo3118.cn

Ruby: a, b = pair
来源：https://ug.zhonguo2118.cn

C#:   var (a, b) = pair;
来源：https://jt.zhonguo7118.cn

[C16] 函数 / 方法重载
来源：https://vg.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ej.zhonguo2118.cn

PHP:  // 无重载
来源：https://jh.zhonguo1118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://jl.zhonguo7118.cn

TS:   // 用联合类型或重载签名声明
来源：https://ec.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ra.zhonguo8118.cn

Go:   // 无重载：用不同函数名
来源：https://fm.zhonguo6118.cn

Ruby: # 无重载：靠动态参数
来源：https://rv.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://am.zhonguo2118.cn

================================================================================
来源：https://fq.zhonguo4118.cn

D. 数组 / 列表 / 集合
来源：https://em.zhonguo4118.cn

================================================================================
来源：https://xm.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://wp.zhonguo6118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://wf.zhonguo4118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://wj.zhonguo7118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ma.zhonguo4118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://aj.zhonguo6118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://fu.zhonguo7118.cn

Go:   arr := []int{1, 2, 3}
来源：https://ym.zhonguo3118.cn

Ruby: arr = [1, 2, 3]
来源：https://at.zhonguo5118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://ie.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://gj.zhonguo8118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://vt.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://jn.zhonguo6118.cn

JS:   arr.push(4);
来源：https://qr.zhonguo1118.cn

TS:   arr.push(4);
来源：https://gr.zhonguo3118.cn

Java: list.add(4);
来源：https://qe.zhonguo7118.cn

Go:   arr = append(arr, 4)
来源：https://kq.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://ot.zhonguo6118.cn

C#:   list.Add(4);
来源：https://fp.zhonguo8118.cn

[D03] 在指定位置插入元素
来源：https://vf.zhonguo2118.cn

Py:   arr.insert(0, 0)
来源：https://kx.zhonguo8118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://ru.zhonguo6118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://cb.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://gh.zhonguo6118.cn

Java: list.add(0, 0);
来源：https://ik.zhonguo1118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://rh.zhonguo8118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://xt.zhonguo3118.cn

C#:   list.Insert(0, 0);
来源：https://nk.zhonguo6118.cn

[D04] 删除元素
来源：https://nf.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://ei.zhonguo7118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://wm.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://ew.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://wu.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://st.zhonguo2118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ci.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://oo.zhonguo3118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://rv.zhonguo1118.cn

[D05] 访问与修改元素
来源：https://zr.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://qy.zhonguo1118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://ko.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://np.zhonguo2118.cn

TS:   arr[0]; arr.at(-1);
来源：https://at.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://yd.zhonguo2118.cn

Go:   arr[0]; arr[0] = 9
来源：https://mr.zhonguo7118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://cf.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ls.zhonguo8118.cn

[D06] 数组长度
来源：https://ni.zhonguo5118.cn

Py:   len(arr)
来源：https://zc.zhonguo1118.cn

PHP:  count($arr);
来源：https://dp.zhonguo7118.cn

JS:   arr.length
来源：https://gy.zhonguo1118.cn

TS:   arr.length
来源：https://wk.zhonguo6118.cn

Java: list.size();
来源：https://gr.zhonguo2118.cn

Go:   len(arr)
来源：https://sk.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://wy.zhonguo6118.cn

C#:   list.Count;
来源：https://sv.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://dp.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://dw.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://iy.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://xx.zhonguo4118.cn


<!-- 参考信息 -->