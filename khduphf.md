代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：https://xb.zhonguo8118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://yp.zhonguo3118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://ux.zhonguo2118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://cb.zhonguo6118.cn

[B13] 判断是否为数字
来源：https://nb.zhonguo2118.cn

Py:   isinstance(x, (int, float))
来源：https://sx.zhonguo7118.cn

PHP:  is_numeric($x)
来源：https://jd.zhonguo6118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fe.zhonguo1118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://dp.zhonguo8118.cn

Java: x instanceof Number
来源：https://mo.zhonguo5118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://dd.zhonguo7118.cn

Ruby: x.is_a?(Numeric)
来源：https://hm.zhonguo4118.cn

C#:   x is int or double or decimal
来源：https://rv.zhonguo5118.cn

[B14] 判断值是否在集合内
来源：https://ig.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://rh.zhonguo2118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://hy.zhonguo6118.cn

JS:   [1, 2, 3].includes(x)
来源：https://tu.zhonguo4118.cn

TS:   [1, 2, 3].includes(x)
来源：https://hu.zhonguo8118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://by.zhonguo7118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://yj.zhonguo3118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://gr.zhonguo3118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://mq.zhonguo2118.cn

[B15] 布尔运算与取反
来源：https://hm.zhonguo7118.cn

Py:   a and b or not c
来源：https://pe.zhonguo4118.cn

PHP:  $a && $b || !$c
来源：https://zc.zhonguo5118.cn

JS:   a && b || !c
来源：https://bz.zhonguo5118.cn

TS:   a && b || !c
来源：https://zd.zhonguo4118.cn

Java: a && b || !c
来源：https://qn.zhonguo1118.cn

Go:   a && b || !c
来源：https://rz.zhonguo6118.cn

Ruby: a && b || !c
来源：https://li.zhonguo6118.cn

C#:   a && b || !c
来源：https://bi.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://ok.zhonguo1118.cn

Py:   if not data: return
来源：https://za.zhonguo6118.cn

PHP:  if (!$data) { return; }
来源：https://vk.zhonguo7118.cn

JS:   if (!data) return;
来源：https://kw.zhonguo7118.cn

TS:   if (!data) return;
来源：https://ep.zhonguo4118.cn

Java: if (data == null) return;
来源：https://tl.zhonguo4118.cn

Go:   if data == nil { return }
来源：https://vp.zhonguo4118.cn

Ruby: return if data.nil?
来源：https://qy.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://ec.zhonguo8118.cn

================================================================================
来源：https://he.zhonguo1118.cn

C. 函数与作用域
来源：https://ay.zhonguo4118.cn

================================================================================
来源：https://cm.zhonguo6118.cn

[C01] 定义函数
来源：https://lz.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://xe.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://lj.zhonguo6118.cn

JS:   function add(a, b) { return a + b; }
来源：https://dw.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://cs.zhonguo6118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://as.zhonguo2118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://ru.zhonguo5118.cn

Ruby: def add(a, b); a + b; end
来源：https://cr.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ek.zhonguo1118.cn

[C02] 默认参数
来源：https://ms.zhonguo6118.cn

Py:   def greet(name="World"): return name
来源：https://ht.zhonguo8118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://lo.zhonguo8118.cn

JS:   function greet(name = "World") { return name; }
来源：https://zz.zhonguo8118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://kh.zhonguo1118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://lr.zhonguo3118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://te.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://pc.zhonguo1118.cn

C#:   string Greet(string name = "World") => name;
来源：https://rm.zhonguo3118.cn

[C03] 可变参数
来源：https://ei.zhonguo1118.cn

Py:   def total(*args): return sum(args)
来源：https://bq.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://do.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://zo.zhonguo3118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://xq.zhonguo8118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://be.zhonguo1118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://ah.zhonguo1118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://zq.zhonguo2118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://dr.zhonguo4118.cn

[C04] 命名参数 / 关键字参数
来源：https://lq.zhonguo3118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://bf.zhonguo8118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://yh.zhonguo1118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://uy.zhonguo1118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://cr.zhonguo6118.cn

Java: // 无：用 Builder 模式或 record
来源：https://te.zhonguo1118.cn

Go:   // 无：用配置结构体参数
来源：https://ky.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://ag.zhonguo8118.cn

C#:   f(a: 1, b: 2)
来源：https://ry.zhonguo2118.cn

[C05] 返回多个值
来源：https://nk.zhonguo6118.cn

Py:   return a, b
来源：https://lb.zhonguo3118.cn

PHP:  return [$a, $b];
来源：https://oy.zhonguo3118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://wk.zhonguo7118.cn

TS:   return { a, b };
来源：https://lv.zhonguo2118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://gp.zhonguo2118.cn

Go:   return a, b
来源：https://pb.zhonguo8118.cn

Ruby: return a, b
来源：https://kb.zhonguo3118.cn

