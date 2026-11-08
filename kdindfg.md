代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://yh.zhonguo4118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://nz.zhonguo5118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://yf.zhonguo5118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://tr.zhonguo3118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://hx.zhonguo5118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://sx.zhonguo6118.cn

[B07] while 循环
来源：https://wu.zhonguo2118.cn

Py:   while i < 10: i += 1
来源：https://tp.zhonguo5118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://si.zhonguo3118.cn

JS:   while (i < 10) { i++; }
来源：https://nd.zhonguo1118.cn

TS:   while (i < 10) { i++; }
来源：https://rj.zhonguo4118.cn

Java: while (i < 10) { i++; }
来源：https://pq.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://sf.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://gu.zhonguo6118.cn

C#:   while (i < 10) { i++; }
来源：https://el.zhonguo1118.cn

[B08] do-while（至少执行一次）
来源：https://zq.zhonguo1118.cn

Py:   # 无 do-while：用 while True + break
来源：https://sq.zhonguo1118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://sb.zhonguo4118.cn

JS:   do { i++; } while (i < 10);
来源：https://pe.zhonguo2118.cn

TS:   do { i++; } while (i < 10);
来源：https://xq.zhonguo8118.cn

Java: do { i++; } while (i < 10);
来源：https://we.zhonguo7118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://wd.zhonguo8118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://pk.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://se.zhonguo7118.cn

[B09] break 与 continue
来源：https://jy.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://po.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://oh.zhonguo8118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://eb.zhonguo5118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ss.zhonguo7118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ul.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://sw.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://fs.zhonguo2118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://bc.zhonguo3118.cn

[B10] 遍历同时拿索引
来源：https://vq.zhonguo6118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://dx.zhonguo2118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://wx.zhonguo3118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://pt.zhonguo7118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://lr.zhonguo6118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://py.zhonguo2118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://jk.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://uo.zhonguo8118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://mj.zhonguo1118.cn

[B11] 生成数字序列 / 区间
来源：https://oq.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://jb.zhonguo7118.cn

PHP:  range(0, 10, 2);
来源：https://gw.zhonguo8118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://cj.zhonguo7118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://tk.zhonguo1118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ij.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://ud.zhonguo8118.cn

Ruby: (0...10).step(2).to_a
来源：https://uv.zhonguo3118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://dw.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://qb.zhonguo5118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://to.zhonguo2118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://mi.zhonguo3118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://vj.zhonguo1118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://cp.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://if.zhonguo5118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://bx.zhonguo6118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://vg.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://uq.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://uw.zhonguo3118.cn

Py:   isinstance(x, (int, float))
来源：https://hn.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://kz.zhonguo7118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vx.zhonguo1118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ej.zhonguo6118.cn

Java: x instanceof Number
来源：https://jf.zhonguo8118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ro.zhonguo5118.cn

Ruby: x.is_a?(Numeric)
来源：https://yw.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://jf.zhonguo4118.cn

[B14] 判断值是否在集合内
来源：https://nj.zhonguo6118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://lv.zhonguo8118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://al.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://bp.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://tc.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://dj.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://wc.zhonguo4118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://cw.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://by.zhonguo2118.cn

[B15] 布尔运算与取反
来源：https://xv.zhonguo2118.cn

Py:   a and b or not c
来源：https://ab.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://we.zhonguo5118.cn

JS:   a && b || !c
来源：https://qh.zhonguo5118.cn

TS:   a && b || !c
来源：https://ag.zhonguo4118.cn

Java: a && b || !c
来源：https://fl.zhonguo4118.cn

Go:   a && b || !c
来源：https://eq.zhonguo1118.cn

Ruby: a && b || !c
来源：https://fd.zhonguo3118.cn

C#:   a && b || !c
来源：https://ni.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://lf.zhonguo2118.cn

Py:   if not data: return
来源：https://am.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://zm.zhonguo4118.cn

JS:   if (!data) return;
来源：https://ob.zhonguo6118.cn

TS:   if (!data) return;
来源：https://yo.zhonguo3118.cn

Java: if (data == null) return;
来源：https://up.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://mp.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://tw.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://kp.zhonguo5118.cn

================================================================================
来源：https://ln.zhonguo3118.cn

C. 函数与作用域
来源：https://ef.zhonguo2118.cn

================================================================================
来源：https://xi.zhonguo5118.cn

[C01] 定义函数
来源：https://dl.zhonguo2118.cn

Py:   def add(a, b): return a + b
来源：https://mc.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://jv.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://jv.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://mw.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://jb.zhonguo2118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://vu.zhonguo8118.cn

Ruby: def add(a, b); a + b; end
来源：https://ub.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://pj.zhonguo2118.cn

