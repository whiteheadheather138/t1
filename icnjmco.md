代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：https://se.zhonguo6118.cn

PHP:  # 无标签：用 goto 或函数返回
来源：https://ea.zhonguo7118.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：https://yq.zhonguo5118.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：https://zr.zhonguo4118.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：https://yu.zhonguo2118.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：https://mk.zhonguo2118.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：https://qo.zhonguo4118.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：https://mh.zhonguo8118.cn

[B13] 判断是否为数字
来源：https://yi.zhonguo6118.cn

Py:   isinstance(x, (int, float))
来源：https://yl.zhonguo5118.cn

PHP:  is_numeric($x)
来源：https://ry.zhonguo4118.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：https://ef.zhonguo7118.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：https://fm.zhonguo7118.cn

Java: x instanceof Number
来源：https://ou.zhonguo7118.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：https://ot.zhonguo5118.cn

Ruby: x.is_a?(Numeric)
来源：https://ea.zhonguo4118.cn

C#:   x is int or double or decimal
来源：https://sf.zhonguo3118.cn

[B14] 判断值是否在集合内
来源：https://zo.zhonguo1118.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：https://sd.zhonguo6118.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：https://zy.zhonguo1118.cn

JS:   [1, 2, 3].includes(x)
来源：https://ht.zhonguo3118.cn

TS:   [1, 2, 3].includes(x)
来源：https://km.zhonguo1118.cn

Java: List.of(1, 2, 3).contains(x)
来源：https://yb.zhonguo8118.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：https://bj.zhonguo7118.cn

Ruby: [1, 2, 3].include?(x)
来源：https://sb.zhonguo8118.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：https://nw.zhonguo6118.cn

[B15] 布尔运算与取反
来源：https://ss.zhonguo1118.cn

Py:   a and b or not c
来源：https://qx.zhonguo2118.cn

PHP:  $a && $b || !$c
来源：https://gw.zhonguo4118.cn

JS:   a && b || !c
来源：https://sc.zhonguo7118.cn

TS:   a && b || !c
来源：https://us.zhonguo6118.cn

Java: a && b || !c
来源：https://dg.zhonguo5118.cn

Go:   a && b || !c
来源：https://ya.zhonguo4118.cn

Ruby: a && b || !c
来源：https://fo.zhonguo1118.cn

C#:   a && b || !c
来源：https://bb.zhonguo7118.cn

[B16] 卫语句：不满足条件提前返回
来源：https://qq.zhonguo5118.cn

Py:   if not data: return
来源：https://hd.zhonguo8118.cn

PHP:  if (!$data) { return; }
来源：https://fd.zhonguo1118.cn

JS:   if (!data) return;
来源：https://vw.zhonguo4118.cn

TS:   if (!data) return;
来源：https://nc.zhonguo1118.cn

Java: if (data == null) return;
来源：https://nu.zhonguo5118.cn

Go:   if data == nil { return }
来源：https://xt.zhonguo1118.cn

Ruby: return if data.nil?
来源：https://kx.zhonguo8118.cn

C#:   if (data == null) return;
来源：https://tk.zhonguo6118.cn

================================================================================
来源：https://mw.zhonguo4118.cn

C. 函数与作用域
来源：https://mh.zhonguo4118.cn

================================================================================
来源：https://nd.zhonguo5118.cn

[C01] 定义函数
来源：https://jl.zhonguo3118.cn

Py:   def add(a, b): return a + b
来源：https://rm.zhonguo7118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://aw.zhonguo3118.cn

JS:   function add(a, b) { return a + b; }
来源：https://zv.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://zn.zhonguo4118.cn

Java: static int add(int a, int b) { return a + b; }
来源：https://mt.zhonguo7118.cn

Go:   func add(a, b int) int { return a + b }
来源：https://bi.zhonguo8118.cn

Ruby: def add(a, b); a + b; end
来源：https://zz.zhonguo3118.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：https://so.zhonguo2118.cn

[C02] 默认参数
来源：https://dh.zhonguo5118.cn

