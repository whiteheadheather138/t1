代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：https://oe.zhonguo3118.cn

[C07] 把函数作为参数传入
来源：https://dm.zhonguo5118.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：https://mj.zhonguo4118.cn

PHP:  array_map("strtoupper", $arr);
来源：https://vp.zhonguo1118.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：https://my.zhonguo5118.cn

TS:   arr.map(String)
来源：https://ou.zhonguo4118.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：https://zg.zhonguo3118.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：https://qo.zhonguo2118.cn

Ruby: arr.map(&:upcase)
来源：https://vb.zhonguo1118.cn

C#:   arr.Select(s => s.ToUpper())
来源：https://wc.zhonguo2118.cn

[C08] 闭包
来源：https://ir.zhonguo5118.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：https://dj.zhonguo4118.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：https://rp.zhonguo2118.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：https://fr.zhonguo5118.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：https://xu.zhonguo2118.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：https://hy.zhonguo1118.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：https://fv.zhonguo5118.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：https://zp.zhonguo5118.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：https://yi.zhonguo2118.cn

[C09] 递归
来源：https://lt.zhonguo8118.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：https://vy.zhonguo6118.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：https://em.zhonguo6118.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://jk.zhonguo4118.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：https://dc.zhonguo3118.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：https://ew.zhonguo2118.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：https://qp.zhonguo2118.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：https://ua.zhonguo4118.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：https://sy.zhonguo5118.cn

[C10] 变量作用域
来源：https://ki.zhonguo7118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://tx.zhonguo4118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://pf.zhonguo6118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://xw.zhonguo2118.cn

TS:   同 JS
来源：https://om.zhonguo5118.cn

Java: 方法内为块级作用域
来源：https://ms.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://av.zhonguo5118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://xx.zhonguo7118.cn

C#:   块级作用域
来源：https://wh.zhonguo5118.cn

[C11] 模块导入与导出
来源：https://kr.zhonguo5118.cn

Py:   from module import func
来源：https://ro.zhonguo2118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://xs.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://vp.zhonguo2118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://mp.zhonguo1118.cn

Java: import java.util.List;
来源：https://xs.zhonguo6118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://cg.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://fg.zhonguo2118.cn

C#:   using System.Text;
来源：https://tu.zhonguo4118.cn

[C12] 立即执行函数 IIFE
来源：https://nv.zhonguo7118.cn

Py:   (lambda: print("run"))()
来源：https://eh.zhonguo4118.cn

PHP:  (function () { echo "run"; })();
来源：https://zb.zhonguo8118.cn

JS:   (() => { console.log("run"); })();
来源：https://yp.zhonguo7118.cn

TS:   (() => { console.log("run"); })();
来源：https://hz.zhonguo8118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://dw.zhonguo7118.cn

Go:   func() { fmt.Println("run") }()
来源：https://jm.zhonguo8118.cn

Ruby: -> { puts "run" }.call
来源：https://jc.zhonguo8118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://um.zhonguo1118.cn

[C13] 类型声明 / 类型注解
来源：https://zt.zhonguo5118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://wj.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://qh.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://vk.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://vm.zhonguo4118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://ni.zhonguo8118.cn

Go:   func add(a, b int) int
来源：https://bi.zhonguo7118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://ir.zhonguo8118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://yr.zhonguo8118.cn

[C14] 泛型函数
来源：https://kr.zhonguo6118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://jy.zhonguo1118.cn

PHP:  // 无泛型
来源：https://ok.zhonguo7118.cn

JS:   // 无泛型
来源：https://bz.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://qw.zhonguo4118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://gj.zhonguo4118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://yg.zhonguo8118.cn

Ruby: # 无泛型
来源：https://gs.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://xf.zhonguo6118.cn

[C15] 解构 / 展开参数
来源：https://aa.zhonguo6118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://gy.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://mg.zhonguo3118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://zv.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://oc.zhonguo6118.cn

Java: // 无解构
来源：https://qa.zhonguo1118.cn

Go:   // 无解构
来源：https://di.zhonguo8118.cn

Ruby: a, b = pair
来源：https://of.zhonguo1118.cn

C#:   var (a, b) = pair;
来源：https://zy.zhonguo6118.cn

[C16] 函数 / 方法重载
来源：https://ba.zhonguo4118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ec.zhonguo8118.cn

PHP:  // 无重载
来源：https://cd.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://xv.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://pj.zhonguo5118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://mq.zhonguo6118.cn

Go:   // 无重载：用不同函数名
来源：https://lm.zhonguo1118.cn

Ruby: # 无重载：靠动态参数
来源：https://ab.zhonguo8118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jt.zhonguo5118.cn

================================================================================
来源：https://kn.zhonguo2118.cn

