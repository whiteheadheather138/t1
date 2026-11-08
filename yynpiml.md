代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：https://st.zhonguo6118.cn

Java: list.add(0, 0);
来源：https://jf.zhonguo2118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://mg.zhonguo6118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://og.zhonguo8118.cn

C#:   list.Insert(0, 0);
来源：https://js.zhonguo4118.cn

[D04] 删除元素
来源：https://vz.zhonguo2118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://un.zhonguo3118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://qg.zhonguo5118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://sk.zhonguo2118.cn

TS:   arr.splice(0, 1);
来源：https://vm.zhonguo5118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://dc.zhonguo7118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://vd.zhonguo3118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://sj.zhonguo5118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://hp.zhonguo7118.cn

[D05] 访问与修改元素
来源：https://jw.zhonguo5118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://dr.zhonguo6118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://tb.zhonguo6118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://bp.zhonguo7118.cn

TS:   arr[0]; arr.at(-1);
来源：https://oy.zhonguo7118.cn

Java: list.get(0); list.set(0, 9);
来源：https://rh.zhonguo4118.cn

Go:   arr[0]; arr[0] = 9
来源：https://yb.zhonguo3118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://mj.zhonguo5118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://cf.zhonguo7118.cn

[D06] 数组长度
来源：https://fg.zhonguo8118.cn

Py:   len(arr)
来源：https://pn.zhonguo2118.cn

PHP:  count($arr);
来源：https://fz.zhonguo3118.cn

JS:   arr.length
来源：https://gv.zhonguo5118.cn

TS:   arr.length
来源：https://ij.zhonguo5118.cn

Java: list.size();
来源：https://vy.zhonguo5118.cn

Go:   len(arr)
来源：https://ga.zhonguo6118.cn

Ruby: arr.length; arr.size
来源：https://zm.zhonguo6118.cn

C#:   list.Count;
来源：https://ro.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://vh.zhonguo8118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://wc.zhonguo8118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://ks.zhonguo2118.cn

JS:   arr.slice(1, 4);
来源：https://es.zhonguo6118.cn

TS:   arr.slice(1, 4);
来源：https://wy.zhonguo3118.cn

Java: list.subList(1, 4);
来源：https://pq.zhonguo7118.cn

Go:   arr[1:4]
来源：https://jt.zhonguo6118.cn

Ruby: arr[1, 3]
来源：https://vk.zhonguo2118.cn

C#:   list.GetRange(1, 3);
来源：https://kv.zhonguo7118.cn

[D08] 合并两个数组
来源：https://ea.zhonguo7118.cn

Py:   a + b;  a.extend(b)
来源：https://ej.zhonguo8118.cn

PHP:  array_merge($a, $b);
来源：https://wl.zhonguo8118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ix.zhonguo6118.cn

TS:   [...a, ...b];
来源：https://fy.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://sl.zhonguo2118.cn

Go:   append(a, b...)
来源：https://iv.zhonguo2118.cn

Ruby: a + b;  a.concat(b)
来源：https://dc.zhonguo2118.cn

C#:   a.Concat(b).ToList()
来源：https://ta.zhonguo5118.cn

[D09] 排序（升序）
来源：https://pz.zhonguo5118.cn

Py:   sorted(arr);  arr.sort()
来源：https://rv.zhonguo2118.cn

PHP:  sort($arr);
来源：https://nk.zhonguo3118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://qz.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://nf.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://wg.zhonguo5118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://xl.zhonguo4118.cn

Ruby: arr.sort
来源：https://lh.zhonguo4118.cn

C#:   list.Sort();
来源：https://ku.zhonguo3118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://fv.zhonguo6118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://yg.zhonguo6118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://vk.zhonguo8118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://aq.zhonguo5118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://nl.zhonguo4118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://kp.zhonguo3118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://nf.zhonguo1118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://oc.zhonguo1118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://qe.zhonguo5118.cn

[D11] 反转数组
来源：https://tf.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://bh.zhonguo2118.cn

PHP:  array_reverse($arr);
来源：https://pd.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://ft.zhonguo1118.cn

TS:   [...arr].reverse();
来源：https://kr.zhonguo4118.cn

Java: Collections.reverse(list);
来源：https://yp.zhonguo6118.cn

Go:   slices.Reverse(arr)
来源：https://sk.zhonguo4118.cn

Ruby: arr.reverse
来源：https://ki.zhonguo5118.cn

C#:   list.Reverse();
来源：https://yh.zhonguo7118.cn

[D12] 查找元素下标
来源：https://be.zhonguo4118.cn

Py:   arr.index(x);  x in arr
来源：https://ad.zhonguo3118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://km.zhonguo7118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://zn.zhonguo1118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jx.zhonguo6118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://nb.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://da.zhonguo1118.cn

Ruby: arr.index(x)
来源：https://sd.zhonguo5118.cn

C#:   list.IndexOf(x);
来源：https://zt.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://uk.zhonguo5118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://zd.zhonguo3118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://fj.zhonguo5118.cn

