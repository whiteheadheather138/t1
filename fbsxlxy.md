代发 wailian999

[C10] 变量作用域
来源：https://mn.zhonguo3118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://wx.zhonguo8118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://ki.zhonguo4118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://bp.zhonguo8118.cn

TS:   同 JS
来源：https://fq.zhonguo4118.cn

Java: 方法内为块级作用域
来源：https://hf.zhonguo2118.cn

Go:   花括号块级作用域
来源：https://nl.zhonguo2118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://rc.zhonguo8118.cn

C#:   块级作用域
来源：https://bo.zhonguo3118.cn

[C11] 模块导入与导出
来源：https://kh.zhonguo3118.cn

Py:   from module import func
来源：https://jg.zhonguo8118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://lk.zhonguo7118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://by.zhonguo6118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://kw.zhonguo3118.cn

Java: import java.util.List;
来源：https://fo.zhonguo6118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://au.zhonguo7118.cn

Ruby: require "json"; require_relative "./util"
来源：https://qn.zhonguo7118.cn

C#:   using System.Text;
来源：https://or.zhonguo7118.cn

[C12] 立即执行函数 IIFE
来源：https://hp.zhonguo6118.cn

Py:   (lambda: print("run"))()
来源：https://tr.zhonguo7118.cn

PHP:  (function () { echo "run"; })();
来源：https://tj.zhonguo8118.cn

JS:   (() => { console.log("run"); })();
来源：https://dj.zhonguo8118.cn

TS:   (() => { console.log("run"); })();
来源：https://dx.zhonguo5118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://nh.zhonguo1118.cn

Go:   func() { fmt.Println("run") }()
来源：https://ht.zhonguo1118.cn

Ruby: -> { puts "run" }.call
来源：https://ib.zhonguo8118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://uf.zhonguo2118.cn

[C13] 类型声明 / 类型注解
来源：https://bf.zhonguo2118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://yy.zhonguo1118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://ru.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://af.zhonguo6118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://tf.zhonguo6118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://mq.zhonguo3118.cn

Go:   func add(a, b int) int
来源：https://ph.zhonguo3118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://nu.zhonguo7118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://vw.zhonguo5118.cn

[C14] 泛型函数
来源：https://kt.zhonguo6118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://zo.zhonguo8118.cn

PHP:  // 无泛型
来源：https://vy.zhonguo7118.cn

JS:   // 无泛型
来源：https://ep.zhonguo5118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://md.zhonguo7118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://hd.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://fl.zhonguo1118.cn

Ruby: # 无泛型
来源：https://ri.zhonguo7118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://ij.zhonguo7118.cn

[C15] 解构 / 展开参数
来源：https://ub.zhonguo8118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://re.zhonguo7118.cn

PHP:  [$a, $b] = $pair;
来源：https://rn.zhonguo3118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://js.zhonguo8118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://pp.zhonguo6118.cn

Java: // 无解构
来源：https://yd.zhonguo5118.cn

Go:   // 无解构
来源：https://sa.zhonguo8118.cn

Ruby: a, b = pair
来源：https://cw.zhonguo1118.cn

C#:   var (a, b) = pair;
来源：https://rk.zhonguo4118.cn

[C16] 函数 / 方法重载
来源：https://ck.zhonguo8118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://az.zhonguo6118.cn

PHP:  // 无重载
来源：https://sm.zhonguo2118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://qm.zhonguo8118.cn

TS:   // 用联合类型或重载签名声明
来源：https://jm.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://zh.zhonguo7118.cn

Go:   // 无重载：用不同函数名
来源：https://np.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://yq.zhonguo3118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://he.zhonguo6118.cn

================================================================================
来源：https://yu.zhonguo4118.cn

D. 数组 / 列表 / 集合
来源：https://hz.zhonguo6118.cn

================================================================================
来源：https://lg.zhonguo7118.cn

[D01] 创建数组 / 列表
来源：https://ge.zhonguo5118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://ho.zhonguo6118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://ej.zhonguo7118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://uh.zhonguo1118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://wk.zhonguo5118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://lx.zhonguo6118.cn

Go:   arr := []int{1, 2, 3}
来源：https://qh.zhonguo8118.cn

Ruby: arr = [1, 2, 3]
来源：https://ri.zhonguo2118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://ob.zhonguo7118.cn

[D02] 追加元素到末尾
来源：https://do.zhonguo6118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://dy.zhonguo2118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://hu.zhonguo7118.cn

JS:   arr.push(4);
来源：https://of.zhonguo8118.cn

TS:   arr.push(4);
来源：https://qi.zhonguo5118.cn

Java: list.add(4);
来源：https://gk.zhonguo2118.cn

Go:   arr = append(arr, 4)
来源：https://oo.zhonguo5118.cn

Ruby: arr << 4; arr.push(5)
来源：https://qk.zhonguo6118.cn

C#:   list.Add(4);
来源：https://fj.zhonguo8118.cn

