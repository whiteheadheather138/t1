代发 wailian999

TS:   arr.slice(1, 4);
来源：https://gu.zhonguo6118.cn

Java: list.subList(1, 4);
来源：https://jh.zhonguo7118.cn

Go:   arr[1:4]
来源：https://xn.zhonguo3118.cn

Ruby: arr[1, 3]
来源：https://fo.zhonguo5118.cn

C#:   list.GetRange(1, 3);
来源：https://bz.zhonguo6118.cn

[D08] 合并两个数组
来源：https://ok.zhonguo4118.cn

Py:   a + b;  a.extend(b)
来源：https://mk.zhonguo5118.cn

PHP:  array_merge($a, $b);
来源：https://id.zhonguo1118.cn

JS:   [...a, ...b];  a.concat(b);
来源：https://ug.zhonguo5118.cn

TS:   [...a, ...b];
来源：https://gu.zhonguo8118.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：https://sm.zhonguo7118.cn

Go:   append(a, b...)
来源：https://qu.zhonguo4118.cn

Ruby: a + b;  a.concat(b)
来源：https://ym.zhonguo8118.cn

C#:   a.Concat(b).ToList()
来源：https://bs.zhonguo2118.cn

[D09] 排序（升序）
来源：https://hk.zhonguo8118.cn

Py:   sorted(arr);  arr.sort()
来源：https://du.zhonguo4118.cn

PHP:  sort($arr);
来源：https://wn.zhonguo1118.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：https://qm.zhonguo5118.cn

TS:   [...arr].sort((x, y) => x - y);
来源：https://vu.zhonguo6118.cn

Java: Collections.sort(list);  list.sort(null);
来源：https://zi.zhonguo8118.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：https://wf.zhonguo8118.cn

Ruby: arr.sort
来源：https://ko.zhonguo8118.cn

C#:   list.Sort();
来源：https://ii.zhonguo5118.cn

[D10] 自定义排序（按字段 / 多条件）
来源：https://fp.zhonguo7118.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：https://xk.zhonguo1118.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：https://fd.zhonguo8118.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：https://br.zhonguo1118.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：https://yz.zhonguo5118.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：https://vq.zhonguo6118.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：https://yi.zhonguo1118.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：https://jv.zhonguo8118.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：https://dz.zhonguo5118.cn

[D11] 反转数组
来源：https://sx.zhonguo2118.cn

Py:   arr[::-1];  arr.reverse()
来源：https://jh.zhonguo4118.cn

PHP:  array_reverse($arr);
来源：https://kr.zhonguo7118.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：https://gr.zhonguo6118.cn

TS:   [...arr].reverse();
来源：https://ty.zhonguo5118.cn

Java: Collections.reverse(list);
来源：https://co.zhonguo8118.cn

Go:   slices.Reverse(arr)
来源：https://hd.zhonguo1118.cn

Ruby: arr.reverse
来源：https://mb.zhonguo8118.cn

C#:   list.Reverse();
来源：https://ml.zhonguo1118.cn

[D12] 查找元素下标
来源：https://zl.zhonguo6118.cn

Py:   arr.index(x);  x in arr
来源：https://xa.zhonguo4118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://xy.zhonguo3118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://jn.zhonguo1118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://km.zhonguo7118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://ak.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://ls.zhonguo3118.cn

Ruby: arr.index(x)
来源：https://om.zhonguo3118.cn

C#:   list.IndexOf(x);
来源：https://jz.zhonguo6118.cn

[D13] 过滤（保留满足条件的）
来源：https://aa.zhonguo3118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://el.zhonguo8118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://ih.zhonguo2118.cn

JS:   arr.filter(x => x > 3)
来源：https://bb.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://zu.zhonguo5118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://mi.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://bz.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://fb.zhonguo2118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://iy.zhonguo8118.cn

[D14] 映射转换（每个元素变形）
来源：https://xv.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://ct.zhonguo5118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ug.zhonguo5118.cn

JS:   arr.map(x => x * 2)
来源：https://kd.zhonguo6118.cn

TS:   arr.map(x => x * 2)
来源：https://pr.zhonguo5118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://qn.zhonguo8118.cn

Go:   // 手写循环
来源：https://og.zhonguo4118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vp.zhonguo1118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://et.zhonguo8118.cn

[D15] 去重
来源：https://ds.zhonguo5118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://rt.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://ly.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://oe.zhonguo4118.cn

TS:   [...new Set(arr)]
来源：https://kh.zhonguo4118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ro.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://wn.zhonguo5118.cn

Ruby: arr.uniq
来源：https://ql.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://at.zhonguo1118.cn

[D16] 求和与平均值
来源：https://wg.zhonguo4118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://ir.zhonguo8118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://au.zhonguo1118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://jl.zhonguo2118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://lb.zhonguo7118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://jm.zhonguo8118.cn

Go:   // 手写循环累加
来源：https://lo.zhonguo1118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://bl.zhonguo8118.cn

C#:   list.Sum();  list.Average()
来源：https://eq.zhonguo5118.cn

