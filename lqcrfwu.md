代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：https://zv.zhonguo8118.cn

Go:   return a, b
来源：https://ic.zhonguo2118.cn

Ruby: return a, b
来源：https://og.zhonguo5118.cn

C#:   return (a, b);              // ValueTuple
来源：https://tw.zhonguo7118.cn

[C06] 匿名函数 / lambda
来源：https://ox.zhonguo1118.cn

Py:   square = lambda x: x * x
来源：https://zu.zhonguo7118.cn

PHP:  $square = fn($x) => $x * $x;
来源：https://gg.zhonguo3118.cn

JS:   const square = x => x * x;
来源：https://wq.zhonguo5118.cn

TS:   const square = (x: number): number => x * x;
来源：https://xo.zhonguo1118.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：https://lh.zhonguo5118.cn

Go:   sq := func(x int) int { return x * x }
来源：https://lk.zhonguo8118.cn

Ruby: square = ->(x) { x * x }
来源：https://cl.zhonguo8118.cn

C#:   Func<int, int> square = x => x * x;
来源：https://hu.zhonguo1118.cn

[C07] 把函数作为参数传入
来源：https://qk.zhonguo1118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://nf.zhonguo7118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://mx.zhonguo2118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://fi.zhonguo5118.cn

TS:   arr.map(String)
来源：https://gf.zhonguo3118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://yo.zhonguo3118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://vo.zhonguo5118.cn

Ruby: arr.map(&:upcase)
来源：https://dx.zhonguo2118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://ox.zhonguo5118.cn

[C08] 闭包
来源：https://ny.zhonguo5118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://ld.zhonguo7118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://ax.zhonguo6118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://or.zhonguo4118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://uc.zhonguo4118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://xw.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://lw.zhonguo7118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://cb.zhonguo6118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://zl.zhonguo3118.cn

[C09] 递归
来源：https://pp.zhonguo4118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://mo.zhonguo2118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://pv.zhonguo6118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://th.zhonguo8118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://qu.zhonguo2118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://vq.zhonguo4118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://gg.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://hx.zhonguo5118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://kz.zhonguo2118.cn

[C10] 变量作用域
来源：https://df.zhonguo1118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://pq.zhonguo3118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ip.zhonguo7118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://rp.zhonguo2118.cn

TS:   同 JS
来源：https://jy.zhonguo1118.cn

Java: 方法内为块级作用域
来源：https://bm.zhonguo4118.cn

Go:   花括号块级作用域
来源：https://ez.zhonguo4118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://ln.zhonguo1118.cn

C#:   块级作用域
来源：https://wz.zhonguo4118.cn

[C11] 模块导入与导出
来源：https://qb.zhonguo5118.cn

Py:   from module import func
来源：https://vx.zhonguo4118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://ur.zhonguo5118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://xz.zhonguo1118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://lv.zhonguo5118.cn

Java: import java.util.List;
来源：https://ur.zhonguo5118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://zo.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://an.zhonguo7118.cn

C#:   using System.Text;
来源：https://sn.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://ii.zhonguo2118.cn

Py:   (lambda: print("run"))()
来源：https://hn.zhonguo4118.cn

PHP:  (function () { echo "run"; })();
来源：https://px.zhonguo5118.cn

JS:   (() => { console.log("run"); })();
来源：https://th.zhonguo7118.cn

TS:   (() => { console.log("run"); })();
来源：https://wt.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://wl.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://no.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://gu.zhonguo5118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://rx.zhonguo7118.cn

[C13] 类型声明 / 类型注解
来源：https://kf.zhonguo1118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://ry.zhonguo2118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://hu.zhonguo6118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://ab.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://bh.zhonguo4118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://he.zhonguo3118.cn

Go:   func add(a, b int) int
来源：https://ig.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://rf.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://ke.zhonguo7118.cn

[C14] 泛型函数
来源：https://zw.zhonguo7118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://ma.zhonguo6118.cn

PHP:  // 无泛型
来源：https://yl.zhonguo1118.cn

JS:   // 无泛型
来源：https://lz.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://zh.zhonguo2118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://ax.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://wv.zhonguo8118.cn

Ruby: # 无泛型
来源：https://ne.zhonguo4118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://jd.zhonguo3118.cn

[C15] 解构 / 展开参数
来源：https://bi.zhonguo3118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://tl.zhonguo7118.cn

PHP:  [$a, $b] = $pair;
来源：https://qy.zhonguo7118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://dz.zhonguo3118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://ym.zhonguo4118.cn

Java: // 无解构
来源：https://zu.zhonguo1118.cn

Go:   // 无解构
来源：https://xm.zhonguo1118.cn

Ruby: a, b = pair
来源：https://qr.zhonguo2118.cn

C#:   var (a, b) = pair;
来源：https://ui.zhonguo6118.cn