C#:   return (a, b);              // ValueTuple
来源：https://bt.zhonguo6118.cn

[C06] 匿名函数 / lambda
来源：https://up.zhonguo5118.cn

Py:   square = lambda x: x * x
来源：https://uf.zhonguo3118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://vj.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://js.zhonguo3118.cn

TS:   const square = (x: number): number => x * x;
来源：https://cf.zhonguo7118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://fn.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://by.zhonguo2118.cn

Ruby: square = ->(x) { x * x }
来源：https://uc.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://vj.zhonguo8118.cn

[C07] 把函数作为参数传入
来源：https://bl.zhonguo7118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://pb.zhonguo4118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://ha.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://qu.zhonguo5118.cn

TS:   arr.map(String)
来源：https://dy.zhonguo2118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://bk.zhonguo5118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://ok.zhonguo1118.cn

Ruby: arr.map(&:upcase)
来源：https://xf.zhonguo6118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://tc.zhonguo2118.cn

[C08] 闭包
来源：https://qd.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ql.zhonguo4118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://sn.zhonguo4118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://fu.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://ap.zhonguo7118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://pt.zhonguo7118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://uw.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://wy.zhonguo8118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://qo.zhonguo3118.cn

[C09] 递归
来源：https://jg.zhonguo2118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ck.zhonguo4118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://tz.zhonguo5118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://rr.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://sj.zhonguo1118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://lo.zhonguo7118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://zs.zhonguo5118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://zr.zhonguo8118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://vo.zhonguo7118.cn

[C10] 变量作用域
来源：https://tz.zhonguo8118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://wk.zhonguo1118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://up.zhonguo7118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://ws.zhonguo4118.cn

TS:   同 JS
来源：https://gx.zhonguo5118.cn

Java: 方法内为块级作用域
来源：https://jl.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://qt.zhonguo6118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://ai.zhonguo1118.cn

C#:   块级作用域
来源：https://ff.zhonguo1118.cn

[C11] 模块导入与导出
来源：https://uw.zhonguo8118.cn

Py:   from module import func
来源：https://to.zhonguo1118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://ec.zhonguo6118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://yz.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://uy.zhonguo8118.cn

Java: import java.util.List;
来源：https://tt.zhonguo8118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://wd.zhonguo2118.cn

Ruby: require "json"; require_relative "./util"
来源：https://lz.zhonguo6118.cn

C#:   using System.Text;
来源：https://dg.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://mn.zhonguo5118.cn

Py:   (lambda: print("run"))()
来源：https://tf.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://sv.zhonguo6118.cn

JS:   (() => { console.log("run"); })();
来源：https://iq.zhonguo7118.cn

TS:   (() => { console.log("run"); })();
来源：https://aw.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://fy.zhonguo6118.cn

Go:   func() { fmt.Println("run") }()
来源：https://oo.zhonguo4118.cn

Ruby: -> { puts "run" }.call
来源：https://zs.zhonguo5118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://za.zhonguo8118.cn

[C13] 类型声明 / 类型注解
来源：https://id.zhonguo6118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://zm.zhonguo2118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://kq.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://ad.zhonguo7118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ay.zhonguo7118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://on.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://cd.zhonguo6118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://lm.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://md.zhonguo8118.cn

[C14] 泛型函数
来源：https://gr.zhonguo7118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ho.zhonguo8118.cn

PHP:  // 无泛型
来源：https://wt.zhonguo6118.cn

JS:   // 无泛型
来源：https://ce.zhonguo4118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://mb.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://qe.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ca.zhonguo3118.cn

Ruby: # 无泛型
来源：https://bp.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://ex.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://ty.zhonguo3118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://qq.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://ax.zhonguo1118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://by.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://vl.zhonguo1118.cn

Java: // 无解构
来源：https://lz.zhonguo1118.cn

Go:   // 无解构
来源：https://hr.zhonguo2118.cn

Ruby: a, b = pair
来源：https://yf.zhonguo8118.cn

C#:   var (a, b) = pair;
来源：https://br.zhonguo1118.cn

[C16] 函数 / 方法重载
来源：https://bm.zhonguo4118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://yj.zhonguo8118.cn

PHP:  // 无重载
来源：https://qq.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://uk.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://af.zhonguo8118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://km.zhonguo2118.cn

Go:   // 无重载：用不同函数名
来源：https://jh.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://sb.zhonguo4118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://od.zhonguo4118.cn

================================================================================
来源：https://lr.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://vm.zhonguo1118.cn

================================================================================
来源：https://iv.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://nu.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://pn.zhonguo8118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://uq.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ba.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://ik.zhonguo8118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://vb.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://if.zhonguo6118.cn

Ruby: arr = [1, 2, 3]
来源：https://xw.zhonguo1118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://yd.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://qw.zhonguo5118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://yd.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://br.zhonguo6118.cn

