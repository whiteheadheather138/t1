代发 wailian999

[C10] 变量作用域
来源：https://kz.zhonguo8118.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：https://gw.zhonguo6118.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：https://rb.zhonguo8118.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：https://qn.zhonguo1118.cn

TS:   同 JS
来源：https://rt.zhonguo6118.cn

Java: 方法内为块级作用域
来源：https://hg.zhonguo5118.cn

Go:   花括号块级作用域
来源：https://kq.zhonguo6118.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：https://hs.zhonguo2118.cn

C#:   块级作用域
来源：https://cb.zhonguo8118.cn

[C11] 模块导入与导出
来源：https://cr.zhonguo5118.cn

Py:   from module import func
来源：https://qu.zhonguo4118.cn

PHP:  require "file.php";  或 use App\Service;
来源：https://kn.zhonguo4118.cn

JS:   export default function f() {};  import f from "./m.js";
来源：https://ml.zhonguo4118.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：https://pr.zhonguo2118.cn

Java: import java.util.List;
来源：https://my.zhonguo1118.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：https://nk.zhonguo6118.cn

Ruby: require "json"; require_relative "./util"
来源：https://pn.zhonguo8118.cn

C#:   using System.Text;
来源：https://hm.zhonguo2118.cn

[C12] 立即执行函数 IIFE
来源：https://au.zhonguo5118.cn

Py:   (lambda: print("run"))()
来源：https://kq.zhonguo3118.cn

PHP:  (function () { echo "run"; })();
来源：https://tr.zhonguo4118.cn

JS:   (() => { console.log("run"); })();
来源：https://nf.zhonguo2118.cn

TS:   (() => { console.log("run"); })();
来源：https://ir.zhonguo6118.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：https://ha.zhonguo3118.cn

Go:   func() { fmt.Println("run") }()
来源：https://zs.zhonguo5118.cn

Ruby: -> { puts "run" }.call
来源：https://wt.zhonguo2118.cn

C#:   // 无 IIFE：用静态构造函数
来源：https://kr.zhonguo7118.cn

[C13] 类型声明 / 类型注解
来源：https://vg.zhonguo8118.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：https://yq.zhonguo5118.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：https://yb.zhonguo4118.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：https://dt.zhonguo8118.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：https://qz.zhonguo8118.cn

Java: int add(int a, int b) { return a + b; }
来源：https://qc.zhonguo7118.cn

Go:   func add(a, b int) int
来源：https://cw.zhonguo6118.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：https://iu.zhonguo6118.cn

C#:   int Add(int a, int b) => a + b;
来源：https://pn.zhonguo6118.cn

[C14] 泛型函数
来源：https://uy.zhonguo1118.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：https://xe.zhonguo7118.cn

PHP:  // 无泛型
来源：https://ge.zhonguo4118.cn

JS:   // 无泛型
来源：https://sa.zhonguo8118.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：https://ed.zhonguo3118.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：https://if.zhonguo8118.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：https://zd.zhonguo2118.cn

Ruby: # 无泛型
来源：https://ix.zhonguo6118.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：https://kb.zhonguo5118.cn

[C15] 解构 / 展开参数
来源：https://nc.zhonguo3118.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：https://wa.zhonguo1118.cn

PHP:  [$a, $b] = $pair;
来源：https://vo.zhonguo1118.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：https://ki.zhonguo2118.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：https://gd.zhonguo3118.cn

Java: // 无解构
来源：https://bu.zhonguo3118.cn

Go:   // 无解构
来源：https://ou.zhonguo3118.cn

Ruby: a, b = pair
来源：https://cr.zhonguo4118.cn

C#:   var (a, b) = pair;
来源：https://ka.zhonguo3118.cn

[C16] 函数 / 方法重载
来源：https://cm.zhonguo1118.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：https://ws.zhonguo2118.cn

PHP:  // 无重载
来源：https://rc.zhonguo1118.cn

JS:   // 无重载：靠 arguments.length 分支
来源：https://qt.zhonguo2118.cn

