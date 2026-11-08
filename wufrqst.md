代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：https://ou.zhonguo8118.cn

PHP:  do { $i++; } while ($i < 10);
来源：https://us.zhonguo7118.cn

JS:   do { i++; } while (i < 10);
来源：https://pv.zhonguo6118.cn

TS:   do { i++; } while (i < 10);
来源：https://at.zhonguo3118.cn

Java: do { i++; } while (i < 10);
来源：https://ao.zhonguo8118.cn

Go:   for { i++; if i >= 10 { break } }
来源：https://el.zhonguo7118.cn

Ruby: begin; i += 1; end while i < 10
来源：https://xm.zhonguo6118.cn

C#:   do { i++; } while (i < 10);
来源：https://xx.zhonguo4118.cn

[B09] break 与 continue
来源：https://aq.zhonguo2118.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：https://ce.zhonguo8118.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：https://eo.zhonguo3118.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://ua.zhonguo8118.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://bk.zhonguo6118.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://eo.zhonguo3118.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：https://tq.zhonguo5118.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：https://mj.zhonguo6118.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：https://yt.zhonguo2118.cn

[B10] 遍历同时拿索引
来源：https://uh.zhonguo7118.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：https://ea.zhonguo8118.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：https://af.zhonguo5118.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：https://lm.zhonguo3118.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：https://ki.zhonguo2118.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：https://nv.zhonguo1118.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：https://yx.zhonguo6118.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：https://zo.zhonguo1118.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：https://qq.zhonguo6118.cn

[B11] 生成数字序列 / 区间
来源：https://zf.zhonguo5118.cn

Py:   list(range(0, 10, 2))
来源：https://ac.zhonguo3118.cn

PHP:  range(0, 10, 2);
来源：https://wf.zhonguo7118.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://ra.zhonguo3118.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：https://vq.zhonguo3118.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：https://ws.zhonguo5118.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：https://tf.zhonguo5118.cn

Ruby: (0...10).step(2).to_a
来源：https://nk.zhonguo2118.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：https://fb.zhonguo6118.cn

[B12] 跳出多层循环
来源：https://aw.zhonguo6118.cn

Py:   # 无标签跳转：抽成函数用 return
来源：https://hs.zhonguo3118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://cg.zhonguo1118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://lp.zhonguo4118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://ln.zhonguo8118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://lp.zhonguo1118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://jc.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ww.zhonguo5118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://ug.zhonguo4118.cn

[B13] 判断是否为数字
来源：https://zi.zhonguo4118.cn

Py:   isinstance(x, (int, float))
来源：https://uu.zhonguo3118.cn

PHP:  is_numeric($x)
来源：https://sq.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://te.zhonguo4118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ge.zhonguo3118.cn

Java: x instanceof Number
来源：https://qc.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://lp.zhonguo2118.cn

Ruby: x.is_a?(Numeric)
来源：https://qn.zhonguo8118.cn

C#:   x is int or double or decimal
来源：https://wn.zhonguo5118.cn

[B14] 判断值是否在集合内
来源：https://uj.zhonguo4118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://ps.zhonguo4118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://vm.zhonguo3118.cn

JS:   [1, 2, 3].includes(x)
来源：https://sd.zhonguo4118.cn

TS:   [1, 2, 3].includes(x)
来源：https://vb.zhonguo3118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://cv.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://qk.zhonguo6118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://pl.zhonguo7118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://lg.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://um.zhonguo6118.cn

Py:   a and b or not c
来源：https://gg.zhonguo7118.cn

PHP:  $a && $b || !$c
来源：https://aw.zhonguo7118.cn

JS:   a && b || !c
来源：https://go.zhonguo8118.cn

TS:   a && b || !c
来源：https://ih.zhonguo3118.cn

Java: a && b || !c
来源：https://pm.zhonguo5118.cn

Go:   a && b || !c
来源：https://yd.zhonguo6118.cn

Ruby: a && b || !c
来源：https://oy.zhonguo6118.cn

C#:   a && b || !c
来源：https://ve.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://kf.zhonguo2118.cn

Py:   if not data: return
来源：https://pc.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://nz.zhonguo4118.cn

JS:   if (!data) return;
来源：https://no.zhonguo8118.cn

TS:   if (!data) return;
来源：https://jp.zhonguo1118.cn

Java: if (data == null) return;
来源：https://bs.zhonguo8118.cn

Go:   if data == nil { return }
来源：https://te.zhonguo6118.cn

Ruby: return if data.nil?
来源：https://pu.zhonguo3118.cn

C#:   if (data == null) return;
来源：https://yt.zhonguo2118.cn

================================================================================
来源：https://qr.zhonguo1118.cn

C. 函数与作用域
来源：https://fz.zhonguo5118.cn

================================================================================
来源：https://zd.zhonguo3118.cn

[C01] 定义函数
来源：https://vb.zhonguo5118.cn

Py:   def add(a, b): return a + b
来源：https://zi.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://dh.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://vs.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://dc.zhonguo3118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://tl.zhonguo8118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://rx.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://kd.zhonguo2118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ow.zhonguo8118.cn