[D17] 最大值与最小值
来源：https://br.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://bo.zhonguo6118.cn

PHP:  max($arr);  min($arr);
来源：https://te.zhonguo1118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://nk.zhonguo3118.cn

TS:   Math.max(...arr);
来源：https://mh.zhonguo2118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://df.zhonguo1118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://gp.zhonguo1118.cn

Ruby: arr.max;  arr.min
来源：https://tp.zhonguo1118.cn

C#:   list.Max();  list.Min()
来源：https://qs.zhonguo6118.cn

[D18] 扁平化嵌套数组
来源：https://ha.zhonguo6118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://xy.zhonguo2118.cn

PHP:  array_merge(...$nested);
来源：https://dh.zhonguo1118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://dy.zhonguo7118.cn

TS:   nested.flat();
来源：https://dq.zhonguo3118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://du.zhonguo2118.cn

Go:   // 手写双层循环
来源：https://lw.zhonguo1118.cn

Ruby: nested.flatten
来源：https://zt.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://iw.zhonguo3118.cn

[D19] 按字段分组
来源：https://pb.zhonguo3118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ea.zhonguo6118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://nd.zhonguo2118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://ze.zhonguo4118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://zy.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://ie.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://ro.zhonguo6118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://id.zhonguo8118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://ha.zhonguo4118.cn

[D20] 统计每个元素出现次数
来源：https://ts.zhonguo2118.cn

Py:   Counter(arr)
来源：https://pq.zhonguo2118.cn

PHP:  array_count_values($arr);
来源：https://sd.zhonguo4118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://jz.zhonguo2118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://yf.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://xj.zhonguo4118.cn

Go:   // 手写 map[T]int
来源：https://we.zhonguo1118.cn

Ruby: arr.tally
来源：https://ma.zhonguo7118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://ke.zhonguo3118.cn

[D21] 判断是否包含某元素
来源：https://wd.zhonguo2118.cn

Py:   x in arr
来源：https://mh.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://bo.zhonguo8118.cn

JS:   arr.includes(x)
来源：https://vl.zhonguo3118.cn

TS:   arr.includes(x)
来源：https://uk.zhonguo5118.cn

Java: list.contains(x)
来源：https://rz.zhonguo7118.cn

Go:   slices.Contains(arr, x)
来源：https://yr.zhonguo1118.cn

Ruby: arr.include?(x)
来源：https://wc.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://sw.zhonguo5118.cn

[D22] 复制数组（避免共享引用）
来源：https://fh.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://ew.zhonguo7118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://fq.zhonguo6118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://nn.zhonguo5118.cn

TS:   [...arr];
来源：https://mu.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://ma.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://ib.zhonguo7118.cn

Ruby: arr.dup;  arr.clone
来源：https://bf.zhonguo1118.cn

C#:   new List<int>(list);
来源：https://dp.zhonguo6118.cn

[D23] reduce 累积计算
来源：https://tq.zhonguo5118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://hd.zhonguo1118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://kf.zhonguo2118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://om.zhonguo2118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://fu.zhonguo1118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://fe.zhonguo6118.cn

Go:   // 手写循环
来源：https://ox.zhonguo5118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://et.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://jf.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://vh.zhonguo3118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://av.zhonguo5118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://wy.zhonguo1118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://yz.zhonguo5118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://nt.zhonguo5118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://xc.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://pw.zhonguo7118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://pr.zhonguo5118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://mf.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://gl.zhonguo6118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://ta.zhonguo2118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://qm.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://bz.zhonguo7118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://gp.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://bw.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://jy.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://tt.zhonguo7118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://qo.zhonguo8118.cn

[D26] 数组转字符串
来源：https://rk.zhonguo4118.cn

Py:   ", ".join(map(str, arr))
来源：https://pj.zhonguo4118.cn

PHP:  implode(", ", $arr);
来源：https://zl.zhonguo2118.cn

JS:   arr.join(", ")
来源：https://dx.zhonguo7118.cn

TS:   arr.join(", ")
来源：https://hm.zhonguo2118.cn

Java: String.join(", ", list)
来源：https://yf.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://mu.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://rf.zhonguo2118.cn

C#:   string.Join(", ", list)
来源：https://wk.zhonguo4118.cn

================================================================================
来源：https://xi.zhonguo5118.cn

E. 字符串处理
来源：https://ie.zhonguo8118.cn

================================================================================
来源：https://in.zhonguo1118.cn

[E01] 拼接字符串
来源：https://dl.zhonguo5118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://np.zhonguo3118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://ec.zhonguo1118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ex.zhonguo8118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://xw.zhonguo6118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ob.zhonguo4118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://em.zhonguo6118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://id.zhonguo3118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://lj.zhonguo2118.cn

[E02] 重复字符串
来源：https://qm.zhonguo5118.cn

Py:   "ab" * 3
来源：https://yr.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://qq.zhonguo5118.cn

JS:   "ab".repeat(3)
来源：https://tk.zhonguo8118.cn

TS:   "ab".repeat(3)
来源：https://jw.zhonguo5118.cn

