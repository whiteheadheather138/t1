代发 wailian999

C#:   list.Insert(0, 0);
来源：https://jz.zhonguo4118.cn

[D04] 删除元素
来源：https://fl.zhonguo7118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://li.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://or.zhonguo3118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://jy.zhonguo8118.cn

TS:   arr.splice(0, 1);
来源：https://yh.zhonguo7118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://ck.zhonguo1118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://pw.zhonguo3118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://kj.zhonguo1118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://fm.zhonguo5118.cn

[D05] 访问与修改元素
来源：https://tn.zhonguo4118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://tb.zhonguo5118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://jc.zhonguo5118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://xl.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://dg.zhonguo4118.cn

Java: list.get(0); list.set(0, 9);
来源：https://uh.zhonguo7118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ft.zhonguo4118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://ss.zhonguo4118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://gj.zhonguo6118.cn

[D06] 数组长度
来源：https://mx.zhonguo8118.cn

Py:   len(arr)
来源：https://xg.zhonguo8118.cn

PHP:  count($arr);
来源：https://qz.zhonguo3118.cn

JS:   arr.length
来源：https://uq.zhonguo7118.cn

TS:   arr.length
来源：https://wv.zhonguo4118.cn

Java: list.size();
来源：https://la.zhonguo2118.cn

Go:   len(arr)
来源：https://yd.zhonguo2118.cn

Ruby: arr.length; arr.size
来源：https://kh.zhonguo2118.cn

C#:   list.Count;
来源：https://aa.zhonguo4118.cn

[D07] 切片 / 取子数组
来源：https://yo.zhonguo5118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://hc.zhonguo3118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://jk.zhonguo8118.cn

JS:   arr.slice(1, 4);
来源：https://la.zhonguo1118.cn

TS:   arr.slice(1, 4);
来源：https://wd.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://nu.zhonguo6118.cn

Go:   arr[1:4]
来源：https://ib.zhonguo3118.cn

Ruby: arr[1, 3]
来源：https://qn.zhonguo8118.cn

C#:   list.GetRange(1, 3);
来源：https://ta.zhonguo5118.cn

[D08] 合并两个数组
来源：https://ua.zhonguo1118.cn

Py:   a + b;  a.extend(b)
来源：https://rj.zhonguo3118.cn

PHP:  array_merge($a, $b);
来源：https://om.zhonguo7118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://me.zhonguo6118.cn

TS:   [...a, ...b];
来源：https://mc.zhonguo1118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://tr.zhonguo2118.cn

Go:   append(a, b...)
来源：https://gc.zhonguo3118.cn

Ruby: a + b;  a.concat(b)
来源：https://mo.zhonguo1118.cn

C#:   a.Concat(b).ToList()
来源：https://ai.zhonguo6118.cn

[D09] 排序（升序）
来源：https://df.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://mn.zhonguo6118.cn

PHP:  sort($arr);
来源：https://hy.zhonguo7118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://vw.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://rm.zhonguo7118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://kj.zhonguo3118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://nd.zhonguo5118.cn

Ruby: arr.sort
来源：https://tv.zhonguo3118.cn

C#:   list.Sort();
来源：https://io.zhonguo7118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://mj.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://lb.zhonguo5118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://gi.zhonguo8118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://ii.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://nl.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://lm.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://gd.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://zx.zhonguo8118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://mu.zhonguo6118.cn

[D11] 反转数组
来源：https://zk.zhonguo7118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://fr.zhonguo8118.cn

PHP:  array_reverse($arr);
来源：https://mt.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://fk.zhonguo3118.cn

TS:   [...arr].reverse();
来源：https://un.zhonguo8118.cn

Java: Collections.reverse(list);
来源：https://lu.zhonguo7118.cn

Go:   slices.Reverse(arr)
来源：https://zi.zhonguo4118.cn

Ruby: arr.reverse
来源：https://dn.zhonguo7118.cn

C#:   list.Reverse();
来源：https://av.zhonguo5118.cn

[D12] 查找元素下标
来源：https://co.zhonguo8118.cn

Py:   arr.index(x);  x in arr
来源：https://is.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://dq.zhonguo4118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ss.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ri.zhonguo7118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://wx.zhonguo7118.cn

Go:   slices.Index(arr, x)
来源：https://gk.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://fz.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://ap.zhonguo4118.cn

[D13] 过滤（保留满足条件的）
来源：https://cp.zhonguo2118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://hm.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://up.zhonguo6118.cn

JS:   arr.filter(x => x > 3)
来源：https://mi.zhonguo7118.cn

