代发 wailian999

C#:   x is int or double or decimal
来源：https://ua.zhonguo4118.cn

[B14] 判断值是否在集合内
来源：https://hn.zhonguo3118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://ou.zhonguo5118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://sc.zhonguo5118.cn

JS:   [1, 2, 3].includes(x)
来源：https://dl.zhonguo6118.cn

TS:   [1, 2, 3].includes(x)
来源：https://mp.zhonguo4118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://mr.zhonguo6118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://sc.zhonguo2118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://kq.zhonguo3118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://gk.zhonguo5118.cn

[B15] 布尔运算与取反
来源：https://nn.zhonguo4118.cn

Py:   a and b or not c
来源：https://nw.zhonguo5118.cn

PHP:  $a && $b || !$c
来源：https://wc.zhonguo8118.cn

JS:   a && b || !c
来源：https://be.zhonguo3118.cn

TS:   a && b || !c
来源：https://ou.zhonguo5118.cn

Java: a && b || !c
来源：https://uw.zhonguo2118.cn

Go:   a && b || !c
来源：https://hn.zhonguo8118.cn

Ruby: a && b || !c
来源：https://mm.zhonguo6118.cn

C#:   a && b || !c
来源：https://tv.zhonguo6118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://rj.zhonguo2118.cn

Py:   if not data: return
来源：https://ra.zhonguo2118.cn

PHP:  if (!$data) { return; }
来源：https://br.zhonguo8118.cn

JS:   if (!data) return;
来源：https://um.zhonguo4118.cn

TS:   if (!data) return;
来源：https://ev.zhonguo4118.cn

Java: if (data == null) return;
来源：https://jb.zhonguo5118.cn

Go:   if data == nil { return }
来源：https://de.zhonguo7118.cn

Ruby: return if data.nil?
来源：https://vm.zhonguo7118.cn

C#:   if (data == null) return;
来源：https://an.zhonguo7118.cn

================================================================================
来源：https://iu.zhonguo1118.cn

C. 函数与作用域
来源：https://gi.zhonguo4118.cn

================================================================================
来源：https://hr.zhonguo6118.cn

[C01] 定义函数
来源：https://ws.zhonguo7118.cn

Py:   def add(a, b): return a + b
来源：https://jc.zhonguo2118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://lt.zhonguo7118.cn

JS:   function add(a, b) { return a + b; }
来源：https://xq.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://gh.zhonguo1118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://je.zhonguo7118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://es.zhonguo3118.cn

Ruby: def add(a, b); a + b; end
来源：https://cp.zhonguo3118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://ia.zhonguo6118.cn

[C02] 默认参数
来源：https://av.zhonguo3118.cn

Py:   def greet(name="World"): return name
来源：https://vm.zhonguo6118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://mi.zhonguo5118.cn

JS:   function greet(name = "World") { return name; }
来源：https://kn.zhonguo6118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://re.zhonguo4118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://kn.zhonguo5118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://gc.zhonguo1118.cn

Ruby: def greet(name = "World") = name
来源：https://zp.zhonguo6118.cn

C#:   string Greet(string name = "World") => name;
来源：https://qy.zhonguo6118.cn

[C03] 可变参数
来源：https://hy.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://sv.zhonguo6118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://lk.zhonguo1118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://ja.zhonguo4118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://rs.zhonguo6118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://vj.zhonguo7118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://mw.zhonguo6118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://rt.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://wy.zhonguo3118.cn

[C04] 命名参数 / 关键字参数
来源：https://lk.zhonguo1118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://xq.zhonguo5118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://rq.zhonguo7118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://rc.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://bp.zhonguo2118.cn

Java: // 无：用 Builder 模式或 record
来源：https://sh.zhonguo2118.cn

Go:   // 无：用配置结构体参数
来源：https://hn.zhonguo8118.cn

Ruby: f(a: 1, b: 2)
来源：https://vy.zhonguo5118.cn

C#:   f(a: 1, b: 2)
来源：https://fy.zhonguo7118.cn

[C05] 返回多个值
来源：https://rb.zhonguo4118.cn

Py:   return a, b
来源：https://tq.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://sm.zhonguo5118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://yp.zhonguo2118.cn

TS:   return { a, b };
来源：https://ld.zhonguo4118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://xe.zhonguo3118.cn

Go:   return a, b
来源：https://es.zhonguo2118.cn

Ruby: return a, b
来源：https://el.zhonguo7118.cn

C#:   return (a, b);              // ValueTuple
来源：https://bz.zhonguo3118.cn

[C06] 匿名函数 / lambda
来源：https://oj.zhonguo2118.cn

Py:   square = lambda x: x * x
来源：https://ul.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://ng.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://oy.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://ri.zhonguo2118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://sk.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://kp.zhonguo6118.cn