TS:   // 用联合类型或重载签名声明
来源：https://dr.zhonguo6118.cn

Java: void f(int a) {}  void f(String a) {}
来源：https://mn.zhonguo3118.cn

Go:   // 无重载：用不同函数名
来源：https://xu.zhonguo2118.cn

Ruby: # 无重载：靠动态参数
来源：https://gl.zhonguo2118.cn

C#:   void F(int a) {}  void F(string a) {}
来源：https://iq.zhonguo7118.cn

================================================================================
来源：https://em.zhonguo2118.cn

D. 数组 / 列表 / 集合
来源：https://yc.zhonguo5118.cn

================================================================================
来源：https://fa.zhonguo8118.cn

[D01] 创建数组 / 列表
来源：https://jg.zhonguo4118.cn

Py:   arr = [1, 2, 3];  empty = []
来源：https://hf.zhonguo2118.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：https://ai.zhonguo6118.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：https://qk.zhonguo4118.cn

TS:   const arr: number[] = [1, 2, 3];
来源：https://xm.zhonguo4118.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：https://gu.zhonguo7118.cn

Go:   arr := []int{1, 2, 3}
来源：https://us.zhonguo1118.cn

Ruby: arr = [1, 2, 3]
来源：https://ie.zhonguo1118.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：https://zi.zhonguo3118.cn

[D02] 追加元素到末尾
来源：https://cq.zhonguo1118.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：https://pt.zhonguo4118.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：https://uk.zhonguo1118.cn

JS:   arr.push(4);
来源：https://ed.zhonguo8118.cn

TS:   arr.push(4);
来源：https://uc.zhonguo3118.cn

Java: list.add(4);
来源：https://ei.zhonguo5118.cn

Go:   arr = append(arr, 4)
来源：https://ee.zhonguo4118.cn

Ruby: arr << 4; arr.push(5)
来源：https://uy.zhonguo1118.cn

C#:   list.Add(4);
来源：https://di.zhonguo4118.cn

[D03] 在指定位置插入元素
来源：https://sc.zhonguo2118.cn

Py:   arr.insert(0, 0)
来源：https://uk.zhonguo6118.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：https://vu.zhonguo6118.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：https://fx.zhonguo3118.cn

TS:   arr.splice(0, 0, 0);
来源：https://sr.zhonguo8118.cn

Java: list.add(0, 0);
来源：https://fx.zhonguo4118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://lf.zhonguo5118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://zr.zhonguo5118.cn

C#:   list.Insert(0, 0);
来源：https://bh.zhonguo4118.cn

[D04] 删除元素
来源：https://cw.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://wn.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://ck.zhonguo5118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://yg.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://sd.zhonguo6118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://lg.zhonguo1118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://dm.zhonguo4118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://gu.zhonguo5118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://vz.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://zp.zhonguo6118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://xj.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://bc.zhonguo3118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://wr.zhonguo3118.cn

TS:   arr[0]; arr.at(-1);
来源：https://ip.zhonguo1118.cn

Java: list.get(0); list.set(0, 9);
来源：https://qc.zhonguo8118.cn

Go:   arr[0]; arr[0] = 9
来源：https://qk.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://je.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://mf.zhonguo3118.cn

[D06] 数组长度
来源：https://ea.zhonguo7118.cn

Py:   len(arr)
来源：https://gv.zhonguo7118.cn

PHP:  count($arr);
来源：https://hn.zhonguo6118.cn

JS:   arr.length
来源：https://si.zhonguo3118.cn

TS:   arr.length
来源：https://ff.zhonguo7118.cn

Java: list.size();
来源：https://da.zhonguo3118.cn

Go:   len(arr)
来源：https://ue.zhonguo5118.cn

Ruby: arr.length; arr.size
来源：https://mg.zhonguo5118.cn

C#:   list.Count;
来源：https://hj.zhonguo5118.cn

[D07] 切片 / 取子数组
来源：https://dz.zhonguo1118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://yx.zhonguo8118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://pt.zhonguo4118.cn

