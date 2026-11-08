代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：https://vy.zhonguo8118.cn

[B06] 遍历字典 / 对象
来源：https://kk.zhonguo3118.cn

Py:   for k, v in d.items(): print(k, v)
来源：https://az.zhonguo2118.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：https://rs.zhonguo3118.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://jm.zhonguo6118.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：https://om.zhonguo4118.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：https://ec.zhonguo4118.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：https://ph.zhonguo7118.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：https://zi.zhonguo8118.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：https://ly.zhonguo4118.cn

[B07] while 循环
来源：https://nx.zhonguo1118.cn

Py:   while i < 10: i += 1
来源：https://ua.zhonguo4118.cn

PHP:  while ($i < 10) { $i++; }
来源：https://tc.zhonguo4118.cn

JS:   while (i < 10) { i++; }
来源：https://gw.zhonguo6118.cn

TS:   while (i < 10) { i++; }
来源：https://ej.zhonguo8118.cn

Java: while (i < 10) { i++; }
来源：https://ej.zhonguo6118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://yo.zhonguo8118.cn

Ruby: while i < 10; i += 1; end
来源：https://zn.zhonguo8118.cn

C#:   while (i < 10) { i++; }
来源：https://lo.zhonguo6118.cn

[B08] do-while（至少执行一次）
来源：https://ll.zhonguo1118.cn

Py:   # 无 do-while：用 while True + break
来源：https://co.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://jt.zhonguo4118.cn

JS:   do { i++; } while (i < 10);
来源：https://ge.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://hm.zhonguo2118.cn

Java: do { i++; } while (i < 10);
来源：https://vf.zhonguo2118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://ls.zhonguo4118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://vj.zhonguo3118.cn

C#:   do { i++; } while (i < 10);
来源：https://wp.zhonguo2118.cn

[B09] break 与 continue
来源：https://eg.zhonguo8118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://mq.zhonguo7118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://qy.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fi.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fj.zhonguo5118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://wo.zhonguo7118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://pa.zhonguo6118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://ts.zhonguo4118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ys.zhonguo5118.cn

[B10] 遍历同时拿索引
来源：https://sr.zhonguo5118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ep.zhonguo3118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://aa.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://dw.zhonguo7118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://no.zhonguo5118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://zo.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://if.zhonguo8118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://xi.zhonguo5118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://eb.zhonguo6118.cn

[B11] 生成数字序列 / 区间
来源：https://na.zhonguo2118.cn

Py:   list(range(0, 10, 2))
来源：https://zp.zhonguo4118.cn

PHP:  range(0, 10, 2);
来源：https://fb.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://nj.zhonguo3118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://vi.zhonguo6118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://db.zhonguo7118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://sy.zhonguo5118.cn

Ruby: (0...10).step(2).to_a
来源：https://er.zhonguo7118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://cq.zhonguo8118.cn

[B12] 跳出多层循环
来源：https://aq.zhonguo4118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://cz.zhonguo2118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://ht.zhonguo6118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://jl.zhonguo2118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://xw.zhonguo2118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://kr.zhonguo4118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://uz.zhonguo1118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://vg.zhonguo1118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://wm.zhonguo8118.cn

[B13] 判断是否为数字
来源：https://nm.zhonguo8118.cn

Py:   isinstance(x, (int, float))
来源：https://nz.zhonguo1118.cn

PHP:  is_numeric($x)
来源：https://ne.zhonguo8118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ji.zhonguo4118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://pe.zhonguo7118.cn

Java: x instanceof Number
来源：https://xj.zhonguo5118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://zq.zhonguo7118.cn

Ruby: x.is_a?(Numeric)
来源：https://dz.zhonguo7118.cn

C#:   x is int or double or decimal
来源：https://ss.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://nl.zhonguo2118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://hj.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ku.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ll.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://fn.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://yh.zhonguo1118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://cq.zhonguo1118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://md.zhonguo3118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://rr.zhonguo8118.cn

[B15] 布尔运算与取反
来源：https://zg.zhonguo8118.cn

Py:   a and b or not c
来源：https://jd.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://qr.zhonguo8118.cn

JS:   a && b || !c
来源：https://of.zhonguo7118.cn

TS:   a && b || !c
来源：https://zb.zhonguo7118.cn

Java: a && b || !c
来源：https://uy.zhonguo7118.cn

Go:   a && b || !c
来源：https://hc.zhonguo1118.cn

Ruby: a && b || !c
来源：https://zx.zhonguo3118.cn

C#:   a && b || !c
来源：https://mf.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://cs.zhonguo3118.cn

Py:   if not data: return
来源：https://dj.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://qx.zhonguo3118.cn

JS:   if (!data) return;
来源：https://hu.zhonguo6118.cn

