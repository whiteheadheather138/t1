代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：https://gz.zhonguo7118.cn

Ruby: while i < 10; i += 1; end
来源：https://ro.zhonguo3118.cn

C#:   while (i < 10) { i++; }
来源：https://uz.zhonguo2118.cn

[B08] do-while（至少执行一次）
来源：https://ot.zhonguo8118.cn

Py:   # 无 do-while：用 while True + break
来源：https://uh.zhonguo5118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://pm.zhonguo2118.cn

JS:   do { i++; } while (i < 10);
来源：https://jt.zhonguo8118.cn

TS:   do { i++; } while (i < 10);
来源：https://oq.zhonguo1118.cn

Java: do { i++; } while (i < 10);
来源：https://bp.zhonguo3118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://uz.zhonguo3118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://ff.zhonguo7118.cn

C#:   do { i++; } while (i < 10);
来源：https://up.zhonguo6118.cn

[B09] break 与 continue
来源：https://hr.zhonguo4118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://xc.zhonguo4118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://mz.zhonguo5118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ib.zhonguo1118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ss.zhonguo5118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://pl.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://ez.zhonguo2118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://qw.zhonguo8118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://fo.zhonguo8118.cn

[B10] 遍历同时拿索引
来源：https://pv.zhonguo5118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://th.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://ks.zhonguo1118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://vr.zhonguo8118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ps.zhonguo7118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://sw.zhonguo3118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://ey.zhonguo7118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://sk.zhonguo4118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://mp.zhonguo7118.cn

[B11] 生成数字序列 / 区间
来源：https://tb.zhonguo6118.cn

Py:   list(range(0, 10, 2))
来源：https://ys.zhonguo6118.cn

PHP:  range(0, 10, 2);
来源：https://pu.zhonguo1118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://qn.zhonguo6118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://vd.zhonguo7118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://vu.zhonguo3118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://wi.zhonguo1118.cn

Ruby: (0...10).step(2).to_a
来源：https://bg.zhonguo4118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://go.zhonguo5118.cn

[B12] 跳出多层循环
来源：https://ad.zhonguo1118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://mx.zhonguo7118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://yc.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://dw.zhonguo8118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://qj.zhonguo6118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://vf.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://hh.zhonguo5118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://xk.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://sg.zhonguo3118.cn

[B13] 判断是否为数字
来源：https://vp.zhonguo6118.cn

Py:   isinstance(x, (int, float))
来源：https://et.zhonguo4118.cn

PHP:  is_numeric($x)
来源：https://do.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://vr.zhonguo2118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://sr.zhonguo1118.cn

Java: x instanceof Number
来源：https://ma.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://jr.zhonguo1118.cn

Ruby: x.is_a?(Numeric)
来源：https://yx.zhonguo3118.cn

C#:   x is int or double or decimal
来源：https://ev.zhonguo2118.cn

[B14] 判断值是否在集合内
来源：https://kg.zhonguo5118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://xt.zhonguo8118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://xe.zhonguo8118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ej.zhonguo7118.cn

TS:   [1, 2, 3].includes(x)
来源：https://ky.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://ad.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://au.zhonguo8118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://qv.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://yy.zhonguo6118.cn

[B15] 布尔运算与取反
来源：https://xg.zhonguo5118.cn

Py:   a and b or not c
来源：https://pk.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://qm.zhonguo8118.cn

JS:   a && b || !c
来源：https://tq.zhonguo7118.cn

TS:   a && b || !c
来源：https://ux.zhonguo5118.cn

Java: a && b || !c
来源：https://lb.zhonguo8118.cn

Go:   a && b || !c
来源：https://ni.zhonguo2118.cn

Ruby: a && b || !c
来源：https://ew.zhonguo2118.cn

C#:   a && b || !c
来源：https://ll.zhonguo1118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://rp.zhonguo7118.cn

Py:   if not data: return
来源：https://mc.zhonguo3118.cn

PHP:  if (!$data) { return; }
来源：https://pe.zhonguo5118.cn

JS:   if (!data) return;
来源：https://ty.zhonguo7118.cn

TS:   if (!data) return;
来源：https://cw.zhonguo6118.cn

Java: if (data == null) return;
来源：https://ru.zhonguo7118.cn

Go:   if data == nil { return }
来源：https://hy.zhonguo8118.cn

Ruby: return if data.nil?
来源：https://gn.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://zb.zhonguo4118.cn

================================================================================
来源：https://pj.zhonguo3118.cn

C. 函数与作用域
来源：https://kp.zhonguo8118.cn

================================================================================
来源：https://pq.zhonguo8118.cn

[C01] 定义函数
来源：https://ke.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://eq.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qn.zhonguo4118.cn

JS:   function add(a, b) { return a + b; }
来源：https://ns.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://rx.zhonguo5118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://ye.zhonguo1118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://xq.zhonguo2118.cn