[C16] 函数 / 方法重载
来源：https://me.zhonguo4118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://do.zhonguo6118.cn

PHP:  // 无重载
来源：https://bu.zhonguo1118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://hw.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://fq.zhonguo7118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://tj.zhonguo5118.cn

Go:   // 无重载：用不同函数名
来源：https://wh.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://pk.zhonguo2118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://rx.zhonguo1118.cn

================================================================================
来源：https://fk.zhonguo5118.cn

D. 数组 / 列表 / 集合
来源：https://qe.zhonguo1118.cn

================================================================================
来源：https://ko.zhonguo7118.cn

[D01] 创建数组 / 列表
来源：https://nt.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://rz.zhonguo5118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://up.zhonguo1118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ch.zhonguo8118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://ny.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://kz.zhonguo2118.cn

Go:   arr := []int{1, 2, 3}
来源：https://lt.zhonguo2118.cn

Ruby: arr = [1, 2, 3]
来源：https://re.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://ev.zhonguo4118.cn

[D02] 追加元素到末尾
来源：https://vg.zhonguo8118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://zw.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://jo.zhonguo6118.cn

JS:   arr.push(4);
来源：https://yu.zhonguo8118.cn

TS:   arr.push(4);
来源：https://kz.zhonguo4118.cn

Java: list.add(4);
来源：https://uw.zhonguo7118.cn

Go:   arr = append(arr, 4)
来源：https://nc.zhonguo6118.cn

Ruby: arr << 4; arr.push(5)
来源：https://gy.zhonguo7118.cn

C#:   list.Add(4);
来源：https://ic.zhonguo4118.cn

[D03] 在指定位置插入元素
来源：https://ar.zhonguo5118.cn

Py:   arr.insert(0, 0)
来源：https://bt.zhonguo1118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://fl.zhonguo2118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://fa.zhonguo6118.cn

TS:   arr.splice(0, 0, 0);
来源：https://go.zhonguo1118.cn

Java: list.add(0, 0);
来源：https://us.zhonguo8118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://jl.zhonguo6118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://jr.zhonguo8118.cn

C#:   list.Insert(0, 0);
来源：https://bq.zhonguo7118.cn

[D04] 删除元素
来源：https://ev.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://eo.zhonguo1118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ub.zhonguo2118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://ul.zhonguo2118.cn

TS:   arr.splice(0, 1);
来源：https://sb.zhonguo2118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://qc.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://pm.zhonguo2118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://nt.zhonguo2118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://qj.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://wv.zhonguo5118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://sj.zhonguo7118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://oa.zhonguo8118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://ex.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://fy.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://lo.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://qy.zhonguo2118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://oo.zhonguo1118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://rv.zhonguo7118.cn

[D06] 数组长度
来源：https://oq.zhonguo1118.cn

Py:   len(arr)
来源：https://wl.zhonguo7118.cn

PHP:  count($arr);
来源：https://ke.zhonguo3118.cn

JS:   arr.length
来源：https://ez.zhonguo3118.cn

TS:   arr.length
来源：https://po.zhonguo1118.cn

Java: list.size();
来源：https://ne.zhonguo4118.cn

Go:   len(arr)
来源：https://hy.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://xi.zhonguo7118.cn

C#:   list.Count;
来源：https://rq.zhonguo2118.cn

[D07] 切片 / 取子数组
来源：https://nz.zhonguo2118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://hi.zhonguo4118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://jt.zhonguo7118.cn

JS:   arr.slice(1, 4);
来源：https://re.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://lm.zhonguo7118.cn

Java: list.subList(1, 4);
来源：https://iz.zhonguo5118.cn

Go:   arr[1:4]
来源：https://xe.zhonguo1118.cn

Ruby: arr[1, 3]
来源：https://bx.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://pw.zhonguo4118.cn

[D08] 合并两个数组
来源：https://ux.zhonguo2118.cn

Py:   a + b;  a.extend(b)
来源：https://uk.zhonguo6118.cn

PHP:  array_merge($a, $b);
来源：https://bx.zhonguo3118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://sv.zhonguo7118.cn

TS:   [...a, ...b];
来源：https://kj.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ns.zhonguo7118.cn

Go:   append(a, b...)
来源：https://fi.zhonguo8118.cn

Ruby: a + b;  a.concat(b)
来源：https://qd.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://va.zhonguo6118.cn

[D09] 排序（升序）
来源：https://rv.zhonguo4118.cn

Py:   sorted(arr);  arr.sort()
来源：https://jy.zhonguo3118.cn

PHP:  sort($arr);
来源：https://qq.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://jm.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://kq.zhonguo1118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://pa.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://nq.zhonguo8118.cn

Ruby: arr.sort
来源：https://gd.zhonguo5118.cn

C#:   list.Sort();
来源：https://uq.zhonguo1118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://cl.zhonguo4118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://vu.zhonguo7118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://eb.zhonguo2118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://qx.zhonguo7118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://pr.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://fb.zhonguo8118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://er.zhonguo1118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ak.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://nh.zhonguo4118.cn

