代发 wailian999

================================================================================
来源：https://rf.zhonguo6118.cn

C. 函数与作用域
来源：https://lc.zhonguo8118.cn

================================================================================
来源：https://dy.zhonguo8118.cn

[C01] 定义函数
来源：https://sf.zhonguo1118.cn

Py:   def add(a, b): return a + b
来源：https://cd.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://hz.zhonguo6118.cn

JS:   function add(a, b) { return a + b; }
来源：https://qo.zhonguo4118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://tr.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://jn.zhonguo5118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://qz.zhonguo1118.cn

Ruby: def add(a, b); a + b; end
来源：https://ge.zhonguo4118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://zz.zhonguo2118.cn

[C02] 默认参数
来源：https://hx.zhonguo8118.cn

Py:   def greet(name="World"): return name
来源：https://ih.zhonguo5118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://ai.zhonguo1118.cn

JS:   function greet(name = "World") { return name; }
来源：https://wx.zhonguo5118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://tz.zhonguo3118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://qv.zhonguo2118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://fp.zhonguo6118.cn

Ruby: def greet(name = "World") = name
来源：https://ub.zhonguo3118.cn

C#:   string Greet(string name = "World") => name;
来源：https://jj.zhonguo8118.cn

[C03] 可变参数
来源：https://um.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://uv.zhonguo3118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://zl.zhonguo5118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://ei.zhonguo4118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://wo.zhonguo5118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://ch.zhonguo4118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://lq.zhonguo7118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://yd.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://jn.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://gz.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://au.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://jg.zhonguo6118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://yp.zhonguo7118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://ov.zhonguo4118.cn

Java: // 无：用 Builder 模式或 record
来源：https://jz.zhonguo8118.cn

Go:   // 无：用配置结构体参数
来源：https://hg.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://ex.zhonguo2118.cn

C#:   f(a: 1, b: 2)
来源：https://cz.zhonguo7118.cn

[C05] 返回多个值
来源：https://ea.zhonguo1118.cn

Py:   return a, b
来源：https://ti.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://aw.zhonguo4118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://vy.zhonguo8118.cn

TS:   return { a, b };
来源：https://bl.zhonguo8118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ae.zhonguo6118.cn

Go:   return a, b
来源：https://gt.zhonguo4118.cn

Ruby: return a, b
来源：https://uy.zhonguo3118.cn

C#:   return (a, b);              // ValueTuple
来源：https://hl.zhonguo8118.cn

[C06] 匿名函数 / lambda
来源：https://mk.zhonguo7118.cn

Py:   square = lambda x: x * x
来源：https://de.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://ig.zhonguo1118.cn

JS:   const square = x => x * x;
来源：https://gg.zhonguo2118.cn

TS:   const square = (x: number): number => x * x;
来源：https://yy.zhonguo1118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://ia.zhonguo3118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://gb.zhonguo2118.cn

Ruby: square = ->(x) { x * x }
来源：https://pt.zhonguo1118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://cr.zhonguo6118.cn

[C07] 把函数作为参数传入
来源：https://jd.zhonguo8118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://ho.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://yn.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://qe.zhonguo5118.cn

TS:   arr.map(String)
来源：https://xo.zhonguo3118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://fr.zhonguo6118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://ju.zhonguo8118.cn

Ruby: arr.map(&:upcase)
来源：https://qt.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://mk.zhonguo7118.cn

[C08] 闭包
来源：https://bk.zhonguo3118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://cv.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://rn.zhonguo4118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://oh.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://ro.zhonguo3118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://cb.zhonguo2118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://xf.zhonguo6118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://te.zhonguo8118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://xr.zhonguo6118.cn

[C09] 递归
来源：https://qi.zhonguo7118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://tt.zhonguo7118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://mc.zhonguo1118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://yq.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://zo.zhonguo2118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://yy.zhonguo5118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ys.zhonguo4118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://bd.zhonguo7118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://rf.zhonguo7118.cn

[C10] 变量作用域
来源：https://kc.zhonguo4118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://jn.zhonguo6118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://pc.zhonguo1118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://zi.zhonguo8118.cn

TS:   同 JS
来源：https://rn.zhonguo4118.cn

Java: 方法内为块级作用域
来源：https://zu.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://ge.zhonguo6118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://xe.zhonguo5118.cn

C#:   块级作用域
来源：https://ih.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://fq.zhonguo5118.cn

Py:   from module import func
来源：https://my.zhonguo7118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://lz.zhonguo8118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://tl.zhonguo6118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://rv.zhonguo8118.cn

Java: import java.util.List;
来源：https://ob.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://cx.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://zi.zhonguo2118.cn