D. 数组 / 列表 / 集合
来源：https://ay.zhonguo4118.cn

================================================================================
来源：https://cs.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://ic.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://vd.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://my.zhonguo3118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://hd.zhonguo5118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://lh.zhonguo7118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://mi.zhonguo7118.cn

Go:   arr := []int{1, 2, 3}
来源：https://uf.zhonguo3118.cn

Ruby: arr = [1, 2, 3]
来源：https://yl.zhonguo4118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://nv.zhonguo4118.cn

[D02] 追加元素到末尾
来源：https://oy.zhonguo4118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://eb.zhonguo3118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://mm.zhonguo4118.cn

JS:   arr.push(4);
来源：https://sa.zhonguo4118.cn

TS:   arr.push(4);
来源：https://sr.zhonguo7118.cn

Java: list.add(4);
来源：https://rz.zhonguo8118.cn

Go:   arr = append(arr, 4)
来源：https://hq.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://zc.zhonguo1118.cn

C#:   list.Add(4);
来源：https://va.zhonguo5118.cn

[D03] 在指定位置插入元素
来源：https://sz.zhonguo5118.cn

Py:   arr.insert(0, 0)
来源：https://xj.zhonguo1118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://vo.zhonguo4118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://fu.zhonguo7118.cn

TS:   arr.splice(0, 0, 0);
来源：https://xc.zhonguo1118.cn

Java: list.add(0, 0);
来源：https://ni.zhonguo4118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://lw.zhonguo8118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://iw.zhonguo7118.cn

C#:   list.Insert(0, 0);
来源：https://yn.zhonguo1118.cn

[D04] 删除元素
来源：https://bb.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://ok.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://fx.zhonguo4118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://nj.zhonguo1118.cn

TS:   arr.splice(0, 1);
来源：https://ct.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://nm.zhonguo5118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://rs.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://zm.zhonguo1118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://qg.zhonguo2118.cn

[D05] 访问与修改元素
来源：https://da.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ih.zhonguo6118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://dr.zhonguo5118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://da.zhonguo6118.cn

TS:   arr[0]; arr.at(-1);
来源：https://qs.zhonguo5118.cn

Java: list.get(0); list.set(0, 9);
来源：https://ho.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://dy.zhonguo5118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://yj.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ik.zhonguo6118.cn

[D06] 数组长度
来源：https://nd.zhonguo8118.cn

Py:   len(arr)
来源：https://va.zhonguo7118.cn

PHP:  count($arr);
来源：https://wl.zhonguo2118.cn

JS:   arr.length
来源：https://ox.zhonguo4118.cn

TS:   arr.length
来源：https://dw.zhonguo1118.cn

Java: list.size();
来源：https://tt.zhonguo6118.cn

Go:   len(arr)
来源：https://qd.zhonguo2118.cn

Ruby: arr.length; arr.size
来源：https://hs.zhonguo7118.cn

C#:   list.Count;
来源：https://pw.zhonguo3118.cn

[D07] 切片 / 取子数组
来源：https://ii.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://ja.zhonguo5118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://dy.zhonguo3118.cn

JS:   arr.slice(1, 4);
来源：https://xa.zhonguo4118.cn

TS:   arr.slice(1, 4);
来源：https://ml.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://su.zhonguo2118.cn

Go:   arr[1:4]
来源：https://mm.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://hm.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://nj.zhonguo4118.cn

[D08] 合并两个数组
来源：https://lv.zhonguo6118.cn

Py:   a + b;  a.extend(b)
来源：https://kp.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://nu.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://lo.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://xw.zhonguo5118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://lk.zhonguo2118.cn

Go:   append(a, b...)
来源：https://ni.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://vx.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://fb.zhonguo6118.cn

[D09] 排序（升序）
来源：https://ky.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://dd.zhonguo8118.cn

PHP:  sort($arr);
来源：https://iw.zhonguo5118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://vm.zhonguo3118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://jv.zhonguo5118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://nf.zhonguo1118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://ue.zhonguo1118.cn

Ruby: arr.sort
来源：https://hf.zhonguo2118.cn

C#:   list.Sort();
来源：https://ef.zhonguo5118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://fs.zhonguo8118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://zn.zhonguo2118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://ox.zhonguo6118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://ap.zhonguo4118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://qz.zhonguo6118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://gb.zhonguo6118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://nb.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ya.zhonguo3118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://er.zhonguo6118.cn

[D11] 反转数组
来源：https://nn.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://yh.zhonguo1118.cn

PHP:  array_reverse($arr);
来源：https://mm.zhonguo2118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://yj.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://rh.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://jz.zhonguo1118.cn

Go:   slices.Reverse(arr)
来源：https://oy.zhonguo7118.cn