JS:   arr.slice(1, 4);
来源：https://bp.zhonguo3118.cn

TS:   arr.slice(1, 4);
来源：https://ox.zhonguo1118.cn

Java: list.subList(1, 4);
来源：https://wn.zhonguo4118.cn

Go:   arr[1:4]
来源：https://iq.zhonguo8118.cn

Ruby: arr[1, 3]
来源：https://go.zhonguo2118.cn

C#:   list.GetRange(1, 3);
来源：https://sx.zhonguo1118.cn

[D08] 合并两个数组
来源：https://nb.zhonguo3118.cn

Py:   a + b;  a.extend(b)
来源：https://dc.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://aa.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ma.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://sl.zhonguo7118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://tn.zhonguo4118.cn

Go:   append(a, b...)
来源：https://sh.zhonguo6118.cn

Ruby: a + b;  a.concat(b)
来源：https://zd.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://sy.zhonguo6118.cn

[D09] 排序（升序）
来源：https://ji.zhonguo6118.cn

Py:   sorted(arr);  arr.sort()
来源：https://pl.zhonguo1118.cn

PHP:  sort($arr);
来源：https://bv.zhonguo7118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://yp.zhonguo4118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://ci.zhonguo5118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://ao.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://bd.zhonguo5118.cn

Ruby: arr.sort
来源：https://xq.zhonguo4118.cn

C#:   list.Sort();
来源：https://jz.zhonguo5118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://qa.zhonguo6118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://kr.zhonguo5118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://au.zhonguo8118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://gh.zhonguo6118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://fe.zhonguo1118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://tr.zhonguo7118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://om.zhonguo7118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ej.zhonguo4118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://tl.zhonguo3118.cn

[D11] 反转数组
来源：https://el.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://ot.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://yp.zhonguo8118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://kk.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://es.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://ta.zhonguo6118.cn

Go:   slices.Reverse(arr)
来源：https://ic.zhonguo8118.cn

Ruby: arr.reverse
来源：https://sj.zhonguo6118.cn

C#:   list.Reverse();
来源：https://sy.zhonguo1118.cn

[D12] 查找元素下标
来源：https://xx.zhonguo2118.cn

Py:   arr.index(x);  x in arr
来源：https://hz.zhonguo7118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://bh.zhonguo2118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ki.zhonguo7118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jv.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://wq.zhonguo7118.cn

Go:   slices.Index(arr, x)
来源：https://to.zhonguo8118.cn

Ruby: arr.index(x)
来源：https://cs.zhonguo1118.cn

C#:   list.IndexOf(x);
来源：https://qd.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://qu.zhonguo8118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://bp.zhonguo6118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://pv.zhonguo8118.cn

JS:   arr.filter(x => x > 3)
来源：https://om.zhonguo1118.cn

TS:   arr.filter(x => x > 3)
来源：https://fg.zhonguo6118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://ih.zhonguo6118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://jo.zhonguo2118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ae.zhonguo8118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://vt.zhonguo4118.cn

[D14] 映射转换（每个元素变形）
来源：https://lq.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://bn.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://po.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://sb.zhonguo4118.cn

TS:   arr.map(x => x * 2)
来源：https://gt.zhonguo1118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://zq.zhonguo6118.cn

Go:   // 手写循环
来源：https://sm.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vf.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://dn.zhonguo5118.cn

[D15] 去重
来源：https://nr.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ib.zhonguo1118.cn

PHP:  array_unique($arr);
来源：https://as.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://dg.zhonguo2118.cn

TS:   [...new Set(arr)]
来源：https://yr.zhonguo4118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ts.zhonguo4118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://sa.zhonguo8118.cn

Ruby: arr.uniq
来源：https://qf.zhonguo6118.cn

C#:   list.Distinct().ToList()
来源：https://co.zhonguo3118.cn

[D16] 求和与平均值
来源：https://fg.zhonguo7118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://eg.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://bj.zhonguo7118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://by.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://oa.zhonguo1118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://xt.zhonguo1118.cn

Go:   // 手写循环累加
来源：https://yi.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://rg.zhonguo7118.cn

