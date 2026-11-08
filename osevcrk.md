代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：https://hj.zhonguo2118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://uc.zhonguo5118.cn

[B15] 布尔运算与取反
来源：https://kp.zhonguo3118.cn

Py:   a and b or not c
来源：https://ia.zhonguo8118.cn

PHP:  $a && $b || !$c
来源：https://vd.zhonguo8118.cn

JS:   a && b || !c
来源：https://rm.zhonguo6118.cn

TS:   a && b || !c
来源：https://tz.zhonguo8118.cn

Java: a && b || !c
来源：https://yj.zhonguo3118.cn

Go:   a && b || !c
来源：https://ti.zhonguo2118.cn

Ruby: a && b || !c
来源：https://di.zhonguo6118.cn

C#:   a && b || !c
来源：https://lm.zhonguo4118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://hs.zhonguo8118.cn

Py:   if not data: return
来源：https://nx.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://tn.zhonguo8118.cn

JS:   if (!data) return;
来源：https://ze.zhonguo1118.cn

TS:   if (!data) return;
来源：https://rg.zhonguo5118.cn

Java: if (data == null) return;
来源：https://vh.zhonguo3118.cn

Go:   if data == nil { return }
来源：https://yc.zhonguo2118.cn

Ruby: return if data.nil?
来源：https://hw.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://pg.zhonguo8118.cn

================================================================================
来源：https://md.zhonguo3118.cn

C. 函数与作用域
来源：https://ey.zhonguo2118.cn

================================================================================
来源：https://ym.zhonguo1118.cn

[C01] 定义函数
来源：https://zo.zhonguo6118.cn

Py:   def add(a, b): return a + b
来源：https://rt.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://od.zhonguo6118.cn

JS:   function add(a, b) { return a + b; }
来源：https://ri.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://st.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://hw.zhonguo1118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://ra.zhonguo3118.cn

Ruby: def add(a, b); a + b; end
来源：https://ou.zhonguo8118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://wh.zhonguo6118.cn

[C02] 默认参数
来源：https://lg.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://bn.zhonguo4118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://oj.zhonguo6118.cn

JS:   function greet(name = "World") { return name; }
来源：https://ud.zhonguo2118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://fw.zhonguo8118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://gr.zhonguo7118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://jf.zhonguo2118.cn

Ruby: def greet(name = "World") = name
来源：https://se.zhonguo6118.cn

C#:   string Greet(string name = "World") => name;
来源：https://tp.zhonguo3118.cn

[C03] 可变参数
来源：https://uv.zhonguo2118.cn

Py:   def total(*args): return sum(args)
来源：https://zj.zhonguo5118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://iz.zhonguo6118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://av.zhonguo6118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://fp.zhonguo8118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://dg.zhonguo5118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://hz.zhonguo3118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ni.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://fs.zhonguo8118.cn

[C04] 命名参数 / 关键字参数
来源：https://wm.zhonguo5118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ko.zhonguo1118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://uo.zhonguo8118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://ro.zhonguo4118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://wx.zhonguo6118.cn

Java: // 无：用 Builder 模式或 record
来源：https://nk.zhonguo3118.cn

Go:   // 无：用配置结构体参数
来源：https://hr.zhonguo3118.cn

Ruby: f(a: 1, b: 2)
来源：https://jk.zhonguo5118.cn

C#:   f(a: 1, b: 2)
来源：https://vd.zhonguo1118.cn

[C05] 返回多个值
来源：https://qe.zhonguo8118.cn

Py:   return a, b
来源：https://ch.zhonguo2118.cn

PHP:  return [$a, $b];
来源：https://io.zhonguo3118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://lf.zhonguo1118.cn

TS:   return { a, b };
来源：https://le.zhonguo6118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://tg.zhonguo4118.cn

Go:   return a, b
来源：https://le.zhonguo3118.cn

Ruby: return a, b
来源：https://fi.zhonguo5118.cn

C#:   return (a, b);              // ValueTuple
来源：https://mz.zhonguo2118.cn

[C06] 匿名函数 / lambda
来源：https://zx.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://xg.zhonguo3118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://gi.zhonguo5118.cn

JS:   const square = x => x * x;
来源：https://on.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://lm.zhonguo3118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://mj.zhonguo1118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://dg.zhonguo3118.cn

Ruby: square = ->(x) { x * x }
来源：https://ij.zhonguo7118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://im.zhonguo8118.cn

[C07] 把函数作为参数传入
来源：https://su.zhonguo6118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://fw.zhonguo6118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://km.zhonguo7118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://bd.zhonguo1118.cn

TS:   arr.map(String)
来源：https://dx.zhonguo7118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://vo.zhonguo8118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://jx.zhonguo8118.cn

Ruby: arr.map(&:upcase)
来源：https://pi.zhonguo6118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://iz.zhonguo2118.cn

