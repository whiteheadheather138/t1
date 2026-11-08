代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://fy.zhonguo5118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://hz.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://nq.zhonguo5118.cn

TS:   arr.map(x => x * 2)
来源：https://uh.zhonguo7118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://hr.zhonguo7118.cn

Go:   // 手写循环
来源：https://ze.zhonguo6118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://ij.zhonguo6118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://wt.zhonguo2118.cn

[D15] 去重
来源：https://qs.zhonguo8118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://eb.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://uz.zhonguo6118.cn

JS:   [...new Set(arr)]
来源：https://yr.zhonguo3118.cn

TS:   [...new Set(arr)]
来源：https://cw.zhonguo7118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://mj.zhonguo4118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://hd.zhonguo6118.cn

Ruby: arr.uniq
来源：https://zu.zhonguo1118.cn

C#:   list.Distinct().ToList()
来源：https://df.zhonguo4118.cn

[D16] 求和与平均值
来源：https://la.zhonguo2118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://cs.zhonguo2118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://ol.zhonguo1118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://yu.zhonguo5118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://qb.zhonguo6118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://bh.zhonguo4118.cn

Go:   // 手写循环累加
来源：https://zr.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://wc.zhonguo6118.cn

C#:   list.Sum();  list.Average()
来源：https://si.zhonguo1118.cn

[D17] 最大值与最小值
来源：https://cy.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://zf.zhonguo5118.cn

PHP:  max($arr);  min($arr);
来源：https://os.zhonguo7118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://zv.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://od.zhonguo4118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://hs.zhonguo4118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ny.zhonguo8118.cn

Ruby: arr.max;  arr.min
来源：https://uo.zhonguo6118.cn

C#:   list.Max();  list.Min()
来源：https://hj.zhonguo6118.cn

[D18] 扁平化嵌套数组
来源：https://fo.zhonguo2118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://vb.zhonguo2118.cn

PHP:  array_merge(...$nested);
来源：https://cx.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://az.zhonguo3118.cn

TS:   nested.flat();
来源：https://xu.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://ti.zhonguo1118.cn

Go:   // 手写双层循环
来源：https://gz.zhonguo2118.cn

Ruby: nested.flatten
来源：https://vy.zhonguo1118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://qx.zhonguo7118.cn

[D19] 按字段分组
来源：https://ot.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://ad.zhonguo4118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://hj.zhonguo4118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://vh.zhonguo6118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://eo.zhonguo3118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://zu.zhonguo1118.cn

Go:   // 手写 map[string][]T
来源：https://ob.zhonguo3118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://bc.zhonguo4118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://sq.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://yw.zhonguo7118.cn

Py:   Counter(arr)
来源：https://dn.zhonguo1118.cn

PHP:  array_count_values($arr);
来源：https://ln.zhonguo8118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://xs.zhonguo4118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://he.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://rk.zhonguo4118.cn

Go:   // 手写 map[T]int
来源：https://rp.zhonguo7118.cn

Ruby: arr.tally
来源：https://ls.zhonguo2118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://li.zhonguo7118.cn

[D21] 判断是否包含某元素
来源：https://ib.zhonguo4118.cn

Py:   x in arr
来源：https://sy.zhonguo3118.cn

PHP:  in_array($x, $arr, true);
来源：https://fc.zhonguo7118.cn

JS:   arr.includes(x)
来源：https://ws.zhonguo3118.cn

TS:   arr.includes(x)
来源：https://mx.zhonguo4118.cn

Java: list.contains(x)
来源：https://jx.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://lk.zhonguo6118.cn

Ruby: arr.include?(x)
来源：https://zp.zhonguo6118.cn

C#:   list.Contains(x)
来源：https://ro.zhonguo3118.cn

[D22] 复制数组（避免共享引用）
来源：https://gd.zhonguo5118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://bf.zhonguo2118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://jk.zhonguo4118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://kf.zhonguo5118.cn

TS:   [...arr];
来源：https://eb.zhonguo1118.cn

Java: new ArrayList<>(list);
来源：https://kt.zhonguo5118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://do.zhonguo8118.cn

Ruby: arr.dup;  arr.clone
来源：https://pb.zhonguo6118.cn

C#:   new List<int>(list);
来源：https://ot.zhonguo1118.cn

[D23] reduce 累积计算
来源：https://dt.zhonguo3118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://ex.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://um.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ex.zhonguo1118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ru.zhonguo7118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://nb.zhonguo8118.cn

Go:   // 手写循环
来源：https://sc.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://un.zhonguo2118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://bf.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://ru.zhonguo4118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://um.zhonguo8118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://al.zhonguo6118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://pd.zhonguo2118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://hn.zhonguo6118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://lr.zhonguo6118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://od.zhonguo3118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://mz.zhonguo4118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://zx.zhonguo4118.cn

[D25] Set 集合去重与交并差
来源：https://th.zhonguo5118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://xo.zhonguo3118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://zd.zhonguo4118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://oz.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ee.zhonguo3118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://yu.zhonguo3118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://qi.zhonguo6118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://ri.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://yd.zhonguo2118.cn

