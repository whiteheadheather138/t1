代发 wailian999

Py:   if not data: return
来源：https://nc.zhonguo7118.cn

PHP:  if (!$data) { return; }
来源：https://ce.zhonguo7118.cn

JS:   if (!data) return;
来源：https://ci.zhonguo8118.cn

TS:   if (!data) return;
来源：https://xa.zhonguo4118.cn

Java: if (data == null) return;
来源：https://ug.zhonguo2118.cn

Go:   if data == nil { return }
来源：https://eg.zhonguo5118.cn

Ruby: return if data.nil?
来源：https://di.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://ev.zhonguo2118.cn

================================================================================
来源：https://jl.zhonguo3118.cn

C. 函数与作用域
来源：https://fy.zhonguo7118.cn

================================================================================
来源：https://yb.zhonguo1118.cn

[C01] 定义函数
来源：https://rg.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://mc.zhonguo7118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://wb.zhonguo1118.cn

JS:   function add(a, b) { return a + b; }
来源：https://hj.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://zf.zhonguo2118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://am.zhonguo3118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://ys.zhonguo7118.cn

Ruby: def add(a, b); a + b; end
来源：https://gg.zhonguo5118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://fp.zhonguo7118.cn

[C02] 默认参数
来源：https://tr.zhonguo7118.cn

Py:   def greet(name="World"): return name
来源：https://dj.zhonguo1118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://ev.zhonguo6118.cn

JS:   function greet(name = "World") { return name; }
来源：https://du.zhonguo2118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://rq.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://af.zhonguo1118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://na.zhonguo7118.cn

Ruby: def greet(name = "World") = name
来源：https://tx.zhonguo2118.cn

C#:   string Greet(string name = "World") => name;
来源：https://zo.zhonguo2118.cn

[C03] 可变参数
来源：https://ry.zhonguo7118.cn

Py:   def total(*args): return sum(args)
来源：https://mm.zhonguo4118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://gr.zhonguo3118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://tm.zhonguo4118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://un.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://mj.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://jy.zhonguo5118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ap.zhonguo2118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://wa.zhonguo7118.cn

[C04] 命名参数 / 关键字参数
来源：https://dw.zhonguo4118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://bl.zhonguo6118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://dy.zhonguo8118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://pp.zhonguo7118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://as.zhonguo3118.cn

Java: // 无：用 Builder 模式或 record
来源：https://ak.zhonguo1118.cn

Go:   // 无：用配置结构体参数
来源：https://td.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://qn.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://tn.zhonguo6118.cn

[C05] 返回多个值
来源：https://fm.zhonguo1118.cn

Py:   return a, b
来源：https://hx.zhonguo5118.cn

PHP:  return [$a, $b];
来源：https://dq.zhonguo3118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://tj.zhonguo7118.cn

TS:   return { a, b };
来源：https://sg.zhonguo5118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://sv.zhonguo7118.cn

Go:   return a, b
来源：https://mp.zhonguo6118.cn

Ruby: return a, b
来源：https://id.zhonguo6118.cn

C#:   return (a, b);              // ValueTuple
来源：https://ez.zhonguo1118.cn

[C06] 匿名函数 / lambda
来源：https://gc.zhonguo2118.cn

Py:   square = lambda x: x * x
来源：https://yr.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://mb.zhonguo6118.cn

JS:   const square = x => x * x;
来源：https://sq.zhonguo1118.cn

TS:   const square = (x: number): number => x * x;
来源：https://wx.zhonguo7118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://mh.zhonguo1118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://fe.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://ky.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://lh.zhonguo8118.cn

[C07] 把函数作为参数传入
来源：https://kg.zhonguo3118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://gv.zhonguo2118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://iy.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://rn.zhonguo3118.cn

TS:   arr.map(String)
来源：https://eu.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://qh.zhonguo4118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://xj.zhonguo7118.cn

Ruby: arr.map(&:upcase)
来源：https://rs.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://hk.zhonguo7118.cn

[C08] 闭包
来源：https://dr.zhonguo7118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://bv.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://id.zhonguo8118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://ni.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://fj.zhonguo7118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://fw.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://ie.zhonguo5118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ri.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://jn.zhonguo7118.cn

[C09] 递归
来源：https://ee.zhonguo2118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ew.zhonguo8118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://nr.zhonguo4118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://cy.zhonguo6118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://pd.zhonguo8118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://ha.zhonguo6118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ux.zhonguo8118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://aa.zhonguo2118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://gw.zhonguo5118.cn

[C10] 变量作用域
来源：https://ge.zhonguo7118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ql.zhonguo6118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ph.zhonguo8118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://vb.zhonguo4118.cn

TS:   同 JS
来源：https://mf.zhonguo7118.cn