Ruby: arr.reverse
来源：https://oc.zhonguo3118.cn

C#:   list.Reverse();
来源：https://vy.zhonguo7118.cn

[D12] 查找元素下标
来源：https://yp.zhonguo7118.cn

Py:   arr.index(x);  x in arr
来源：https://ih.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://yn.zhonguo1118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jc.zhonguo3118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://bt.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://aw.zhonguo2118.cn

Go:   slices.Index(arr, x)
来源：https://ql.zhonguo7118.cn

Ruby: arr.index(x)
来源：https://um.zhonguo3118.cn

C#:   list.IndexOf(x);
来源：https://ra.zhonguo2118.cn

[D13] 过滤（保留满足条件的）
来源：https://uf.zhonguo4118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://vz.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://ml.zhonguo1118.cn

JS:   arr.filter(x => x > 3)
来源：https://iu.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://bs.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://sc.zhonguo3118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://wm.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ah.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://gt.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://aq.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://jk.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ch.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://bv.zhonguo3118.cn

TS:   arr.map(x => x * 2)
来源：https://qb.zhonguo1118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ac.zhonguo2118.cn

Go:   // 手写循环
来源：https://sy.zhonguo8118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://oa.zhonguo6118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://tj.zhonguo7118.cn

[D15] 去重
来源：https://xa.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://bm.zhonguo8118.cn

PHP:  array_unique($arr);
来源：https://ea.zhonguo2118.cn

JS:   [...new Set(arr)]
来源：https://gf.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://bm.zhonguo5118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ng.zhonguo3118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://qt.zhonguo3118.cn

Ruby: arr.uniq
来源：https://kd.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://fn.zhonguo1118.cn

[D16] 求和与平均值
来源：https://ex.zhonguo6118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://vw.zhonguo4118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://fz.zhonguo4118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://ia.zhonguo5118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://iz.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://dh.zhonguo7118.cn

Go:   // 手写循环累加
来源：https://ho.zhonguo5118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://fa.zhonguo2118.cn

C#:   list.Sum();  list.Average()
来源：https://sv.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://ib.zhonguo1118.cn

Py:   max(arr);  min(arr)
来源：https://yg.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://ue.zhonguo2118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://bi.zhonguo2118.cn

TS:   Math.max(...arr);
来源：https://zq.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://vn.zhonguo1118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://iu.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://cj.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://om.zhonguo4118.cn

[D18] 扁平化嵌套数组
来源：https://de.zhonguo7118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ru.zhonguo7118.cn

PHP:  array_merge(...$nested);
来源：https://fu.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://mq.zhonguo6118.cn

TS:   nested.flat();
来源：https://qu.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://xn.zhonguo4118.cn

Go:   // 手写双层循环
来源：https://gk.zhonguo1118.cn

Ruby: nested.flatten
来源：https://et.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://gi.zhonguo8118.cn

[D19] 按字段分组
来源：https://hl.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://wn.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://sy.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://zj.zhonguo1118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://cg.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://gp.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://ed.zhonguo6118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://yr.zhonguo5118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://wq.zhonguo5118.cn

[D20] 统计每个元素出现次数
来源：https://be.zhonguo4118.cn

Py:   Counter(arr)
来源：https://nd.zhonguo8118.cn

PHP:  array_count_values($arr);
来源：https://nj.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ca.zhonguo5118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://rw.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://xz.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://eb.zhonguo3118.cn

Ruby: arr.tally
来源：https://bq.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://qa.zhonguo3118.cn

[D21] 判断是否包含某元素
来源：https://tr.zhonguo4118.cn

Py:   x in arr
来源：https://fs.zhonguo5118.cn

PHP:  in_array($x, $arr, true);
来源：https://vd.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://nx.zhonguo2118.cn

TS:   arr.includes(x)
来源：https://ep.zhonguo8118.cn

Java: list.contains(x)
来源：https://sj.zhonguo5118.cn

Go:   slices.Contains(arr, x)
来源：https://zc.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://ig.zhonguo3118.cn

C#:   list.Contains(x)
来源：https://jq.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://tg.zhonguo2118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://sw.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://gv.zhonguo6118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://tv.zhonguo5118.cn

TS:   [...arr];
来源：https://cp.zhonguo2118.cn

Java: new ArrayList<>(list);
来源：https://je.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://za.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://cw.zhonguo3118.cn

C#:   new List<int>(list);
来源：https://tg.zhonguo1118.cn

[D23] reduce 累积计算
来源：https://dq.zhonguo4118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://zv.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://jr.zhonguo2118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ap.zhonguo8118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://bm.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://zu.zhonguo2118.cn

Go:   // 手写循环
来源：https://ex.zhonguo8118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://dy.zhonguo2118.cn


<!-- 参考信息 -->