[D26] 数组转字符串
来源：https://jd.zhonguo5118.cn

Py:   ", ".join(map(str, arr))
来源：https://yw.zhonguo3118.cn

PHP:  implode(", ", $arr);
来源：https://xd.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://dg.zhonguo1118.cn

TS:   arr.join(", ")
来源：https://bz.zhonguo8118.cn

Java: String.join(", ", list)
来源：https://gx.zhonguo2118.cn

Go:   strings.Join(strs, ", ")
来源：https://pq.zhonguo5118.cn

Ruby: arr.join(", ")
来源：https://yl.zhonguo3118.cn

C#:   string.Join(", ", list)
来源：https://mo.zhonguo7118.cn

================================================================================
来源：https://on.zhonguo8118.cn

E. 字符串处理
来源：https://xu.zhonguo4118.cn

================================================================================
来源：https://wd.zhonguo7118.cn

[E01] 拼接字符串
来源：https://od.zhonguo5118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ax.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://lg.zhonguo3118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://tw.zhonguo5118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://iy.zhonguo2118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://ah.zhonguo1118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://tr.zhonguo7118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://hp.zhonguo5118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://uk.zhonguo8118.cn

[E02] 重复字符串
来源：https://me.zhonguo6118.cn

Py:   "ab" * 3
来源：https://lk.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://pa.zhonguo3118.cn

JS:   "ab".repeat(3)
来源：https://fu.zhonguo4118.cn

TS:   "ab".repeat(3)
来源：https://sf.zhonguo1118.cn

Java: "ab".repeat(3)
来源：https://zr.zhonguo6118.cn

Go:   strings.Repeat("ab", 3)
来源：https://zj.zhonguo5118.cn

Ruby: "ab" * 3
来源：https://pz.zhonguo4118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://sr.zhonguo4118.cn

[E03] 截取子串
来源：https://os.zhonguo5118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://dc.zhonguo4118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://sx.zhonguo6118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://rz.zhonguo6118.cn

TS:   s.slice(1, 4)
来源：https://hf.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://yf.zhonguo6118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://ff.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://as.zhonguo1118.cn

C#:   s.Substring(1, 3)
来源：https://ab.zhonguo4118.cn

[E04] 查找子串位置
来源：https://pm.zhonguo5118.cn

Py:   s.find("x");  s.index("x")
来源：https://go.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://zq.zhonguo6118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://hf.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://dl.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://jy.zhonguo8118.cn

Go:   strings.Index(s, "x")
来源：https://md.zhonguo5118.cn

Ruby: s.index("x")
来源：https://ik.zhonguo2118.cn

C#:   s.IndexOf("x")
来源：https://fa.zhonguo7118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://pb.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://hr.zhonguo3118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://fi.zhonguo7118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://vj.zhonguo8118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://fy.zhonguo7118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://to.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://hc.zhonguo2118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://as.zhonguo6118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://xi.zhonguo1118.cn

[E06] 替换子串
来源：https://sk.zhonguo4118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://rf.zhonguo7118.cn

PHP:  str_replace("a", "b", $s);
来源：https://ze.zhonguo5118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://kf.zhonguo6118.cn

TS:   s.replaceAll("a", "b")
来源：https://ad.zhonguo6118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://fo.zhonguo8118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://lq.zhonguo8118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://qu.zhonguo3118.cn

C#:   s.Replace("a", "b")
来源：https://sk.zhonguo2118.cn

[E07] 按分隔符拆分
来源：https://pg.zhonguo5118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://qi.zhonguo6118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://kl.zhonguo8118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://aj.zhonguo1118.cn

TS:   s.split(",")
来源：https://ae.zhonguo8118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://iw.zhonguo5118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://bi.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://lm.zhonguo5118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://bf.zhonguo4118.cn

[E08] 数组按分隔符合并
来源：https://yl.zhonguo5118.cn

Py:   ",".join(items)
来源：https://ju.zhonguo2118.cn

PHP:  implode(",", $items);
来源：https://er.zhonguo1118.cn

JS:   items.join(",")
来源：https://le.zhonguo7118.cn

TS:   items.join(",")
来源：https://jz.zhonguo6118.cn

Java: String.join(",", items)
来源：https://vv.zhonguo1118.cn

Go:   strings.Join(items, ",")
来源：https://nk.zhonguo2118.cn

Ruby: items.join(",")
来源：https://xn.zhonguo7118.cn

C#:   string.Join(",", items)
来源：https://cv.zhonguo5118.cn

[E09] 去除所有空白字符
来源：https://cw.zhonguo7118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://tx.zhonguo8118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://co.zhonguo6118.cn

JS:   s.replace(/\s+/g, "")
来源：https://nt.zhonguo2118.cn

TS:   s.replace(/\s+/g, "")
来源：https://ho.zhonguo7118.cn