[D11] 反转数组
来源：https://pu.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://dk.zhonguo5118.cn

PHP:  array_reverse($arr);
来源：https://ri.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://vq.zhonguo8118.cn

TS:   [...arr].reverse();
来源：https://hz.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://gs.zhonguo7118.cn

Go:   slices.Reverse(arr)
来源：https://vc.zhonguo2118.cn

Ruby: arr.reverse
来源：https://hx.zhonguo5118.cn

C#:   list.Reverse();
来源：https://zy.zhonguo5118.cn

[D12] 查找元素下标
来源：https://al.zhonguo2118.cn

Py:   arr.index(x);  x in arr
来源：https://xx.zhonguo5118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://tu.zhonguo6118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://fw.zhonguo4118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ez.zhonguo1118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://nx.zhonguo1118.cn

Go:   slices.Index(arr, x)
来源：https://ht.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://nk.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://of.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://ry.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://vu.zhonguo2118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://gr.zhonguo1118.cn

JS:   arr.filter(x => x > 3)
来源：https://nu.zhonguo3118.cn

TS:   arr.filter(x => x > 3)
来源：https://wq.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://hj.zhonguo7118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://mc.zhonguo6118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://au.zhonguo3118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://hc.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://mq.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://qd.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://tu.zhonguo6118.cn

JS:   arr.map(x => x * 2)
来源：https://vf.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://pg.zhonguo3118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://vq.zhonguo3118.cn

Go:   // 手写循环
来源：https://vl.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://hc.zhonguo4118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://ra.zhonguo8118.cn

[D15] 去重
来源：https://oa.zhonguo7118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://tg.zhonguo5118.cn

PHP:  array_unique($arr);
来源：https://aa.zhonguo3118.cn

JS:   [...new Set(arr)]
来源：https://qb.zhonguo1118.cn

TS:   [...new Set(arr)]
来源：https://dg.zhonguo6118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ib.zhonguo2118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://fu.zhonguo8118.cn

Ruby: arr.uniq
来源：https://xy.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://qg.zhonguo1118.cn

[D16] 求和与平均值
来源：https://lx.zhonguo3118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://bc.zhonguo4118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ug.zhonguo8118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://ad.zhonguo4118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://dr.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://sc.zhonguo4118.cn

Go:   // 手写循环累加
来源：https://de.zhonguo5118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ac.zhonguo7118.cn

C#:   list.Sum();  list.Average()
来源：https://km.zhonguo8118.cn

[D17] 最大值与最小值
来源：https://dr.zhonguo8118.cn

Py:   max(arr);  min(arr)
来源：https://ls.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://kf.zhonguo2118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://jv.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://er.zhonguo3118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://tv.zhonguo1118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://yo.zhonguo2118.cn

Ruby: arr.max;  arr.min
来源：https://qw.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://xb.zhonguo7118.cn

[D18] 扁平化嵌套数组
来源：https://lc.zhonguo7118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://gb.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://ky.zhonguo6118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://eq.zhonguo6118.cn

TS:   nested.flat();
来源：https://oj.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ko.zhonguo7118.cn

Go:   // 手写双层循环
来源：https://is.zhonguo6118.cn

Ruby: nested.flatten
来源：https://rk.zhonguo5118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://lj.zhonguo6118.cn

[D19] 按字段分组
来源：https://uk.zhonguo5118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://xn.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://et.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://on.zhonguo2118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ur.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://br.zhonguo4118.cn

Go:   // 手写 map[string][]T
来源：https://af.zhonguo8118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://mm.zhonguo4118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://zr.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://nu.zhonguo2118.cn

Py:   Counter(arr)
来源：https://op.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://et.zhonguo5118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ua.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://xx.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://wv.zhonguo6118.cn

Go:   // 手写 map[T]int
来源：https://hu.zhonguo7118.cn

Ruby: arr.tally
来源：https://bv.zhonguo5118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://sy.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://pw.zhonguo4118.cn

Py:   x in arr
来源：https://rt.zhonguo1118.cn

PHP:  in_array($x, $arr, true);
来源：https://ii.zhonguo6118.cn

JS:   arr.includes(x)
来源：https://ac.zhonguo2118.cn

TS:   arr.includes(x)
来源：https://df.zhonguo1118.cn

Java: list.contains(x)
来源：https://uv.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://ik.zhonguo7118.cn

Ruby: arr.include?(x)
来源：https://aq.zhonguo6118.cn

C#:   list.Contains(x)
来源：https://se.zhonguo3118.cn

[D22] 复制数组（避免共享引用）
来源：https://ke.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://mz.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://kw.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://zh.zhonguo1118.cn

TS:   [...arr];
来源：https://kd.zhonguo7118.cn


<!-- 参考信息 -->