[C02] 默认参数
来源：https://up.zhonguo4118.cn

Py:   def greet(name="World"): return name
来源：https://ti.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://um.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://bb.zhonguo8118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://sp.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://xx.zhonguo2118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://dr.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://jj.zhonguo8118.cn

C#:   string Greet(string name = "World") => name;
来源：https://my.zhonguo4118.cn

[C03] 可变参数
来源：https://jp.zhonguo1118.cn

Py:   def total(*args): return sum(args)
来源：https://pv.zhonguo8118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://xq.zhonguo8118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://ca.zhonguo8118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://un.zhonguo5118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ue.zhonguo7118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://ul.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://nq.zhonguo4118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://qw.zhonguo6118.cn

[C04] 命名参数 / 关键字参数
来源：https://nj.zhonguo1118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://fw.zhonguo6118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://zb.zhonguo6118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://nt.zhonguo1118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://mr.zhonguo4118.cn

Java: // 无：用 Builder 模式或 record
来源：https://xc.zhonguo5118.cn

Go:   // 无：用配置结构体参数
来源：https://hs.zhonguo3118.cn

Ruby: f(a: 1, b: 2)
来源：https://vp.zhonguo1118.cn

C#:   f(a: 1, b: 2)
来源：https://wn.zhonguo2118.cn

[C05] 返回多个值
来源：https://lz.zhonguo8118.cn

Py:   return a, b
来源：https://ge.zhonguo4118.cn

PHP:  return [$a, $b];
来源：https://pg.zhonguo1118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://ha.zhonguo5118.cn

TS:   return { a, b };
来源：https://sl.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://gp.zhonguo1118.cn

Go:   return a, b
来源：https://sg.zhonguo7118.cn

Ruby: return a, b
来源：https://hx.zhonguo1118.cn

C#:   return (a, b);              // ValueTuple
来源：https://bl.zhonguo4118.cn

[C06] 匿名函数 / lambda
来源：https://da.zhonguo7118.cn

Py:   square = lambda x: x * x
来源：https://pe.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://ws.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://gq.zhonguo7118.cn

TS:   const square = (x: number): number => x * x;
来源：https://yf.zhonguo4118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://zw.zhonguo8118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://jg.zhonguo8118.cn

Ruby: square = ->(x) { x * x }
来源：https://lz.zhonguo4118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://uy.zhonguo8118.cn

[C07] 把函数作为参数传入
来源：https://iu.zhonguo4118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://br.zhonguo7118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://bo.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://wn.zhonguo6118.cn

TS:   arr.map(String)
来源：https://yh.zhonguo2118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://gc.zhonguo1118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://bc.zhonguo8118.cn

Ruby: arr.map(&:upcase)
来源：https://vb.zhonguo3118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://sk.zhonguo3118.cn

[C08] 闭包
来源：https://tj.zhonguo3118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ur.zhonguo8118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://mi.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://gm.zhonguo4118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://hk.zhonguo3118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://vi.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://dj.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://vs.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://ej.zhonguo3118.cn

[C09] 递归
来源：https://wu.zhonguo7118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ee.zhonguo6118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://ns.zhonguo2118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://rc.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://ns.zhonguo2118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://kj.zhonguo7118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://vt.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://vy.zhonguo8118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://mf.zhonguo5118.cn

[C10] 变量作用域
来源：https://nk.zhonguo3118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://pk.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://wu.zhonguo3118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://gc.zhonguo1118.cn

TS:   同 JS
来源：https://dq.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://bo.zhonguo2118.cn

Go:   花括号块级作用域
来源：https://sb.zhonguo5118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://hb.zhonguo6118.cn

C#:   块级作用域
来源：https://pn.zhonguo7118.cn

[C11] 模块导入与导出
来源：https://lj.zhonguo3118.cn

Py:   from module import func
来源：https://iw.zhonguo7118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://zn.zhonguo2118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://qe.zhonguo4118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://xv.zhonguo7118.cn

Java: import java.util.List;
来源：https://ew.zhonguo1118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://xy.zhonguo3118.cn

Ruby: require "json"; require_relative "./util"
来源：https://da.zhonguo8118.cn

C#:   using System.Text;
来源：https://hl.zhonguo1118.cn

[C12] 立即执行函数 IIFE
来源：https://sk.zhonguo3118.cn

Py:   (lambda: print("run"))()
来源：https://of.zhonguo4118.cn

PHP:  (function () { echo "run"; })();
来源：https://hv.zhonguo2118.cn

JS:   (() => { console.log("run"); })();
来源：https://xh.zhonguo4118.cn

TS:   (() => { console.log("run"); })();
来源：https://lo.zhonguo7118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://vs.zhonguo4118.cn

