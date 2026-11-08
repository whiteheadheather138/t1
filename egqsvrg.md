代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：https://oj.zhonguo4118.cn

Java: list.add(0, 0);
来源：https://fn.zhonguo7118.cn

Go:   arr = append([]int{0}, arr...)
来源：https://qb.zhonguo5118.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：https://td.zhonguo2118.cn

C#:   list.Insert(0, 0);
来源：https://sb.zhonguo1118.cn

[D04] 删除元素
来源：https://mq.zhonguo1118.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：https://zd.zhonguo4118.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：https://xx.zhonguo6118.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：https://gx.zhonguo3118.cn

TS:   arr.splice(0, 1);
来源：https://qc.zhonguo3118.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：https://pq.zhonguo2118.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：https://gm.zhonguo1118.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：https://aw.zhonguo4118.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：https://rf.zhonguo8118.cn

[D05] 访问与修改元素
来源：https://dj.zhonguo1118.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：https://ys.zhonguo2118.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：https://mx.zhonguo7118.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：https://jl.zhonguo1118.cn

TS:   arr[0]; arr.at(-1);
来源：https://fz.zhonguo5118.cn

Java: list.get(0); list.set(0, 9);
来源：https://vm.zhonguo5118.cn

Go:   arr[0]; arr[0] = 9
来源：https://ae.zhonguo1118.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：https://ax.zhonguo4118.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：https://ep.zhonguo6118.cn

[D06] 数组长度
来源：https://uv.zhonguo2118.cn

Py:   len(arr)
来源：https://lm.zhonguo5118.cn

PHP:  count($arr);
来源：https://uo.zhonguo2118.cn

JS:   arr.length
来源：https://vb.zhonguo5118.cn

TS:   arr.length
来源：https://ca.zhonguo4118.cn

Java: list.size();
来源：https://jd.zhonguo5118.cn

Go:   len(arr)
来源：https://ky.zhonguo3118.cn

Ruby: arr.length; arr.size
来源：https://fa.zhonguo1118.cn

C#:   list.Count;
来源：https://xs.zhonguo8118.cn

[D07] 切片 / 取子数组
来源：https://bn.zhonguo2118.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：https://cn.zhonguo3118.cn

PHP:  array_slice($arr, 1, 3);
来源：https://bk.zhonguo6118.cn

JS:   arr.slice(1, 4);
来源：https://yi.zhonguo1118.cn

TS:   arr.slice(1, 4);
来源：https://em.zhonguo8118.cn

Java: list.subList(1, 4);
来源：https://yw.zhonguo3118.cn

Go:   arr[1:4]
来源：https://gz.zhonguo8118.cn

Ruby: arr[1, 3]
来源：https://hg.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://sq.zhonguo1118.cn

[D08] 合并两个数组
来源：https://zu.zhonguo7118.cn

Py:   a + b;  a.extend(b)
来源：https://xz.zhonguo2118.cn

PHP:  array_merge($a, $b);
来源：https://ad.zhonguo3118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://cf.zhonguo1118.cn

TS:   [...a, ...b];
来源：https://ql.zhonguo1118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://ta.zhonguo4118.cn

Go:   append(a, b...)
来源：https://os.zhonguo1118.cn

Ruby: a + b;  a.concat(b)
来源：https://vl.zhonguo8118.cn

C#:   a.Concat(b).ToList()
来源：https://lo.zhonguo3118.cn

[D09] 排序（升序）
来源：https://iy.zhonguo1118.cn

Py:   sorted(arr);  arr.sort()
来源：https://rd.zhonguo7118.cn

PHP:  sort($arr);
来源：https://og.zhonguo6118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://ad.zhonguo3118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://sw.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://hk.zhonguo7118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://op.zhonguo6118.cn

Ruby: arr.sort
来源：https://wo.zhonguo8118.cn

C#:   list.Sort();
来源：https://px.zhonguo7118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://rg.zhonguo1118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://iq.zhonguo8118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://kd.zhonguo3118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://uo.zhonguo2118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://zc.zhonguo1118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://sf.zhonguo8118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://is.zhonguo4118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://aa.zhonguo7118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://qe.zhonguo5118.cn

[D11] 反转数组
来源：https://fv.zhonguo6118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://vb.zhonguo8118.cn

PHP:  array_reverse($arr);
来源：https://jx.zhonguo6118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://lm.zhonguo4118.cn

TS:   [...arr].reverse();
来源：https://or.zhonguo1118.cn

Java: Collections.reverse(list);
来源：https://iw.zhonguo4118.cn

Go:   slices.Reverse(arr)
来源：https://ib.zhonguo3118.cn

Ruby: arr.reverse
来源：https://zg.zhonguo4118.cn

C#:   list.Reverse();
来源：https://rf.zhonguo3118.cn

[D12] 查找元素下标
来源：https://nr.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://wg.zhonguo5118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://ld.zhonguo2118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://dp.zhonguo8118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://xj.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://is.zhonguo2118.cn

