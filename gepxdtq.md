代发 wailian999

Py:   return a, b
来源：https://lz.zhonguo2118.cn

PHP:  return [$a, $b];
来源：https://sv.zhonguo8118.cn

JS:   return [a, b];             // 或 return { a, b };
来源：https://yl.zhonguo7118.cn

TS:   return { a, b };
来源：https://wa.zhonguo5118.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://al.zhonguo2118.cn

Go:   return a, b
来源：https://wp.zhonguo4118.cn

Ruby: return a, b
来源：https://fx.zhonguo4118.cn

C#:   return (a, b);              // ValueTuple
来源：https://es.zhonguo2118.cn

[C06] 匿名函数 / lambda
来源：https://tq.zhonguo2118.cn

Py:   square = lambda x: x * x
来源：https://wg.zhonguo5118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://qd.zhonguo2118.cn

JS:   const square = x => x * x;
来源：https://wi.zhonguo7118.cn

TS:   const square = (x: number): number => x * x;
来源：https://wn.zhonguo1118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://um.zhonguo6118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://kq.zhonguo7118.cn

Ruby: square = ->(x) { x * x }
来源：https://zh.zhonguo6118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://ra.zhonguo2118.cn

[C07] 把函数作为参数传入
来源：https://tj.zhonguo6118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://xa.zhonguo8118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://cr.zhonguo4118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://go.zhonguo6118.cn

TS:   arr.map(String)
来源：https://cr.zhonguo5118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://mr.zhonguo7118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://do.zhonguo6118.cn

Ruby: arr.map(&:upcase)
来源：https://up.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://dl.zhonguo1118.cn

[C08] 闭包
来源：https://qd.zhonguo4118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://kz.zhonguo1118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ap.zhonguo3118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://pf.zhonguo4118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://sj.zhonguo6118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://sl.zhonguo2118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://qr.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://ls.zhonguo4118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://hr.zhonguo5118.cn

[C09] 递归
来源：https://af.zhonguo7118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://qd.zhonguo3118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://qh.zhonguo1118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://lu.zhonguo6118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://fc.zhonguo6118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://ls.zhonguo3118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://br.zhonguo4118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://xk.zhonguo2118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://bs.zhonguo1118.cn

[C10] 变量作用域
来源：https://bn.zhonguo8118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://te.zhonguo4118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://xe.zhonguo5118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://ds.zhonguo7118.cn

TS:   同 JS
来源：https://nw.zhonguo2118.cn

Java: 方法内为块级作用域
来源：https://uz.zhonguo5118.cn

Go:   花括号块级作用域
来源：https://re.zhonguo4118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://mz.zhonguo8118.cn

C#:   块级作用域
来源：https://sy.zhonguo6118.cn

[C11] 模块导入与导出
来源：https://bc.zhonguo8118.cn

Py:   from module import func
来源：https://nv.zhonguo6118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://ep.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://vd.zhonguo8118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://ak.zhonguo6118.cn

Java: import java.util.List;
来源：https://wh.zhonguo8118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://qb.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://mc.zhonguo2118.cn

C#:   using System.Text;
来源：https://wj.zhonguo4118.cn

[C12] 立即执行函数 IIFE
来源：https://og.zhonguo8118.cn

Py:   (lambda: print("run"))()
来源：https://qu.zhonguo1118.cn

PHP:  (function () { echo "run"; })();
来源：https://jk.zhonguo1118.cn

JS:   (() => { console.log("run"); })();
来源：https://jn.zhonguo4118.cn

TS:   (() => { console.log("run"); })();
来源：https://gn.zhonguo3118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://hg.zhonguo1118.cn

Go:   func() { fmt.Println("run") }()
来源：https://nd.zhonguo7118.cn

Ruby: -> { puts "run" }.call
来源：https://yd.zhonguo2118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://vj.zhonguo6118.cn

[C13] 类型声明 / 类型注解
来源：https://cw.zhonguo6118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ne.zhonguo6118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qn.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://bw.zhonguo1118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://pi.zhonguo3118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://gb.zhonguo7118.cn

Go:   func add(a, b int) int
来源：https://wn.zhonguo2118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://yd.zhonguo3118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://tp.zhonguo4118.cn

[C14] 泛型函数
来源：https://qz.zhonguo8118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://eu.zhonguo3118.cn

PHP:  // 无泛型
来源：https://oa.zhonguo8118.cn

JS:   // 无泛型
来源：https://rp.zhonguo8118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://xg.zhonguo2118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://yy.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://bj.zhonguo1118.cn

Ruby: # 无泛型
来源：https://hl.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://in.zhonguo8118.cn

[C15] 解构 / 展开参数
来源：https://uh.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://oj.zhonguo2118.cn

PHP:  [$a, $b] = $pair;
来源：https://wq.zhonguo5118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://lv.zhonguo5118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ah.zhonguo1118.cn