C#:   list.Sum();  list.Average()
来源：https://ut.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://dz.zhonguo6118.cn

Py:   max(arr);  min(arr)
来源：https://yh.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://qe.zhonguo1118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://qd.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://xh.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://rf.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://lf.zhonguo5118.cn

Ruby: arr.max;  arr.min
来源：https://cy.zhonguo2118.cn

C#:   list.Max();  list.Min()
来源：https://vs.zhonguo5118.cn

[D18] 扁平化嵌套数组
来源：https://ca.zhonguo3118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://sv.zhonguo7118.cn

PHP:  array_merge(...$nested);
来源：https://jk.zhonguo1118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://if.zhonguo3118.cn

TS:   nested.flat();
来源：https://xu.zhonguo3118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ry.zhonguo2118.cn

Go:   // 手写双层循环
来源：https://jf.zhonguo3118.cn

Ruby: nested.flatten
来源：https://nf.zhonguo4118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://mm.zhonguo8118.cn

[D19] 按字段分组
来源：https://sy.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://do.zhonguo5118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://mg.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://no.zhonguo7118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://cn.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://am.zhonguo3118.cn

Go:   // 手写 map[string][]T
来源：https://kc.zhonguo1118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://mw.zhonguo1118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://cd.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://jq.zhonguo7118.cn

Py:   Counter(arr)
来源：https://mr.zhonguo7118.cn

PHP:  array_count_values($arr);
来源：https://ek.zhonguo5118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ex.zhonguo7118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://yo.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://sq.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://wx.zhonguo4118.cn

Ruby: arr.tally
来源：https://xf.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://zi.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://zn.zhonguo3118.cn

Py:   x in arr
来源：https://jg.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://br.zhonguo4118.cn

JS:   arr.includes(x)
来源：https://xg.zhonguo4118.cn

TS:   arr.includes(x)
来源：https://uo.zhonguo1118.cn

Java: list.contains(x)
来源：https://bg.zhonguo4118.cn

Go:   slices.Contains(arr, x)
来源：https://hb.zhonguo3118.cn

Ruby: arr.include?(x)
来源：https://wk.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://pz.zhonguo8118.cn

[D22] 复制数组（避免共享引用）
来源：https://fx.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ke.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://au.zhonguo2118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://xc.zhonguo5118.cn

TS:   [...arr];
来源：https://hs.zhonguo8118.cn

Java: new ArrayList<>(list);
来源：https://hy.zhonguo8118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://qx.zhonguo5118.cn

Ruby: arr.dup;  arr.clone
来源：https://uv.zhonguo3118.cn

C#:   new List<int>(list);
来源：https://iv.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://re.zhonguo6118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://pp.zhonguo3118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://yw.zhonguo8118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ur.zhonguo1118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zb.zhonguo3118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://lk.zhonguo6118.cn

Go:   // 手写循环
来源：https://th.zhonguo8118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://yk.zhonguo7118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://gk.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://vp.zhonguo4118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ia.zhonguo5118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://zy.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://cj.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://bc.zhonguo7118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://vf.zhonguo2118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://sn.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://ph.zhonguo8118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ep.zhonguo6118.cn

[D25] Set 集合去重与交并差
来源：https://kx.zhonguo8118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://bs.zhonguo7118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://dy.zhonguo7118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://bf.zhonguo5118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://bv.zhonguo3118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://xq.zhonguo2118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://gd.zhonguo8118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://pn.zhonguo7118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://zk.zhonguo5118.cn

[D26] 数组转字符串
来源：https://ct.zhonguo2118.cn

Py:   ", ".join(map(str, arr))
来源：https://da.zhonguo5118.cn

PHP:  implode(", ", $arr);
来源：https://ff.zhonguo1118.cn

JS:   arr.join(", ")
来源：https://tt.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://dx.zhonguo4118.cn

Java: String.join(", ", list)
来源：https://ho.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://uc.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://hh.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://fi.zhonguo1118.cn


<!-- 参考信息 -->