Ruby: def add(a, b); a + b; end
来源：https://sd.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://yr.zhonguo1118.cn

[C02] 默认参数
来源：https://mc.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://cw.zhonguo4118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://nt.zhonguo5118.cn

JS:   function greet(name = "World") { return name; }
来源：https://aj.zhonguo4118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://hn.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://mh.zhonguo3118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://rp.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://ik.zhonguo2118.cn

C#:   string Greet(string name = "World") => name;
来源：https://kv.zhonguo8118.cn

[C03] 可变参数
来源：https://zh.zhonguo1118.cn

Py:   def total(*args): return sum(args)
来源：https://mf.zhonguo5118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://ci.zhonguo3118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://tc.zhonguo1118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://ns.zhonguo2118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://yx.zhonguo8118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://hf.zhonguo2118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://zt.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://tk.zhonguo3118.cn

[C04] 命名参数 / 关键字参数
来源：https://rj.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://aw.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://lt.zhonguo6118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://mu.zhonguo4118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://jo.zhonguo8118.cn

Java: // 无：用 Builder 模式或 record
来源：https://kx.zhonguo2118.cn

Go:   // 无：用配置结构体参数
来源：https://qm.zhonguo1118.cn

Ruby: f(a: 1, b: 2)
来源：https://kf.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://gr.zhonguo3118.cn

[C05] 返回多个值
来源：https://cd.zhonguo1118.cn

Py:   return a, b
来源：https://wf.zhonguo5118.cn

PHP:  return [$a, $b];
来源：https://ly.zhonguo5118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://gr.zhonguo4118.cn

TS:   return { a, b };
来源：https://mm.zhonguo8118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://fo.zhonguo5118.cn

Go:   return a, b
来源：https://gj.zhonguo2118.cn

Ruby: return a, b
来源：https://qa.zhonguo7118.cn

C#:   return (a, b);              // ValueTuple
来源：https://xz.zhonguo6118.cn

[C06] 匿名函数 / lambda
来源：https://mw.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://tm.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://dv.zhonguo2118.cn

JS:   const square = x => x * x;
来源：https://yl.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://qv.zhonguo3118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://hh.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://cy.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://yj.zhonguo4118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://lg.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://zl.zhonguo8118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://eh.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://vp.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://ma.zhonguo4118.cn

TS:   arr.map(String)
来源：https://xs.zhonguo6118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://gh.zhonguo4118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://hx.zhonguo1118.cn

Ruby: arr.map(&:upcase)
来源：https://zc.zhonguo6118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://lw.zhonguo2118.cn

[C08] 闭包
来源：https://vi.zhonguo5118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ow.zhonguo2118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ip.zhonguo8118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://ce.zhonguo6118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://zr.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://zn.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://jp.zhonguo4118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://na.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://cw.zhonguo6118.cn

[C09] 递归
来源：https://jy.zhonguo1118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://kl.zhonguo4118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://ry.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://jb.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://wr.zhonguo5118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://gc.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ed.zhonguo8118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://tq.zhonguo6118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://ne.zhonguo1118.cn

[C10] 变量作用域
来源：https://wi.zhonguo3118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://eq.zhonguo4118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://go.zhonguo1118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://hb.zhonguo5118.cn

TS:   同 JS
来源：https://fi.zhonguo7118.cn

Java: 方法内为块级作用域
来源：https://ou.zhonguo8118.cn

Go:   花括号块级作用域
来源：https://is.zhonguo7118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://pw.zhonguo8118.cn

C#:   块级作用域
来源：https://mq.zhonguo5118.cn

[C11] 模块导入与导出
来源：https://su.zhonguo6118.cn

Py:   from module import func
来源：https://id.zhonguo3118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://in.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://br.zhonguo5118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://gl.zhonguo5118.cn

Java: import java.util.List;
来源：https://ax.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://cy.zhonguo1118.cn

Ruby: require "json"; require_relative "./util"
来源：https://vn.zhonguo7118.cn

C#:   using System.Text;
来源：https://zm.zhonguo7118.cn

[C12] 立即执行函数 IIFE
来源：https://yn.zhonguo1118.cn

Py:   (lambda: print("run"))()
来源：https://pw.zhonguo4118.cn

PHP:  (function () { echo "run"; })();
来源：https://gk.zhonguo1118.cn

JS:   (() => { console.log("run"); })();
来源：https://zo.zhonguo7118.cn

TS:   (() => { console.log("run"); })();
来源：https://hj.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ut.zhonguo5118.cn

Go:   func() { fmt.Println("run") }()
来源：https://vx.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://jf.zhonguo2118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://is.zhonguo8118.cn

[C13] 类型声明 / 类型注解
来源：https://es.zhonguo5118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://fq.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://pq.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://lf.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://no.zhonguo2118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://oe.zhonguo1118.cn

Go:   func add(a, b int) int
来源：https://vs.zhonguo8118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://xc.zhonguo3118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://eb.zhonguo3118.cn

