代发 wailian999

TS:   同 JS
来源：https://oo.zhonguo4118.cn

Java: 方法内为块级作用域
来源：https://vo.zhonguo3118.cn

Go:   花括号块级作用域
来源：https://pi.zhonguo4118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://so.zhonguo1118.cn

C#:   块级作用域
来源：https://uc.zhonguo6118.cn

[C11] 模块导入与导出
来源：https://hf.zhonguo1118.cn

Py:   from module import func
来源：https://ng.zhonguo2118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://ee.zhonguo1118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://uf.zhonguo4118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://xm.zhonguo2118.cn

Java: import java.util.List;
来源：https://qn.zhonguo2118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://tj.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://mx.zhonguo1118.cn

C#:   using System.Text;
来源：https://kr.zhonguo1118.cn

[C12] 立即执行函数 IIFE
来源：https://eg.zhonguo1118.cn

Py:   (lambda: print("run"))()
来源：https://pv.zhonguo3118.cn

PHP:  (function () { echo "run"; })();
来源：https://qz.zhonguo3118.cn

JS:   (() => { console.log("run"); })();
来源：https://rf.zhonguo2118.cn

TS:   (() => { console.log("run"); })();
来源：https://zs.zhonguo2118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ux.zhonguo7118.cn

Go:   func() { fmt.Println("run") }()
来源：https://ea.zhonguo8118.cn

Ruby: -> { puts "run" }.call
来源：https://ud.zhonguo1118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://fl.zhonguo8118.cn

[C13] 类型声明 / 类型注解
来源：https://ru.zhonguo7118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://lp.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://na.zhonguo1118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://bq.zhonguo2118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://bu.zhonguo5118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://ww.zhonguo6118.cn

Go:   func add(a, b int) int
来源：https://ba.zhonguo6118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://lu.zhonguo5118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://ri.zhonguo2118.cn

[C14] 泛型函数
来源：https://au.zhonguo4118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://gi.zhonguo1118.cn

PHP:  // 无泛型
来源：https://hz.zhonguo5118.cn

JS:   // 无泛型
来源：https://ti.zhonguo1118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://kq.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://kz.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://zs.zhonguo5118.cn

Ruby: # 无泛型
来源：https://mr.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://ge.zhonguo8118.cn

[C15] 解构 / 展开参数
来源：https://ub.zhonguo7118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://uw.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://vq.zhonguo1118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://ye.zhonguo2118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://md.zhonguo7118.cn

Java: // 无解构
来源：https://oc.zhonguo5118.cn

Go:   // 无解构
来源：https://sj.zhonguo6118.cn

Ruby: a, b = pair
来源：https://dj.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://qa.zhonguo7118.cn

[C16] 函数 / 方法重载
来源：https://su.zhonguo3118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://hc.zhonguo3118.cn

PHP:  // 无重载
来源：https://vt.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://fa.zhonguo8118.cn

TS:   // 用联合类型或重载签名声明
来源：https://qh.zhonguo8118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://sj.zhonguo4118.cn

Go:   // 无重载：用不同函数名
来源：https://js.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://id.zhonguo1118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://pi.zhonguo3118.cn

================================================================================
来源：https://zx.zhonguo6118.cn

D. 数组 / 列表 / 集合
来源：https://pj.zhonguo5118.cn

================================================================================
来源：https://ge.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://bz.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://tx.zhonguo5118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://rg.zhonguo4118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://ju.zhonguo2118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://id.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://oz.zhonguo6118.cn

Go:   arr := []int{1, 2, 3}
来源：https://sg.zhonguo3118.cn

Ruby: arr = [1, 2, 3]
来源：https://uu.zhonguo1118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://mf.zhonguo1118.cn

[D02] 追加元素到末尾
来源：https://ia.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://yu.zhonguo1118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://yw.zhonguo3118.cn

JS:   arr.push(4);
来源：https://vz.zhonguo4118.cn

TS:   arr.push(4);
来源：https://pf.zhonguo1118.cn

Java: list.add(4);
来源：https://sz.zhonguo6118.cn

Go:   arr = append(arr, 4)
来源：https://qe.zhonguo6118.cn

Ruby: arr << 4; arr.push(5)
来源：https://ck.zhonguo3118.cn

C#:   list.Add(4);
来源：https://gb.zhonguo7118.cn

[D03] 在指定位置插入元素
来源：https://on.zhonguo4118.cn

Py:   arr.insert(0, 0)
来源：https://lg.zhonguo2118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://vv.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://ja.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://eu.zhonguo7118.cn

Java: list.add(0, 0);
来源：https://gp.zhonguo3118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://wf.zhonguo1118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://gm.zhonguo4118.cn

C#:   list.Insert(0, 0);
来源：https://ce.zhonguo2118.cn

