代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：https://ja.zhonguo5118.cn

JS:   while (i < 10) { i++; }
来源：https://ul.zhonguo2118.cn

TS:   while (i < 10) { i++; }
来源：https://vx.zhonguo3118.cn

Java: while (i < 10) { i++; }
来源：https://ux.zhonguo8118.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://us.zhonguo1118.cn

Ruby: while i < 10; i += 1; end
来源：https://tv.zhonguo5118.cn

C#:   while (i < 10) { i++; }
来源：https://aw.zhonguo5118.cn

[B08] do-while（至少执行一次）
来源：https://wf.zhonguo2118.cn

Py:   # 无 do-while：用 while True + break
来源：https://gs.zhonguo7118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://cd.zhonguo5118.cn

JS:   do { i++; } while (i < 10);
来源：https://qu.zhonguo1118.cn

TS:   do { i++; } while (i < 10);
来源：https://ol.zhonguo4118.cn

Java: do { i++; } while (i < 10);
来源：https://ft.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://qm.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://lx.zhonguo8118.cn

C#:   do { i++; } while (i < 10);
来源：https://ff.zhonguo4118.cn

[B09] break 与 continue
来源：https://wr.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://xq.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://xh.zhonguo7118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yo.zhonguo2118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://di.zhonguo3118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://nx.zhonguo1118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://nn.zhonguo3118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://li.zhonguo3118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://po.zhonguo4118.cn

[B10] 遍历同时拿索引
来源：https://ym.zhonguo1118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ca.zhonguo4118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://dj.zhonguo4118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://vi.zhonguo5118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://nq.zhonguo6118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://xc.zhonguo3118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://tn.zhonguo1118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://nv.zhonguo7118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://tu.zhonguo7118.cn

[B11] 生成数字序列 / 区间
来源：https://it.zhonguo4118.cn

Py:   list(range(0, 10, 2))
来源：https://pk.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://pm.zhonguo4118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ei.zhonguo5118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://kd.zhonguo6118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://df.zhonguo1118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://ut.zhonguo6118.cn

Ruby: (0...10).step(2).to_a
来源：https://md.zhonguo6118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://bu.zhonguo1118.cn

[B12] 跳出多层循环
来源：https://pc.zhonguo8118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://bl.zhonguo1118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://eg.zhonguo4118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://xe.zhonguo6118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://mk.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://ia.zhonguo4118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://mu.zhonguo1118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://pg.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://bm.zhonguo7118.cn

[B13] 判断是否为数字
来源：https://ha.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://db.zhonguo8118.cn

PHP:  is_numeric($x)
来源：https://sp.zhonguo2118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ld.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vk.zhonguo3118.cn

Java: x instanceof Number
来源：https://gw.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://jb.zhonguo7118.cn

Ruby: x.is_a?(Numeric)
来源：https://ft.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://po.zhonguo6118.cn

[B14] 判断值是否在集合内
来源：https://nj.zhonguo4118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://dt.zhonguo8118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://ab.zhonguo7118.cn

JS:   [1, 2, 3].includes(x)
来源：https://on.zhonguo6118.cn

TS:   [1, 2, 3].includes(x)
来源：https://bv.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://lf.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://lh.zhonguo5118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://yp.zhonguo5118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://ir.zhonguo7118.cn

[B15] 布尔运算与取反
来源：https://yq.zhonguo7118.cn

Py:   a and b or not c
来源：https://vq.zhonguo3118.cn

PHP:  $a && $b || !$c
来源：https://fo.zhonguo4118.cn

JS:   a && b || !c
来源：https://iy.zhonguo3118.cn

TS:   a && b || !c
来源：https://cw.zhonguo3118.cn

Java: a && b || !c
来源：https://sr.zhonguo1118.cn

Go:   a && b || !c
来源：https://wh.zhonguo6118.cn

Ruby: a && b || !c
来源：https://da.zhonguo1118.cn

C#:   a && b || !c
来源：https://op.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://qm.zhonguo2118.cn

Py:   if not data: return
来源：https://wf.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://ke.zhonguo3118.cn

JS:   if (!data) return;
来源：https://kz.zhonguo7118.cn

TS:   if (!data) return;
来源：https://ee.zhonguo1118.cn

Java: if (data == null) return;
来源：https://gz.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://hv.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://gb.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://zo.zhonguo8118.cn

================================================================================
来源：https://zp.zhonguo1118.cn

C. 函数与作用域
来源：https://ki.zhonguo8118.cn

================================================================================
来源：https://ti.zhonguo6118.cn

[C01] 定义函数
来源：https://fg.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://mc.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qe.zhonguo8118.cn

JS:   function add(a, b) { return a + b; }
来源：https://sb.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://jf.zhonguo5118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://yq.zhonguo7118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://wj.zhonguo7118.cn

Ruby: def add(a, b); a + b; end
来源：https://sw.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://co.zhonguo1118.cn