Go:   slices.Index(arr, x)
来源：https://rw.zhonguo4118.cn

Ruby: arr.index(x)
来源：https://hx.zhonguo4118.cn

C#:   list.IndexOf(x);
来源：https://al.zhonguo7118.cn

[D13] 过滤（保留满足条件的）
来源：https://vh.zhonguo1118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://qv.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://dp.zhonguo3118.cn

JS:   arr.filter(x => x > 3)
来源：https://gs.zhonguo8118.cn

TS:   arr.filter(x => x > 3)
来源：https://hl.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://aa.zhonguo8118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://jt.zhonguo6118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fh.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ba.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://wf.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://mg.zhonguo3118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://lb.zhonguo8118.cn

JS:   arr.map(x => x * 2)
来源：https://fj.zhonguo2118.cn

TS:   arr.map(x => x * 2)
来源：https://jz.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ya.zhonguo1118.cn

Go:   // 手写循环
来源：https://fs.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://lp.zhonguo1118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://fr.zhonguo3118.cn

[D15] 去重
来源：https://wb.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://hb.zhonguo2118.cn

PHP:  array_unique($arr);
来源：https://zv.zhonguo3118.cn

JS:   [...new Set(arr)]
来源：https://wi.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://yu.zhonguo6118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://np.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://pz.zhonguo4118.cn

Ruby: arr.uniq
来源：https://kj.zhonguo5118.cn

C#:   list.Distinct().ToList()
来源：https://ik.zhonguo2118.cn

[D16] 求和与平均值
来源：https://fk.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://es.zhonguo3118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://co.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://fq.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://ok.zhonguo5118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://xj.zhonguo7118.cn

Go:   // 手写循环累加
来源：https://tg.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ry.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://yl.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://wj.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://vz.zhonguo7118.cn

PHP:  max($arr);  min($arr);
来源：https://ax.zhonguo2118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://dc.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://kc.zhonguo3118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://np.zhonguo5118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://jq.zhonguo2118.cn

Ruby: arr.max;  arr.min
来源：https://ql.zhonguo7118.cn

C#:   list.Max();  list.Min()
来源：https://ej.zhonguo6118.cn

[D18] 扁平化嵌套数组
来源：https://ap.zhonguo7118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://tr.zhonguo2118.cn

PHP:  array_merge(...$nested);
来源：https://rr.zhonguo3118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://kv.zhonguo2118.cn

TS:   nested.flat();
来源：https://bc.zhonguo2118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://vl.zhonguo7118.cn

Go:   // 手写双层循环
来源：https://pp.zhonguo5118.cn

Ruby: nested.flatten
来源：https://tm.zhonguo2118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://si.zhonguo7118.cn

[D19] 按字段分组
来源：https://ae.zhonguo3118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ew.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://bd.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://pc.zhonguo1118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://gj.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://lr.zhonguo3118.cn

Go:   // 手写 map[string][]T
来源：https://pg.zhonguo1118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://fu.zhonguo8118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://nn.zhonguo8118.cn

[D20] 统计每个元素出现次数
来源：https://ni.zhonguo5118.cn

Py:   Counter(arr)
来源：https://eo.zhonguo5118.cn

PHP:  array_count_values($arr);
来源：https://nw.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://qx.zhonguo8118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ou.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://pa.zhonguo1118.cn

Go:   // 手写 map[T]int
来源：https://jx.zhonguo5118.cn

Ruby: arr.tally
来源：https://oi.zhonguo1118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://mx.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://zo.zhonguo4118.cn

Py:   x in arr
来源：https://mc.zhonguo3118.cn

PHP:  in_array($x, $arr, true);
来源：https://gw.zhonguo1118.cn

JS:   arr.includes(x)
来源：https://ud.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://td.zhonguo5118.cn

Java: list.contains(x)
来源：https://oa.zhonguo1118.cn

Go:   slices.Contains(arr, x)
来源：https://ht.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://gw.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://ka.zhonguo2118.cn

[D22] 复制数组（避免共享引用）
来源：https://fe.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://db.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://yk.zhonguo1118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://ez.zhonguo1118.cn

TS:   [...arr];
来源：https://ey.zhonguo7118.cn

Java: new ArrayList<>(list);
来源：https://ks.zhonguo3118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://up.zhonguo6118.cn

Ruby: arr.dup;  arr.clone
来源：https://ib.zhonguo5118.cn

C#:   new List<int>(list);
来源：https://uf.zhonguo3118.cn

[D23] reduce 累积计算
来源：https://yv.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ln.zhonguo6118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://ks.zhonguo6118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://xi.zhonguo2118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://nb.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://sg.zhonguo3118.cn

Go:   // 手写循环
来源：https://gi.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://qj.zhonguo4118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://ud.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://am.zhonguo3118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ue.zhonguo1118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://hl.zhonguo3118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://zi.zhonguo1118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://yr.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://us.zhonguo7118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://wr.zhonguo4118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://tz.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ne.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://jn.zhonguo4118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://pg.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ax.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://nj.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://zc.zhonguo7118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://ck.zhonguo5118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://xf.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://lf.zhonguo8118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ux.zhonguo3118.cn