JS:   arr.filter(x => x > 3)
来源：https://vk.zhonguo7118.cn

TS:   arr.filter(x => x > 3)
来源：https://xc.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://id.zhonguo8118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://fz.zhonguo8118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fq.zhonguo5118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://gt.zhonguo4118.cn

[D14] 映射转换（每个元素变形）
来源：https://zn.zhonguo4118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://uv.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://cr.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://ai.zhonguo6118.cn

TS:   arr.map(x => x * 2)
来源：https://yf.zhonguo2118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://xl.zhonguo1118.cn

Go:   // 手写循环
来源：https://vn.zhonguo3118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://tv.zhonguo5118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://qr.zhonguo2118.cn

[D15] 去重
来源：https://fe.zhonguo4118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://mx.zhonguo2118.cn

PHP:  array_unique($arr);
来源：https://vq.zhonguo3118.cn

JS:   [...new Set(arr)]
来源：https://zh.zhonguo1118.cn

TS:   [...new Set(arr)]
来源：https://tu.zhonguo2118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ht.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://id.zhonguo2118.cn

Ruby: arr.uniq
来源：https://bu.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://qm.zhonguo6118.cn

[D16] 求和与平均值
来源：https://ej.zhonguo3118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://od.zhonguo7118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://gc.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://te.zhonguo8118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://bs.zhonguo6118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://vh.zhonguo1118.cn

Go:   // 手写循环累加
来源：https://df.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://tq.zhonguo1118.cn

C#:   list.Sum();  list.Average()
来源：https://pf.zhonguo6118.cn

[D17] 最大值与最小值
来源：https://ue.zhonguo1118.cn

Py:   max(arr);  min(arr)
来源：https://hg.zhonguo7118.cn

PHP:  max($arr);  min($arr);
来源：https://su.zhonguo3118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://us.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://ow.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://pn.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://dd.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://bn.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://kb.zhonguo7118.cn

[D18] 扁平化嵌套数组
来源：https://ix.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://zs.zhonguo8118.cn

PHP:  array_merge(...$nested);
来源：https://lp.zhonguo3118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://fs.zhonguo4118.cn

TS:   nested.flat();
来源：https://sq.zhonguo7118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://vr.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://ux.zhonguo6118.cn

Ruby: nested.flatten
来源：https://km.zhonguo8118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://vl.zhonguo4118.cn

[D19] 按字段分组
来源：https://ot.zhonguo7118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://sl.zhonguo3118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://hf.zhonguo5118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://sy.zhonguo5118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://xa.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ap.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://qc.zhonguo2118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://so.zhonguo3118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://yy.zhonguo8118.cn

[D20] 统计每个元素出现次数
来源：https://tk.zhonguo8118.cn

Py:   Counter(arr)
来源：https://et.zhonguo6118.cn

PHP:  array_count_values($arr);
来源：https://ck.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://go.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ul.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://so.zhonguo2118.cn

Go:   // 手写 map[T]int
来源：https://ni.zhonguo7118.cn

Ruby: arr.tally
来源：https://zu.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://uh.zhonguo2118.cn

[D21] 判断是否包含某元素
来源：https://cz.zhonguo5118.cn

Py:   x in arr
来源：https://kc.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://md.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://su.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://dk.zhonguo7118.cn

Java: list.contains(x)
来源：https://ph.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://ge.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://db.zhonguo6118.cn

C#:   list.Contains(x)
来源：https://np.zhonguo5118.cn

[D22] 复制数组（避免共享引用）
来源：https://tm.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://qw.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://ng.zhonguo6118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://by.zhonguo7118.cn

TS:   [...arr];
来源：https://if.zhonguo2118.cn

Java: new ArrayList<>(list);
来源：https://vu.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://dt.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://yq.zhonguo7118.cn

C#:   new List<int>(list);
来源：https://mw.zhonguo2118.cn

[D23] reduce 累积计算
来源：https://bk.zhonguo7118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://pc.zhonguo7118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://br.zhonguo5118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://vu.zhonguo7118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://zt.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://su.zhonguo1118.cn

Go:   // 手写循环
来源：https://xw.zhonguo8118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://yy.zhonguo5118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://fg.zhonguo4118.cn

[D24] 字典 / Map 基本操作
来源：https://pz.zhonguo1118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://sz.zhonguo2118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://yj.zhonguo5118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://hx.zhonguo8118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://ly.zhonguo2118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://zp.zhonguo8118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://qh.zhonguo8118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://wn.zhonguo1118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://kp.zhonguo1118.cn

[D25] Set 集合去重与交并差
来源：https://qc.zhonguo1118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://mh.zhonguo1118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://cp.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://bt.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://kk.zhonguo8118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://dv.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://ed.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://tw.zhonguo1118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ln.zhonguo1118.cn

[D26] 数组转字符串
来源：https://xe.zhonguo3118.cn