Java: // 无解构
来源：https://jo.zhonguo6118.cn

Go:   // 无解构
来源：https://vc.zhonguo7118.cn

Ruby: a, b = pair
来源：https://hm.zhonguo6118.cn

C#:   var (a, b) = pair;
来源：https://xp.zhonguo6118.cn

[C16] 函数 / 方法重载
来源：https://ie.zhonguo4118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ht.zhonguo6118.cn

PHP:  // 无重载
来源：https://ao.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://zw.zhonguo1118.cn

TS:   // 用联合类型或重载签名声明
来源：https://bx.zhonguo5118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://vo.zhonguo8118.cn

Go:   // 无重载：用不同函数名
来源：https://vn.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://au.zhonguo5118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://le.zhonguo8118.cn

================================================================================
来源：https://ft.zhonguo2118.cn

D. 数组 / 列表 / 集合
来源：https://je.zhonguo6118.cn

================================================================================
来源：https://vk.zhonguo1118.cn

[D01] 创建数组 / 列表
来源：https://rz.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://bs.zhonguo7118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://fi.zhonguo5118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://pr.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://pt.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://ak.zhonguo8118.cn

Go:   arr := []int{1, 2, 3}
来源：https://gn.zhonguo6118.cn

Ruby: arr = [1, 2, 3]
来源：https://at.zhonguo5118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://ob.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://hi.zhonguo5118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://ag.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://rw.zhonguo8118.cn

JS:   arr.push(4);
来源：https://nx.zhonguo3118.cn

TS:   arr.push(4);
来源：https://dw.zhonguo7118.cn

Java: list.add(4);
来源：https://xx.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://ru.zhonguo5118.cn

Ruby: arr << 4; arr.push(5)
来源：https://eo.zhonguo2118.cn

C#:   list.Add(4);
来源：https://hx.zhonguo4118.cn

[D03] 在指定位置插入元素
来源：https://fc.zhonguo4118.cn

Py:   arr.insert(0, 0)
来源：https://mc.zhonguo2118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://mk.zhonguo2118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://bf.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://gi.zhonguo3118.cn

Java: list.add(0, 0);
来源：https://sj.zhonguo4118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://iw.zhonguo4118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://bu.zhonguo4118.cn

C#:   list.Insert(0, 0);
来源：https://bm.zhonguo3118.cn

[D04] 删除元素
来源：https://qi.zhonguo6118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://nq.zhonguo6118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://of.zhonguo7118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://vj.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://px.zhonguo4118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://iv.zhonguo2118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://sg.zhonguo7118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ts.zhonguo7118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://kw.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://cb.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://id.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://ke.zhonguo3118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://sl.zhonguo8118.cn

TS:   arr[0]; arr.at(-1);
来源：https://dy.zhonguo2118.cn

Java: list.get(0); list.set(0, 9);
来源：https://ch.zhonguo5118.cn

Go:   arr[0]; arr[0] = 9
来源：https://hk.zhonguo2118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://sd.zhonguo3118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://yj.zhonguo3118.cn

[D06] 数组长度
来源：https://il.zhonguo6118.cn

Py:   len(arr)
来源：https://cv.zhonguo5118.cn

PHP:  count($arr);
来源：https://kq.zhonguo2118.cn

JS:   arr.length
来源：https://yw.zhonguo8118.cn

TS:   arr.length
来源：https://ud.zhonguo7118.cn

Java: list.size();
来源：https://gy.zhonguo2118.cn

Go:   len(arr)
来源：https://kz.zhonguo1118.cn

Ruby: arr.length; arr.size
来源：https://ve.zhonguo8118.cn

C#:   list.Count;
来源：https://te.zhonguo3118.cn

[D07] 切片 / 取子数组
来源：https://gw.zhonguo4118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://fq.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://qb.zhonguo3118.cn

JS:   arr.slice(1, 4);
来源：https://cl.zhonguo7118.cn

TS:   arr.slice(1, 4);
来源：https://ez.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://ba.zhonguo2118.cn

Go:   arr[1:4]
来源：https://cr.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://oj.zhonguo2118.cn

C#:   list.GetRange(1, 3);
来源：https://dw.zhonguo3118.cn

[D08] 合并两个数组
来源：https://ct.zhonguo8118.cn

Py:   a + b;  a.extend(b)
来源：https://hc.zhonguo4118.cn

PHP:  array_merge($a, $b);
来源：https://mb.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://qt.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://px.zhonguo3118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://dj.zhonguo1118.cn

Go:   append(a, b...)
来源：https://xx.zhonguo3118.cn

Ruby: a + b;  a.concat(b)
来源：https://ip.zhonguo4118.cn

C#:   a.Concat(b).ToList()
来源：https://ox.zhonguo4118.cn

[D09] 排序（升序）
来源：https://bq.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pa.zhonguo6118.cn

