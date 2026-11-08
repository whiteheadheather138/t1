代发 wailian999

[C10] 变量作用域
来源：https://th.zhonguo6118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://qk.zhonguo7118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://mm.zhonguo7118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://lc.zhonguo8118.cn

TS:   同 JS
来源：https://uv.zhonguo5118.cn

Java: 方法内为块级作用域
来源：https://zw.zhonguo7118.cn

Go:   花括号块级作用域
来源：https://uy.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://qb.zhonguo4118.cn

C#:   块级作用域
来源：https://nq.zhonguo1118.cn

[C11] 模块导入与导出
来源：https://ou.zhonguo6118.cn

Py:   from module import func
来源：https://rd.zhonguo8118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://iw.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://ir.zhonguo4118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://re.zhonguo3118.cn

Java: import java.util.List;
来源：https://nn.zhonguo8118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://lq.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://qx.zhonguo2118.cn

C#:   using System.Text;
来源：https://se.zhonguo6118.cn

[C12] 立即执行函数 IIFE
来源：https://te.zhonguo4118.cn

Py:   (lambda: print("run"))()
来源：https://pv.zhonguo7118.cn

PHP:  (function () { echo "run"; })();
来源：https://cj.zhonguo7118.cn

JS:   (() => { console.log("run"); })();
来源：https://hu.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://si.zhonguo7118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ca.zhonguo8118.cn

Go:   func() { fmt.Println("run") }()
来源：https://ks.zhonguo7118.cn

Ruby: -> { puts "run" }.call
来源：https://yk.zhonguo5118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://tk.zhonguo3118.cn

[C13] 类型声明 / 类型注解
来源：https://vf.zhonguo7118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://hp.zhonguo3118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://jy.zhonguo5118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://ww.zhonguo5118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://ls.zhonguo7118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://lr.zhonguo4118.cn

Go:   func add(a, b int) int
来源：https://ps.zhonguo1118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://cj.zhonguo1118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://iz.zhonguo3118.cn

[C14] 泛型函数
来源：https://up.zhonguo5118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://dh.zhonguo3118.cn

PHP:  // 无泛型
来源：https://wc.zhonguo5118.cn

JS:   // 无泛型
来源：https://qz.zhonguo5118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://cz.zhonguo4118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://rw.zhonguo3118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://pd.zhonguo2118.cn

Ruby: # 无泛型
来源：https://xo.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://kv.zhonguo4118.cn

[C15] 解构 / 展开参数
来源：https://rv.zhonguo2118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://gr.zhonguo5118.cn

PHP:  [$a, $b] = $pair;
来源：https://cm.zhonguo4118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://nu.zhonguo5118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://gf.zhonguo2118.cn

Java: // 无解构
来源：https://ot.zhonguo4118.cn

Go:   // 无解构
来源：https://uu.zhonguo1118.cn

Ruby: a, b = pair
来源：https://yt.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://uy.zhonguo3118.cn

[C16] 函数 / 方法重载
来源：https://ou.zhonguo2118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://uf.zhonguo1118.cn

PHP:  // 无重载
来源：https://gv.zhonguo8118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://ai.zhonguo6118.cn

TS:   // 用联合类型或重载签名声明
来源：https://vd.zhonguo1118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://hu.zhonguo2118.cn

Go:   // 无重载：用不同函数名
来源：https://pp.zhonguo7118.cn

Ruby: # 无重载：靠动态参数
来源：https://qz.zhonguo4118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://jt.zhonguo7118.cn

================================================================================
来源：https://tj.zhonguo3118.cn

D. 数组 / 列表 / 集合
来源：https://th.zhonguo4118.cn

================================================================================
来源：https://ke.zhonguo6118.cn

[D01] 创建数组 / 列表
来源：https://di.zhonguo3118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://za.zhonguo8118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://uc.zhonguo5118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://lh.zhonguo6118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://zr.zhonguo2118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://vp.zhonguo7118.cn

Go:   arr := []int{1, 2, 3}
来源：https://jp.zhonguo4118.cn

Ruby: arr = [1, 2, 3]
来源：https://yh.zhonguo8118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://la.zhonguo8118.cn

[D02] 追加元素到末尾
来源：https://gb.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://zx.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://tm.zhonguo5118.cn

JS:   arr.push(4);
来源：https://oo.zhonguo7118.cn

TS:   arr.push(4);
来源：https://od.zhonguo2118.cn

Java: list.add(4);
来源：https://qm.zhonguo7118.cn

Go:   arr = append(arr, 4)
来源：https://kj.zhonguo7118.cn

Ruby: arr << 4; arr.push(5)
来源：https://cl.zhonguo3118.cn

C#:   list.Add(4);
来源：https://kb.zhonguo6118.cn

[D03] 在指定位置插入元素
来源：https://ef.zhonguo8118.cn