[D03] 在指定位置插入元素
来源：https://vs.zhonguo7118.cn

Py:   arr.insert(0, 0)
来源：https://sh.zhonguo5118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://oc.zhonguo7118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://yu.zhonguo1118.cn

TS:   arr.splice(0, 0, 0);
来源：https://jj.zhonguo3118.cn

Java: list.add(0, 0);
来源：https://dp.zhonguo6118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://es.zhonguo7118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://zj.zhonguo2118.cn

C#:   list.Insert(0, 0);
来源：https://ny.zhonguo7118.cn

[D04] 删除元素
来源：https://my.zhonguo5118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://it.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ia.zhonguo6118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://kt.zhonguo4118.cn

TS:   arr.splice(0, 1);
来源：https://am.zhonguo1118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://lh.zhonguo3118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://od.zhonguo6118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://gi.zhonguo6118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://tz.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://vd.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://eq.zhonguo3118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://pm.zhonguo1118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://pa.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ng.zhonguo6118.cn

Java: list.get(0); list.set(0, 9);
来源：https://qt.zhonguo1118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ld.zhonguo6118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://ru.zhonguo1118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://qd.zhonguo3118.cn

[D06] 数组长度
来源：https://hp.zhonguo3118.cn

Py:   len(arr)
来源：https://ru.zhonguo4118.cn

PHP:  count($arr);
来源：https://dy.zhonguo6118.cn

JS:   arr.length
来源：https://zx.zhonguo5118.cn

TS:   arr.length
来源：https://ij.zhonguo5118.cn

Java: list.size();
来源：https://rc.zhonguo6118.cn

Go:   len(arr)
来源：https://yx.zhonguo8118.cn

Ruby: arr.length; arr.size
来源：https://lr.zhonguo5118.cn

C#:   list.Count;
来源：https://ep.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://pp.zhonguo8118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://cw.zhonguo1118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://jc.zhonguo7118.cn

JS:   arr.slice(1, 4);
来源：https://at.zhonguo8118.cn

TS:   arr.slice(1, 4);
来源：https://nq.zhonguo5118.cn

Java: list.subList(1, 4);
来源：https://vi.zhonguo4118.cn

Go:   arr[1:4]
来源：https://qd.zhonguo3118.cn

Ruby: arr[1, 3]
来源：https://ky.zhonguo4118.cn

C#:   list.GetRange(1, 3);
来源：https://xz.zhonguo2118.cn

[D08] 合并两个数组
来源：https://my.zhonguo6118.cn

Py:   a + b;  a.extend(b)
来源：https://ql.zhonguo2118.cn

PHP:  array_merge($a, $b);
来源：https://ze.zhonguo4118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ua.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://yu.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://sc.zhonguo7118.cn

Go:   append(a, b...)
来源：https://in.zhonguo3118.cn

Ruby: a + b;  a.concat(b)
来源：https://uk.zhonguo2118.cn

C#:   a.Concat(b).ToList()
来源：https://zo.zhonguo6118.cn

[D09] 排序（升序）
来源：https://da.zhonguo3118.cn

Py:   sorted(arr);  arr.sort()
来源：https://at.zhonguo2118.cn

PHP:  sort($arr);
来源：https://ux.zhonguo5118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://kk.zhonguo6118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://rd.zhonguo5118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://yj.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://lz.zhonguo6118.cn

Ruby: arr.sort
来源：https://ql.zhonguo2118.cn

C#:   list.Sort();
来源：https://cx.zhonguo7118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://mx.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://rl.zhonguo7118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://tm.zhonguo8118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://dn.zhonguo7118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://wh.zhonguo7118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://ny.zhonguo4118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://jk.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://uj.zhonguo2118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://pw.zhonguo7118.cn

[D11] 反转数组
来源：https://wa.zhonguo3118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://ia.zhonguo6118.cn

PHP:  array_reverse($arr);
来源：https://ue.zhonguo1118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://gd.zhonguo8118.cn

TS:   [...arr].reverse();
来源：https://hw.zhonguo3118.cn

Java: Collections.reverse(list);
来源：https://xz.zhonguo5118.cn

Go:   slices.Reverse(arr)
来源：https://ld.zhonguo3118.cn

Ruby: arr.reverse
来源：https://ph.zhonguo1118.cn

C#:   list.Reverse();
来源：https://fo.zhonguo8118.cn

[D12] 查找元素下标
来源：https://xh.zhonguo7118.cn

Py:   arr.index(x);  x in arr
来源：https://yw.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://bw.zhonguo6118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jv.zhonguo6118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://cv.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://zo.zhonguo8118.cn

Go:   slices.Index(arr, x)
来源：https://qo.zhonguo1118.cn

Ruby: arr.index(x)
来源：https://ra.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://cm.zhonguo2118.cn

[D13] 过滤（保留满足条件的）
来源：https://uj.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://qt.zhonguo5118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://rn.zhonguo3118.cn

JS:   arr.filter(x => x > 3)
来源：https://ml.zhonguo6118.cn