Java: "ab".repeat(3)
来源：https://wt.zhonguo5118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wj.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://wq.zhonguo8118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://kn.zhonguo5118.cn

[E03] 截取子串
来源：https://at.zhonguo7118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ze.zhonguo6118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ig.zhonguo8118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://vc.zhonguo5118.cn

TS:   s.slice(1, 4)
来源：https://kj.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://qh.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ln.zhonguo2118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://je.zhonguo1118.cn

C#:   s.Substring(1, 3)
来源：https://ng.zhonguo1118.cn

[E04] 查找子串位置
来源：https://go.zhonguo6118.cn

Py:   s.find("x");  s.index("x")
来源：https://gh.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://zr.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://ak.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://sd.zhonguo8118.cn

Java: s.indexOf("x")
来源：https://mw.zhonguo6118.cn

Go:   strings.Index(s, "x")
来源：https://fo.zhonguo8118.cn

Ruby: s.index("x")
来源：https://me.zhonguo5118.cn

C#:   s.IndexOf("x")
来源：https://mt.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://hj.zhonguo8118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://rx.zhonguo6118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://oc.zhonguo7118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://kt.zhonguo1118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://qr.zhonguo6118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://vm.zhonguo3118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://el.zhonguo3118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://xt.zhonguo1118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://ah.zhonguo4118.cn

[E06] 替换子串
来源：https://di.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://mo.zhonguo8118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ql.zhonguo6118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://gs.zhonguo7118.cn

TS:   s.replaceAll("a", "b")
来源：https://di.zhonguo2118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://tx.zhonguo8118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://rp.zhonguo2118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://hj.zhonguo5118.cn

C#:   s.Replace("a", "b")
来源：https://ly.zhonguo7118.cn

[E07] 按分隔符拆分
来源：https://us.zhonguo5118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://qe.zhonguo8118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://uk.zhonguo6118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://pt.zhonguo6118.cn

TS:   s.split(",")
来源：https://cj.zhonguo6118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://jj.zhonguo3118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://ot.zhonguo8118.cn

Ruby: s.split(",");  s.split
来源：https://cr.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://mk.zhonguo8118.cn

[E08] 数组按分隔符合并
来源：https://vv.zhonguo4118.cn

Py:   ",".join(items)
来源：https://fp.zhonguo3118.cn

PHP:  implode(",", $items);
来源：https://fz.zhonguo1118.cn

JS:   items.join(",")
来源：https://iq.zhonguo2118.cn

TS:   items.join(",")
来源：https://nx.zhonguo4118.cn

Java: String.join(",", items)
来源：https://og.zhonguo2118.cn

Go:   strings.Join(items, ",")
来源：https://vb.zhonguo2118.cn

Ruby: items.join(",")
来源：https://fc.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://yj.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://qj.zhonguo4118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://sm.zhonguo2118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://at.zhonguo2118.cn

JS:   s.replace(/\s+/g, "")
来源：https://sx.zhonguo1118.cn

TS:   s.replace(/\s+/g, "")
来源：https://gp.zhonguo4118.cn

Java: s.replaceAll("\\s+", "")
来源：https://ck.zhonguo6118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vu.zhonguo1118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://kb.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://ks.zhonguo4118.cn

[E10] 左侧补零 / 定长填充
来源：https://ku.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://hy.zhonguo6118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://ie.zhonguo2118.cn

JS:   "7".padStart(3, "0")
来源：https://mf.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://gd.zhonguo4118.cn

Java: String.format("%03d", 7)
来源：https://lg.zhonguo7118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://eq.zhonguo3118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://zm.zhonguo5118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://zb.zhonguo2118.cn

[E11] 反转字符串
来源：https://om.zhonguo8118.cn

Py:   s[::-1]
来源：https://bk.zhonguo7118.cn

PHP:  strrev($s);
来源：https://gi.zhonguo3118.cn

JS:   [...s].reverse().join("")
来源：https://sp.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://je.zhonguo8118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ms.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://zb.zhonguo3118.cn

Ruby: s.reverse
来源：https://fn.zhonguo8118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://kv.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://wb.zhonguo1118.cn

Py:   s.count("a")
来源：https://ts.zhonguo3118.cn

PHP:  substr_count($s, "a");
来源：https://xr.zhonguo4118.cn

JS:   s.split("a").length - 1
来源：https://oy.zhonguo4118.cn

TS:   s.split("a").length - 1
来源：https://gy.zhonguo5118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://iu.zhonguo5118.cn

Go:   strings.Count(s, "a")
来源：https://bg.zhonguo7118.cn

Ruby: s.count("a")
来源：https://ra.zhonguo8118.cn

C#:   s.Count(c => c == 'a')
来源：https://xr.zhonguo1118.cn

[E13] 逐字符遍历
来源：https://bz.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://xq.zhonguo5118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://ok.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://we.zhonguo3118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://lh.zhonguo6118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://vd.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://lb.zhonguo5118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://ny.zhonguo8118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://bb.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://jv.zhonguo2118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://ek.zhonguo5118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://cx.zhonguo7118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://za.zhonguo3118.cn


<!-- 参考信息 -->