PHP:  sort($arr);
来源：https://px.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://df.zhonguo3118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://wh.zhonguo7118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://nj.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://lx.zhonguo1118.cn

Ruby: arr.sort
来源：https://kv.zhonguo4118.cn

C#:   list.Sort();
来源：https://wt.zhonguo6118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://qa.zhonguo5118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://gl.zhonguo4118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://vh.zhonguo1118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://oe.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://zt.zhonguo5118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://id.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://ay.zhonguo8118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://uv.zhonguo5118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://un.zhonguo1118.cn

[D11] 反转数组
来源：https://vx.zhonguo1118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://xk.zhonguo7118.cn

PHP:  array_reverse($arr);
来源：https://pq.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://fz.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://nn.zhonguo4118.cn

Java: Collections.reverse(list);
来源：https://wm.zhonguo8118.cn

Go:   slices.Reverse(arr)
来源：https://lu.zhonguo4118.cn

Ruby: arr.reverse
来源：https://ri.zhonguo5118.cn

C#:   list.Reverse();
来源：https://mb.zhonguo7118.cn

[D12] 查找元素下标
来源：https://uj.zhonguo3118.cn

Py:   arr.index(x);  x in arr
来源：https://sy.zhonguo1118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://as.zhonguo6118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://xb.zhonguo6118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ut.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://tj.zhonguo3118.cn

Go:   slices.Index(arr, x)
来源：https://od.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://ye.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://sv.zhonguo8118.cn

[D13] 过滤（保留满足条件的）
来源：https://vh.zhonguo4118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://xv.zhonguo6118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://rx.zhonguo4118.cn

JS:   arr.filter(x => x > 3)
来源：https://jn.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://it.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://av.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://en.zhonguo2118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://tj.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://nj.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://kk.zhonguo1118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://hs.zhonguo1118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://xn.zhonguo8118.cn

JS:   arr.map(x => x * 2)
来源：https://wn.zhonguo8118.cn

TS:   arr.map(x => x * 2)
来源：https://gh.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://qr.zhonguo5118.cn

Go:   // 手写循环
来源：https://bo.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://qw.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://lr.zhonguo2118.cn

[D15] 去重
来源：https://uo.zhonguo7118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://bz.zhonguo7118.cn

PHP:  array_unique($arr);
来源：https://vn.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://ip.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://mh.zhonguo6118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://bt.zhonguo3118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ds.zhonguo8118.cn

Ruby: arr.uniq
来源：https://oo.zhonguo3118.cn

C#:   list.Distinct().ToList()
来源：https://wp.zhonguo7118.cn

[D16] 求和与平均值
来源：https://gq.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://io.zhonguo1118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://qt.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://pb.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://as.zhonguo6118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://vq.zhonguo2118.cn

Go:   // 手写循环累加
来源：https://pe.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ey.zhonguo4118.cn

C#:   list.Sum();  list.Average()
来源：https://zy.zhonguo4118.cn

[D17] 最大值与最小值
来源：https://al.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://xb.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://yx.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://zj.zhonguo1118.cn

TS:   Math.max(...arr);
来源：https://ic.zhonguo1118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://mf.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://lm.zhonguo2118.cn

Ruby: arr.max;  arr.min
来源：https://er.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://er.zhonguo8118.cn

[D18] 扁平化嵌套数组
来源：https://oa.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://il.zhonguo2118.cn

PHP:  array_merge(...$nested);
来源：https://cf.zhonguo7118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://wc.zhonguo4118.cn

TS:   nested.flat();
来源：https://oo.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://cw.zhonguo6118.cn

Go:   // 手写双层循环
来源：https://kr.zhonguo4118.cn

Ruby: nested.flatten
来源：https://so.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://pc.zhonguo1118.cn

[D19] 按字段分组
来源：https://he.zhonguo1118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ye.zhonguo3118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ji.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://aj.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ng.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://em.zhonguo6118.cn

Go:   // 手写 map[string][]T
来源：https://vx.zhonguo2118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://mz.zhonguo1118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://hr.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://tl.zhonguo4118.cn

Py:   Counter(arr)
来源：https://kv.zhonguo8118.cn

PHP:  array_count_values($arr);
来源：https://bk.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://jx.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://tq.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://xk.zhonguo6118.cn

Go:   // 手写 map[T]int
来源：https://ay.zhonguo7118.cn

Ruby: arr.tally
来源：https://sl.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://wa.zhonguo5118.cn

[D21] 判断是否包含某元素
来源：https://so.zhonguo8118.cn

Py:   x in arr
来源：https://zc.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://zl.zhonguo2118.cn

JS:   arr.includes(x)
来源：https://vv.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://an.zhonguo7118.cn

Java: list.contains(x)
来源：https://il.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://az.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://wr.zhonguo5118.cn

C#:   list.Contains(x)
来源：https://hn.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://do.zhonguo4118.cn


<!-- 参考信息 -->