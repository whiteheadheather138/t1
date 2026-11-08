代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：https://ln.zhonguo2118.cn

TS:   [...a, ...b];
来源：https://rd.zhonguo4118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://or.zhonguo1118.cn

Go:   append(a, b...)
来源：https://tm.zhonguo8118.cn

Ruby: a + b;  a.concat(b)
来源：https://uk.zhonguo3118.cn

C#:   a.Concat(b).ToList()
来源：https://nc.zhonguo6118.cn

[D09] 排序（升序）
来源：https://dx.zhonguo2118.cn

Py:   sorted(arr);  arr.sort()
来源：https://gu.zhonguo1118.cn

PHP:  sort($arr);
来源：https://as.zhonguo2118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://nf.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://qm.zhonguo3118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://pg.zhonguo4118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://dq.zhonguo1118.cn

Ruby: arr.sort
来源：https://oc.zhonguo4118.cn

C#:   list.Sort();
来源：https://qb.zhonguo3118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://th.zhonguo2118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://bu.zhonguo7118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://lo.zhonguo5118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://zp.zhonguo4118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://ht.zhonguo3118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://lr.zhonguo5118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://vi.zhonguo6118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://ti.zhonguo6118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://na.zhonguo3118.cn

[D11] 反转数组
来源：https://zf.zhonguo3118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://lb.zhonguo3118.cn

PHP:  array_reverse($arr);
来源：https://md.zhonguo8118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://ma.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://lv.zhonguo8118.cn

Java: Collections.reverse(list);
来源：https://ct.zhonguo5118.cn

Go:   slices.Reverse(arr)
来源：https://yd.zhonguo1118.cn

Ruby: arr.reverse
来源：https://va.zhonguo6118.cn

C#:   list.Reverse();
来源：https://ql.zhonguo3118.cn

[D12] 查找元素下标
来源：https://jj.zhonguo8118.cn

Py:   arr.index(x);  x in arr
来源：https://jc.zhonguo5118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://rw.zhonguo8118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://ii.zhonguo2118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://xk.zhonguo5118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://vj.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://lb.zhonguo6118.cn

Ruby: arr.index(x)
来源：https://qx.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://qm.zhonguo5118.cn

[D13] 过滤（保留满足条件的）
来源：https://ud.zhonguo3118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://rl.zhonguo6118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://ym.zhonguo7118.cn

JS:   arr.filter(x => x > 3)
来源：https://vw.zhonguo3118.cn

TS:   arr.filter(x => x > 3)
来源：https://pn.zhonguo4118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://fz.zhonguo6118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://er.zhonguo4118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fw.zhonguo1118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ly.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://cb.zhonguo8118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://pv.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://fe.zhonguo3118.cn

JS:   arr.map(x => x * 2)
来源：https://qw.zhonguo2118.cn

TS:   arr.map(x => x * 2)
来源：https://zk.zhonguo4118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://jq.zhonguo2118.cn

Go:   // 手写循环
来源：https://to.zhonguo8118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://kq.zhonguo7118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://ep.zhonguo1118.cn

[D15] 去重
来源：https://rh.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://kk.zhonguo8118.cn

PHP:  array_unique($arr);
来源：https://cn.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://er.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://cd.zhonguo4118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://nl.zhonguo1118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://cl.zhonguo3118.cn

Ruby: arr.uniq
来源：https://jz.zhonguo4118.cn

C#:   list.Distinct().ToList()
来源：https://ka.zhonguo8118.cn

[D16] 求和与平均值
来源：https://jb.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://kg.zhonguo2118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://zs.zhonguo8118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://tt.zhonguo7118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://hx.zhonguo2118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://mc.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://mu.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://mo.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://ii.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://wn.zhonguo8118.cn

Py:   max(arr);  min(arr)
来源：https://js.zhonguo7118.cn

PHP:  max($arr);  min($arr);
来源：https://nf.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://ow.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://ml.zhonguo7118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://at.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://lr.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://ds.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://de.zhonguo1118.cn

[D18] 扁平化嵌套数组
来源：https://fd.zhonguo1118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://bt.zhonguo7118.cn

PHP:  array_merge(...$nested);
来源：https://fx.zhonguo5118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://jj.zhonguo1118.cn

TS:   nested.flat();
来源：https://hf.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ai.zhonguo7118.cn

Go:   // 手写双层循环
来源：https://oj.zhonguo4118.cn

Ruby: nested.flatten
来源：https://dl.zhonguo3118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://us.zhonguo5118.cn