TS:   arr.filter(x => x > 3)
来源：https://go.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://fj.zhonguo1118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://qb.zhonguo3118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fc.zhonguo3118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ai.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://ws.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://dd.zhonguo7118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://oe.zhonguo2118.cn

JS:   arr.map(x => x * 2)
来源：https://gm.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://wh.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://qp.zhonguo5118.cn

Go:   // 手写循环
来源：https://gl.zhonguo3118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vi.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://iu.zhonguo5118.cn

[D15] 去重
来源：https://zw.zhonguo6118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://zn.zhonguo6118.cn

PHP:  array_unique($arr);
来源：https://vs.zhonguo7118.cn

JS:   [...new Set(arr)]
来源：https://iq.zhonguo6118.cn

TS:   [...new Set(arr)]
来源：https://le.zhonguo3118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://gs.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://wb.zhonguo5118.cn

Ruby: arr.uniq
来源：https://vv.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://wm.zhonguo6118.cn

[D16] 求和与平均值
来源：https://rt.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://vf.zhonguo5118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://rn.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://ja.zhonguo2118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://gh.zhonguo7118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://st.zhonguo4118.cn

Go:   // 手写循环累加
来源：https://pv.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://zw.zhonguo2118.cn

C#:   list.Sum();  list.Average()
来源：https://uy.zhonguo3118.cn

[D17] 最大值与最小值
来源：https://te.zhonguo4118.cn

Py:   max(arr);  min(arr)
来源：https://ad.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://gu.zhonguo2118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://kl.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://bh.zhonguo4118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://vd.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://qk.zhonguo3118.cn

Ruby: arr.max;  arr.min
来源：https://tq.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://nq.zhonguo4118.cn

[D18] 扁平化嵌套数组
来源：https://fu.zhonguo6118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://qy.zhonguo6118.cn

PHP:  array_merge(...$nested);
来源：https://sx.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://jb.zhonguo4118.cn

TS:   nested.flat();
来源：https://di.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://jl.zhonguo1118.cn

Go:   // 手写双层循环
来源：https://xz.zhonguo5118.cn

Ruby: nested.flatten
来源：https://jv.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://tb.zhonguo2118.cn

[D19] 按字段分组
来源：https://qy.zhonguo7118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://jo.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://eh.zhonguo4118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://hh.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://am.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://tu.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://cc.zhonguo8118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://yh.zhonguo7118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://us.zhonguo4118.cn

[D20] 统计每个元素出现次数
来源：https://pg.zhonguo1118.cn

Py:   Counter(arr)
来源：https://oc.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://mg.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://js.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://eo.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://mt.zhonguo5118.cn

Go:   // 手写 map[T]int
来源：https://gv.zhonguo2118.cn

Ruby: arr.tally
来源：https://ro.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://fl.zhonguo8118.cn

[D21] 判断是否包含某元素
来源：https://vz.zhonguo2118.cn

Py:   x in arr
来源：https://vf.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://nn.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://lb.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://hh.zhonguo8118.cn

Java: list.contains(x)
来源：https://ba.zhonguo6118.cn

Go:   slices.Contains(arr, x)
来源：https://cz.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://ah.zhonguo3118.cn

C#:   list.Contains(x)
来源：https://lc.zhonguo7118.cn

[D22] 复制数组（避免共享引用）
来源：https://rl.zhonguo1118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ln.zhonguo6118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://zg.zhonguo2118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://bo.zhonguo1118.cn

TS:   [...arr];
来源：https://ca.zhonguo4118.cn

Java: new ArrayList<>(list);
来源：https://hl.zhonguo3118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ns.zhonguo6118.cn

Ruby: arr.dup;  arr.clone
来源：https://kq.zhonguo8118.cn

C#:   new List<int>(list);
来源：https://aj.zhonguo7118.cn

[D23] reduce 累积计算
来源：https://kg.zhonguo7118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://yo.zhonguo8118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://uy.zhonguo7118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://vs.zhonguo4118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://bi.zhonguo8118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://lk.zhonguo2118.cn

Go:   // 手写循环
来源：https://rh.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://is.zhonguo5118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://xw.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://ta.zhonguo2118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://gg.zhonguo4118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://kd.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://pe.zhonguo1118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://ju.zhonguo4118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://jk.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://se.zhonguo1118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://zk.zhonguo2118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://vm.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://wf.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ci.zhonguo5118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ol.zhonguo8118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://iy.zhonguo2118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://qm.zhonguo5118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://el.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://vv.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://rn.zhonguo6118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://gh.zhonguo7118.cn

[D26] 数组转字符串
来源：https://fk.zhonguo7118.cn

Py:   ", ".join(map(str, arr))
来源：https://pg.zhonguo6118.cn

PHP:  implode(", ", $arr);
来源：https://nn.zhonguo8118.cn

