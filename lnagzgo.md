代发 wailian999

TS:   [...arr].reverse();
来源：https://bl.zhonguo6118.cn

Java: Collections.reverse(list);
来源：https://yh.zhonguo7118.cn

Go:   slices.Reverse(arr)
来源：https://bi.zhonguo8118.cn

Ruby: arr.reverse
来源：https://kk.zhonguo3118.cn

C#:   list.Reverse();
来源：https://uv.zhonguo2118.cn

[D12] 查找元素下标
来源：https://cs.zhonguo7118.cn

Py:   arr.index(x);  x in arr
来源：https://hb.zhonguo7118.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：https://zl.zhonguo2118.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://yt.zhonguo6118.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：https://lc.zhonguo8118.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：https://er.zhonguo5118.cn

Go:   slices.Index(arr, x)
来源：https://sp.zhonguo2118.cn

Ruby: arr.index(x)
来源：https://jb.zhonguo8118.cn

C#:   list.IndexOf(x);
来源：https://ze.zhonguo4118.cn

[D13] 过滤（保留满足条件的）
来源：https://sv.zhonguo1118.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：https://xs.zhonguo4118.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://iq.zhonguo7118.cn

JS:   arr.filter(x => x > 3)
来源：https://da.zhonguo2118.cn

TS:   arr.filter(x => x > 3)
来源：https://ct.zhonguo1118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://jl.zhonguo4118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://fs.zhonguo5118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://sv.zhonguo5118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ei.zhonguo6118.cn

[D14] 映射转换（每个元素变形）
来源：https://hv.zhonguo6118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://gg.zhonguo4118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://ki.zhonguo1118.cn

JS:   arr.map(x => x * 2)
来源：https://dh.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://ak.zhonguo1118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://ce.zhonguo5118.cn

Go:   // 手写循环
来源：https://dx.zhonguo8118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vx.zhonguo3118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://bu.zhonguo7118.cn

[D15] 去重
来源：https://rv.zhonguo4118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://af.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://yf.zhonguo4118.cn

JS:   [...new Set(arr)]
来源：https://co.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://we.zhonguo1118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://up.zhonguo2118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://yq.zhonguo7118.cn

Ruby: arr.uniq
来源：https://wu.zhonguo2118.cn

C#:   list.Distinct().ToList()
来源：https://tn.zhonguo5118.cn

[D16] 求和与平均值
来源：https://wd.zhonguo3118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://wp.zhonguo5118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://aq.zhonguo3118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://le.zhonguo8118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://af.zhonguo8118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://tu.zhonguo4118.cn

Go:   // 手写循环累加
来源：https://ij.zhonguo8118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://xe.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://av.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://ax.zhonguo4118.cn

Py:   max(arr);  min(arr)
来源：https://vw.zhonguo3118.cn

PHP:  max($arr);  min($arr);
来源：https://ms.zhonguo8118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://yx.zhonguo5118.cn

TS:   Math.max(...arr);
来源：https://xc.zhonguo5118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://lh.zhonguo2118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://zx.zhonguo1118.cn

Ruby: arr.max;  arr.min
来源：https://zm.zhonguo4118.cn

C#:   list.Max();  list.Min()
来源：https://ke.zhonguo5118.cn

[D18] 扁平化嵌套数组
来源：https://xd.zhonguo4118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://ky.zhonguo1118.cn

PHP:  array_merge(...$nested);
来源：https://fx.zhonguo6118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://ms.zhonguo3118.cn

TS:   nested.flat();
来源：https://jt.zhonguo8118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://rx.zhonguo5118.cn

Go:   // 手写双层循环
来源：https://ib.zhonguo8118.cn

Ruby: nested.flatten
来源：https://qx.zhonguo8118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://wd.zhonguo1118.cn

[D19] 按字段分组
来源：https://be.zhonguo4118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://jj.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://ek.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://wr.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ap.zhonguo1118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://vt.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://by.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://vl.zhonguo6118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://mc.zhonguo7118.cn

[D20] 统计每个元素出现次数
来源：https://te.zhonguo2118.cn

Py:   Counter(arr)
来源：https://vy.zhonguo5118.cn

PHP:  array_count_values($arr);
来源：https://ga.zhonguo3118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://gh.zhonguo3118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://tx.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://wx.zhonguo6118.cn

Go:   // 手写 map[T]int
来源：https://ih.zhonguo4118.cn

Ruby: arr.tally
来源：https://jq.zhonguo5118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://tx.zhonguo1118.cn

[D21] 判断是否包含某元素
来源：https://cq.zhonguo8118.cn

Py:   x in arr
来源：https://xr.zhonguo4118.cn

PHP:  in_array($x, $arr, true);
来源：https://kt.zhonguo8118.cn

JS:   arr.includes(x)
来源：https://nf.zhonguo6118.cn

TS:   arr.includes(x)
来源：https://kp.zhonguo3118.cn

Java: list.contains(x)
来源：https://zx.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://on.zhonguo2118.cn

Ruby: arr.include?(x)
来源：https://lv.zhonguo7118.cn