Java: 方法内为块级作用域
来源：https://ya.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://go.zhonguo1118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://ty.zhonguo4118.cn

C#:   块级作用域
来源：https://ta.zhonguo2118.cn

[C11] 模块导入与导出
来源：https://er.zhonguo4118.cn

Py:   from module import func
来源：https://jw.zhonguo3118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://wb.zhonguo1118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://do.zhonguo3118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://im.zhonguo5118.cn

Java: import java.util.List;
来源：https://gc.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://hg.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://vf.zhonguo5118.cn

C#:   using System.Text;
来源：https://lv.zhonguo5118.cn

[C12] 立即执行函数 IIFE
来源：https://tv.zhonguo1118.cn

Py:   (lambda: print("run"))()
来源：https://zv.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://jh.zhonguo8118.cn

JS:   (() => { console.log("run"); })();
来源：https://ck.zhonguo3118.cn

TS:   (() => { console.log("run"); })();
来源：https://vp.zhonguo8118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://bb.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://jo.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://hw.zhonguo5118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://tm.zhonguo7118.cn

[C13] 类型声明 / 类型注解
来源：https://xm.zhonguo2118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://zg.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://wz.zhonguo2118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://id.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://wx.zhonguo5118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://vi.zhonguo3118.cn

Go:   func add(a, b int) int
来源：https://kl.zhonguo2118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://wx.zhonguo4118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://nm.zhonguo5118.cn

[C14] 泛型函数
来源：https://qj.zhonguo7118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://zb.zhonguo2118.cn

PHP:  // 无泛型
来源：https://fa.zhonguo8118.cn

JS:   // 无泛型
来源：https://ch.zhonguo2118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://kl.zhonguo8118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://eh.zhonguo1118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://yj.zhonguo6118.cn

Ruby: # 无泛型
来源：https://sl.zhonguo5118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://vt.zhonguo8118.cn

[C15] 解构 / 展开参数
来源：https://oe.zhonguo4118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://zb.zhonguo3118.cn

PHP:  [$a, $b] = $pair;
来源：https://xu.zhonguo3118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://yq.zhonguo3118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://um.zhonguo6118.cn

Java: // 无解构
来源：https://na.zhonguo6118.cn

Go:   // 无解构
来源：https://zc.zhonguo1118.cn

Ruby: a, b = pair
来源：https://wy.zhonguo2118.cn

C#:   var (a, b) = pair;
来源：https://mx.zhonguo5118.cn

[C16] 函数 / 方法重载
来源：https://qx.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://zp.zhonguo7118.cn

PHP:  // 无重载
来源：https://ue.zhonguo7118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ma.zhonguo8118.cn

TS:   // 用联合类型或重载签名声明
来源：https://se.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ui.zhonguo2118.cn

Go:   // 无重载：用不同函数名
来源：https://hq.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://mv.zhonguo4118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://wa.zhonguo8118.cn

================================================================================
来源：https://cc.zhonguo7118.cn

D. 数组 / 列表 / 集合
来源：https://kj.zhonguo1118.cn

================================================================================
来源：https://ec.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://he.zhonguo6118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://pe.zhonguo1118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://cv.zhonguo5118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://hr.zhonguo2118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://gt.zhonguo6118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://go.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://om.zhonguo4118.cn

Ruby: arr = [1, 2, 3]
来源：https://na.zhonguo6118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://hr.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://gq.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://xx.zhonguo8118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://et.zhonguo1118.cn

JS:   arr.push(4);
来源：https://xf.zhonguo6118.cn

TS:   arr.push(4);
来源：https://ec.zhonguo1118.cn

Java: list.add(4);
来源：https://jk.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://xc.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://mn.zhonguo6118.cn

C#:   list.Add(4);
来源：https://tu.zhonguo8118.cn

[D03] 在指定位置插入元素
来源：https://hc.zhonguo7118.cn

Py:   arr.insert(0, 0)
来源：https://il.zhonguo1118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://bi.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://ai.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://tz.zhonguo6118.cn

Java: list.add(0, 0);
来源：https://ro.zhonguo8118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://of.zhonguo4118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://qa.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://ri.zhonguo6118.cn

[D04] 删除元素
来源：https://dl.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://jm.zhonguo6118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://jx.zhonguo7118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://xh.zhonguo7118.cn

TS:   arr.splice(0, 1);
来源：https://lj.zhonguo7118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://gw.zhonguo5118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ph.zhonguo6118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://lw.zhonguo3118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://tq.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://qw.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ho.zhonguo3118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://xq.zhonguo6118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://oh.zhonguo8118.cn

TS:   arr[0]; arr.at(-1);
来源：https://tr.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://qs.zhonguo7118.cn