[D19] 按字段分组
来源：https://xq.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://vi.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://gs.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://ts.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://bl.zhonguo7118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://hm.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://tn.zhonguo6118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ep.zhonguo2118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://hh.zhonguo5118.cn

[D20] 统计每个元素出现次数
来源：https://ey.zhonguo1118.cn

Py:   Counter(arr)
来源：https://so.zhonguo7118.cn

PHP:  array_count_values($arr);
来源：https://gc.zhonguo4118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://je.zhonguo8118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ec.zhonguo6118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://hs.zhonguo3118.cn

Go:   // 手写 map[T]int
来源：https://ca.zhonguo5118.cn

Ruby: arr.tally
来源：https://wr.zhonguo5118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://qy.zhonguo3118.cn

[D21] 判断是否包含某元素
来源：https://uf.zhonguo5118.cn

Py:   x in arr
来源：https://wi.zhonguo6118.cn

PHP:  in_array($x, $arr, true);
来源：https://xu.zhonguo4118.cn

JS:   arr.includes(x)
来源：https://nd.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://wq.zhonguo8118.cn

Java: list.contains(x)
来源：https://lv.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://fk.zhonguo3118.cn

Ruby: arr.include?(x)
来源：https://ar.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://uc.zhonguo5118.cn

[D22] 复制数组（避免共享引用）
来源：https://ik.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://zm.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://mv.zhonguo7118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://si.zhonguo3118.cn

TS:   [...arr];
来源：https://px.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://oo.zhonguo7118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://sb.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://ns.zhonguo7118.cn

C#:   new List<int>(list);
来源：https://gh.zhonguo5118.cn

[D23] reduce 累积计算
来源：https://jr.zhonguo2118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ql.zhonguo7118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://qs.zhonguo3118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://fa.zhonguo6118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://au.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://xh.zhonguo5118.cn

Go:   // 手写循环
来源：https://kp.zhonguo7118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://zo.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://sm.zhonguo6118.cn

[D24] 字典 / Map 基本操作
来源：https://xm.zhonguo5118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://dm.zhonguo8118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://nj.zhonguo2118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://lz.zhonguo4118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://oh.zhonguo2118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://lz.zhonguo2118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://te.zhonguo8118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://gp.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://dv.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://iq.zhonguo1118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ne.zhonguo2118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://gu.zhonguo8118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://cl.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://yb.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://ud.zhonguo5118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://qa.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://op.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://id.zhonguo4118.cn

[D26] 数组转字符串
来源：https://tp.zhonguo8118.cn

Py:   ", ".join(map(str, arr))
来源：https://cl.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://tm.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://ou.zhonguo1118.cn

TS:   arr.join(", ")
来源：https://pb.zhonguo5118.cn

Java: String.join(", ", list)
来源：https://rl.zhonguo4118.cn

Go:   strings.Join(strs, ", ")
来源：https://jm.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://tr.zhonguo1118.cn

C#:   string.Join(", ", list)
来源：https://ms.zhonguo3118.cn

================================================================================
来源：https://qk.zhonguo1118.cn

E. 字符串处理
来源：https://gy.zhonguo5118.cn

================================================================================
来源：https://ft.zhonguo1118.cn

[E01] 拼接字符串
来源：https://oy.zhonguo6118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://wn.zhonguo3118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://oe.zhonguo7118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ar.zhonguo1118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://ut.zhonguo3118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://to.zhonguo3118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://lf.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://ma.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://wk.zhonguo8118.cn

[E02] 重复字符串
来源：https://un.zhonguo4118.cn

Py:   "ab" * 3
来源：https://ck.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://zn.zhonguo3118.cn

JS:   "ab".repeat(3)
来源：https://gn.zhonguo2118.cn

TS:   "ab".repeat(3)
来源：https://bb.zhonguo2118.cn

Java: "ab".repeat(3)
来源：https://tk.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://du.zhonguo7118.cn

Ruby: "ab" * 3
来源：https://ln.zhonguo7118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://th.zhonguo8118.cn

[E03] 截取子串
来源：https://wz.zhonguo4118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://lm.zhonguo5118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ml.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://sc.zhonguo5118.cn

TS:   s.slice(1, 4)
来源：https://ds.zhonguo7118.cn

Java: s.substring(1, 4)
来源：https://vy.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://xw.zhonguo2118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://pz.zhonguo3118.cn

C#:   s.Substring(1, 3)
来源：https://kk.zhonguo8118.cn

[E04] 查找子串位置
来源：https://xo.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://zy.zhonguo5118.cn