[C14] 泛型函数
来源：https://xe.zhonguo8118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://qr.zhonguo6118.cn

PHP:  // 无泛型
来源：https://at.zhonguo4118.cn

JS:   // 无泛型
来源：https://zw.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://fi.zhonguo5118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://ba.zhonguo7118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://lx.zhonguo7118.cn

Ruby: # 无泛型
来源：https://ch.zhonguo5118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://wh.zhonguo7118.cn

[C15] 解构 / 展开参数
来源：https://rd.zhonguo3118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://mq.zhonguo6118.cn

PHP:  [$a, $b] = $pair;
来源：https://pr.zhonguo1118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://jd.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ob.zhonguo5118.cn

Java: // 无解构
来源：https://bz.zhonguo4118.cn

Go:   // 无解构
来源：https://jo.zhonguo5118.cn

Ruby: a, b = pair
来源：https://lo.zhonguo3118.cn

C#:   var (a, b) = pair;
来源：https://ly.zhonguo4118.cn

[C16] 函数 / 方法重载
来源：https://ze.zhonguo2118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://tk.zhonguo4118.cn

PHP:  // 无重载
来源：https://eq.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://pt.zhonguo3118.cn

TS:   // 用联合类型或重载签名声明
来源：https://pl.zhonguo2118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://eg.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://ck.zhonguo4118.cn

Ruby: # 无重载：靠动态参数
来源：https://xx.zhonguo4118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://qb.zhonguo3118.cn

================================================================================
来源：https://jw.zhonguo1118.cn

D. 数组 / 列表 / 集合
来源：https://ou.zhonguo4118.cn

================================================================================
来源：https://fy.zhonguo3118.cn

[D01] 创建数组 / 列表
来源：https://rl.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://fe.zhonguo3118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://rx.zhonguo2118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://qi.zhonguo4118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://xz.zhonguo5118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://tg.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://no.zhonguo1118.cn

Ruby: arr = [1, 2, 3]
来源：https://th.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://fp.zhonguo1118.cn

[D02] 追加元素到末尾
来源：https://hp.zhonguo5118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://db.zhonguo5118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://uu.zhonguo2118.cn

JS:   arr.push(4);
来源：https://kt.zhonguo3118.cn

TS:   arr.push(4);
来源：https://fk.zhonguo3118.cn

Java: list.add(4);
来源：https://hq.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://de.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://nc.zhonguo7118.cn

C#:   list.Add(4);
来源：https://cm.zhonguo8118.cn

[D03] 在指定位置插入元素
来源：https://mh.zhonguo2118.cn

Py:   arr.insert(0, 0)
来源：https://zn.zhonguo1118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://xu.zhonguo5118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://ku.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://gd.zhonguo3118.cn

Java: list.add(0, 0);
来源：https://bj.zhonguo3118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://td.zhonguo7118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://lb.zhonguo4118.cn

C#:   list.Insert(0, 0);
来源：https://pw.zhonguo1118.cn

[D04] 删除元素
来源：https://km.zhonguo8118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://cn.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://wk.zhonguo5118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://mu.zhonguo8118.cn

TS:   arr.splice(0, 1);
来源：https://xp.zhonguo4118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ye.zhonguo5118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ft.zhonguo7118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ou.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://yo.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://uu.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://xr.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://du.zhonguo2118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://xv.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://gv.zhonguo2118.cn

Java: list.get(0); list.set(0, 9);
来源：https://fe.zhonguo5118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ij.zhonguo5118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://bh.zhonguo6118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ko.zhonguo2118.cn

[D06] 数组长度
来源：https://px.zhonguo3118.cn

Py:   len(arr)
来源：https://nd.zhonguo7118.cn

PHP:  count($arr);
来源：https://ph.zhonguo7118.cn

JS:   arr.length
来源：https://dc.zhonguo7118.cn

TS:   arr.length
来源：https://ge.zhonguo6118.cn

Java: list.size();
来源：https://ac.zhonguo5118.cn

Go:   len(arr)
来源：https://zr.zhonguo1118.cn

Ruby: arr.length; arr.size
来源：https://jq.zhonguo5118.cn

C#:   list.Count;
来源：https://ix.zhonguo1118.cn

[D07] 切片 / 取子数组
来源：https://fw.zhonguo6118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://if.zhonguo7118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://oq.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://tc.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://nw.zhonguo7118.cn

Java: list.subList(1, 4);
来源：https://zf.zhonguo7118.cn

Go:   arr[1:4]
来源：https://lo.zhonguo6118.cn

Ruby: arr[1, 3]
来源：https://bu.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://px.zhonguo3118.cn

[D08] 合并两个数组
来源：https://ut.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://bx.zhonguo6118.cn

PHP:  array_merge($a, $b);
来源：https://ew.zhonguo2118.cn


<!-- 参考信息 -->