[C08] 闭包
来源：https://eu.zhonguo3118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://cf.zhonguo2118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://wr.zhonguo1118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://md.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://lc.zhonguo6118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://zr.zhonguo2118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://fe.zhonguo4118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://aq.zhonguo3118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://kt.zhonguo6118.cn

[C09] 递归
来源：https://ac.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ur.zhonguo3118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://dp.zhonguo5118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://fg.zhonguo7118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://pe.zhonguo7118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://rc.zhonguo3118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://nz.zhonguo8118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://me.zhonguo2118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://la.zhonguo7118.cn

[C10] 变量作用域
来源：https://np.zhonguo2118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ue.zhonguo2118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ju.zhonguo1118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://nd.zhonguo3118.cn

TS:   同 JS
来源：https://ee.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://ae.zhonguo5118.cn

Go:   花括号块级作用域
来源：https://ph.zhonguo5118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://uo.zhonguo7118.cn

C#:   块级作用域
来源：https://vf.zhonguo7118.cn

[C11] 模块导入与导出
来源：https://ke.zhonguo6118.cn

Py:   from module import func
来源：https://ft.zhonguo7118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://fx.zhonguo3118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://ac.zhonguo2118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://yw.zhonguo2118.cn

Java: import java.util.List;
来源：https://rl.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://uk.zhonguo4118.cn

Ruby: require "json"; require_relative "./util"
来源：https://td.zhonguo8118.cn

C#:   using System.Text;
来源：https://sq.zhonguo4118.cn

[C12] 立即执行函数 IIFE
来源：https://lq.zhonguo7118.cn

Py:   (lambda: print("run"))()
来源：https://sb.zhonguo4118.cn

PHP:  (function () { echo "run"; })();
来源：https://nx.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://lb.zhonguo3118.cn

TS:   (() => { console.log("run"); })();
来源：https://nj.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://td.zhonguo2118.cn

Go:   func() { fmt.Println("run") }()
来源：https://qa.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://sf.zhonguo2118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://zc.zhonguo6118.cn

[C13] 类型声明 / 类型注解
来源：https://ns.zhonguo2118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://jv.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://nd.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://th.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://mm.zhonguo2118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://vi.zhonguo6118.cn

Go:   func add(a, b int) int
来源：https://lz.zhonguo2118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ej.zhonguo3118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://pb.zhonguo4118.cn

[C14] 泛型函数
来源：https://kb.zhonguo3118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://co.zhonguo8118.cn

PHP:  // 无泛型
来源：https://av.zhonguo2118.cn

JS:   // 无泛型
来源：https://sa.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://jt.zhonguo6118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://hz.zhonguo5118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://mk.zhonguo2118.cn

Ruby: # 无泛型
来源：https://yb.zhonguo8118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://xi.zhonguo4118.cn

[C15] 解构 / 展开参数
来源：https://mk.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://bs.zhonguo8118.cn

PHP:  [$a, $b] = $pair;
来源：https://nd.zhonguo4118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://lk.zhonguo2118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://zo.zhonguo6118.cn

Java: // 无解构
来源：https://bq.zhonguo8118.cn

Go:   // 无解构
来源：https://md.zhonguo8118.cn

Ruby: a, b = pair
来源：https://jk.zhonguo6118.cn

C#:   var (a, b) = pair;
来源：https://tg.zhonguo1118.cn

[C16] 函数 / 方法重载
来源：https://yi.zhonguo7118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://io.zhonguo7118.cn

PHP:  // 无重载
来源：https://tq.zhonguo6118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://kl.zhonguo4118.cn

TS:   // 用联合类型或重载签名声明
来源：https://zl.zhonguo8118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://cc.zhonguo6118.cn

Go:   // 无重载：用不同函数名
来源：https://ar.zhonguo1118.cn

Ruby: # 无重载：靠动态参数
来源：https://gj.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://iy.zhonguo5118.cn

================================================================================
来源：https://li.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://ao.zhonguo7118.cn

================================================================================
来源：https://np.zhonguo5118.cn

[D01] 创建数组 / 列表
来源：https://nl.zhonguo6118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://ex.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://sm.zhonguo6118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://yl.zhonguo3118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://vv.zhonguo2118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://bj.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://lj.zhonguo5118.cn

Ruby: arr = [1, 2, 3]
来源：https://ec.zhonguo1118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://cs.zhonguo3118.cn

[D02] 追加元素到末尾
来源：https://zz.zhonguo2118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://zz.zhonguo2118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://pq.zhonguo1118.cn

JS:   arr.push(4);
来源：https://ut.zhonguo3118.cn

TS:   arr.push(4);
来源：https://gp.zhonguo4118.cn

Java: list.add(4);
来源：https://ei.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://fo.zhonguo6118.cn

Ruby: arr << 4; arr.push(5)
来源：https://xs.zhonguo7118.cn

C#:   list.Add(4);
来源：https://bd.zhonguo2118.cn

[D03] 在指定位置插入元素
来源：https://pe.zhonguo1118.cn