[D04] 删除元素
来源：https://wl.zhonguo3118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://nu.zhonguo6118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://vb.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://nm.zhonguo6118.cn

TS:   arr.splice(0, 1);
来源：https://zy.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://qk.zhonguo4118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://yx.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://ka.zhonguo5118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://yz.zhonguo3118.cn

[D05] 访问与修改元素
来源：https://tk.zhonguo2118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://bm.zhonguo4118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://rv.zhonguo5118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://gg.zhonguo5118.cn

TS:   arr[0]; arr.at(-1);
来源：https://hp.zhonguo1118.cn

Java: list.get(0); list.set(0, 9);
来源：https://jz.zhonguo6118.cn

Go:   arr[0]; arr[0] = 9
来源：https://lv.zhonguo2118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://pz.zhonguo7118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://xd.zhonguo3118.cn

[D06] 数组长度
来源：https://bx.zhonguo2118.cn

Py:   len(arr)
来源：https://nz.zhonguo4118.cn

PHP:  count($arr);
来源：https://cu.zhonguo3118.cn

JS:   arr.length
来源：https://ha.zhonguo4118.cn

TS:   arr.length
来源：https://vn.zhonguo3118.cn

Java: list.size();
来源：https://tc.zhonguo1118.cn

Go:   len(arr)
来源：https://us.zhonguo7118.cn

Ruby: arr.length; arr.size
来源：https://pz.zhonguo7118.cn

C#:   list.Count;
来源：https://az.zhonguo6118.cn

[D07] 切片 / 取子数组
来源：https://tg.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://uh.zhonguo2118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://fl.zhonguo8118.cn

JS:   arr.slice(1, 4);
来源：https://nl.zhonguo2118.cn

TS:   arr.slice(1, 4);
来源：https://cr.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://uk.zhonguo8118.cn

Go:   arr[1:4]
来源：https://dh.zhonguo5118.cn

Ruby: arr[1, 3]
来源：https://hf.zhonguo7118.cn

C#:   list.GetRange(1, 3);
来源：https://fl.zhonguo5118.cn

[D08] 合并两个数组
来源：https://eq.zhonguo7118.cn

Py:   a + b;  a.extend(b)
来源：https://jl.zhonguo5118.cn

PHP:  array_merge($a, $b);
来源：https://ec.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://xm.zhonguo4118.cn

TS:   [...a, ...b];
来源：https://rn.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ca.zhonguo2118.cn

Go:   append(a, b...)
来源：https://za.zhonguo2118.cn

Ruby: a + b;  a.concat(b)
来源：https://iz.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://be.zhonguo4118.cn

[D09] 排序（升序）
来源：https://bp.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://qe.zhonguo3118.cn

PHP:  sort($arr);
来源：https://ed.zhonguo3118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://am.zhonguo8118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ej.zhonguo7118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://zd.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://uj.zhonguo2118.cn

Ruby: arr.sort
来源：https://gn.zhonguo8118.cn

C#:   list.Sort();
来源：https://ee.zhonguo4118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://lr.zhonguo3118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://bo.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fm.zhonguo6118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://ww.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ud.zhonguo6118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://ou.zhonguo7118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://yi.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ka.zhonguo5118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://iu.zhonguo5118.cn

[D11] 反转数组
来源：https://av.zhonguo3118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://gs.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://fq.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://lp.zhonguo8118.cn

TS:   [...arr].reverse();
来源：https://dl.zhonguo7118.cn

Java: Collections.reverse(list);
来源：https://ji.zhonguo1118.cn

Go:   slices.Reverse(arr)
来源：https://id.zhonguo6118.cn

Ruby: arr.reverse
来源：https://rn.zhonguo4118.cn

C#:   list.Reverse();
来源：https://su.zhonguo2118.cn

[D12] 查找元素下标
来源：https://vg.zhonguo7118.cn

Py:   arr.index(x);  x in arr
来源：https://gy.zhonguo8118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://uw.zhonguo4118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ez.zhonguo7118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://wq.zhonguo2118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://pm.zhonguo2118.cn

Go:   slices.Index(arr, x)
来源：https://qp.zhonguo4118.cn

Ruby: arr.index(x)
来源：https://re.zhonguo7118.cn

C#:   list.IndexOf(x);
来源：https://mm.zhonguo3118.cn

[D13] 过滤（保留满足条件的）
来源：https://ji.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://fs.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://rs.zhonguo8118.cn

JS:   arr.filter(x => x > 3)
来源：https://wr.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://ei.zhonguo3118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://xv.zhonguo3118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://aj.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fd.zhonguo7118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://yq.zhonguo1118.cn

[D14] 映射转换（每个元素变形）
来源：https://kd.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://is.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://or.zhonguo6118.cn

JS:   arr.map(x => x * 2)
来源：https://al.zhonguo5118.cn