Ruby: square = ->(x) { x * x }
来源：https://qz.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://vl.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://uk.zhonguo3118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://en.zhonguo2118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://qm.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://jg.zhonguo1118.cn

TS:   arr.map(String)
来源：https://ve.zhonguo8118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://hw.zhonguo8118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://ez.zhonguo7118.cn

Ruby: arr.map(&:upcase)
来源：https://dn.zhonguo5118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://dh.zhonguo1118.cn

[C08] 闭包
来源：https://ns.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ca.zhonguo4118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://mq.zhonguo3118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://lu.zhonguo3118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://vc.zhonguo5118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://vn.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://cz.zhonguo6118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ru.zhonguo1118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://tj.zhonguo8118.cn

[C09] 递归
来源：https://kx.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://kg.zhonguo4118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://qn.zhonguo7118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://vs.zhonguo6118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://cy.zhonguo4118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://qe.zhonguo5118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ke.zhonguo8118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://sw.zhonguo7118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://bb.zhonguo5118.cn

[C10] 变量作用域
来源：https://xz.zhonguo2118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ad.zhonguo3118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://to.zhonguo4118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://ex.zhonguo8118.cn

TS:   同 JS
来源：https://xe.zhonguo6118.cn

Java: 方法内为块级作用域
来源：https://au.zhonguo1118.cn

Go:   花括号块级作用域
来源：https://cn.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://xf.zhonguo4118.cn

C#:   块级作用域
来源：https://xe.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://we.zhonguo4118.cn

Py:   from module import func
来源：https://er.zhonguo2118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://hg.zhonguo6118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://sr.zhonguo6118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://zf.zhonguo8118.cn

Java: import java.util.List;
来源：https://sn.zhonguo4118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://ly.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://ie.zhonguo3118.cn

C#:   using System.Text;
来源：https://rz.zhonguo7118.cn

[C12] 立即执行函数 IIFE
来源：https://ln.zhonguo1118.cn

Py:   (lambda: print("run"))()
来源：https://ib.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://al.zhonguo1118.cn

JS:   (() => { console.log("run"); })();
来源：https://qm.zhonguo2118.cn

TS:   (() => { console.log("run"); })();
来源：https://id.zhonguo1118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://zh.zhonguo5118.cn

Go:   func() { fmt.Println("run") }()
来源：https://qu.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://fm.zhonguo6118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://qd.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://ly.zhonguo5118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://hd.zhonguo7118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://fq.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://uo.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://uo.zhonguo3118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://qi.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://me.zhonguo5118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://sp.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://aa.zhonguo8118.cn

[C14] 泛型函数
来源：https://rt.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ja.zhonguo6118.cn

PHP:  // 无泛型
来源：https://ix.zhonguo1118.cn

JS:   // 无泛型
来源：https://kp.zhonguo4118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://zk.zhonguo2118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://sa.zhonguo1118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://hi.zhonguo6118.cn

Ruby: # 无泛型
来源：https://tc.zhonguo3118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://tc.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://rk.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://ix.zhonguo6118.cn

PHP:  [$a, $b] = $pair;
来源：https://og.zhonguo3118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://hx.zhonguo2118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://sv.zhonguo4118.cn

Java: // 无解构
来源：https://zw.zhonguo3118.cn

Go:   // 无解构
来源：https://hu.zhonguo4118.cn

Ruby: a, b = pair
来源：https://fe.zhonguo3118.cn

C#:   var (a, b) = pair;
来源：https://je.zhonguo4118.cn

[C16] 函数 / 方法重载
来源：https://qk.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ud.zhonguo2118.cn

PHP:  // 无重载
来源：https://qt.zhonguo4118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://nq.zhonguo4118.cn

TS:   // 用联合类型或重载签名声明
来源：https://mr.zhonguo3118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ns.zhonguo7118.cn

Go:   // 无重载：用不同函数名
来源：https://vk.zhonguo5118.cn

Ruby: # 无重载：靠动态参数
来源：https://ck.zhonguo1118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://lu.zhonguo3118.cn

================================================================================
来源：https://rc.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://uc.zhonguo7118.cn

================================================================================
来源：https://kb.zhonguo3118.cn

[D01] 创建数组 / 列表
来源：https://qw.zhonguo1118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://hr.zhonguo5118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://xj.zhonguo1118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://xd.zhonguo2118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://pr.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://zb.zhonguo4118.cn

Go:   arr := []int{1, 2, 3}
来源：https://ov.zhonguo8118.cn

Ruby: arr = [1, 2, 3]
来源：https://om.zhonguo3118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://fj.zhonguo3118.cn

[D02] 追加元素到末尾
来源：https://ne.zhonguo6118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://bx.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://dt.zhonguo1118.cn

JS:   arr.push(4);
来源：https://yb.zhonguo2118.cn

TS:   arr.push(4);
来源：https://xp.zhonguo4118.cn

Java: list.add(4);
来源：https://cj.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://xi.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://zq.zhonguo2118.cn