TS:   if (!data) return;
来源：https://uc.zhonguo6118.cn

Java: if (data == null) return;
来源：https://hq.zhonguo7118.cn

Go:   if data == nil { return }
来源：https://cc.zhonguo6118.cn

Ruby: return if data.nil?
来源：https://lw.zhonguo3118.cn

C#:   if (data == null) return;
来源：https://os.zhonguo7118.cn

================================================================================
来源：https://bg.zhonguo2118.cn

C. 函数与作用域
来源：https://mj.zhonguo6118.cn

================================================================================
来源：https://yu.zhonguo7118.cn

[C01] 定义函数
来源：https://tu.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://qk.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://df.zhonguo8118.cn

JS:   function add(a, b) { return a + b; }
来源：https://aq.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://vs.zhonguo7118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://wx.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://ng.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://hh.zhonguo1118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ig.zhonguo1118.cn

[C02] 默认参数
来源：https://np.zhonguo8118.cn

Py:   def greet(name="World"): return name
来源：https://ep.zhonguo3118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://gs.zhonguo7118.cn

JS:   function greet(name = "World") { return name; }
来源：https://rf.zhonguo7118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://yc.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://mw.zhonguo3118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://kb.zhonguo8118.cn

Ruby: def greet(name = "World") = name
来源：https://ba.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://cv.zhonguo2118.cn

[C03] 可变参数
来源：https://ra.zhonguo5118.cn

Py:   def total(*args): return sum(args)
来源：https://pw.zhonguo4118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://bj.zhonguo8118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://eq.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://yb.zhonguo2118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://wf.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://qd.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://vh.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://wc.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://jj.zhonguo4118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ss.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://qd.zhonguo8118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://pw.zhonguo3118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://bu.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://bs.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://vt.zhonguo2118.cn

Ruby: f(a: 1, b: 2)
来源：https://mc.zhonguo4118.cn

C#:   f(a: 1, b: 2)
来源：https://wj.zhonguo4118.cn

[C05] 返回多个值
来源：https://ll.zhonguo6118.cn

Py:   return a, b
来源：https://lo.zhonguo4118.cn

PHP:  return [$a, $b];
来源：https://he.zhonguo3118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://km.zhonguo3118.cn

TS:   return { a, b };
来源：https://vd.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://qc.zhonguo1118.cn

Go:   return a, b
来源：https://rz.zhonguo5118.cn

Ruby: return a, b
来源：https://mq.zhonguo1118.cn

C#:   return (a, b);              // ValueTuple
来源：https://hv.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://ks.zhonguo5118.cn

Py:   square = lambda x: x * x
来源：https://mq.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://dh.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://sw.zhonguo2118.cn

TS:   const square = (x: number): number => x * x;
来源：https://jy.zhonguo8118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://lf.zhonguo8118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://oe.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://ku.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://eb.zhonguo1118.cn

[C07] 把函数作为参数传入
来源：https://ka.zhonguo7118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://sn.zhonguo3118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://eu.zhonguo6118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://bp.zhonguo8118.cn

TS:   arr.map(String)
来源：https://vq.zhonguo2118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://jj.zhonguo1118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://pj.zhonguo7118.cn

Ruby: arr.map(&:upcase)
来源：https://xm.zhonguo6118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://gv.zhonguo5118.cn

[C08] 闭包
来源：https://lw.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://au.zhonguo3118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://tc.zhonguo1118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://xe.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://vg.zhonguo2118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://ld.zhonguo3118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://dn.zhonguo6118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://rt.zhonguo7118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://xa.zhonguo6118.cn

[C09] 递归
来源：https://ka.zhonguo2118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://vp.zhonguo6118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://vy.zhonguo8118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://qo.zhonguo6118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://tf.zhonguo4118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://po.zhonguo2118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://kb.zhonguo1118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://zp.zhonguo1118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://ku.zhonguo2118.cn

[C10] 变量作用域
来源：https://bw.zhonguo5118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://sv.zhonguo2118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://lf.zhonguo2118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://yi.zhonguo3118.cn

TS:   同 JS
来源：https://cj.zhonguo6118.cn

Java: 方法内为块级作用域
来源：https://xu.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://yd.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://ia.zhonguo8118.cn

C#:   块级作用域
来源：https://kj.zhonguo7118.cn

[C11] 模块导入与导出
来源：https://uv.zhonguo4118.cn

Py:   from module import func
来源：https://hf.zhonguo2118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://gs.zhonguo2118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://kj.zhonguo4118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://sd.zhonguo4118.cn

Java: import java.util.List;
来源：https://ym.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://cf.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://jt.zhonguo7118.cn

C#:   using System.Text;
来源：https://oz.zhonguo8118.cn

[C12] 立即执行函数 IIFE
来源：https://gc.zhonguo2118.cn