TS:   arr.filter(x => x > 3)
来源：https://dm.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://vu.zhonguo1118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://jo.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://qt.zhonguo5118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://pd.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://xl.zhonguo7118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://sg.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://jc.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://ep.zhonguo6118.cn

TS:   arr.map(x => x * 2)
来源：https://ck.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://sn.zhonguo2118.cn

Go:   // 手写循环
来源：https://ez.zhonguo7118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://rn.zhonguo1118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://da.zhonguo5118.cn

[D15] 去重
来源：https://ti.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://cx.zhonguo2118.cn

PHP:  array_unique($arr);
来源：https://zs.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://iu.zhonguo1118.cn

TS:   [...new Set(arr)]
来源：https://pm.zhonguo1118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://st.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://ca.zhonguo5118.cn

Ruby: arr.uniq
来源：https://ch.zhonguo8118.cn

C#:   list.Distinct().ToList()
来源：https://fg.zhonguo2118.cn

[D16] 求和与平均值
来源：https://nv.zhonguo3118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://rx.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://nz.zhonguo7118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://kc.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://og.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://gd.zhonguo3118.cn

Go:   // 手写循环累加
来源：https://wb.zhonguo7118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://et.zhonguo5118.cn

C#:   list.Sum();  list.Average()
来源：https://eo.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://ds.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://zt.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://xq.zhonguo7118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://ne.zhonguo6118.cn

TS:   Math.max(...arr);
来源：https://xu.zhonguo6118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://lm.zhonguo5118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://wy.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://bb.zhonguo3118.cn

C#:   list.Max();  list.Min()
来源：https://am.zhonguo5118.cn

[D18] 扁平化嵌套数组
来源：https://bd.zhonguo7118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://yg.zhonguo3118.cn

PHP:  array_merge(...$nested);
来源：https://df.zhonguo2118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://jh.zhonguo1118.cn

TS:   nested.flat();
来源：https://kp.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://mw.zhonguo4118.cn

Go:   // 手写双层循环
来源：https://nc.zhonguo4118.cn

Ruby: nested.flatten
来源：https://ej.zhonguo8118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://qc.zhonguo4118.cn

[D19] 按字段分组
来源：https://le.zhonguo1118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://vt.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://kt.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://je.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://na.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://lh.zhonguo4118.cn

Go:   // 手写 map[string][]T
来源：https://ae.zhonguo6118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ou.zhonguo2118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://hj.zhonguo4118.cn

[D20] 统计每个元素出现次数
来源：https://yj.zhonguo5118.cn

Py:   Counter(arr)
来源：https://av.zhonguo8118.cn

PHP:  array_count_values($arr);
来源：https://hf.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://sd.zhonguo5118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://zn.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://op.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://qw.zhonguo1118.cn

Ruby: arr.tally
来源：https://cw.zhonguo1118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://gy.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://ax.zhonguo3118.cn

Py:   x in arr
来源：https://wr.zhonguo6118.cn

PHP:  in_array($x, $arr, true);
来源：https://qp.zhonguo4118.cn

JS:   arr.includes(x)
来源：https://lm.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://fk.zhonguo8118.cn

Java: list.contains(x)
来源：https://bk.zhonguo1118.cn

Go:   slices.Contains(arr, x)
来源：https://ki.zhonguo1118.cn

Ruby: arr.include?(x)
来源：https://aj.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://ao.zhonguo6118.cn

[D22] 复制数组（避免共享引用）
来源：https://hv.zhonguo8118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://cs.zhonguo8118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ds.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://yr.zhonguo1118.cn

TS:   [...arr];
来源：https://cj.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://uu.zhonguo6118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://jr.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://kh.zhonguo4118.cn

C#:   new List<int>(list);
来源：https://gk.zhonguo8118.cn

[D23] reduce 累积计算
来源：https://du.zhonguo5118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ry.zhonguo2118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://oe.zhonguo3118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ms.zhonguo5118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://qs.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://pa.zhonguo4118.cn

Go:   // 手写循环
来源：https://ys.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://kf.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://yg.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://fl.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://xg.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://vd.zhonguo2118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://mw.zhonguo1118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://fv.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://gt.zhonguo3118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://eh.zhonguo3118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://hd.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ct.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://ds.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ce.zhonguo3118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://jr.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://ed.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://lk.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://ar.zhonguo7118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://kg.zhonguo3118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://ph.zhonguo2118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ge.zhonguo1118.cn

[D26] 数组转字符串
来源：https://bv.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://oj.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://tb.zhonguo3118.cn

JS:   arr.join(", ")
来源：https://wa.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://oi.zhonguo2118.cn

Java: String.join(", ", list)
来源：https://ho.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://vv.zhonguo6118.cn

Ruby: arr.join(", ")
来源：https://jb.zhonguo2118.cn

C#:   string.Join(", ", list)
来源：https://gb.zhonguo7118.cn


<!-- 参考信息 -->