Go:   arr[0]; arr[0] = 9
来源：https://yy.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://pm.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://xo.zhonguo3118.cn

[D06] 数组长度
来源：https://gy.zhonguo6118.cn

Py:   len(arr)
来源：https://py.zhonguo8118.cn

PHP:  count($arr);
来源：https://ut.zhonguo5118.cn

JS:   arr.length
来源：https://ow.zhonguo1118.cn

TS:   arr.length
来源：https://rz.zhonguo1118.cn

Java: list.size();
来源：https://ct.zhonguo3118.cn

Go:   len(arr)
来源：https://kh.zhonguo4118.cn

Ruby: arr.length; arr.size
来源：https://cs.zhonguo1118.cn

C#:   list.Count;
来源：https://xx.zhonguo2118.cn

[D07] 切片 / 取子数组
来源：https://nl.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://nc.zhonguo4118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://ep.zhonguo1118.cn

JS:   arr.slice(1, 4);
来源：https://xo.zhonguo5118.cn

TS:   arr.slice(1, 4);
来源：https://dh.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://xa.zhonguo1118.cn

Go:   arr[1:4]
来源：https://uw.zhonguo2118.cn

Ruby: arr[1, 3]
来源：https://oy.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://mo.zhonguo4118.cn

[D08] 合并两个数组
来源：https://mz.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://uz.zhonguo3118.cn

PHP:  array_merge($a, $b);
来源：https://zo.zhonguo6118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://cn.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://ti.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://uu.zhonguo4118.cn

Go:   append(a, b...)
来源：https://oz.zhonguo5118.cn

Ruby: a + b;  a.concat(b)
来源：https://lb.zhonguo2118.cn

C#:   a.Concat(b).ToList()
来源：https://wc.zhonguo6118.cn

[D09] 排序（升序）
来源：https://wz.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://im.zhonguo3118.cn

PHP:  sort($arr);
来源：https://mv.zhonguo2118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://jm.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://xs.zhonguo5118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://kn.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://yl.zhonguo3118.cn

Ruby: arr.sort
来源：https://ki.zhonguo8118.cn

C#:   list.Sort();
来源：https://ha.zhonguo8118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://xn.zhonguo2118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://fo.zhonguo2118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://qr.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://uk.zhonguo8118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://mv.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://nh.zhonguo2118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://fx.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://vz.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://ls.zhonguo7118.cn

[D11] 反转数组
来源：https://vc.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://rs.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://lt.zhonguo3118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://vr.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://np.zhonguo2118.cn

Java: Collections.reverse(list);
来源：https://sp.zhonguo6118.cn

Go:   slices.Reverse(arr)
来源：https://xo.zhonguo8118.cn

Ruby: arr.reverse
来源：https://jw.zhonguo1118.cn

C#:   list.Reverse();
来源：https://ji.zhonguo3118.cn

[D12] 查找元素下标
来源：https://la.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://ws.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://bf.zhonguo7118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://kt.zhonguo4118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://iw.zhonguo6118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://xu.zhonguo6118.cn

Go:   slices.Index(arr, x)
来源：https://ti.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://ow.zhonguo7118.cn

C#:   list.IndexOf(x);
来源：https://nc.zhonguo6118.cn

[D13] 过滤（保留满足条件的）
来源：https://fk.zhonguo8118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://cr.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://vw.zhonguo2118.cn

JS:   arr.filter(x => x > 3)
来源：https://en.zhonguo4118.cn

TS:   arr.filter(x => x > 3)
来源：https://cq.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://tc.zhonguo4118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://mh.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://jr.zhonguo1118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ly.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://gj.zhonguo1118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://he.zhonguo2118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://sa.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://ai.zhonguo2118.cn

TS:   arr.map(x => x * 2)
来源：https://nx.zhonguo3118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://kc.zhonguo7118.cn

Go:   // 手写循环
来源：https://jg.zhonguo6118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://mr.zhonguo2118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://of.zhonguo6118.cn

[D15] 去重
来源：https://tc.zhonguo2118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://vs.zhonguo7118.cn

PHP:  array_unique($arr);
来源：https://wo.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://rh.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://au.zhonguo2118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://rb.zhonguo4118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://vu.zhonguo5118.cn

Ruby: arr.uniq
来源：https://dz.zhonguo4118.cn

C#:   list.Distinct().ToList()
来源：https://fj.zhonguo1118.cn

[D16] 求和与平均值
来源：https://rz.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://cw.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://xx.zhonguo7118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://nw.zhonguo4118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://cm.zhonguo3118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://nl.zhonguo4118.cn

Go:   // 手写循环累加
来源：https://ty.zhonguo2118.cn


<!-- 参考信息 -->