Go:   func() { fmt.Println("run") }()
来源：https://hs.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://at.zhonguo1118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://tv.zhonguo4118.cn

[C13] 类型声明 / 类型注解
来源：https://mj.zhonguo7118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://nq.zhonguo4118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://bo.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://xd.zhonguo3118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://es.zhonguo6118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://yh.zhonguo7118.cn

Go:   func add(a, b int) int
来源：https://nb.zhonguo2118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ai.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://es.zhonguo7118.cn

[C14] 泛型函数
来源：https://sf.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://wp.zhonguo2118.cn

PHP:  // 无泛型
来源：https://cq.zhonguo5118.cn

JS:   // 无泛型
来源：https://ms.zhonguo6118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://iv.zhonguo4118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://xc.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://wn.zhonguo1118.cn

Ruby: # 无泛型
来源：https://lq.zhonguo2118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://uv.zhonguo4118.cn

[C15] 解构 / 展开参数
来源：https://vq.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://nr.zhonguo6118.cn

PHP:  [$a, $b] = $pair;
来源：https://td.zhonguo5118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://bf.zhonguo3118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://lt.zhonguo6118.cn

Java: // 无解构
来源：https://dk.zhonguo6118.cn

Go:   // 无解构
来源：https://qd.zhonguo4118.cn

Ruby: a, b = pair
来源：https://wt.zhonguo5118.cn

C#:   var (a, b) = pair;
来源：https://ik.zhonguo1118.cn

[C16] 函数 / 方法重载
来源：https://el.zhonguo6118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://by.zhonguo8118.cn

PHP:  // 无重载
来源：https://zk.zhonguo6118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ky.zhonguo3118.cn

TS:   // 用联合类型或重载签名声明
来源：https://cr.zhonguo3118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ki.zhonguo1118.cn

Go:   // 无重载：用不同函数名
来源：https://ou.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://ui.zhonguo7118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://ob.zhonguo4118.cn

================================================================================
来源：https://ha.zhonguo4118.cn

D. 数组 / 列表 / 集合
来源：https://uk.zhonguo8118.cn

================================================================================
来源：https://rg.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://lu.zhonguo5118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://wc.zhonguo4118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://nn.zhonguo1118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://iz.zhonguo5118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://cd.zhonguo8118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ib.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://kf.zhonguo4118.cn

Ruby: arr = [1, 2, 3]
来源：https://wk.zhonguo5118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://qf.zhonguo1118.cn

[D02] 追加元素到末尾
来源：https://yf.zhonguo2118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://fq.zhonguo3118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://vw.zhonguo2118.cn

JS:   arr.push(4);
来源：https://on.zhonguo5118.cn

TS:   arr.push(4);
来源：https://fh.zhonguo7118.cn

Java: list.add(4);
来源：https://ij.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://nr.zhonguo1118.cn

Ruby: arr << 4; arr.push(5)
来源：https://pd.zhonguo1118.cn

C#:   list.Add(4);
来源：https://bm.zhonguo2118.cn

[D03] 在指定位置插入元素
来源：https://dn.zhonguo1118.cn

Py:   arr.insert(0, 0)
来源：https://hr.zhonguo5118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://tj.zhonguo3118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://sz.zhonguo4118.cn

TS:   arr.splice(0, 0, 0);
来源：https://pk.zhonguo2118.cn

Java: list.add(0, 0);
来源：https://dz.zhonguo8118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://dp.zhonguo1118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://pb.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://id.zhonguo3118.cn

[D04] 删除元素
来源：https://iv.zhonguo8118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://cm.zhonguo7118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://rl.zhonguo7118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://zc.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://xx.zhonguo6118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://jn.zhonguo6118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://vk.zhonguo1118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://qz.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://tk.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://vn.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://my.zhonguo5118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://qg.zhonguo4118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://ga.zhonguo8118.cn

TS:   arr[0]; arr.at(-1);
来源：https://jp.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://vj.zhonguo3118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ts.zhonguo2118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://uz.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://au.zhonguo1118.cn

[D06] 数组长度
来源：https://ui.zhonguo8118.cn

Py:   len(arr)
来源：https://tx.zhonguo8118.cn

PHP:  count($arr);
来源：https://cw.zhonguo5118.cn

JS:   arr.length
来源：https://sf.zhonguo7118.cn

TS:   arr.length
来源：https://kx.zhonguo6118.cn

Java: list.size();
来源：https://hm.zhonguo3118.cn

Go:   len(arr)
来源：https://kd.zhonguo3118.cn

Ruby: arr.length; arr.size
来源：https://el.zhonguo7118.cn

C#:   list.Count;
来源：https://tw.zhonguo5118.cn


<!-- 参考信息 -->