代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：https://rd.zhonguo3118.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：https://go.zhonguo5118.cn

[C04] 命名参数 / 关键字参数
来源：https://aq.zhonguo2118.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：https://ny.zhonguo2118.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：https://qy.zhonguo3118.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：https://yo.zhonguo5118.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：https://ye.zhonguo8118.cn

Java: // 无：用 Builder 模式或 record
来源：https://ti.zhonguo1118.cn

Go:   // 无：用配置结构体参数
来源：https://qi.zhonguo4118.cn

Ruby: f(a: 1, b: 2)
来源：https://ua.zhonguo7118.cn

C#:   f(a: 1, b: 2)
来源：https://hg.zhonguo2118.cn

[C05] 返回多个值
来源：https://ru.zhonguo2118.cn

Py:   return a, b
来源：https://tz.zhonguo1118.cn

PHP:  return [$a, $b];
来源：https://lb.zhonguo5118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://gx.zhonguo6118.cn

TS:   return { a, b };
来源：https://vi.zhonguo5118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://eb.zhonguo5118.cn

Go:   return a, b
来源：https://to.zhonguo2118.cn

Ruby: return a, b
来源：https://bu.zhonguo2118.cn

C#:   return (a, b);              // ValueTuple
来源：https://gd.zhonguo4118.cn

[C06] 匿名函数 / lambda
来源：https://yt.zhonguo3118.cn

Py:   square = lambda x: x * x
来源：https://ii.zhonguo3118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://sn.zhonguo1118.cn

JS:   const square = x => x * x;
来源：https://hm.zhonguo1118.cn

TS:   const square = (x: number): number => x * x;
来源：https://uv.zhonguo7118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://wp.zhonguo7118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://ix.zhonguo5118.cn

Ruby: square = ->(x) { x * x }
来源：https://to.zhonguo2118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://un.zhonguo7118.cn

[C07] 把函数作为参数传入
来源：https://li.zhonguo7118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://hj.zhonguo5118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://dj.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://tv.zhonguo7118.cn

TS:   arr.map(String)
来源：https://mf.zhonguo2118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://vi.zhonguo7118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://kt.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://pi.zhonguo8118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ma.zhonguo5118.cn

[C08] 闭包
来源：https://tz.zhonguo2118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://mw.zhonguo6118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://wc.zhonguo5118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://lz.zhonguo7118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://ce.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://gh.zhonguo8118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://ra.zhonguo2118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://cm.zhonguo4118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://yz.zhonguo6118.cn

[C09] 递归
来源：https://ov.zhonguo6118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://wp.zhonguo1118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://ij.zhonguo3118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://gi.zhonguo2118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://yu.zhonguo1118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://rh.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://ff.zhonguo6118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://au.zhonguo1118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://dg.zhonguo2118.cn

[C10] 变量作用域
来源：https://gi.zhonguo5118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://ke.zhonguo1118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://jp.zhonguo8118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://of.zhonguo1118.cn

TS:   同 JS
来源：https://gs.zhonguo3118.cn

Java: 方法内为块级作用域
来源：https://dk.zhonguo8118.cn

Go:   花括号块级作用域
来源：https://pf.zhonguo8118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://yi.zhonguo1118.cn

C#:   块级作用域
来源：https://dz.zhonguo8118.cn

[C11] 模块导入与导出
来源：https://mg.zhonguo3118.cn

Py:   from module import func
来源：https://uh.zhonguo4118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://go.zhonguo2118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://bi.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://rt.zhonguo8118.cn

Java: import java.util.List;
来源：https://os.zhonguo3118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://rc.zhonguo8118.cn

Ruby: require "json"; require_relative "./util"
来源：https://jh.zhonguo2118.cn

C#:   using System.Text;
来源：https://ns.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://bd.zhonguo4118.cn

Py:   (lambda: print("run"))()
来源：https://xb.zhonguo5118.cn

PHP:  (function () { echo "run"; })();
来源：https://ps.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://bd.zhonguo6118.cn

TS:   (() => { console.log("run"); })();
来源：https://uh.zhonguo7118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://km.zhonguo7118.cn

Go:   func() { fmt.Println("run") }()
来源：https://vf.zhonguo3118.cn

Ruby: -> { puts "run" }.call
来源：https://so.zhonguo3118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://ly.zhonguo8118.cn

[C13] 类型声明 / 类型注解
来源：https://ku.zhonguo1118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://zh.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qn.zhonguo2118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://hl.zhonguo3118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ps.zhonguo6118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://ds.zhonguo6118.cn

Go:   func add(a, b int) int
来源：https://bg.zhonguo5118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://xm.zhonguo3118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://xj.zhonguo3118.cn

[C14] 泛型函数
来源：https://df.zhonguo8118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ih.zhonguo1118.cn

PHP:  // 无泛型
来源：https://la.zhonguo6118.cn