Py:   arr.insert(0, 0)
来源：https://wc.zhonguo6118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://rb.zhonguo2118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://zi.zhonguo5118.cn

TS:   arr.splice(0, 0, 0);
来源：https://dx.zhonguo6118.cn

Java: list.add(0, 0);
来源：https://vs.zhonguo6118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://nj.zhonguo2118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://qk.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://yl.zhonguo8118.cn

[D04] 删除元素
来源：https://ib.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://wt.zhonguo2118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ap.zhonguo8118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://lb.zhonguo5118.cn

TS:   arr.splice(0, 1);
来源：https://on.zhonguo7118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ys.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://ec.zhonguo1118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://dc.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://kw.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://li.zhonguo7118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://wi.zhonguo5118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://wu.zhonguo1118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://ht.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://gf.zhonguo5118.cn

Java: list.get(0); list.set(0, 9);
来源：https://fp.zhonguo3118.cn

Go:   arr[0]; arr[0] = 9
来源：https://je.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://hh.zhonguo7118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://im.zhonguo3118.cn

[D06] 数组长度
来源：https://pt.zhonguo4118.cn

Py:   len(arr)
来源：https://oa.zhonguo7118.cn

PHP:  count($arr);
来源：https://pw.zhonguo1118.cn

JS:   arr.length
来源：https://ni.zhonguo8118.cn

TS:   arr.length
来源：https://rq.zhonguo7118.cn

Java: list.size();
来源：https://qt.zhonguo8118.cn

Go:   len(arr)
来源：https://vc.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://aq.zhonguo6118.cn

C#:   list.Count;
来源：https://lm.zhonguo2118.cn

[D07] 切片 / 取子数组
来源：https://kt.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://hw.zhonguo1118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://sj.zhonguo8118.cn

JS:   arr.slice(1, 4);
来源：https://si.zhonguo8118.cn

TS:   arr.slice(1, 4);
来源：https://tp.zhonguo2118.cn

Java: list.subList(1, 4);
来源：https://ha.zhonguo2118.cn

Go:   arr[1:4]
来源：https://ip.zhonguo3118.cn

Ruby: arr[1, 3]
来源：https://gm.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://aw.zhonguo1118.cn

[D08] 合并两个数组
来源：https://mc.zhonguo5118.cn

Py:   a + b;  a.extend(b)
来源：https://dq.zhonguo3118.cn

PHP:  array_merge($a, $b);
来源：https://cs.zhonguo8118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://lm.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://kc.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://sm.zhonguo6118.cn

Go:   append(a, b...)
来源：https://ea.zhonguo8118.cn

Ruby: a + b;  a.concat(b)
来源：https://jq.zhonguo7118.cn

C#:   a.Concat(b).ToList()
来源：https://rk.zhonguo8118.cn

[D09] 排序（升序）
来源：https://na.zhonguo7118.cn

Py:   sorted(arr);  arr.sort()
来源：https://ei.zhonguo3118.cn

PHP:  sort($arr);
来源：https://cq.zhonguo2118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://dz.zhonguo2118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ea.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://wu.zhonguo2118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://yx.zhonguo1118.cn

Ruby: arr.sort
来源：https://xo.zhonguo5118.cn

C#:   list.Sort();
来源：https://ol.zhonguo2118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://zu.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://cg.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://is.zhonguo7118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://sg.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://nc.zhonguo7118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://yh.zhonguo1118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://na.zhonguo2118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://jt.zhonguo4118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://rk.zhonguo2118.cn

[D11] 反转数组
来源：https://cm.zhonguo3118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://sg.zhonguo4118.cn

PHP:  array_reverse($arr);
来源：https://jr.zhonguo5118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://rf.zhonguo7118.cn

TS:   [...arr].reverse();
来源：https://yr.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://fs.zhonguo4118.cn

Go:   slices.Reverse(arr)
来源：https://sx.zhonguo5118.cn

Ruby: arr.reverse
来源：https://ca.zhonguo5118.cn

C#:   list.Reverse();
来源：https://fy.zhonguo5118.cn

[D12] 查找元素下标
来源：https://sj.zhonguo1118.cn

Py:   arr.index(x);  x in arr
来源：https://ha.zhonguo6118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://rt.zhonguo3118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://dj.zhonguo3118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://dx.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://lt.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://bz.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://xy.zhonguo7118.cn

C#:   list.IndexOf(x);
来源：https://ml.zhonguo3118.cn

[D13] 过滤（保留满足条件的）
来源：https://ur.zhonguo7118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://it.zhonguo7118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://jx.zhonguo6118.cn

JS:   arr.filter(x => x > 3)
来源：https://sj.zhonguo1118.cn

TS:   arr.filter(x => x > 3)
来源：https://nh.zhonguo7118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://nq.zhonguo4118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://tc.zhonguo1118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://wm.zhonguo6118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://pp.zhonguo1118.cn