Py:   def greet(name="World"): return name
来源：https://ss.zhonguo1118.cn

PHP:  function greet($name = "World") { return $name; }
来源：https://nj.zhonguo3118.cn

JS:   function greet(name = "World") { return name; }
来源：https://cc.zhonguo3118.cn

TS:   function greet(name: string = "World") { return name; }
来源：https://ym.zhonguo1118.cn

Java: // 无默认参数：方法重载或 Optional
来源：https://pr.zhonguo4118.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：https://td.zhonguo5118.cn

Ruby: def greet(name = "World") = name
来源：https://uh.zhonguo2118.cn

C#:   string Greet(string name = "World") => name;
来源：https://zg.zhonguo4118.cn

[C03] 可变参数
来源：https://ga.zhonguo3118.cn

Py:   def total(*args): return sum(args)
来源：https://jf.zhonguo3118.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：https://sz.zhonguo8118.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：https://kz.zhonguo6118.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：https://jh.zhonguo4118.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：https://pd.zhonguo6118.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：https://za.zhonguo5118.cn

Ruby: def total(*nums); nums.sum; end
来源：https://ti.zhonguo7118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://ur.zhonguo5118.cn

[C04] 命名参数 / 关键字参数
来源：https://sy.zhonguo3118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://tv.zhonguo3118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://pg.zhonguo2118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://kd.zhonguo8118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://un.zhonguo5118.cn

Java: // 无：用 Builder 模式或 record
来源：https://fk.zhonguo2118.cn

Go:   // 无：用配置结构体参数
来源：https://rq.zhonguo1118.cn

Ruby: f(a: 1, b: 2)
来源：https://am.zhonguo3118.cn

C#:   f(a: 1, b: 2)
来源：https://wh.zhonguo2118.cn

[C05] 返回多个值
来源：https://gx.zhonguo1118.cn

Py:   return a, b
来源：https://an.zhonguo5118.cn

PHP:  return [$a, $b];
来源：https://hl.zhonguo4118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://uo.zhonguo3118.cn

TS:   return { a, b };
来源：https://ji.zhonguo7118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://ky.zhonguo6118.cn

Go:   return a, b
来源：https://jq.zhonguo2118.cn

Ruby: return a, b
来源：https://sv.zhonguo8118.cn

C#:   return (a, b);              // ValueTuple
来源：https://zz.zhonguo4118.cn

[C06] 匿名函数 / lambda
来源：https://am.zhonguo4118.cn

Py:   square = lambda x: x * x
来源：https://vd.zhonguo2118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://ne.zhonguo4118.cn

JS:   const square = x => x * x;
来源：https://yy.zhonguo6118.cn

TS:   const square = (x: number): number => x * x;
来源：https://cj.zhonguo5118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://vt.zhonguo4118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://jv.zhonguo5118.cn

Ruby: square = ->(x) { x * x }
来源：https://gw.zhonguo4118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://mw.zhonguo5118.cn

[C07] 把函数作为参数传入
来源：https://gk.zhonguo7118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://yt.zhonguo8118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://ts.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://kb.zhonguo7118.cn

TS:   arr.map(String)
来源：https://jt.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://rv.zhonguo4118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://ju.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://ba.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://gh.zhonguo5118.cn

[C08] 闭包
来源：https://bd.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://si.zhonguo8118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://zl.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://mo.zhonguo3118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://sp.zhonguo6118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://qt.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://jl.zhonguo3118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ky.zhonguo8118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://er.zhonguo2118.cn

[C09] 递归
来源：https://ar.zhonguo2118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://ed.zhonguo4118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://ya.zhonguo7118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://gh.zhonguo7118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://zk.zhonguo2118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://xg.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://dp.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://su.zhonguo1118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://wk.zhonguo1118.cn

[C10] 变量作用域
来源：https://jo.zhonguo8118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ln.zhonguo3118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://yu.zhonguo5118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://gi.zhonguo1118.cn

TS:   同 JS
来源：https://hi.zhonguo8118.cn