[C02] 默认参数
来源：https://jb.zhonguo1118.cn

Py:   def greet(name="World"): return name
来源：https://nt.zhonguo7118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://ce.zhonguo5118.cn

JS:   function greet(name = "World") { return name; }
来源：https://tg.zhonguo4118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://le.zhonguo3118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://ds.zhonguo1118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://um.zhonguo6118.cn

Ruby: def greet(name = "World") = name
来源：https://da.zhonguo4118.cn

C#:   string Greet(string name = "World") => name;
来源：https://yx.zhonguo6118.cn

[C03] 可变参数
来源：https://zn.zhonguo6118.cn

Py:   def total(*args): return sum(args)
来源：https://io.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://bp.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://qw.zhonguo6118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://pb.zhonguo5118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://wu.zhonguo2118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://hj.zhonguo3118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://mm.zhonguo5118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://xd.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://xl.zhonguo8118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ib.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://jt.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://ea.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://fa.zhonguo7118.cn

Java: // 无：用 Builder 模式或 record
来源：https://zq.zhonguo5118.cn

Go:   // 无：用配置结构体参数
来源：https://jo.zhonguo6118.cn

Ruby: f(a: 1, b: 2)
来源：https://xq.zhonguo5118.cn

C#:   f(a: 1, b: 2)
来源：https://lt.zhonguo8118.cn

[C05] 返回多个值
来源：https://eu.zhonguo2118.cn

Py:   return a, b
来源：https://tg.zhonguo3118.cn

PHP:  return [$a, $b];
来源：https://gy.zhonguo7118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://sm.zhonguo8118.cn

TS:   return { a, b };
来源：https://xs.zhonguo3118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ye.zhonguo7118.cn

Go:   return a, b
来源：https://rm.zhonguo5118.cn

Ruby: return a, b
来源：https://ma.zhonguo2118.cn

C#:   return (a, b);              // ValueTuple
来源：https://kl.zhonguo7118.cn

[C06] 匿名函数 / lambda
来源：https://zs.zhonguo1118.cn

Py:   square = lambda x: x * x
来源：https://zx.zhonguo6118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://gd.zhonguo8118.cn

JS:   const square = x => x * x;
来源：https://au.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://iq.zhonguo5118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://tq.zhonguo7118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://mg.zhonguo5118.cn

Ruby: square = ->(x) { x * x }
来源：https://es.zhonguo2118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://nl.zhonguo1118.cn

[C07] 把函数作为参数传入
来源：https://cw.zhonguo8118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://tt.zhonguo4118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://ub.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://tp.zhonguo8118.cn

TS:   arr.map(String)
来源：https://nl.zhonguo3118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://cg.zhonguo4118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://cc.zhonguo4118.cn

Ruby: arr.map(&:upcase)
来源：https://ta.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ec.zhonguo4118.cn

[C08] 闭包
来源：https://ki.zhonguo3118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://pj.zhonguo5118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://uf.zhonguo6118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://rm.zhonguo3118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://tx.zhonguo5118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://lg.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://ee.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://rf.zhonguo3118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://is.zhonguo4118.cn

[C09] 递归
来源：https://ti.zhonguo4118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://id.zhonguo5118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://tk.zhonguo6118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://nm.zhonguo1118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://yn.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://xl.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://nl.zhonguo6118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://gh.zhonguo4118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://yg.zhonguo2118.cn

[C10] 变量作用域
来源：https://ho.zhonguo4118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ti.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://cy.zhonguo4118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://hy.zhonguo1118.cn

TS:   同 JS
来源：https://es.zhonguo8118.cn

Java: 方法内为块级作用域
来源：https://ce.zhonguo2118.cn

Go:   花括号块级作用域
来源：https://lw.zhonguo4118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://if.zhonguo1118.cn

C#:   块级作用域
来源：https://mx.zhonguo6118.cn

[C11] 模块导入与导出
来源：https://oc.zhonguo1118.cn

Py:   from module import func
来源：https://uq.zhonguo6118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://cp.zhonguo1118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://wp.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://ny.zhonguo6118.cn

Java: import java.util.List;
来源：https://vz.zhonguo6118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://vt.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://nw.zhonguo6118.cn

C#:   using System.Text;
来源：https://kh.zhonguo5118.cn

[C12] 立即执行函数 IIFE
来源：https://jz.zhonguo2118.cn

Py:   (lambda: print("run"))()
来源：https://dx.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://ua.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://kp.zhonguo5118.cn

TS:   (() => { console.log("run"); })();
来源：https://hq.zhonguo4118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ck.zhonguo2118.cn

Go:   func() { fmt.Println("run") }()
来源：https://hg.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://kj.zhonguo6118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://jf.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://wc.zhonguo8118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://uw.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://pn.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://jn.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://vm.zhonguo1118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://lp.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://ig.zhonguo3118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ok.zhonguo2118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://yv.zhonguo8118.cn

