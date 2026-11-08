代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：https://po.zhonguo7118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://ib.zhonguo3118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://wc.zhonguo5118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://wx.zhonguo1118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://vi.zhonguo3118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://ns.zhonguo5118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://kp.zhonguo8118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://il.zhonguo8118.cn

[B13] 判断是否为数字
来源：https://xh.zhonguo4118.cn

Py:   isinstance(x, (int, float))
来源：https://mn.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://ok.zhonguo3118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://sq.zhonguo5118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://by.zhonguo8118.cn

Java: x instanceof Number
来源：https://ng.zhonguo2118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ns.zhonguo1118.cn

Ruby: x.is_a?(Numeric)
来源：https://gw.zhonguo1118.cn

C#:   x is int or double or decimal
来源：https://kn.zhonguo1118.cn

[B14] 判断值是否在集合内
来源：https://xn.zhonguo1118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://he.zhonguo1118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://fx.zhonguo1118.cn

JS:   [1, 2, 3].includes(x)
来源：https://lz.zhonguo5118.cn

TS:   [1, 2, 3].includes(x)
来源：https://gt.zhonguo6118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://yh.zhonguo4118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://ca.zhonguo4118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://tu.zhonguo4118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://sj.zhonguo4118.cn

[B15] 布尔运算与取反
来源：https://tl.zhonguo2118.cn

Py:   a and b or not c
来源：https://pl.zhonguo3118.cn

PHP:  $a && $b || !$c
来源：https://yq.zhonguo3118.cn

JS:   a && b || !c
来源：https://yd.zhonguo4118.cn

TS:   a && b || !c
来源：https://nt.zhonguo3118.cn

Java: a && b || !c
来源：https://gr.zhonguo1118.cn

Go:   a && b || !c
来源：https://ys.zhonguo6118.cn

Ruby: a && b || !c
来源：https://rm.zhonguo5118.cn

C#:   a && b || !c
来源：https://gn.zhonguo8118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://dy.zhonguo7118.cn

Py:   if not data: return
来源：https://ug.zhonguo4118.cn

PHP:  if (!$data) { return; }
来源：https://bg.zhonguo3118.cn

JS:   if (!data) return;
来源：https://yf.zhonguo4118.cn

TS:   if (!data) return;
来源：https://xq.zhonguo3118.cn

Java: if (data == null) return;
来源：https://qs.zhonguo7118.cn

Go:   if data == nil { return }
来源：https://dw.zhonguo5118.cn

Ruby: return if data.nil?
来源：https://zq.zhonguo4118.cn

C#:   if (data == null) return;
来源：https://ju.zhonguo1118.cn

================================================================================
来源：https://id.zhonguo2118.cn

C. 函数与作用域
来源：https://dm.zhonguo2118.cn

================================================================================
来源：https://po.zhonguo8118.cn

[C01] 定义函数
来源：https://qx.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://hg.zhonguo2118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://eb.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://sa.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://xx.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://ut.zhonguo6118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://zg.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://fd.zhonguo1118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://on.zhonguo6118.cn

[C02] 默认参数
来源：https://wi.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://rp.zhonguo1118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://hs.zhonguo6118.cn

JS:   function greet(name = "World") { return name; }
来源：https://rd.zhonguo8118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://oa.zhonguo2118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://lt.zhonguo7118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://bq.zhonguo1118.cn

Ruby: def greet(name = "World") = name
来源：https://pu.zhonguo4118.cn

C#:   string Greet(string name = "World") => name;
来源：https://ou.zhonguo5118.cn

[C03] 可变参数
来源：https://cr.zhonguo2118.cn

Py:   def total(*args): return sum(args)
来源：https://mu.zhonguo2118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://sj.zhonguo2118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://er.zhonguo5118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://de.zhonguo1118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ls.zhonguo2118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://kd.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://im.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://sn.zhonguo3118.cn

[C04] 命名参数 / 关键字参数
来源：https://wj.zhonguo7118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://nt.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://ky.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://zr.zhonguo3118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://pm.zhonguo6118.cn

Java: // 无：用 Builder 模式或 record
来源：https://pj.zhonguo8118.cn

Go:   // 无：用配置结构体参数
来源：https://kw.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://ft.zhonguo5118.cn

C#:   f(a: 1, b: 2)
来源：https://di.zhonguo3118.cn

[C05] 返回多个值
来源：https://ma.zhonguo2118.cn

Py:   return a, b
来源：https://rb.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://vx.zhonguo1118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://ts.zhonguo8118.cn

TS:   return { a, b };
来源：https://yp.zhonguo7118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://kj.zhonguo5118.cn

Go:   return a, b
来源：https://ab.zhonguo3118.cn

Ruby: return a, b
来源：https://et.zhonguo3118.cn