Java: 方法内为块级作用域
来源：https://qn.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://fn.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://nh.zhonguo2118.cn

C#:   块级作用域
来源：https://la.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://zn.zhonguo6118.cn

Py:   from module import func
来源：https://ep.zhonguo8118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://md.zhonguo8118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://yk.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://oa.zhonguo3118.cn

Java: import java.util.List;
来源：https://wf.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://ld.zhonguo4118.cn

Ruby: require "json"; require_relative "./util"
来源：https://rg.zhonguo3118.cn

C#:   using System.Text;
来源：https://wy.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://so.zhonguo2118.cn

Py:   (lambda: print("run"))()
来源：https://kw.zhonguo6118.cn

PHP:  (function () { echo "run"; })();
来源：https://wl.zhonguo7118.cn

JS:   (() => { console.log("run"); })();
来源：https://mv.zhonguo5118.cn

TS:   (() => { console.log("run"); })();
来源：https://vv.zhonguo2118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://hk.zhonguo5118.cn

Go:   func() { fmt.Println("run") }()
来源：https://lo.zhonguo4118.cn

Ruby: -> { puts "run" }.call
来源：https://vq.zhonguo7118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://ry.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://kt.zhonguo5118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ct.zhonguo8118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qr.zhonguo7118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://ih.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://aa.zhonguo2118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://ms.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://za.zhonguo8118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://hu.zhonguo1118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://bj.zhonguo4118.cn

[C14] 泛型函数
来源：https://sq.zhonguo3118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://qd.zhonguo5118.cn

PHP:  // 无泛型
来源：https://wz.zhonguo6118.cn

JS:   // 无泛型
来源：https://ri.zhonguo3118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://zi.zhonguo7118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://aa.zhonguo6118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ty.zhonguo8118.cn

Ruby: # 无泛型
来源：https://ek.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://tg.zhonguo6118.cn

[C15] 解构 / 展开参数
来源：https://my.zhonguo1118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://vp.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://wm.zhonguo4118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://xp.zhonguo1118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://mi.zhonguo6118.cn

Java: // 无解构
来源：https://lj.zhonguo6118.cn

Go:   // 无解构
来源：https://mv.zhonguo2118.cn

Ruby: a, b = pair
来源：https://rl.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://nf.zhonguo3118.cn

[C16] 函数 / 方法重载
来源：https://ym.zhonguo6118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://zi.zhonguo6118.cn

PHP:  // 无重载
来源：https://lq.zhonguo2118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://py.zhonguo6118.cn

TS:   // 用联合类型或重载签名声明
来源：https://kk.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://hq.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://co.zhonguo8118.cn

Ruby: # 无重载：靠动态参数
来源：https://uh.zhonguo3118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://rs.zhonguo2118.cn

================================================================================
来源：https://px.zhonguo8118.cn

D. 数组 / 列表 / 集合
来源：https://qk.zhonguo6118.cn

================================================================================
来源：https://mq.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://lp.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://xp.zhonguo5118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://sy.zhonguo2118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://qc.zhonguo5118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://su.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://kk.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://od.zhonguo4118.cn

Ruby: arr = [1, 2, 3]
来源：https://cn.zhonguo7118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://bm.zhonguo4118.cn

[D02] 追加元素到末尾
来源：https://mg.zhonguo5118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://rx.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://pi.zhonguo5118.cn

JS:   arr.push(4);
来源：https://yz.zhonguo5118.cn

TS:   arr.push(4);
来源：https://dh.zhonguo4118.cn

Java: list.add(4);
来源：https://jh.zhonguo3118.cn

Go:   arr = append(arr, 4)
来源：https://zl.zhonguo7118.cn

Ruby: arr << 4; arr.push(5)
来源：https://mr.zhonguo6118.cn

C#:   list.Add(4);
来源：https://ep.zhonguo2118.cn

[D03] 在指定位置插入元素
来源：https://bi.zhonguo1118.cn

Py:   arr.insert(0, 0)
来源：https://ie.zhonguo8118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://nx.zhonguo1118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://dz.zhonguo8118.cn