C#:   using System.Text;
来源：https://pr.zhonguo1118.cn

[C12] 立即执行函数 IIFE
来源：https://ur.zhonguo8118.cn

Py:   (lambda: print("run"))()
来源：https://kv.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://if.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://hf.zhonguo6118.cn

TS:   (() => { console.log("run"); })();
来源：https://rv.zhonguo2118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://cz.zhonguo7118.cn

Go:   func() { fmt.Println("run") }()
来源：https://ty.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://zn.zhonguo6118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://rl.zhonguo6118.cn

[C13] 类型声明 / 类型注解
来源：https://vr.zhonguo6118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://eu.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://lj.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://mv.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://rj.zhonguo6118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://is.zhonguo5118.cn

Go:   func add(a, b int) int
来源：https://rr.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://sr.zhonguo5118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://ks.zhonguo3118.cn

[C14] 泛型函数
来源：https://rg.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ez.zhonguo4118.cn

PHP:  // 无泛型
来源：https://up.zhonguo3118.cn

JS:   // 无泛型
来源：https://pv.zhonguo4118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://pl.zhonguo8118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://bc.zhonguo1118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://cr.zhonguo4118.cn

Ruby: # 无泛型
来源：https://yx.zhonguo2118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://yq.zhonguo3118.cn

[C15] 解构 / 展开参数
来源：https://id.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ez.zhonguo2118.cn

PHP:  [$a, $b] = $pair;
来源：https://uu.zhonguo2118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://zc.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://xo.zhonguo2118.cn

Java: // 无解构
来源：https://kb.zhonguo5118.cn

Go:   // 无解构
来源：https://xx.zhonguo8118.cn

Ruby: a, b = pair
来源：https://tp.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://qy.zhonguo1118.cn

[C16] 函数 / 方法重载
来源：https://vw.zhonguo1118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://bg.zhonguo5118.cn

PHP:  // 无重载
来源：https://he.zhonguo3118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://gu.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://nu.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://sx.zhonguo5118.cn

Go:   // 无重载：用不同函数名
来源：https://tf.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://ea.zhonguo2118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://rs.zhonguo1118.cn

================================================================================
来源：https://fk.zhonguo6118.cn

D. 数组 / 列表 / 集合
来源：https://vt.zhonguo6118.cn

================================================================================
来源：https://xk.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://km.zhonguo5118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://gu.zhonguo7118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://va.zhonguo3118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ln.zhonguo3118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://hq.zhonguo6118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://di.zhonguo1118.cn

Go:   arr := []int{1, 2, 3}
来源：https://vv.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://gd.zhonguo6118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://rn.zhonguo6118.cn

[D02] 追加元素到末尾
来源：https://dv.zhonguo7118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://qf.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ei.zhonguo1118.cn

JS:   arr.push(4);
来源：https://un.zhonguo8118.cn

TS:   arr.push(4);
来源：https://fd.zhonguo2118.cn

Java: list.add(4);
来源：https://zg.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://ru.zhonguo1118.cn

Ruby: arr << 4; arr.push(5)
来源：https://vn.zhonguo2118.cn

C#:   list.Add(4);
来源：https://ja.zhonguo5118.cn

[D03] 在指定位置插入元素
来源：https://lh.zhonguo8118.cn

Py:   arr.insert(0, 0)
来源：https://aw.zhonguo7118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://pm.zhonguo6118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://mb.zhonguo7118.cn

TS:   arr.splice(0, 0, 0);
来源：https://du.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://je.zhonguo6118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://cs.zhonguo1118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://op.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://gp.zhonguo4118.cn

[D04] 删除元素
来源：https://vy.zhonguo8118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://jw.zhonguo1118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ci.zhonguo4118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://by.zhonguo7118.cn

TS:   arr.splice(0, 1);
来源：https://eh.zhonguo5118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://qm.zhonguo7118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://so.zhonguo3118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://qo.zhonguo3118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://ij.zhonguo6118.cn

[D05] 访问与修改元素
来源：https://zp.zhonguo8118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://jv.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://eh.zhonguo3118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://sr.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ji.zhonguo5118.cn

Java: list.get(0); list.set(0, 9);
来源：https://sn.zhonguo4118.cn

Go:   arr[0]; arr[0] = 9
来源：https://nk.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://vu.zhonguo8118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://qg.zhonguo1118.cn

[D06] 数组长度
来源：https://qg.zhonguo2118.cn

Py:   len(arr)
来源：https://cg.zhonguo7118.cn

PHP:  count($arr);
来源：https://sj.zhonguo5118.cn