C#:   return (a, b);              // ValueTuple
来源：https://uz.zhonguo7118.cn

[C06] 匿名函数 / lambda
来源：https://ft.zhonguo4118.cn

Py:   square = lambda x: x * x
来源：https://yl.zhonguo1118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://sn.zhonguo7118.cn

JS:   const square = x => x * x;
来源：https://jx.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://gp.zhonguo2118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://pw.zhonguo2118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://vw.zhonguo7118.cn

Ruby: square = ->(x) { x * x }
来源：https://gw.zhonguo2118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://fc.zhonguo7118.cn

[C07] 把函数作为参数传入
来源：https://wg.zhonguo5118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://si.zhonguo1118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://hc.zhonguo8118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://qx.zhonguo7118.cn

TS:   arr.map(String)
来源：https://sk.zhonguo1118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://ut.zhonguo3118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://mr.zhonguo7118.cn

Ruby: arr.map(&:upcase)
来源：https://xl.zhonguo4118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://qt.zhonguo3118.cn

[C08] 闭包
来源：https://pk.zhonguo6118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://mo.zhonguo3118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://rv.zhonguo4118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://sc.zhonguo1118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://dr.zhonguo5118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://we.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://qh.zhonguo5118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://qr.zhonguo2118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://se.zhonguo3118.cn

[C09] 递归
来源：https://mw.zhonguo6118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://xv.zhonguo3118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://pz.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://un.zhonguo1118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://au.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://jm.zhonguo7118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://oi.zhonguo6118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ld.zhonguo7118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://kt.zhonguo6118.cn

[C10] 变量作用域
来源：https://pt.zhonguo4118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://tg.zhonguo7118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://aq.zhonguo8118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://cg.zhonguo5118.cn

TS:   同 JS
来源：https://rk.zhonguo7118.cn

Java: 方法内为块级作用域
来源：https://kx.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://pk.zhonguo3118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://cy.zhonguo1118.cn

C#:   块级作用域
来源：https://le.zhonguo8118.cn

[C11] 模块导入与导出
来源：https://jj.zhonguo6118.cn

Py:   from module import func
来源：https://gb.zhonguo5118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://xh.zhonguo6118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://du.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://aq.zhonguo4118.cn

Java: import java.util.List;
来源：https://ii.zhonguo4118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://vn.zhonguo2118.cn

Ruby: require "json"; require_relative "./util"
来源：https://on.zhonguo3118.cn

C#:   using System.Text;
来源：https://ow.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://pl.zhonguo3118.cn

Py:   (lambda: print("run"))()
来源：https://ud.zhonguo3118.cn

PHP:  (function () { echo "run"; })();
来源：https://gp.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://lo.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://vb.zhonguo4118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://uh.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://pq.zhonguo6118.cn

Ruby: -> { puts "run" }.call
来源：https://mh.zhonguo5118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://uv.zhonguo8118.cn

[C13] 类型声明 / 类型注解
来源：https://dv.zhonguo6118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://un.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ej.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://gi.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://hv.zhonguo4118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://rt.zhonguo1118.cn

Go:   func add(a, b int) int
来源：https://qs.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://jy.zhonguo2118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://gf.zhonguo4118.cn

[C14] 泛型函数
来源：https://nd.zhonguo3118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://uy.zhonguo4118.cn

PHP:  // 无泛型
来源：https://vn.zhonguo1118.cn

JS:   // 无泛型
来源：https://jc.zhonguo3118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://pb.zhonguo1118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://wa.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://mj.zhonguo6118.cn

Ruby: # 无泛型
来源：https://ay.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://nq.zhonguo1118.cn

[C15] 解构 / 展开参数
来源：https://qs.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ff.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://hf.zhonguo6118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://cl.zhonguo3118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://si.zhonguo5118.cn

Java: // 无解构
来源：https://iu.zhonguo1118.cn

Go:   // 无解构
来源：https://kd.zhonguo3118.cn

Ruby: a, b = pair
来源：https://kv.zhonguo6118.cn

C#:   var (a, b) = pair;
来源：https://pt.zhonguo5118.cn

[C16] 函数 / 方法重载
来源：https://vk.zhonguo5118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ap.zhonguo8118.cn

PHP:  // 无重载
来源：https://ap.zhonguo6118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://tx.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://ho.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://jn.zhonguo7118.cn

Go:   // 无重载：用不同函数名
来源：https://dy.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://ap.zhonguo1118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jo.zhonguo4118.cn

================================================================================
来源：https://ep.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://kf.zhonguo8118.cn

================================================================================
来源：https://fd.zhonguo7118.cn

[D01] 创建数组 / 列表
来源：https://pc.zhonguo1118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://fe.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://lx.zhonguo3118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://sq.zhonguo7118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://zf.zhonguo3118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://wr.zhonguo7118.cn