Java: s.replaceAll("\\s+", "")
来源：https://qo.zhonguo6118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://bw.zhonguo6118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://hy.zhonguo2118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://wx.zhonguo3118.cn

[E10] 左侧补零 / 定长填充
来源：https://pk.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://we.zhonguo2118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://yg.zhonguo5118.cn

JS:   "7".padStart(3, "0")
来源：https://dc.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://ix.zhonguo7118.cn

Java: String.format("%03d", 7)
来源：https://ge.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://cx.zhonguo8118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://tt.zhonguo4118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://uj.zhonguo5118.cn

[E11] 反转字符串
来源：https://xv.zhonguo1118.cn

Py:   s[::-1]
来源：https://qq.zhonguo5118.cn

PHP:  strrev($s);
来源：https://oc.zhonguo7118.cn

JS:   [...s].reverse().join("")
来源：https://ar.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://dl.zhonguo1118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://wk.zhonguo5118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://xt.zhonguo8118.cn

Ruby: s.reverse
来源：https://ci.zhonguo1118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://nq.zhonguo7118.cn

[E12] 统计某字符出现次数
来源：https://ei.zhonguo2118.cn

Py:   s.count("a")
来源：https://qw.zhonguo6118.cn

PHP:  substr_count($s, "a");
来源：https://na.zhonguo8118.cn

JS:   s.split("a").length - 1
来源：https://ci.zhonguo1118.cn

TS:   s.split("a").length - 1
来源：https://yv.zhonguo1118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://cq.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://nw.zhonguo5118.cn

Ruby: s.count("a")
来源：https://vc.zhonguo4118.cn

C#:   s.Count(c => c == 'a')
来源：https://ue.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://mz.zhonguo3118.cn

Py:   for ch in s: print(ch)
来源：https://en.zhonguo2118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://xe.zhonguo6118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://qr.zhonguo8118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://ie.zhonguo8118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://nk.zhonguo2118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://jp.zhonguo8118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://na.zhonguo3118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ke.zhonguo6118.cn

[E14] URL 编码与 Base64
来源：https://ii.zhonguo1118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://tw.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://no.zhonguo6118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://vm.zhonguo1118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://kk.zhonguo7118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://nc.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://au.zhonguo2118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://rw.zhonguo7118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://dx.zhonguo2118.cn

[E15] HTML 转义 / 反转义
来源：https://bx.zhonguo6118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://xl.zhonguo2118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://dz.zhonguo2118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://zf.zhonguo3118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://si.zhonguo5118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://un.zhonguo3118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://kf.zhonguo5118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://ew.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://bb.zhonguo3118.cn

[E16] 数字千分位
来源：https://kv.zhonguo5118.cn

Py:   f"{1234567:,}"
来源：https://uq.zhonguo6118.cn

PHP:  number_format(1234567);
来源：https://wq.zhonguo5118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://ff.zhonguo7118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://qp.zhonguo8118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://oz.zhonguo8118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://cs.zhonguo5118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://gn.zhonguo2118.cn

C#:   1234567.ToString("N0")
来源：https://py.zhonguo4118.cn

[E17] 首字母大写
来源：https://xt.zhonguo1118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://aq.zhonguo7118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://xe.zhonguo2118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://yk.zhonguo8118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://or.zhonguo7118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://ee.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://yq.zhonguo1118.cn

Ruby: s.capitalize
来源：https://dv.zhonguo5118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://qf.zhonguo7118.cn

[E18] 模板占位符替换
来源：https://ro.zhonguo1118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://jq.zhonguo2118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://pj.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://mb.zhonguo4118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://ix.zhonguo5118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://pr.zhonguo3118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://tj.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://uf.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://yg.zhonguo2118.cn

[E19] 多行文本按行拆分
来源：https://no.zhonguo3118.cn

Py:   s.splitlines()
来源：https://qg.zhonguo3118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://vc.zhonguo1118.cn

JS:   s.split(/\r?\n/)
来源：https://se.zhonguo8118.cn

TS:   s.split(/\r?\n/)
来源：https://hj.zhonguo2118.cn

Java: s.lines().toList()
来源：https://co.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://hs.zhonguo1118.cn

Ruby: s.lines
来源：https://ba.zhonguo6118.cn

C#:   s.Split('\n')
来源：https://qi.zhonguo6118.cn

[E20] 判断字符串是否为空
来源：https://xo.zhonguo8118.cn

Py:   if not s:
来源：https://ni.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://nz.zhonguo4118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://qu.zhonguo2118.cn

TS:   if (s === "") {}
来源：https://aq.zhonguo3118.cn

Java: if (s.isEmpty()) {}
来源：https://cm.zhonguo4118.cn

Go:   if s == "" {}
来源：https://rr.zhonguo7118.cn

Ruby: if s.empty?
来源：https://id.zhonguo3118.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：https://og.zhonguo4118.cn

[E21] 超长截断加省略号
来源：https://rz.zhonguo5118.cn


<!-- 参考信息 -->