[C14] 泛型函数
来源：https://jr.zhonguo5118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://fu.zhonguo1118.cn

PHP:  // 无泛型
来源：https://iu.zhonguo7118.cn

JS:   // 无泛型
来源：https://ge.zhonguo2118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://ae.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://yd.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://qh.zhonguo3118.cn

Ruby: # 无泛型
来源：https://yc.zhonguo3118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://me.zhonguo1118.cn

[C15] 解构 / 展开参数
来源：https://vn.zhonguo5118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://rx.zhonguo2118.cn

PHP:  [$a, $b] = $pair;
来源：https://pj.zhonguo4118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://lt.zhonguo4118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://cx.zhonguo7118.cn

Java: // 无解构
来源：https://td.zhonguo8118.cn

Go:   // 无解构
来源：https://as.zhonguo5118.cn

Ruby: a, b = pair
来源：https://ou.zhonguo1118.cn

C#:   var (a, b) = pair;
来源：https://jz.zhonguo7118.cn

[C16] 函数 / 方法重载
来源：https://gf.zhonguo7118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://xf.zhonguo7118.cn

PHP:  // 无重载
来源：https://rb.zhonguo6118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ch.zhonguo5118.cn

TS:   // 用联合类型或重载签名声明
来源：https://qd.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ap.zhonguo3118.cn

Go:   // 无重载：用不同函数名
来源：https://hp.zhonguo4118.cn

Ruby: # 无重载：靠动态参数
来源：https://rl.zhonguo3118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://qx.zhonguo7118.cn

================================================================================
来源：https://gf.zhonguo7118.cn

D. 数组 / 列表 / 集合
来源：https://cl.zhonguo8118.cn

================================================================================
来源：https://ti.zhonguo2118.cn

[D01] 创建数组 / 列表
来源：https://bo.zhonguo8118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://ma.zhonguo4118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://cz.zhonguo7118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://su.zhonguo6118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://by.zhonguo8118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ly.zhonguo6118.cn

Go:   arr := []int{1, 2, 3}
来源：https://bv.zhonguo3118.cn

Ruby: arr = [1, 2, 3]
来源：https://gi.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://wc.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://tl.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://tq.zhonguo8118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ac.zhonguo1118.cn

JS:   arr.push(4);
来源：https://zr.zhonguo3118.cn

TS:   arr.push(4);
来源：https://af.zhonguo2118.cn

Java: list.add(4);
来源：https://zu.zhonguo3118.cn

Go:   arr = append(arr, 4)
来源：https://rv.zhonguo7118.cn

Ruby: arr << 4; arr.push(5)
来源：https://pc.zhonguo7118.cn

C#:   list.Add(4);
来源：https://vs.zhonguo3118.cn

[D03] 在指定位置插入元素
来源：https://uu.zhonguo6118.cn

Py:   arr.insert(0, 0)
来源：https://wa.zhonguo3118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://qj.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://vv.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://ie.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://lk.zhonguo1118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://cg.zhonguo5118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://hn.zhonguo6118.cn

C#:   list.Insert(0, 0);
来源：https://fg.zhonguo2118.cn

[D04] 删除元素
来源：https://xq.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://bm.zhonguo8118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://dt.zhonguo3118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://zt.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://co.zhonguo2118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ru.zhonguo5118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://jv.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ml.zhonguo1118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://qx.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://hh.zhonguo4118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ca.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://cw.zhonguo1118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://jl.zhonguo8118.cn

TS:   arr[0]; arr.at(-1);
来源：https://pq.zhonguo3118.cn

Java: list.get(0); list.set(0, 9);
来源：https://tr.zhonguo7118.cn

Go:   arr[0]; arr[0] = 9
来源：https://lk.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://go.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://mq.zhonguo2118.cn

[D06] 数组长度
来源：https://pu.zhonguo1118.cn

Py:   len(arr)
来源：https://zt.zhonguo7118.cn

PHP:  count($arr);
来源：https://rc.zhonguo3118.cn

JS:   arr.length
来源：https://rs.zhonguo8118.cn

TS:   arr.length
来源：https://wg.zhonguo2118.cn

Java: list.size();
来源：https://tt.zhonguo4118.cn

Go:   len(arr)
来源：https://sl.zhonguo1118.cn

Ruby: arr.length; arr.size
来源：https://yb.zhonguo7118.cn

C#:   list.Count;
来源：https://dn.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://cj.zhonguo7118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://mp.zhonguo4118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://mp.zhonguo5118.cn

JS:   arr.slice(1, 4);
来源：https://ep.zhonguo3118.cn

TS:   arr.slice(1, 4);
来源：https://tj.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://nx.zhonguo1118.cn

Go:   arr[1:4]
来源：https://xu.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://ya.zhonguo1118.cn


<!-- 参考信息 -->