Go:   arr := []int{1, 2, 3}
来源：https://ja.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://in.zhonguo8118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://pq.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://yy.zhonguo4118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://jc.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://bq.zhonguo8118.cn

JS:   arr.push(4);
来源：https://vn.zhonguo1118.cn

TS:   arr.push(4);
来源：https://ul.zhonguo5118.cn

Java: list.add(4);
来源：https://wl.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://au.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://ck.zhonguo5118.cn

C#:   list.Add(4);
来源：https://ij.zhonguo2118.cn

[D03] 在指定位置插入元素
来源：https://rg.zhonguo4118.cn

Py:   arr.insert(0, 0)
来源：https://pu.zhonguo4118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://ah.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://qr.zhonguo8118.cn

TS:   arr.splice(0, 0, 0);
来源：https://il.zhonguo6118.cn

Java: list.add(0, 0);
来源：https://ka.zhonguo3118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://cv.zhonguo1118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://iq.zhonguo6118.cn

C#:   list.Insert(0, 0);
来源：https://ml.zhonguo6118.cn

[D04] 删除元素
来源：https://vk.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://dt.zhonguo1118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://cc.zhonguo7118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://jy.zhonguo6118.cn

TS:   arr.splice(0, 1);
来源：https://uv.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://qv.zhonguo6118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://tn.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://qu.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://na.zhonguo1118.cn

[D05] 访问与修改元素
来源：https://ty.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://hf.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://pt.zhonguo5118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://cv.zhonguo4118.cn

TS:   arr[0]; arr.at(-1);
来源：https://dh.zhonguo2118.cn

Java: list.get(0); list.set(0, 9);
来源：https://jn.zhonguo4118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ty.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://fw.zhonguo2118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://be.zhonguo3118.cn

[D06] 数组长度
来源：https://aj.zhonguo8118.cn

Py:   len(arr)
来源：https://pk.zhonguo6118.cn

PHP:  count($arr);
来源：https://fd.zhonguo3118.cn

JS:   arr.length
来源：https://pl.zhonguo1118.cn

TS:   arr.length
来源：https://qp.zhonguo6118.cn

Java: list.size();
来源：https://pn.zhonguo7118.cn

Go:   len(arr)
来源：https://gy.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://pe.zhonguo6118.cn

C#:   list.Count;
来源：https://yv.zhonguo2118.cn

[D07] 切片 / 取子数组
来源：https://ua.zhonguo6118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://nf.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://pu.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://mv.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://dv.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://ou.zhonguo5118.cn

Go:   arr[1:4]
来源：https://ed.zhonguo8118.cn

Ruby: arr[1, 3]
来源：https://vr.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://lr.zhonguo1118.cn

[D08] 合并两个数组
来源：https://by.zhonguo6118.cn

Py:   a + b;  a.extend(b)
来源：https://vc.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://kp.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://cz.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://my.zhonguo5118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://jc.zhonguo1118.cn

Go:   append(a, b...)
来源：https://qy.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://zk.zhonguo1118.cn

C#:   a.Concat(b).ToList()
来源：https://wr.zhonguo6118.cn

[D09] 排序（升序）
来源：https://pf.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://hf.zhonguo6118.cn

PHP:  sort($arr);
来源：https://ef.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://tw.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://wi.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://xs.zhonguo3118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://it.zhonguo7118.cn

Ruby: arr.sort
来源：https://wg.zhonguo5118.cn

C#:   list.Sort();
来源：https://gj.zhonguo8118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://lg.zhonguo3118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://ux.zhonguo5118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://sr.zhonguo6118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://wy.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ct.zhonguo5118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://st.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://og.zhonguo5118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://sf.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://vf.zhonguo8118.cn

[D11] 反转数组
来源：https://ke.zhonguo8118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://my.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://kc.zhonguo4118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://rx.zhonguo2118.cn

TS:   [...arr].reverse();
来源：https://ev.zhonguo2118.cn

Java: Collections.reverse(list);
来源：https://od.zhonguo1118.cn

Go:   slices.Reverse(arr)
来源：https://qi.zhonguo7118.cn

Ruby: arr.reverse
来源：https://hs.zhonguo2118.cn

C#:   list.Reverse();
来源：https://wo.zhonguo5118.cn

[D12] 查找元素下标
来源：https://dz.zhonguo7118.cn

Py:   arr.index(x);  x in arr
来源：https://ct.zhonguo2118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://sl.zhonguo8118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://nt.zhonguo5118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://nh.zhonguo4118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://nd.zhonguo3118.cn

Go:   slices.Index(arr, x)
来源：https://dq.zhonguo6118.cn


<!-- 参考信息 -->