TS:   arr.splice(0, 0, 0);
来源：https://jf.zhonguo1118.cn

Java: list.add(0, 0);
来源：https://kp.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://bv.zhonguo6118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://bv.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://sd.zhonguo3118.cn

[D04] 删除元素
来源：https://zg.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://zh.zhonguo1118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://xt.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://he.zhonguo8118.cn

TS:   arr.splice(0, 1);
来源：https://jp.zhonguo5118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://kd.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://rd.zhonguo6118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://jg.zhonguo8118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://mw.zhonguo1118.cn

[D05] 访问与修改元素
来源：https://rg.zhonguo3118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://it.zhonguo6118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://um.zhonguo4118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://pl.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://od.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://zc.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://kq.zhonguo3118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://ct.zhonguo6118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://wv.zhonguo6118.cn

[D06] 数组长度
来源：https://pj.zhonguo1118.cn

Py:   len(arr)
来源：https://be.zhonguo6118.cn

PHP:  count($arr);
来源：https://te.zhonguo8118.cn

JS:   arr.length
来源：https://bu.zhonguo1118.cn

TS:   arr.length
来源：https://my.zhonguo1118.cn

Java: list.size();
来源：https://gw.zhonguo6118.cn

Go:   len(arr)
来源：https://os.zhonguo4118.cn

Ruby: arr.length; arr.size
来源：https://ce.zhonguo8118.cn

C#:   list.Count;
来源：https://rt.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://ix.zhonguo4118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://pf.zhonguo7118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://uy.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://gb.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://fw.zhonguo7118.cn

Java: list.subList(1, 4);
来源：https://jk.zhonguo8118.cn

Go:   arr[1:4]
来源：https://dr.zhonguo1118.cn

Ruby: arr[1, 3]
来源：https://xv.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://ln.zhonguo7118.cn

[D08] 合并两个数组
来源：https://ap.zhonguo8118.cn

Py:   a + b;  a.extend(b)
来源：https://sg.zhonguo3118.cn

PHP:  array_merge($a, $b);
来源：https://eh.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://tx.zhonguo4118.cn

TS:   [...a, ...b];
来源：https://sb.zhonguo1118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://uf.zhonguo6118.cn

Go:   append(a, b...)
来源：https://cz.zhonguo5118.cn

Ruby: a + b;  a.concat(b)
来源：https://ep.zhonguo1118.cn

C#:   a.Concat(b).ToList()
来源：https://uj.zhonguo7118.cn

[D09] 排序（升序）
来源：https://is.zhonguo1118.cn

Py:   sorted(arr);  arr.sort()
来源：https://sa.zhonguo2118.cn

PHP:  sort($arr);
来源：https://nd.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://nf.zhonguo4118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://at.zhonguo7118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://pl.zhonguo6118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://gn.zhonguo2118.cn

Ruby: arr.sort
来源：https://tm.zhonguo5118.cn

C#:   list.Sort();
来源：https://nt.zhonguo2118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://wj.zhonguo2118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://kq.zhonguo3118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://hs.zhonguo4118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://vq.zhonguo1118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ns.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://lj.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://wh.zhonguo7118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://vh.zhonguo5118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://sj.zhonguo2118.cn

[D11] 反转数组
来源：https://zn.zhonguo2118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://ec.zhonguo2118.cn

PHP:  array_reverse($arr);
来源：https://nx.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://gv.zhonguo1118.cn

TS:   [...arr].reverse();
来源：https://sv.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://wf.zhonguo1118.cn

Go:   slices.Reverse(arr)
来源：https://cy.zhonguo3118.cn

Ruby: arr.reverse
来源：https://ew.zhonguo5118.cn

C#:   list.Reverse();
来源：https://ro.zhonguo6118.cn

[D12] 查找元素下标
来源：https://du.zhonguo1118.cn

Py:   arr.index(x);  x in arr
来源：https://tq.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://bk.zhonguo7118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ti.zhonguo7118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://qf.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://tn.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://gd.zhonguo7118.cn


<!-- 参考信息 -->