C#:   list.Contains(x)
来源：https://np.zhonguo6118.cn

[D22] 复制数组（避免共享引用）
来源：https://cz.zhonguo3118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://to.zhonguo6118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://we.zhonguo3118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://lz.zhonguo1118.cn

TS:   [...arr];
来源：https://xg.zhonguo3118.cn

Java: new ArrayList<>(list);
来源：https://ak.zhonguo4118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://td.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://zu.zhonguo2118.cn

C#:   new List<int>(list);
来源：https://zy.zhonguo2118.cn

[D23] reduce 累积计算
来源：https://nc.zhonguo3118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://mc.zhonguo3118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://sg.zhonguo7118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://de.zhonguo6118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://fg.zhonguo4118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://vw.zhonguo5118.cn

Go:   // 手写循环
来源：https://hy.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://lo.zhonguo3118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://si.zhonguo2118.cn

[D24] 字典 / Map 基本操作
来源：https://ak.zhonguo8118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://ca.zhonguo8118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://ra.zhonguo4118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://tc.zhonguo3118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://bh.zhonguo2118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://md.zhonguo5118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://he.zhonguo3118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://zu.zhonguo5118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://if.zhonguo8118.cn

[D25] Set 集合去重与交并差
来源：https://no.zhonguo3118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://yy.zhonguo1118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://da.zhonguo3118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://wu.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://cc.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://hk.zhonguo2118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://xc.zhonguo5118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://fc.zhonguo5118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://ql.zhonguo5118.cn

[D26] 数组转字符串
来源：https://ei.zhonguo7118.cn

Py:   ", ".join(map(str, arr))
来源：https://fi.zhonguo8118.cn

PHP:  implode(", ", $arr);
来源：https://ry.zhonguo3118.cn

JS:   arr.join(", ")
来源：https://vo.zhonguo3118.cn

TS:   arr.join(", ")
来源：https://vp.zhonguo2118.cn

Java: String.join(", ", list)
来源：https://ww.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://bl.zhonguo7118.cn

Ruby: arr.join(", ")
来源：https://yw.zhonguo5118.cn

C#:   string.Join(", ", list)
来源：https://is.zhonguo6118.cn

================================================================================
来源：https://ba.zhonguo7118.cn

E. 字符串处理
来源：https://pw.zhonguo8118.cn

================================================================================
来源：https://hh.zhonguo1118.cn

[E01] 拼接字符串
来源：https://hw.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ak.zhonguo6118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://nx.zhonguo5118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://rb.zhonguo4118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://me.zhonguo5118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://iv.zhonguo7118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://gb.zhonguo4118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://hu.zhonguo7118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://zd.zhonguo8118.cn

[E02] 重复字符串
来源：https://bx.zhonguo3118.cn

Py:   "ab" * 3
来源：https://ob.zhonguo1118.cn

PHP:  str_repeat("ab", 3);
来源：https://dk.zhonguo4118.cn

JS:   "ab".repeat(3)
来源：https://ic.zhonguo6118.cn

TS:   "ab".repeat(3)
来源：https://fy.zhonguo8118.cn

Java: "ab".repeat(3)
来源：https://jn.zhonguo1118.cn

Go:   strings.Repeat("ab", 3)
来源：https://wq.zhonguo2118.cn

Ruby: "ab" * 3
来源：https://wo.zhonguo4118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://ei.zhonguo4118.cn

[E03] 截取子串
来源：https://fv.zhonguo6118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://kd.zhonguo2118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://th.zhonguo5118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://qh.zhonguo8118.cn

TS:   s.slice(1, 4)
来源：https://hi.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://oz.zhonguo2118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://tt.zhonguo6118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://fn.zhonguo3118.cn

C#:   s.Substring(1, 3)
来源：https://go.zhonguo6118.cn

[E04] 查找子串位置
来源：https://ur.zhonguo1118.cn

Py:   s.find("x");  s.index("x")
来源：https://bp.zhonguo4118.cn

PHP:  strpos($s, "x");
来源：https://qz.zhonguo1118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://vv.zhonguo6118.cn

TS:   s.indexOf("x")
来源：https://ew.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://eh.zhonguo4118.cn

Go:   strings.Index(s, "x")
来源：https://xg.zhonguo5118.cn

Ruby: s.index("x")
来源：https://vp.zhonguo6118.cn

C#:   s.IndexOf("x")
来源：https://sg.zhonguo3118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://xt.zhonguo4118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://bf.zhonguo6118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://ru.zhonguo2118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://sv.zhonguo2118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://mh.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://up.zhonguo6118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://vq.zhonguo3118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://tn.zhonguo1118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://ak.zhonguo7118.cn

[E06] 替换子串
来源：https://pf.zhonguo6118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://es.zhonguo3118.cn

PHP:  str_replace("a", "b", $s);
来源：https://uj.zhonguo4118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://ph.zhonguo2118.cn

TS:   s.replaceAll("a", "b")
来源：https://jl.zhonguo3118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://mr.zhonguo1118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://wx.zhonguo3118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://hn.zhonguo1118.cn

C#:   s.Replace("a", "b")
来源：https://mw.zhonguo5118.cn