[D26] 数组转字符串
来源：https://oh.zhonguo5118.cn

Py:   ", ".join(map(str, arr))
来源：https://qp.zhonguo1118.cn

PHP:  implode(", ", $arr);
来源：https://rw.zhonguo8118.cn

JS:   arr.join(", ")
来源：https://vo.zhonguo2118.cn

TS:   arr.join(", ")
来源：https://yp.zhonguo8118.cn

Java: String.join(", ", list)
来源：https://xw.zhonguo6118.cn

Go:   strings.Join(strs, ", ")
来源：https://bb.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://ow.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://vw.zhonguo7118.cn

================================================================================
来源：https://tn.zhonguo6118.cn

E. 字符串处理
来源：https://uo.zhonguo2118.cn

================================================================================
来源：https://tu.zhonguo3118.cn

[E01] 拼接字符串
来源：https://ab.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://up.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://zb.zhonguo5118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://yj.zhonguo5118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://sr.zhonguo5118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ac.zhonguo5118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://fg.zhonguo1118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://ap.zhonguo8118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://jx.zhonguo5118.cn

[E02] 重复字符串
来源：https://lx.zhonguo8118.cn

Py:   "ab" * 3
来源：https://gv.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://kg.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://fr.zhonguo7118.cn

TS:   "ab".repeat(3)
来源：https://ec.zhonguo7118.cn

Java: "ab".repeat(3)
来源：https://nh.zhonguo5118.cn

Go:   strings.Repeat("ab", 3)
来源：https://tc.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://iu.zhonguo1118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://oy.zhonguo1118.cn

[E03] 截取子串
来源：https://yx.zhonguo7118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://bm.zhonguo8118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://xs.zhonguo2118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://jq.zhonguo1118.cn

TS:   s.slice(1, 4)
来源：https://vr.zhonguo1118.cn

Java: s.substring(1, 4)
来源：https://eg.zhonguo8118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://hc.zhonguo7118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://qq.zhonguo7118.cn

C#:   s.Substring(1, 3)
来源：https://gs.zhonguo7118.cn

[E04] 查找子串位置
来源：https://hn.zhonguo4118.cn

Py:   s.find("x");  s.index("x")
来源：https://et.zhonguo3118.cn

PHP:  strpos($s, "x");
来源：https://vm.zhonguo7118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://da.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://md.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://ng.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://yz.zhonguo8118.cn

Ruby: s.index("x")
来源：https://nn.zhonguo3118.cn

C#:   s.IndexOf("x")
来源：https://ub.zhonguo5118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://bn.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://fd.zhonguo2118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://hw.zhonguo1118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://tl.zhonguo5118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://bh.zhonguo8118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://tb.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://az.zhonguo2118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://wu.zhonguo8118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://no.zhonguo4118.cn

[E06] 替换子串
来源：https://ly.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://xp.zhonguo2118.cn

PHP:  str_replace("a", "b", $s);
来源：https://qe.zhonguo2118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://dx.zhonguo8118.cn

TS:   s.replaceAll("a", "b")
来源：https://uk.zhonguo6118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://rt.zhonguo5118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://tm.zhonguo4118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://zs.zhonguo3118.cn

C#:   s.Replace("a", "b")
来源：https://an.zhonguo5118.cn

[E07] 按分隔符拆分
来源：https://za.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://fk.zhonguo4118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://za.zhonguo2118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://nz.zhonguo8118.cn

TS:   s.split(",")
来源：https://ur.zhonguo2118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://cl.zhonguo8118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://wi.zhonguo1118.cn

Ruby: s.split(",");  s.split
来源：https://js.zhonguo7118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://rc.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://jw.zhonguo2118.cn

Py:   ",".join(items)
来源：https://pe.zhonguo5118.cn

PHP:  implode(",", $items);
来源：https://ny.zhonguo3118.cn

JS:   items.join(",")
来源：https://vj.zhonguo7118.cn

TS:   items.join(",")
来源：https://kb.zhonguo4118.cn

Java: String.join(",", items)
来源：https://or.zhonguo2118.cn

Go:   strings.Join(items, ",")
来源：https://ce.zhonguo5118.cn

Ruby: items.join(",")
来源：https://ix.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://xd.zhonguo2118.cn

[E09] 去除所有空白字符
来源：https://tv.zhonguo8118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://eo.zhonguo2118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://sr.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://hy.zhonguo5118.cn

TS:   s.replace(/\s+/g, "")
来源：https://bw.zhonguo8118.cn

Java: s.replaceAll("\\s+", "")
来源：https://iw.zhonguo5118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://cb.zhonguo5118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://kj.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://zh.zhonguo3118.cn

[E10] 左侧补零 / 定长填充
来源：https://gl.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://dx.zhonguo1118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://pl.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://co.zhonguo3118.cn


<!-- 参考信息 -->