Py:   ", ".join(map(str, arr))
来源：https://pv.zhonguo4118.cn

PHP:  implode(", ", $arr);
来源：https://jj.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://zk.zhonguo2118.cn

TS:   arr.join(", ")
来源：https://qu.zhonguo6118.cn

Java: String.join(", ", list)
来源：https://oq.zhonguo1118.cn

Go:   strings.Join(strs, ", ")
来源：https://vv.zhonguo4118.cn

Ruby: arr.join(", ")
来源：https://qq.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://dh.zhonguo4118.cn

================================================================================
来源：https://ev.zhonguo6118.cn

E. 字符串处理
来源：https://zf.zhonguo1118.cn

================================================================================
来源：https://fz.zhonguo6118.cn

[E01] 拼接字符串
来源：https://au.zhonguo7118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://xf.zhonguo1118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://hw.zhonguo6118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://am.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://fa.zhonguo5118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://qk.zhonguo7118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://he.zhonguo8118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://hf.zhonguo5118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://iw.zhonguo2118.cn

[E02] 重复字符串
来源：https://ta.zhonguo7118.cn

Py:   "ab" * 3
来源：https://yh.zhonguo6118.cn

PHP:  str_repeat("ab", 3);
来源：https://mx.zhonguo1118.cn

JS:   "ab".repeat(3)
来源：https://bh.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://uo.zhonguo8118.cn

Java: "ab".repeat(3)
来源：https://cr.zhonguo3118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ep.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://ag.zhonguo5118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://xd.zhonguo6118.cn

[E03] 截取子串
来源：https://vi.zhonguo2118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://xe.zhonguo4118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://qs.zhonguo1118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://yb.zhonguo5118.cn

TS:   s.slice(1, 4)
来源：https://lj.zhonguo3118.cn

Java: s.substring(1, 4)
来源：https://qy.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://jf.zhonguo1118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://uq.zhonguo1118.cn

C#:   s.Substring(1, 3)
来源：https://kr.zhonguo5118.cn

[E04] 查找子串位置
来源：https://kk.zhonguo3118.cn

Py:   s.find("x");  s.index("x")
来源：https://jq.zhonguo1118.cn

PHP:  strpos($s, "x");
来源：https://qe.zhonguo7118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://af.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://ks.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://lo.zhonguo5118.cn

Go:   strings.Index(s, "x")
来源：https://jv.zhonguo4118.cn

Ruby: s.index("x")
来源：https://ah.zhonguo4118.cn

C#:   s.IndexOf("x")
来源：https://sv.zhonguo5118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://ew.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://bp.zhonguo4118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://bt.zhonguo5118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://hq.zhonguo7118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://re.zhonguo5118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://sz.zhonguo2118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://tx.zhonguo5118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://of.zhonguo3118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://qn.zhonguo6118.cn

[E06] 替换子串
来源：https://qj.zhonguo1118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://qu.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://sq.zhonguo1118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ls.zhonguo1118.cn

TS:   s.replaceAll("a", "b")
来源：https://vh.zhonguo7118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ir.zhonguo3118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://di.zhonguo8118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://ra.zhonguo3118.cn

C#:   s.Replace("a", "b")
来源：https://zd.zhonguo2118.cn

[E07] 按分隔符拆分
来源：https://ic.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://hx.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://kp.zhonguo5118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://vl.zhonguo8118.cn

TS:   s.split(",")
来源：https://ed.zhonguo1118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://sx.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://so.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://bj.zhonguo1118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://ck.zhonguo4118.cn

[E08] 数组按分隔符合并
来源：https://ev.zhonguo6118.cn

Py:   ",".join(items)
来源：https://ds.zhonguo7118.cn

PHP:  implode(",", $items);
来源：https://ua.zhonguo3118.cn

JS:   items.join(",")
来源：https://fr.zhonguo6118.cn

TS:   items.join(",")
来源：https://ce.zhonguo2118.cn

Java: String.join(",", items)
来源：https://wg.zhonguo4118.cn

Go:   strings.Join(items, ",")
来源：https://db.zhonguo6118.cn

Ruby: items.join(",")
来源：https://gi.zhonguo8118.cn

C#:   string.Join(",", items)
来源：https://ql.zhonguo5118.cn

[E09] 去除所有空白字符
来源：https://eb.zhonguo2118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://md.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://pa.zhonguo3118.cn

JS:   s.replace(/\s+/g, "")
来源：https://le.zhonguo7118.cn

TS:   s.replace(/\s+/g, "")
来源：https://vn.zhonguo2118.cn

Java: s.replaceAll("\\s+", "")
来源：https://hq.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://we.zhonguo1118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://ed.zhonguo7118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://xn.zhonguo8118.cn

[E10] 左侧补零 / 定长填充
来源：https://at.zhonguo5118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://px.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://fc.zhonguo7118.cn

JS:   "7".padStart(3, "0")
来源：https://si.zhonguo1118.cn


<!-- 参考信息 -->