JS:   // 无泛型
来源：https://ky.zhonguo6118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://um.zhonguo6118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://ea.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://ie.zhonguo7118.cn

Ruby: # 无泛型
来源：https://bm.zhonguo2118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://oo.zhonguo6118.cn

[C15] 解构 / 展开参数
来源：https://gu.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://wj.zhonguo3118.cn

PHP:  [$a, $b] = $pair;
来源：https://ag.zhonguo6118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://km.zhonguo3118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://xt.zhonguo7118.cn

Java: // 无解构
来源：https://dv.zhonguo1118.cn

Go:   // 无解构
来源：https://qg.zhonguo3118.cn

Ruby: a, b = pair
来源：https://hp.zhonguo7118.cn

C#:   var (a, b) = pair;
来源：https://aj.zhonguo2118.cn

[C16] 函数 / 方法重载
来源：https://yf.zhonguo3118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ie.zhonguo3118.cn

PHP:  // 无重载
来源：https://ro.zhonguo4118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ui.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://ae.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://ws.zhonguo2118.cn

Go:   // 无重载：用不同函数名
来源：https://br.zhonguo3118.cn

Ruby: # 无重载：靠动态参数
来源：https://fs.zhonguo5118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jx.zhonguo2118.cn

================================================================================
来源：https://ou.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://vc.zhonguo6118.cn

================================================================================
来源：https://zg.zhonguo7118.cn

[D01] 创建数组 / 列表
来源：https://wa.zhonguo5118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://fx.zhonguo5118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://gk.zhonguo2118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://iq.zhonguo1118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://xc.zhonguo2118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://dh.zhonguo3118.cn

Go:   arr := []int{1, 2, 3}
来源：https://es.zhonguo2118.cn

Ruby: arr = [1, 2, 3]
来源：https://lg.zhonguo2118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://uy.zhonguo5118.cn

[D02] 追加元素到末尾
来源：https://xi.zhonguo5118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://ci.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://ma.zhonguo6118.cn

JS:   arr.push(4);
来源：https://zg.zhonguo8118.cn

TS:   arr.push(4);
来源：https://cm.zhonguo2118.cn

Java: list.add(4);
来源：https://fn.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://gm.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://fq.zhonguo2118.cn

C#:   list.Add(4);
来源：https://pz.zhonguo6118.cn

[D03] 在指定位置插入元素
来源：https://hd.zhonguo6118.cn

Py:   arr.insert(0, 0)
来源：https://lu.zhonguo2118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://am.zhonguo8118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://fb.zhonguo4118.cn

TS:   arr.splice(0, 0, 0);
来源：https://vk.zhonguo8118.cn

Java: list.add(0, 0);
来源：https://hs.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://om.zhonguo8118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://zm.zhonguo1118.cn

C#:   list.Insert(0, 0);
来源：https://td.zhonguo8118.cn

[D04] 删除元素
来源：https://vh.zhonguo4118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://bq.zhonguo8118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://as.zhonguo1118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://pu.zhonguo5118.cn

TS:   arr.splice(0, 1);
来源：https://xz.zhonguo7118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ds.zhonguo2118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://jf.zhonguo5118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://lg.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://wk.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://nx.zhonguo8118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://bx.zhonguo7118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://qy.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://hv.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://dj.zhonguo8118.cn

Java: list.get(0); list.set(0, 9);
来源：https://eu.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ed.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://qb.zhonguo6118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ne.zhonguo7118.cn

[D06] 数组长度
来源：https://uv.zhonguo5118.cn

Py:   len(arr)
来源：https://jh.zhonguo6118.cn

PHP:  count($arr);
来源：https://cy.zhonguo5118.cn

JS:   arr.length
来源：https://pj.zhonguo6118.cn

TS:   arr.length
来源：https://zs.zhonguo7118.cn

Java: list.size();
来源：https://fi.zhonguo2118.cn

Go:   len(arr)
来源：https://ic.zhonguo8118.cn

Ruby: arr.length; arr.size
来源：https://hi.zhonguo7118.cn

C#:   list.Count;
来源：https://dv.zhonguo6118.cn

[D07] 切片 / 取子数组
来源：https://ed.zhonguo5118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://br.zhonguo1118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://wn.zhonguo2118.cn

JS:   arr.slice(1, 4);
来源：https://rv.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://xi.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://qp.zhonguo7118.cn

Go:   arr[1:4]
来源：https://nh.zhonguo6118.cn

Ruby: arr[1, 3]
来源：https://ep.zhonguo1118.cn

C#:   list.GetRange(1, 3);
来源：https://dm.zhonguo3118.cn

[D08] 合并两个数组
来源：https://vz.zhonguo5118.cn

Py:   a + b;  a.extend(b)
来源：https://ee.zhonguo6118.cn

PHP:  array_merge($a, $b);
来源：https://vm.zhonguo5118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://wq.zhonguo4118.cn