[C02] 默认参数
来源：https://sw.zhonguo2118.cn

Py:   def greet(name="World"): return name
来源：https://jd.zhonguo7118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://pq.zhonguo1118.cn

JS:   function greet(name = "World") { return name; }
来源：https://re.zhonguo4118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://tc.zhonguo7118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://zf.zhonguo6118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://na.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://te.zhonguo4118.cn

C#:   string Greet(string name = "World") => name;
来源：https://zt.zhonguo3118.cn

[C03] 可变参数
来源：https://lr.zhonguo5118.cn

Py:   def total(*args): return sum(args)
来源：https://ya.zhonguo1118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://ye.zhonguo2118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://pf.zhonguo6118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://pg.zhonguo3118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://bb.zhonguo8118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://oo.zhonguo6118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://bl.zhonguo2118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://yz.zhonguo5118.cn

[C04] 命名参数 / 关键字参数
来源：https://oo.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://wx.zhonguo4118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://uv.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://gs.zhonguo1118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://vn.zhonguo7118.cn

Java: // 无：用 Builder 模式或 record
来源：https://dg.zhonguo5118.cn

Go:   // 无：用配置结构体参数
来源：https://mc.zhonguo6118.cn

Ruby: f(a: 1, b: 2)
来源：https://pk.zhonguo7118.cn

C#:   f(a: 1, b: 2)
来源：https://oq.zhonguo7118.cn

[C05] 返回多个值
来源：https://km.zhonguo3118.cn

Py:   return a, b
来源：https://zz.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://ug.zhonguo4118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://na.zhonguo8118.cn

TS:   return { a, b };
来源：https://nz.zhonguo6118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://fp.zhonguo4118.cn

Go:   return a, b
来源：https://kg.zhonguo4118.cn

Ruby: return a, b
来源：https://rs.zhonguo6118.cn

C#:   return (a, b);              // ValueTuple
来源：https://ks.zhonguo5118.cn

[C06] 匿名函数 / lambda
来源：https://uc.zhonguo7118.cn

Py:   square = lambda x: x * x
来源：https://jy.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://kk.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://mp.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://pa.zhonguo7118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://dt.zhonguo5118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://aw.zhonguo7118.cn

Ruby: square = ->(x) { x * x }
来源：https://kt.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://lq.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://eb.zhonguo3118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://gu.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://hk.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://vk.zhonguo8118.cn

TS:   arr.map(String)
来源：https://ab.zhonguo8118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://wm.zhonguo7118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://kx.zhonguo6118.cn

Ruby: arr.map(&:upcase)
来源：https://cf.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://qj.zhonguo7118.cn

[C08] 闭包
来源：https://wp.zhonguo8118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ub.zhonguo6118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://kc.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://vy.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://wa.zhonguo5118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://ij.zhonguo6118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://vh.zhonguo3118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://le.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://ty.zhonguo7118.cn

[C09] 递归
来源：https://zb.zhonguo1118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://qu.zhonguo7118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://bj.zhonguo8118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://hw.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://bp.zhonguo8118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://be.zhonguo6118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ip.zhonguo3118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ch.zhonguo4118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://nw.zhonguo4118.cn

[C10] 变量作用域
来源：https://sv.zhonguo5118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://cl.zhonguo3118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://vv.zhonguo3118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://ia.zhonguo7118.cn

TS:   同 JS
来源：https://dt.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://ip.zhonguo6118.cn

Go:   花括号块级作用域
来源：https://df.zhonguo1118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://yk.zhonguo3118.cn

C#:   块级作用域
来源：https://qf.zhonguo8118.cn

[C11] 模块导入与导出
来源：https://mg.zhonguo8118.cn

Py:   from module import func
来源：https://iy.zhonguo6118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://vm.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://uf.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://xo.zhonguo6118.cn

Java: import java.util.List;
来源：https://ns.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://br.zhonguo5118.cn

Ruby: require "json"; require_relative "./util"
来源：https://pn.zhonguo7118.cn

C#:   using System.Text;
来源：https://gi.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://nl.zhonguo8118.cn

Py:   (lambda: print("run"))()
来源：https://mt.zhonguo7118.cn

PHP:  (function () { echo "run"; })();
来源：https://ip.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://vw.zhonguo7118.cn

TS:   (() => { console.log("run"); })();
来源：https://hw.zhonguo1118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ko.zhonguo6118.cn

Go:   func() { fmt.Println("run") }()
来源：https://ck.zhonguo7118.cn

Ruby: -> { puts "run" }.call
来源：https://vb.zhonguo7118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://hh.zhonguo5118.cn

[C13] 类型声明 / 类型注解
来源：https://ke.zhonguo5118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://id.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://na.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://gr.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://dj.zhonguo2118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://ha.zhonguo1118.cn

Go:   func add(a, b int) int
来源：https://zf.zhonguo6118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://zm.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://eu.zhonguo5118.cn