Py:   arr.insert(0, 0)
来源：https://vr.zhonguo3118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://di.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://va.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://kk.zhonguo5118.cn

Java: list.add(0, 0);
来源：https://or.zhonguo2118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://mn.zhonguo6118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://op.zhonguo3118.cn

C#:   list.Insert(0, 0);
来源：https://zq.zhonguo6118.cn

[D04] 删除元素
来源：https://id.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://mc.zhonguo2118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://hx.zhonguo3118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://jp.zhonguo7118.cn

TS:   arr.splice(0, 1);
来源：https://ty.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://db.zhonguo7118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://we.zhonguo3118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ky.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://yc.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://sn.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://co.zhonguo7118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://lh.zhonguo5118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://lx.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://fe.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://tu.zhonguo7118.cn

Go:   arr[0]; arr[0] = 9
来源：https://uj.zhonguo8118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://bk.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://nv.zhonguo4118.cn

[D06] 数组长度
来源：https://sk.zhonguo2118.cn

Py:   len(arr)
来源：https://ek.zhonguo7118.cn

PHP:  count($arr);
来源：https://ux.zhonguo3118.cn

JS:   arr.length
来源：https://qe.zhonguo5118.cn

TS:   arr.length
来源：https://cy.zhonguo1118.cn

Java: list.size();
来源：https://ip.zhonguo4118.cn

Go:   len(arr)
来源：https://ba.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://jx.zhonguo6118.cn

C#:   list.Count;
来源：https://tb.zhonguo7118.cn

[D07] 切片 / 取子数组
来源：https://od.zhonguo5118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://ld.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://bo.zhonguo3118.cn

JS:   arr.slice(1, 4);
来源：https://fg.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://zc.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://ha.zhonguo2118.cn

Go:   arr[1:4]
来源：https://ni.zhonguo6118.cn

Ruby: arr[1, 3]
来源：https://ss.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://pb.zhonguo5118.cn

[D08] 合并两个数组
来源：https://zz.zhonguo2118.cn

Py:   a + b;  a.extend(b)
来源：https://iy.zhonguo1118.cn

PHP:  array_merge($a, $b);
来源：https://ny.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://sy.zhonguo3118.cn

TS:   [...a, ...b];
来源：https://mp.zhonguo5118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ol.zhonguo7118.cn

Go:   append(a, b...)
来源：https://xu.zhonguo6118.cn

Ruby: a + b;  a.concat(b)
来源：https://ny.zhonguo1118.cn

C#:   a.Concat(b).ToList()
来源：https://sa.zhonguo5118.cn

[D09] 排序（升序）
来源：https://yt.zhonguo8118.cn

Py:   sorted(arr);  arr.sort()
来源：https://em.zhonguo4118.cn

PHP:  sort($arr);
来源：https://fk.zhonguo2118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://tf.zhonguo3118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ek.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://nu.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://zw.zhonguo5118.cn

Ruby: arr.sort
来源：https://mp.zhonguo5118.cn

C#:   list.Sort();
来源：https://eg.zhonguo8118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://qg.zhonguo2118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://cd.zhonguo5118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://wg.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://za.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://in.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://pf.zhonguo6118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://al.zhonguo5118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://kh.zhonguo2118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://uo.zhonguo4118.cn

[D11] 反转数组
来源：https://uj.zhonguo8118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://it.zhonguo4118.cn

PHP:  array_reverse($arr);
来源：https://rt.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://yk.zhonguo8118.cn

TS:   [...arr].reverse();
来源：https://th.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://ay.zhonguo6118.cn

Go:   slices.Reverse(arr)
来源：https://uk.zhonguo2118.cn

Ruby: arr.reverse
来源：https://qo.zhonguo8118.cn

C#:   list.Reverse();
来源：https://oy.zhonguo8118.cn

[D12] 查找元素下标
来源：https://eb.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://qm.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://uw.zhonguo7118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://hy.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://fj.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://xv.zhonguo6118.cn

Go:   slices.Index(arr, x)
来源：https://co.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://qz.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://xd.zhonguo3118.cn

[D13] 过滤（保留满足条件的）
来源：https://sd.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://ne.zhonguo8118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://gt.zhonguo2118.cn

JS:   arr.filter(x => x > 3)
来源：https://vn.zhonguo5118.cn

TS:   arr.filter(x => x > 3)
来源：https://qj.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://fu.zhonguo4118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://js.zhonguo2118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://qc.zhonguo4118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://kf.zhonguo3118.cn

[D14] 映射转换（每个元素变形）
来源：https://hg.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://cq.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://hp.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://zf.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://dt.zhonguo8118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ei.zhonguo5118.cn

Go:   // 手写循环
来源：https://fz.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://jm.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://uh.zhonguo8118.cn

[D15] 去重
来源：https://zc.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://xm.zhonguo8118.cn

PHP:  array_unique($arr);
来源：https://xp.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://yq.zhonguo2118.cn


<!-- 参考信息 -->