TS:   [...a, ...b];
来源：https://fp.zhonguo5118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://iz.zhonguo2118.cn

Go:   append(a, b...)
来源：https://yy.zhonguo5118.cn

Ruby: a + b;  a.concat(b)
来源：https://pd.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://lx.zhonguo3118.cn

[D09] 排序（升序）
来源：https://ey.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://zq.zhonguo1118.cn

PHP:  sort($arr);
来源：https://fb.zhonguo3118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://gx.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://kj.zhonguo2118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://ex.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://qc.zhonguo2118.cn

Ruby: arr.sort
来源：https://jb.zhonguo4118.cn

C#:   list.Sort();
来源：https://bu.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://ya.zhonguo5118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://ii.zhonguo1118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://oz.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://tf.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://da.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://ie.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://bz.zhonguo1118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ze.zhonguo3118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://ju.zhonguo1118.cn

[D11] 反转数组
来源：https://kf.zhonguo1118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://gh.zhonguo1118.cn

PHP:  array_reverse($arr);
来源：https://uh.zhonguo3118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://tf.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://uh.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://rf.zhonguo6118.cn

Go:   slices.Reverse(arr)
来源：https://mv.zhonguo1118.cn

Ruby: arr.reverse
来源：https://au.zhonguo4118.cn

C#:   list.Reverse();
来源：https://uq.zhonguo2118.cn

[D12] 查找元素下标
来源：https://ja.zhonguo8118.cn

Py:   arr.index(x);  x in arr
来源：https://yn.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://mi.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://wc.zhonguo5118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://al.zhonguo4118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://sv.zhonguo4118.cn

Go:   slices.Index(arr, x)
来源：https://nh.zhonguo4118.cn

Ruby: arr.index(x)
来源：https://er.zhonguo6118.cn

C#:   list.IndexOf(x);
来源：https://qx.zhonguo1118.cn

[D13] 过滤（保留满足条件的）
来源：https://vt.zhonguo3118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://iz.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://kn.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://ee.zhonguo3118.cn

TS:   arr.filter(x => x > 3)
来源：https://nr.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://cf.zhonguo5118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://ck.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ta.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ry.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://uk.zhonguo4118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://he.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://zb.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://dy.zhonguo3118.cn

TS:   arr.map(x => x * 2)
来源：https://zm.zhonguo6118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://zi.zhonguo5118.cn

Go:   // 手写循环
来源：https://ws.zhonguo5118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://uq.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://fa.zhonguo8118.cn

[D15] 去重
来源：https://sw.zhonguo7118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://xd.zhonguo1118.cn

PHP:  array_unique($arr);
来源：https://ha.zhonguo2118.cn

JS:   [...new Set(arr)]
来源：https://iy.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://bh.zhonguo2118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://pq.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://zc.zhonguo3118.cn

Ruby: arr.uniq
来源：https://iy.zhonguo4118.cn

C#:   list.Distinct().ToList()
来源：https://ls.zhonguo3118.cn

[D16] 求和与平均值
来源：https://ik.zhonguo6118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://qx.zhonguo4118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://lw.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://wk.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://bd.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://zk.zhonguo1118.cn

Go:   // 手写循环累加
来源：https://qo.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://vj.zhonguo5118.cn

C#:   list.Sum();  list.Average()
来源：https://om.zhonguo6118.cn

[D17] 最大值与最小值
来源：https://ui.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://qq.zhonguo8118.cn

PHP:  max($arr);  min($arr);
来源：https://hf.zhonguo8118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://eu.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://dk.zhonguo4118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://km.zhonguo5118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://fw.zhonguo6118.cn

Ruby: arr.max;  arr.min
来源：https://ux.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://tx.zhonguo4118.cn

[D18] 扁平化嵌套数组
来源：https://du.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://vt.zhonguo7118.cn

PHP:  array_merge(...$nested);
来源：https://zn.zhonguo1118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://ur.zhonguo8118.cn

TS:   nested.flat();
来源：https://wl.zhonguo1118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://by.zhonguo8118.cn

Go:   // 手写双层循环
来源：https://yg.zhonguo1118.cn

Ruby: nested.flatten
来源：https://xn.zhonguo5118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://jy.zhonguo3118.cn

[D19] 按字段分组
来源：https://pl.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ed.zhonguo1118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://es.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://xn.zhonguo8118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://on.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://so.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://qw.zhonguo1118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://jj.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://ca.zhonguo4118.cn

[D20] 统计每个元素出现次数
来源：https://je.zhonguo3118.cn

Py:   Counter(arr)
来源：https://ox.zhonguo3118.cn

PHP:  array_count_values($arr);
来源：https://wp.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ui.zhonguo2118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://nm.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://ra.zhonguo1118.cn

Go:   // 手写 map[T]int
来源：https://fm.zhonguo2118.cn


<!-- 参考信息 -->