[E07] 按分隔符拆分
来源：https://ra.zhonguo2118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://uc.zhonguo5118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://ah.zhonguo8118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://eh.zhonguo3118.cn

TS:   s.split(",")
来源：https://xk.zhonguo4118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://dk.zhonguo7118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://tm.zhonguo8118.cn

Ruby: s.split(",");  s.split
来源：https://gb.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://cr.zhonguo6118.cn

[E08] 数组按分隔符合并
来源：https://vb.zhonguo6118.cn

Py:   ",".join(items)
来源：https://ug.zhonguo1118.cn

PHP:  implode(",", $items);
来源：https://gg.zhonguo2118.cn

JS:   items.join(",")
来源：https://qu.zhonguo8118.cn

TS:   items.join(",")
来源：https://fd.zhonguo2118.cn

Java: String.join(",", items)
来源：https://ur.zhonguo4118.cn

Go:   strings.Join(items, ",")
来源：https://ls.zhonguo1118.cn

Ruby: items.join(",")
来源：https://wp.zhonguo5118.cn

C#:   string.Join(",", items)
来源：https://ng.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://cm.zhonguo5118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://gu.zhonguo3118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://us.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://cs.zhonguo2118.cn

TS:   s.replace(/\s+/g, "")
来源：https://fm.zhonguo3118.cn

Java: s.replaceAll("\\s+", "")
来源：https://re.zhonguo1118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://ia.zhonguo3118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://ke.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://ul.zhonguo5118.cn

[E10] 左侧补零 / 定长填充
来源：https://ed.zhonguo2118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://ui.zhonguo5118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://fo.zhonguo6118.cn

JS:   "7".padStart(3, "0")
来源：https://rw.zhonguo3118.cn

TS:   "7".padStart(3, "0")
来源：https://kp.zhonguo6118.cn

Java: String.format("%03d", 7)
来源：https://be.zhonguo6118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://zf.zhonguo8118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ba.zhonguo1118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://bc.zhonguo5118.cn

[E11] 反转字符串
来源：https://vg.zhonguo1118.cn

Py:   s[::-1]
来源：https://vr.zhonguo6118.cn

PHP:  strrev($s);
来源：https://oi.zhonguo5118.cn

JS:   [...s].reverse().join("")
来源：https://qx.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://si.zhonguo6118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ei.zhonguo2118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://ql.zhonguo2118.cn

Ruby: s.reverse
来源：https://bv.zhonguo6118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://mf.zhonguo6118.cn

[E12] 统计某字符出现次数
来源：https://hc.zhonguo2118.cn

Py:   s.count("a")
来源：https://gp.zhonguo4118.cn

PHP:  substr_count($s, "a");
来源：https://ma.zhonguo4118.cn

JS:   s.split("a").length - 1
来源：https://rj.zhonguo7118.cn

TS:   s.split("a").length - 1
来源：https://iv.zhonguo7118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://fc.zhonguo3118.cn

Go:   strings.Count(s, "a")
来源：https://bi.zhonguo2118.cn

Ruby: s.count("a")
来源：https://au.zhonguo5118.cn

C#:   s.Count(c => c == 'a')
来源：https://az.zhonguo3118.cn

[E13] 逐字符遍历
来源：https://yp.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://ez.zhonguo7118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://jp.zhonguo4118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://el.zhonguo3118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://gc.zhonguo4118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://ki.zhonguo7118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://rz.zhonguo2118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://uc.zhonguo3118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://sq.zhonguo1118.cn

[E14] URL 编码与 Base64
来源：https://ar.zhonguo5118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://be.zhonguo4118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://ef.zhonguo8118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://ln.zhonguo4118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://mm.zhonguo5118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://og.zhonguo5118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://kl.zhonguo5118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://zk.zhonguo5118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://bl.zhonguo4118.cn

[E15] HTML 转义 / 反转义
来源：https://df.zhonguo8118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://nw.zhonguo2118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://jj.zhonguo8118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://nk.zhonguo8118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://pw.zhonguo5118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://wp.zhonguo1118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://st.zhonguo5118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://qr.zhonguo5118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://yn.zhonguo6118.cn

[E16] 数字千分位
来源：https://sr.zhonguo3118.cn

Py:   f"{1234567:,}"
来源：https://kb.zhonguo4118.cn

PHP:  number_format(1234567);
来源：https://xb.zhonguo6118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://bg.zhonguo1118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://mp.zhonguo2118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://gs.zhonguo7118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://xz.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://ya.zhonguo6118.cn

C#:   1234567.ToString("N0")
来源：https://xt.zhonguo4118.cn

[E17] 首字母大写
来源：https://zp.zhonguo5118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://er.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://ju.zhonguo8118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://tw.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ze.zhonguo5118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://tq.zhonguo7118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://rj.zhonguo5118.cn

Ruby: s.capitalize
来源：https://gh.zhonguo1118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://hv.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://mk.zhonguo5118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://aq.zhonguo3118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://af.zhonguo3118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://sk.zhonguo5118.cn


<!-- 参考信息 -->