Py:   (lambda: print("run"))()
来源：https://qq.zhonguo2118.cn

PHP:  (function () { echo "run"; })();
来源：https://fc.zhonguo2118.cn

JS:   (() => { console.log("run"); })();
来源：https://cs.zhonguo3118.cn

TS:   (() => { console.log("run"); })();
来源：https://uw.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://wb.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://df.zhonguo7118.cn

Ruby: -> { puts "run" }.call
来源：https://hp.zhonguo1118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://wg.zhonguo7118.cn

[C13] 类型声明 / 类型注解
来源：https://zn.zhonguo6118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://op.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://bj.zhonguo1118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://pu.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://no.zhonguo7118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://tw.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://cg.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://nn.zhonguo5118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://yy.zhonguo4118.cn

[C14] 泛型函数
来源：https://fa.zhonguo8118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://po.zhonguo1118.cn

PHP:  // 无泛型
来源：https://ox.zhonguo5118.cn

JS:   // 无泛型
来源：https://uo.zhonguo5118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://om.zhonguo7118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://to.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ug.zhonguo7118.cn

Ruby: # 无泛型
来源：https://za.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://oj.zhonguo8118.cn

[C15] 解构 / 展开参数
来源：https://as.zhonguo5118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://vw.zhonguo4118.cn

PHP:  [$a, $b] = $pair;
来源：https://xi.zhonguo4118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://jv.zhonguo2118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ve.zhonguo7118.cn

Java: // 无解构
来源：https://vd.zhonguo5118.cn

Go:   // 无解构
来源：https://fk.zhonguo5118.cn

Ruby: a, b = pair
来源：https://qd.zhonguo3118.cn

C#:   var (a, b) = pair;
来源：https://ok.zhonguo3118.cn

[C16] 函数 / 方法重载
来源：https://sc.zhonguo2118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://yu.zhonguo3118.cn

PHP:  // 无重载
来源：https://lv.zhonguo4118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://oa.zhonguo5118.cn

TS:   // 用联合类型或重载签名声明
来源：https://gm.zhonguo5118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ci.zhonguo8118.cn

Go:   // 无重载：用不同函数名
来源：https://ci.zhonguo4118.cn

Ruby: # 无重载：靠动态参数
来源：https://iq.zhonguo4118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://os.zhonguo1118.cn

================================================================================
来源：https://ds.zhonguo4118.cn

D. 数组 / 列表 / 集合
来源：https://nz.zhonguo1118.cn

================================================================================
来源：https://ac.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://rd.zhonguo7118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://ol.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://kp.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://tk.zhonguo3118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://pn.zhonguo1118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ue.zhonguo5118.cn

Go:   arr := []int{1, 2, 3}
来源：https://nr.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://rs.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://im.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://qn.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://pu.zhonguo8118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ag.zhonguo6118.cn

JS:   arr.push(4);
来源：https://lp.zhonguo6118.cn

TS:   arr.push(4);
来源：https://om.zhonguo3118.cn

Java: list.add(4);
来源：https://uw.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://oi.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://in.zhonguo1118.cn

C#:   list.Add(4);
来源：https://bi.zhonguo1118.cn

[D03] 在指定位置插入元素
来源：https://wt.zhonguo3118.cn

Py:   arr.insert(0, 0)
来源：https://qk.zhonguo7118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://rt.zhonguo1118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://be.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://za.zhonguo4118.cn

Java: list.add(0, 0);
来源：https://lw.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://eh.zhonguo3118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://kv.zhonguo7118.cn

C#:   list.Insert(0, 0);
来源：https://uc.zhonguo1118.cn

[D04] 删除元素
来源：https://bz.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://iq.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://uc.zhonguo4118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://mu.zhonguo2118.cn

TS:   arr.splice(0, 1);
来源：https://wr.zhonguo4118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://dd.zhonguo2118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://eg.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://nh.zhonguo3118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://vm.zhonguo4118.cn

[D05] 访问与修改元素
来源：https://dn.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://nw.zhonguo8118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://fh.zhonguo1118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://qq.zhonguo2118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ie.zhonguo4118.cn

Java: list.get(0); list.set(0, 9);
来源：https://vd.zhonguo6118.cn

Go:   arr[0]; arr[0] = 9
来源：https://df.zhonguo1118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://kh.zhonguo2118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://wv.zhonguo5118.cn

[D06] 数组长度
来源：https://ly.zhonguo8118.cn

Py:   len(arr)
来源：https://gu.zhonguo5118.cn

PHP:  count($arr);
来源：https://fj.zhonguo7118.cn

JS:   arr.length
来源：https://ko.zhonguo8118.cn

TS:   arr.length
来源：https://dg.zhonguo5118.cn


<!-- 参考信息 -->