JS:   arr.length
来源：https://pv.zhonguo7118.cn

TS:   arr.length
来源：https://xe.zhonguo6118.cn

Java: list.size();
来源：https://oa.zhonguo5118.cn

Go:   len(arr)
来源：https://fy.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://fx.zhonguo2118.cn

C#:   list.Count;
来源：https://nq.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://fj.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://iy.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://or.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://nt.zhonguo3118.cn

TS:   arr.slice(1, 4);
来源：https://kd.zhonguo2118.cn

Java: list.subList(1, 4);
来源：https://vm.zhonguo5118.cn

Go:   arr[1:4]
来源：https://dh.zhonguo7118.cn

Ruby: arr[1, 3]
来源：https://yl.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://bd.zhonguo2118.cn

[D08] 合并两个数组
来源：https://sn.zhonguo8118.cn

Py:   a + b;  a.extend(b)
来源：https://al.zhonguo2118.cn

PHP:  array_merge($a, $b);
来源：https://pm.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://mb.zhonguo7118.cn

TS:   [...a, ...b];
来源：https://ym.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://kc.zhonguo7118.cn

Go:   append(a, b...)
来源：https://ye.zhonguo5118.cn

Ruby: a + b;  a.concat(b)
来源：https://hn.zhonguo2118.cn

C#:   a.Concat(b).ToList()
来源：https://aq.zhonguo7118.cn

[D09] 排序（升序）
来源：https://xx.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pp.zhonguo6118.cn

PHP:  sort($arr);
来源：https://sj.zhonguo8118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://xj.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://bx.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://eo.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://zn.zhonguo4118.cn

Ruby: arr.sort
来源：https://mw.zhonguo8118.cn

C#:   list.Sort();
来源：https://jb.zhonguo4118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://gl.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://tm.zhonguo2118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ud.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://fp.zhonguo4118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://qr.zhonguo1118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://mu.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://lh.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://bp.zhonguo3118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://ec.zhonguo5118.cn

[D11] 反转数组
来源：https://gt.zhonguo5118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://pj.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://qw.zhonguo1118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://as.zhonguo5118.cn

TS:   [...arr].reverse();
来源：https://tx.zhonguo5118.cn

Java: Collections.reverse(list);
来源：https://xg.zhonguo7118.cn

Go:   slices.Reverse(arr)
来源：https://hf.zhonguo6118.cn

Ruby: arr.reverse
来源：https://pv.zhonguo5118.cn

C#:   list.Reverse();
来源：https://jm.zhonguo2118.cn

[D12] 查找元素下标
来源：https://ad.zhonguo1118.cn

Py:   arr.index(x);  x in arr
来源：https://ub.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://ch.zhonguo6118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://dq.zhonguo3118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ay.zhonguo3118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://lw.zhonguo1118.cn

Go:   slices.Index(arr, x)
来源：https://kl.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://er.zhonguo7118.cn

C#:   list.IndexOf(x);
来源：https://ko.zhonguo2118.cn

[D13] 过滤（保留满足条件的）
来源：https://ly.zhonguo2118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://by.zhonguo5118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://dd.zhonguo6118.cn

JS:   arr.filter(x => x > 3)
来源：https://zq.zhonguo5118.cn

TS:   arr.filter(x => x > 3)
来源：https://ji.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://wa.zhonguo5118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://ez.zhonguo3118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://yb.zhonguo4118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://lr.zhonguo1118.cn

[D14] 映射转换（每个元素变形）
来源：https://ko.zhonguo8118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://sz.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://by.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://eq.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://ak.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://dd.zhonguo7118.cn

Go:   // 手写循环
来源：https://bt.zhonguo5118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vh.zhonguo1118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://le.zhonguo1118.cn

[D15] 去重
来源：https://qf.zhonguo3118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ym.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://mq.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://og.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://uq.zhonguo6118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://uo.zhonguo2118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ro.zhonguo7118.cn

Ruby: arr.uniq
来源：https://aq.zhonguo3118.cn

C#:   list.Distinct().ToList()
来源：https://ed.zhonguo1118.cn

[D16] 求和与平均值
来源：https://hn.zhonguo6118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://ma.zhonguo7118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ar.zhonguo8118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://fp.zhonguo2118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://nc.zhonguo7118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://fi.zhonguo3118.cn

Go:   // 手写循环累加
来源：https://wq.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://hk.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://jn.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://uh.zhonguo8118.cn

Py:   max(arr);  min(arr)
来源：https://vk.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://ah.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://ha.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://dg.zhonguo4118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://nu.zhonguo7118.cn


<!-- 参考信息 -->