TS:   arr.map(x => x * 2)
来源：https://zh.zhonguo6118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://tf.zhonguo1118.cn

Go:   // 手写循环
来源：https://zf.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://mm.zhonguo2118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://wc.zhonguo8118.cn

[D15] 去重
来源：https://ep.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://to.zhonguo2118.cn

PHP:  array_unique($arr);
来源：https://pb.zhonguo8118.cn

JS:   [...new Set(arr)]
来源：https://xf.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://rb.zhonguo8118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ex.zhonguo6118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://hx.zhonguo7118.cn

Ruby: arr.uniq
来源：https://ni.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://tv.zhonguo4118.cn

[D16] 求和与平均值
来源：https://vp.zhonguo8118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://gi.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ez.zhonguo6118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://qx.zhonguo5118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://wf.zhonguo1118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://sq.zhonguo5118.cn

Go:   // 手写循环累加
来源：https://yv.zhonguo7118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://hu.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://xx.zhonguo8118.cn

[D17] 最大值与最小值
来源：https://bp.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://ah.zhonguo6118.cn

PHP:  max($arr);  min($arr);
来源：https://pd.zhonguo3118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://oq.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://wu.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://lc.zhonguo3118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://pd.zhonguo1118.cn

Ruby: arr.max;  arr.min
来源：https://tn.zhonguo8118.cn

C#:   list.Max();  list.Min()
来源：https://eg.zhonguo3118.cn

[D18] 扁平化嵌套数组
来源：https://nh.zhonguo1118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://eu.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://fa.zhonguo7118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://cg.zhonguo8118.cn

TS:   nested.flat();
来源：https://oy.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://qz.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://oy.zhonguo6118.cn

Ruby: nested.flatten
来源：https://nk.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://fr.zhonguo7118.cn

[D19] 按字段分组
来源：https://jh.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://pd.zhonguo1118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ah.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://oh.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://gu.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://nk.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://tg.zhonguo4118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://gz.zhonguo6118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://gm.zhonguo3118.cn

[D20] 统计每个元素出现次数
来源：https://cm.zhonguo1118.cn

Py:   Counter(arr)
来源：https://hw.zhonguo4118.cn

PHP:  array_count_values($arr);
来源：https://tf.zhonguo1118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://nc.zhonguo7118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://dk.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://wa.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://aa.zhonguo4118.cn

Ruby: arr.tally
来源：https://ov.zhonguo4118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://fh.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://ps.zhonguo4118.cn

Py:   x in arr
来源：https://vd.zhonguo6118.cn

PHP:  in_array($x, $arr, true);
来源：https://dd.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://ll.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://lv.zhonguo5118.cn

Java: list.contains(x)
来源：https://zo.zhonguo3118.cn

Go:   slices.Contains(arr, x)
来源：https://rw.zhonguo8118.cn

Ruby: arr.include?(x)
来源：https://qs.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://qw.zhonguo4118.cn

[D22] 复制数组（避免共享引用）
来源：https://wt.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://mv.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://af.zhonguo3118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://hb.zhonguo6118.cn

TS:   [...arr];
来源：https://qk.zhonguo8118.cn

Java: new ArrayList<>(list);
来源：https://qq.zhonguo7118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://fs.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://ac.zhonguo2118.cn

C#:   new List<int>(list);
来源：https://ij.zhonguo5118.cn

[D23] reduce 累积计算
来源：https://mg.zhonguo1118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://qf.zhonguo7118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://zq.zhonguo6118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://gb.zhonguo2118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://or.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://lr.zhonguo2118.cn

Go:   // 手写循环
来源：https://rs.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://jj.zhonguo3118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://td.zhonguo1118.cn

[D24] 字典 / Map 基本操作
来源：https://bn.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://iz.zhonguo6118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://uq.zhonguo1118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://ff.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://uo.zhonguo7118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://pi.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://ys.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://vc.zhonguo8118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://gv.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://cl.zhonguo7118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zm.zhonguo8118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ye.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ul.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://sx.zhonguo4118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://uv.zhonguo8118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://he.zhonguo7118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://kh.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://fr.zhonguo3118.cn

[D26] 数组转字符串
来源：https://rd.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://vl.zhonguo5118.cn

PHP:  implode(", ", $arr);
来源：https://mi.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://gb.zhonguo6118.cn

TS:   arr.join(", ")
来源：https://by.zhonguo4118.cn

Java: String.join(", ", list)
来源：https://ri.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://an.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://hi.zhonguo7118.cn

C#:   string.Join(", ", list)
来源：https://wz.zhonguo4118.cn

================================================================================
来源：https://cz.zhonguo7118.cn

E. 字符串处理
来源：https://xg.zhonguo3118.cn

================================================================================
来源：https://ln.zhonguo1118.cn

[E01] 拼接字符串
来源：https://ka.zhonguo3118.cn


<!-- 参考信息 -->