PHP:  strpos($s, "x");
来源：https://yl.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://uc.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://dz.zhonguo4118.cn

Java: s.indexOf("x")
来源：https://pw.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://nc.zhonguo7118.cn

Ruby: s.index("x")
来源：https://tw.zhonguo5118.cn

C#:   s.IndexOf("x")
来源：https://sq.zhonguo1118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://is.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://wi.zhonguo6118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://wy.zhonguo5118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://zg.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://js.zhonguo4118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://px.zhonguo2118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://zw.zhonguo3118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://hi.zhonguo8118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://kk.zhonguo7118.cn

[E06] 替换子串
来源：https://so.zhonguo8118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://pc.zhonguo6118.cn

PHP:  str_replace("a", "b", $s);
来源：https://sl.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://fr.zhonguo1118.cn

TS:   s.replaceAll("a", "b")
来源：https://pc.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ho.zhonguo7118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ci.zhonguo3118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://ui.zhonguo3118.cn

C#:   s.Replace("a", "b")
来源：https://bk.zhonguo4118.cn

[E07] 按分隔符拆分
来源：https://ry.zhonguo8118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://mm.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://wo.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://fj.zhonguo8118.cn

TS:   s.split(",")
来源：https://dm.zhonguo7118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://cv.zhonguo2118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://le.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://gv.zhonguo3118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://rp.zhonguo7118.cn

[E08] 数组按分隔符合并
来源：https://wj.zhonguo2118.cn

Py:   ",".join(items)
来源：https://yr.zhonguo5118.cn

PHP:  implode(",", $items);
来源：https://ma.zhonguo5118.cn

JS:   items.join(",")
来源：https://sr.zhonguo6118.cn

TS:   items.join(",")
来源：https://ww.zhonguo4118.cn

Java: String.join(",", items)
来源：https://zv.zhonguo4118.cn

Go:   strings.Join(items, ",")
来源：https://gx.zhonguo7118.cn

Ruby: items.join(",")
来源：https://uq.zhonguo1118.cn

C#:   string.Join(",", items)
来源：https://aq.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://jn.zhonguo1118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ql.zhonguo4118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://oo.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://rq.zhonguo6118.cn

TS:   s.replace(/\s+/g, "")
来源：https://vu.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://cg.zhonguo4118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://fb.zhonguo4118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://cg.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://kn.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://li.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://hj.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ay.zhonguo2118.cn

JS:   "7".padStart(3, "0")
来源：https://zu.zhonguo7118.cn

TS:   "7".padStart(3, "0")
来源：https://sf.zhonguo4118.cn

Java: String.format("%03d", 7)
来源：https://ew.zhonguo4118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ly.zhonguo1118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://vq.zhonguo2118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://mi.zhonguo4118.cn

[E11] 反转字符串
来源：https://qp.zhonguo3118.cn

Py:   s[::-1]
来源：https://tu.zhonguo7118.cn

PHP:  strrev($s);
来源：https://io.zhonguo8118.cn

JS:   [...s].reverse().join("")
来源：https://sd.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://qg.zhonguo3118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ef.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://kp.zhonguo3118.cn

Ruby: s.reverse
来源：https://bd.zhonguo5118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://zf.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://yb.zhonguo5118.cn

Py:   s.count("a")
来源：https://tx.zhonguo5118.cn

PHP:  substr_count($s, "a");
来源：https://rt.zhonguo2118.cn

JS:   s.split("a").length - 1
来源：https://bg.zhonguo8118.cn

TS:   s.split("a").length - 1
来源：https://lc.zhonguo8118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://jf.zhonguo3118.cn

Go:   strings.Count(s, "a")
来源：https://mj.zhonguo8118.cn

Ruby: s.count("a")
来源：https://mu.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://je.zhonguo6118.cn

[E13] 逐字符遍历
来源：https://sb.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://yz.zhonguo4118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://de.zhonguo1118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://uz.zhonguo3118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ex.zhonguo7118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://bo.zhonguo7118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://mz.zhonguo6118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://qy.zhonguo7118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://mw.zhonguo2118.cn

[E14] URL 编码与 Base64
来源：https://gp.zhonguo7118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://ql.zhonguo6118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://br.zhonguo8118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://gp.zhonguo8118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://ge.zhonguo7118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://zp.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://al.zhonguo3118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://bf.zhonguo2118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://zf.zhonguo3118.cn

[E15] HTML 转义 / 反转义
来源：https://pv.zhonguo5118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://qf.zhonguo5118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://kk.zhonguo2118.cn


<!-- 参考信息 -->