[D14] 映射转换（每个元素变形）
来源：https://me.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://gb.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://xk.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://pw.zhonguo6118.cn

TS:   arr.map(x => x * 2)
来源：https://tq.zhonguo6118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://re.zhonguo7118.cn

Go:   // 手写循环
来源：https://rw.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://bi.zhonguo8118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://hi.zhonguo8118.cn

[D15] 去重
来源：https://tu.zhonguo3118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ei.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://fq.zhonguo8118.cn

JS:   [...new Set(arr)]
来源：https://rb.zhonguo2118.cn

TS:   [...new Set(arr)]
来源：https://eq.zhonguo3118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://do.zhonguo3118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://gj.zhonguo2118.cn

Ruby: arr.uniq
来源：https://hv.zhonguo5118.cn

C#:   list.Distinct().ToList()
来源：https://tz.zhonguo6118.cn

[D16] 求和与平均值
来源：https://fk.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://py.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ou.zhonguo8118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://za.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://if.zhonguo3118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://dy.zhonguo5118.cn

Go:   // 手写循环累加
来源：https://xh.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://mc.zhonguo7118.cn

C#:   list.Sum();  list.Average()
来源：https://qy.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://kz.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://uk.zhonguo4118.cn

PHP:  max($arr);  min($arr);
来源：https://mo.zhonguo5118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://lt.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://nr.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://yo.zhonguo8118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://qf.zhonguo5118.cn

Ruby: arr.max;  arr.min
来源：https://dy.zhonguo5118.cn

C#:   list.Max();  list.Min()
来源：https://nl.zhonguo5118.cn

[D18] 扁平化嵌套数组
来源：https://ov.zhonguo4118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://bj.zhonguo1118.cn

PHP:  array_merge(...$nested);
来源：https://ss.zhonguo4118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://le.zhonguo6118.cn

TS:   nested.flat();
来源：https://tq.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://qo.zhonguo5118.cn

Go:   // 手写双层循环
来源：https://fa.zhonguo1118.cn

Ruby: nested.flatten
来源：https://up.zhonguo4118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://pa.zhonguo4118.cn

[D19] 按字段分组
来源：https://ea.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://kt.zhonguo8118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://cw.zhonguo1118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://wi.zhonguo2118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://cg.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ge.zhonguo7118.cn

Go:   // 手写 map[string][]T
来源：https://dy.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ln.zhonguo6118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://pj.zhonguo7118.cn

[D20] 统计每个元素出现次数
来源：https://wa.zhonguo2118.cn

Py:   Counter(arr)
来源：https://ql.zhonguo7118.cn

PHP:  array_count_values($arr);
来源：https://rh.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://wx.zhonguo8118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://pb.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://sf.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://uk.zhonguo5118.cn

Ruby: arr.tally
来源：https://ii.zhonguo3118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://jd.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://fr.zhonguo1118.cn

Py:   x in arr
来源：https://ib.zhonguo2118.cn

PHP:  in_array($x, $arr, true);
来源：https://kb.zhonguo5118.cn

JS:   arr.includes(x)
来源：https://lc.zhonguo4118.cn

TS:   arr.includes(x)
来源：https://mc.zhonguo4118.cn

Java: list.contains(x)
来源：https://zh.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://ql.zhonguo8118.cn

Ruby: arr.include?(x)
来源：https://db.zhonguo3118.cn

C#:   list.Contains(x)
来源：https://nh.zhonguo8118.cn

[D22] 复制数组（避免共享引用）
来源：https://hx.zhonguo8118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://uv.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://wl.zhonguo2118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://vt.zhonguo6118.cn

TS:   [...arr];
来源：https://vs.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://xj.zhonguo1118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://tj.zhonguo4118.cn

Ruby: arr.dup;  arr.clone
来源：https://ys.zhonguo1118.cn

C#:   new List<int>(list);
来源：https://zb.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://tj.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://en.zhonguo4118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://kv.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://tu.zhonguo1118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://qx.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://gx.zhonguo2118.cn

Go:   // 手写循环
来源：https://tp.zhonguo5118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://kz.zhonguo3118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://ha.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://xl.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://qa.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://za.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://yy.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://ef.zhonguo4118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://lk.zhonguo2118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://hw.zhonguo2118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ax.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://pw.zhonguo6118.cn

[D25] Set 集合去重与交并差
来源：https://oo.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://gy.zhonguo7118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://qt.zhonguo1118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ao.zhonguo6118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://lp.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://rs.zhonguo2118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://wn.zhonguo4118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://tv.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ne.zhonguo2118.cn

[D26] 数组转字符串
来源：https://vv.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://yo.zhonguo1118.cn

PHP:  implode(", ", $arr);
来源：https://fm.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://sn.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://lh.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://wq.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://lt.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://kk.zhonguo7118.cn

C#:   string.Join(", ", list)
来源：https://fe.zhonguo7118.cn


<!-- 参考信息 -->