C#:   list.Add(4);
来源：https://cf.zhonguo6118.cn

[D03] 在指定位置插入元素
来源：https://kw.zhonguo7118.cn

Py:   arr.insert(0, 0)
来源：https://sf.zhonguo8118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://ua.zhonguo6118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://xd.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://ox.zhonguo4118.cn

Java: list.add(0, 0);
来源：https://it.zhonguo4118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://lx.zhonguo7118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://mw.zhonguo1118.cn

C#:   list.Insert(0, 0);
来源：https://kt.zhonguo6118.cn

[D04] 删除元素
来源：https://cg.zhonguo5118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://jp.zhonguo3118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://tz.zhonguo1118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://nv.zhonguo5118.cn

TS:   arr.splice(0, 1);
来源：https://wc.zhonguo3118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ju.zhonguo8118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ky.zhonguo8118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://oc.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://at.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://ss.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://en.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://rq.zhonguo1118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://dc.zhonguo2118.cn

TS:   arr[0]; arr.at(-1);
来源：https://io.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://wx.zhonguo3118.cn

Go:   arr[0]; arr[0] = 9
来源：https://fx.zhonguo1118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://fi.zhonguo4118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://yk.zhonguo2118.cn

[D06] 数组长度
来源：https://xb.zhonguo6118.cn

Py:   len(arr)
来源：https://yh.zhonguo1118.cn

PHP:  count($arr);
来源：https://uu.zhonguo8118.cn

JS:   arr.length
来源：https://vp.zhonguo4118.cn

TS:   arr.length
来源：https://as.zhonguo3118.cn

Java: list.size();
来源：https://zf.zhonguo4118.cn

Go:   len(arr)
来源：https://ou.zhonguo3118.cn

Ruby: arr.length; arr.size
来源：https://nm.zhonguo6118.cn

C#:   list.Count;
来源：https://kg.zhonguo6118.cn

[D07] 切片 / 取子数组
来源：https://rv.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://ib.zhonguo8118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://fr.zhonguo1118.cn

JS:   arr.slice(1, 4);
来源：https://kz.zhonguo2118.cn

TS:   arr.slice(1, 4);
来源：https://ec.zhonguo7118.cn

Java: list.subList(1, 4);
来源：https://tq.zhonguo8118.cn

Go:   arr[1:4]
来源：https://zs.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://xl.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://pu.zhonguo7118.cn

[D08] 合并两个数组
来源：https://kk.zhonguo4118.cn

Py:   a + b;  a.extend(b)
来源：https://ub.zhonguo4118.cn

PHP:  array_merge($a, $b);
来源：https://ol.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ep.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://on.zhonguo1118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://vx.zhonguo2118.cn

Go:   append(a, b...)
来源：https://ty.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://ec.zhonguo1118.cn

C#:   a.Concat(b).ToList()
来源：https://pz.zhonguo6118.cn

[D09] 排序（升序）
来源：https://st.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://fr.zhonguo6118.cn

PHP:  sort($arr);
来源：https://gg.zhonguo3118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://zq.zhonguo7118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ob.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://rk.zhonguo1118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://jw.zhonguo1118.cn

Ruby: arr.sort
来源：https://ri.zhonguo2118.cn

C#:   list.Sort();
来源：https://hv.zhonguo5118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://ss.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://hb.zhonguo3118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://eq.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://cq.zhonguo7118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://eb.zhonguo1118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://zw.zhonguo3118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://nb.zhonguo7118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://wh.zhonguo2118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://yh.zhonguo6118.cn

[D11] 反转数组
来源：https://de.zhonguo1118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://dm.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://dt.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://nk.zhonguo4118.cn

TS:   [...arr].reverse();
来源：https://qa.zhonguo1118.cn

Java: Collections.reverse(list);
来源：https://qe.zhonguo3118.cn

Go:   slices.Reverse(arr)
来源：https://ja.zhonguo2118.cn

Ruby: arr.reverse
来源：https://cw.zhonguo7118.cn

C#:   list.Reverse();
来源：https://vh.zhonguo1118.cn

[D12] 查找元素下标
来源：https://uo.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://vu.zhonguo5118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://fx.zhonguo5118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://xu.zhonguo8118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://rr.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://xb.zhonguo3118.cn

Go:   slices.Index(arr, x)
来源：https://rh.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://yp.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://vy.zhonguo7118.cn

[D13] 过滤（保留满足条件的）
来源：https://go.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://jz.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://gn.zhonguo1118.cn

JS:   arr.filter(x => x > 3)
来源：https://ha.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://ao.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://os.zhonguo5118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://zv.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://yv.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://xu.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://mc.zhonguo8118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://au.zhonguo1118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ma.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://wa.zhonguo1118.cn

TS:   arr.map(x => x * 2)
来源：https://gr.zhonguo3118.cn


<!-- 参考信息 -->