JS:   arr.join(", ")
来源：https://io.zhonguo3118.cn

TS:   arr.join(", ")
来源：https://lb.zhonguo3118.cn

Java: String.join(", ", list)
来源：https://ht.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://om.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://ew.zhonguo7118.cn

C#:   string.Join(", ", list)
来源：https://fv.zhonguo7118.cn

================================================================================
来源：https://tb.zhonguo1118.cn

E. 字符串处理
来源：https://bx.zhonguo1118.cn

================================================================================
来源：https://oe.zhonguo4118.cn

[E01] 拼接字符串
来源：https://dy.zhonguo3118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://kb.zhonguo4118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://dh.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://jt.zhonguo2118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://xt.zhonguo1118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ob.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://uf.zhonguo5118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://db.zhonguo1118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://ao.zhonguo8118.cn

[E02] 重复字符串
来源：https://ie.zhonguo2118.cn

Py:   "ab" * 3
来源：https://jh.zhonguo8118.cn

PHP:  str_repeat("ab", 3);
来源：https://tu.zhonguo7118.cn

JS:   "ab".repeat(3)
来源：https://gk.zhonguo6118.cn

TS:   "ab".repeat(3)
来源：https://gz.zhonguo6118.cn

Java: "ab".repeat(3)
来源：https://tt.zhonguo4118.cn

Go:   strings.Repeat("ab", 3)
来源：https://px.zhonguo7118.cn

Ruby: "ab" * 3
来源：https://ve.zhonguo8118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://eo.zhonguo2118.cn

[E03] 截取子串
来源：https://xu.zhonguo4118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ox.zhonguo6118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://bt.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://cv.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://ac.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://qq.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://iw.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://tt.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://cr.zhonguo5118.cn

[E04] 查找子串位置
来源：https://jq.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://sa.zhonguo3118.cn

PHP:  strpos($s, "x");
来源：https://fq.zhonguo4118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://pj.zhonguo2118.cn

TS:   s.indexOf("x")
来源：https://xk.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://nr.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://ew.zhonguo4118.cn

Ruby: s.index("x")
来源：https://cg.zhonguo3118.cn

C#:   s.IndexOf("x")
来源：https://om.zhonguo4118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://wk.zhonguo7118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ri.zhonguo7118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://jw.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://xa.zhonguo7118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://hb.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://md.zhonguo7118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://uf.zhonguo4118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://re.zhonguo2118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://bt.zhonguo2118.cn

[E06] 替换子串
来源：https://ik.zhonguo6118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://in.zhonguo4118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ug.zhonguo3118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://wl.zhonguo2118.cn

TS:   s.replaceAll("a", "b")
来源：https://ek.zhonguo5118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://nw.zhonguo5118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ws.zhonguo7118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://ax.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://kk.zhonguo1118.cn

[E07] 按分隔符拆分
来源：https://am.zhonguo4118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://bo.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://ee.zhonguo2118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://me.zhonguo5118.cn

TS:   s.split(",")
来源：https://dv.zhonguo1118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://pn.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://oj.zhonguo3118.cn

Ruby: s.split(",");  s.split
来源：https://zv.zhonguo2118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://sq.zhonguo2118.cn

[E08] 数组按分隔符合并
来源：https://zv.zhonguo5118.cn

Py:   ",".join(items)
来源：https://yb.zhonguo3118.cn

PHP:  implode(",", $items);
来源：https://qn.zhonguo8118.cn

JS:   items.join(",")
来源：https://am.zhonguo2118.cn

TS:   items.join(",")
来源：https://bn.zhonguo7118.cn

Java: String.join(",", items)
来源：https://ae.zhonguo2118.cn

Go:   strings.Join(items, ",")
来源：https://ib.zhonguo1118.cn

Ruby: items.join(",")
来源：https://za.zhonguo3118.cn

C#:   string.Join(",", items)
来源：https://tf.zhonguo1118.cn

[E09] 去除所有空白字符
来源：https://dp.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://om.zhonguo3118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://aa.zhonguo3118.cn

JS:   s.replace(/\s+/g, "")
来源：https://af.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://zt.zhonguo2118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ng.zhonguo1118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://ww.zhonguo8118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://xe.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://xg.zhonguo2118.cn

[E10] 左侧补零 / 定长填充
来源：https://im.zhonguo7118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ma.zhonguo7118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ot.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://tl.zhonguo1118.cn

TS:   "7".padStart(3, "0")
来源：https://on.zhonguo5118.cn

Java: String.format("%03d", 7)
来源：https://wv.zhonguo3118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://im.zhonguo3118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://im.zhonguo6118.cn


<!-- 参考信息 -->