JS:   arr.push(4);
来源：https://fr.zhonguo2118.cn

TS:   arr.push(4);
来源：https://by.zhonguo4118.cn

Java: list.add(4);
来源：https://vc.zhonguo3118.cn

Go:   arr = append(arr, 4)
来源：https://nl.zhonguo7118.cn

Ruby: arr << 4; arr.push(5)
来源：https://ta.zhonguo7118.cn

C#:   list.Add(4);
来源：https://ts.zhonguo1118.cn

[D03] 在指定位置插入元素
来源：https://ke.zhonguo5118.cn

Py:   arr.insert(0, 0)
来源：https://dn.zhonguo8118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://pl.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://sp.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://sw.zhonguo8118.cn

Java: list.add(0, 0);
来源：https://dr.zhonguo6118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://gj.zhonguo7118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://mk.zhonguo6118.cn

C#:   list.Insert(0, 0);
来源：https://mp.zhonguo4118.cn

[D04] 删除元素
来源：https://ue.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://bj.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://lp.zhonguo1118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://lo.zhonguo8118.cn

TS:   arr.splice(0, 1);
来源：https://iu.zhonguo4118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://sy.zhonguo4118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://tk.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ne.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://ma.zhonguo8118.cn

[D05] 访问与修改元素
来源：https://iz.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://qw.zhonguo8118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://lh.zhonguo7118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://tg.zhonguo6118.cn

TS:   arr[0]; arr.at(-1);
来源：https://mc.zhonguo3118.cn

Java: list.get(0); list.set(0, 9);
来源：https://oj.zhonguo6118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ne.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://hd.zhonguo2118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://nx.zhonguo7118.cn

[D06] 数组长度
来源：https://ld.zhonguo7118.cn

Py:   len(arr)
来源：https://pd.zhonguo5118.cn

PHP:  count($arr);
来源：https://wk.zhonguo5118.cn

JS:   arr.length
来源：https://fj.zhonguo8118.cn

TS:   arr.length
来源：https://my.zhonguo7118.cn

Java: list.size();
来源：https://gl.zhonguo8118.cn

Go:   len(arr)
来源：https://lr.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://ux.zhonguo5118.cn

C#:   list.Count;
来源：https://us.zhonguo5118.cn

[D07] 切片 / 取子数组
来源：https://um.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://tl.zhonguo6118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://mh.zhonguo1118.cn

JS:   arr.slice(1, 4);
来源：https://pk.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://nj.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://lz.zhonguo1118.cn

Go:   arr[1:4]
来源：https://pt.zhonguo3118.cn

Ruby: arr[1, 3]
来源：https://is.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://rb.zhonguo3118.cn

[D08] 合并两个数组
来源：https://mo.zhonguo6118.cn

Py:   a + b;  a.extend(b)
来源：https://ch.zhonguo7118.cn

PHP:  array_merge($a, $b);
来源：https://vk.zhonguo4118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://co.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://xu.zhonguo3118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ej.zhonguo6118.cn

Go:   append(a, b...)
来源：https://nx.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://yk.zhonguo5118.cn

C#:   a.Concat(b).ToList()
来源：https://kf.zhonguo3118.cn

[D09] 排序（升序）
来源：https://aw.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ih.zhonguo7118.cn

PHP:  sort($arr);
来源：https://kk.zhonguo5118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://ns.zhonguo8118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://tg.zhonguo2118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://lf.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://om.zhonguo2118.cn

Ruby: arr.sort
来源：https://dr.zhonguo2118.cn

C#:   list.Sort();
来源：https://ga.zhonguo4118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://xm.zhonguo6118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://gd.zhonguo3118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ic.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://hf.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ek.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://zg.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ar.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://cx.zhonguo4118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://ca.zhonguo8118.cn

[D11] 反转数组
来源：https://ud.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://ba.zhonguo5118.cn

PHP:  array_reverse($arr);
来源：https://ws.zhonguo6118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://iz.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://qe.zhonguo2118.cn

Java: Collections.reverse(list);
来源：https://zh.zhonguo3118.cn

Go:   slices.Reverse(arr)
来源：https://yv.zhonguo7118.cn

Ruby: arr.reverse
来源：https://ii.zhonguo1118.cn

C#:   list.Reverse();
来源：https://pa.zhonguo4118.cn

[D12] 查找元素下标
来源：https://lx.zhonguo8118.cn

Py:   arr.index(x);  x in arr
来源：https://ex.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://sl.zhonguo4118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ll.zhonguo5118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://az.zhonguo3118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://ov.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://gp.zhonguo5118.cn

Ruby: arr.index(x)
来源：https://bl.zhonguo7118.cn

C#:   list.IndexOf(x);
来源：https://nt.zhonguo4118.cn

[D13] 过滤（保留满足条件的）
来源：https://is.zhonguo1118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://nr.zhonguo7118.cn


<!-- 参考信息 -->