[C14] 泛型函数
来源：https://iw.zhonguo4118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://et.zhonguo4118.cn

PHP:  // 无泛型
来源：https://ax.zhonguo1118.cn

JS:   // 无泛型
来源：https://pc.zhonguo7118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://jq.zhonguo8118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://ks.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://rn.zhonguo5118.cn

Ruby: # 无泛型
来源：https://zg.zhonguo4118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://sn.zhonguo3118.cn

[C15] 解构 / 展开参数
来源：https://go.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ea.zhonguo6118.cn

PHP:  [$a, $b] = $pair;
来源：https://fd.zhonguo6118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://aq.zhonguo6118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://cq.zhonguo6118.cn

Java: // 无解构
来源：https://xz.zhonguo5118.cn

Go:   // 无解构
来源：https://oq.zhonguo7118.cn

Ruby: a, b = pair
来源：https://qj.zhonguo3118.cn

C#:   var (a, b) = pair;
来源：https://ia.zhonguo6118.cn

[C16] 函数 / 方法重载
来源：https://oh.zhonguo2118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://fh.zhonguo5118.cn

PHP:  // 无重载
来源：https://sb.zhonguo5118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ar.zhonguo7118.cn

TS:   // 用联合类型或重载签名声明
来源：https://my.zhonguo8118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ik.zhonguo1118.cn

Go:   // 无重载：用不同函数名
来源：https://ie.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://nw.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://qn.zhonguo4118.cn

================================================================================
来源：https://sv.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://ct.zhonguo3118.cn

================================================================================
来源：https://oq.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://ue.zhonguo6118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://tz.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://gi.zhonguo3118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://jv.zhonguo6118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://zg.zhonguo3118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://jv.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://sd.zhonguo2118.cn

Ruby: arr = [1, 2, 3]
来源：https://to.zhonguo2118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://rv.zhonguo5118.cn

[D02] 追加元素到末尾
来源：https://ds.zhonguo7118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://fr.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ky.zhonguo1118.cn

JS:   arr.push(4);
来源：https://be.zhonguo5118.cn

TS:   arr.push(4);
来源：https://ol.zhonguo6118.cn

Java: list.add(4);
来源：https://ni.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://jw.zhonguo5118.cn

Ruby: arr << 4; arr.push(5)
来源：https://kt.zhonguo8118.cn

C#:   list.Add(4);
来源：https://vq.zhonguo2118.cn

[D03] 在指定位置插入元素
来源：https://fc.zhonguo4118.cn

Py:   arr.insert(0, 0)
来源：https://lg.zhonguo1118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://at.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://cz.zhonguo7118.cn

TS:   arr.splice(0, 0, 0);
来源：https://xn.zhonguo4118.cn

Java: list.add(0, 0);
来源：https://ri.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://ju.zhonguo3118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://lg.zhonguo1118.cn

C#:   list.Insert(0, 0);
来源：https://zl.zhonguo4118.cn

[D04] 删除元素
来源：https://no.zhonguo7118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://we.zhonguo3118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://te.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://rn.zhonguo7118.cn

TS:   arr.splice(0, 1);
来源：https://gl.zhonguo2118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ja.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://jn.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://dq.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://zp.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://tw.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://yw.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://gr.zhonguo7118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://sg.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ai.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://hu.zhonguo6118.cn

Go:   arr[0]; arr[0] = 9
来源：https://og.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://qs.zhonguo3118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://kw.zhonguo7118.cn

[D06] 数组长度
来源：https://us.zhonguo5118.cn

Py:   len(arr)
来源：https://di.zhonguo4118.cn

PHP:  count($arr);
来源：https://vx.zhonguo4118.cn

JS:   arr.length
来源：https://kb.zhonguo6118.cn

TS:   arr.length
来源：https://vc.zhonguo7118.cn

Java: list.size();
来源：https://ol.zhonguo1118.cn

Go:   len(arr)
来源：https://hi.zhonguo2118.cn

Ruby: arr.length; arr.size
来源：https://ys.zhonguo1118.cn

C#:   list.Count;
来源：https://sg.zhonguo3118.cn

[D07] 切片 / 取子数组
来源：https://mg.zhonguo8118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://ej.zhonguo1118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://cs.zhonguo2118.cn

JS:   arr.slice(1, 4);
来源：https://wq.zhonguo1118.cn

TS:   arr.slice(1, 4);
来源：https://yb.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://xn.zhonguo7118.cn

Go:   arr[1:4]
来源：https://wq.zhonguo1118.cn

Ruby: arr[1, 3]
来源：https://aq.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://zd.zhonguo2118.cn

[D08] 合并两个数组
来源：https://xm.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://vq.zhonguo3118.cn

PHP:  array_merge($a, $b);
来源：https://ww.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://rj.zhonguo7118.cn

TS:   [...a, ...b];
来源：https://qb.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ub.zhonguo7118.cn

Go:   append(a, b...)
来源：https://ap.zhonguo6118.cn


<!-- 参考信息 -->