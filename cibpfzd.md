代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://ga.zhonguo7118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://ky.zhonguo7118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ox.zhonguo2118.cn

[D14] 映射转换（每个元素变形）
来源：https://ps.zhonguo5118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://oh.zhonguo6118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://fa.zhonguo7118.cn

JS:   arr.map(x => x * 2)
来源：https://tb.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://st.zhonguo2118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://rh.zhonguo1118.cn

Go:   // 手写循环
来源：https://dt.zhonguo1118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://ya.zhonguo1118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://ls.zhonguo7118.cn

[D15] 去重
来源：https://an.zhonguo4118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://ww.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://cy.zhonguo1118.cn

JS:   [...new Set(arr)]
来源：https://hq.zhonguo8118.cn

TS:   [...new Set(arr)]
来源：https://tm.zhonguo5118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://ua.zhonguo2118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://df.zhonguo7118.cn

Ruby: arr.uniq
来源：https://ue.zhonguo7118.cn

C#:   list.Distinct().ToList()
来源：https://yz.zhonguo8118.cn

[D16] 求和与平均值
来源：https://kf.zhonguo1118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://qb.zhonguo6118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://li.zhonguo7118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://lg.zhonguo6118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://iu.zhonguo4118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://pt.zhonguo3118.cn

Go:   // 手写循环累加
来源：https://xb.zhonguo6118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://ya.zhonguo1118.cn

C#:   list.Sum();  list.Average()
来源：https://af.zhonguo2118.cn

[D17] 最大值与最小值
来源：https://pg.zhonguo5118.cn

Py:   max(arr);  min(arr)
来源：https://mw.zhonguo8118.cn

PHP:  max($arr);  min($arr);
来源：https://fs.zhonguo1118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://kq.zhonguo8118.cn

TS:   Math.max(...arr);
来源：https://gx.zhonguo6118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://ks.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://ba.zhonguo2118.cn

Ruby: arr.max;  arr.min
来源：https://nh.zhonguo5118.cn

C#:   list.Max();  list.Min()
来源：https://gp.zhonguo8118.cn

[D18] 扁平化嵌套数组
来源：https://uo.zhonguo5118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://vd.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://uv.zhonguo1118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://fz.zhonguo2118.cn

TS:   nested.flat();
来源：https://qg.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://sv.zhonguo3118.cn

Go:   // 手写双层循环
来源：https://zp.zhonguo4118.cn

Ruby: nested.flatten
来源：https://ym.zhonguo7118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://pd.zhonguo7118.cn

[D19] 按字段分组
来源：https://tl.zhonguo6118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://mi.zhonguo7118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://kz.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://ux.zhonguo4118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://ve.zhonguo2118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://rb.zhonguo5118.cn

Go:   // 手写 map[string][]T
来源：https://yg.zhonguo7118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://wu.zhonguo2118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://vu.zhonguo1118.cn

[D20] 统计每个元素出现次数
来源：https://to.zhonguo2118.cn

Py:   Counter(arr)
来源：https://pv.zhonguo8118.cn

PHP:  array_count_values($arr);
来源：https://vx.zhonguo7118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://ii.zhonguo4118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://yb.zhonguo8118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://vi.zhonguo7118.cn

Go:   // 手写 map[T]int
来源：https://ar.zhonguo3118.cn

Ruby: arr.tally
来源：https://hz.zhonguo2118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://hs.zhonguo6118.cn

[D21] 判断是否包含某元素
来源：https://zk.zhonguo8118.cn

Py:   x in arr
来源：https://kc.zhonguo6118.cn

PHP:  in_array($x, $arr, true);
来源：https://qv.zhonguo5118.cn

JS:   arr.includes(x)
来源：https://gh.zhonguo1118.cn

TS:   arr.includes(x)
来源：https://oc.zhonguo2118.cn

Java: list.contains(x)
来源：https://ry.zhonguo8118.cn

Go:   slices.Contains(arr, x)
来源：https://lp.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://qs.zhonguo3118.cn

C#:   list.Contains(x)
来源：https://nr.zhonguo3118.cn

[D22] 复制数组（避免共享引用）
来源：https://ug.zhonguo6118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://nh.zhonguo5118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://rx.zhonguo4118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://ax.zhonguo1118.cn

TS:   [...arr];
来源：https://ls.zhonguo2118.cn

Java: new ArrayList<>(list);
来源：https://dg.zhonguo2118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://or.zhonguo1118.cn

Ruby: arr.dup;  arr.clone
来源：https://ty.zhonguo8118.cn

C#:   new List<int>(list);
来源：https://bx.zhonguo5118.cn

[D23] reduce 累积计算
来源：https://as.zhonguo8118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://id.zhonguo5118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://ik.zhonguo4118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://it.zhonguo7118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ow.zhonguo6118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://me.zhonguo1118.cn

Go:   // 手写循环
来源：https://lj.zhonguo6118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://uu.zhonguo8118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://gq.zhonguo8118.cn

[D24] 字典 / Map 基本操作
来源：https://qn.zhonguo4118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://md.zhonguo2118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://xe.zhonguo1118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://qh.zhonguo7118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://kw.zhonguo8118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://bp.zhonguo4118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://uh.zhonguo8118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://gy.zhonguo7118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://gp.zhonguo7118.cn

[D25] Set 集合去重与交并差
来源：https://cj.zhonguo1118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://qw.zhonguo3118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://nd.zhonguo2118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://yz.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ku.zhonguo1118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://im.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://hy.zhonguo5118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://fo.zhonguo4118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://dc.zhonguo2118.cn

[D26] 数组转字符串
来源：https://za.zhonguo5118.cn

Py:   ", ".join(map(str, arr))
来源：https://oo.zhonguo2118.cn

PHP:  implode(", ", $arr);
来源：https://fy.zhonguo5118.cn

JS:   arr.join(", ")
来源：https://oc.zhonguo8118.cn

TS:   arr.join(", ")
来源：https://un.zhonguo3118.cn

Java: String.join(", ", list)
来源：https://ko.zhonguo3118.cn

Go:   strings.Join(strs, ", ")
来源：https://vm.zhonguo4118.cn

Ruby: arr.join(", ")
来源：https://hq.zhonguo7118.cn

C#:   string.Join(", ", list)
来源：https://gu.zhonguo7118.cn

================================================================================
来源：https://cz.zhonguo4118.cn

E. 字符串处理
来源：https://ue.zhonguo3118.cn

================================================================================
来源：https://py.zhonguo8118.cn

[E01] 拼接字符串
来源：https://vr.zhonguo3118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://ut.zhonguo7118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://zy.zhonguo2118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://ux.zhonguo3118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://xc.zhonguo1118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://wp.zhonguo4118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://sc.zhonguo6118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://kb.zhonguo8118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://mc.zhonguo8118.cn

[E02] 重复字符串
来源：https://en.zhonguo2118.cn

Py:   "ab" * 3
来源：https://xd.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://pa.zhonguo6118.cn

JS:   "ab".repeat(3)
来源：https://pl.zhonguo7118.cn

TS:   "ab".repeat(3)
来源：https://xe.zhonguo3118.cn

Java: "ab".repeat(3)
来源：https://ou.zhonguo5118.cn

Go:   strings.Repeat("ab", 3)
来源：https://vw.zhonguo8118.cn

Ruby: "ab" * 3
来源：https://cl.zhonguo5118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://no.zhonguo6118.cn

[E03] 截取子串
来源：https://yg.zhonguo8118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://fp.zhonguo7118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://ud.zhonguo7118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://wa.zhonguo6118.cn

TS:   s.slice(1, 4)
来源：https://dk.zhonguo8118.cn

Java: s.substring(1, 4)
来源：https://rq.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://rl.zhonguo5118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://ko.zhonguo3118.cn

C#:   s.Substring(1, 3)
来源：https://la.zhonguo5118.cn

[E04] 查找子串位置
来源：https://es.zhonguo4118.cn

Py:   s.find("x");  s.index("x")
来源：https://da.zhonguo8118.cn

PHP:  strpos($s, "x");
来源：https://pz.zhonguo8118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://kc.zhonguo7118.cn

TS:   s.indexOf("x")
来源：https://iq.zhonguo5118.cn

Java: s.indexOf("x")
来源：https://lx.zhonguo3118.cn

Go:   strings.Index(s, "x")
来源：https://tj.zhonguo6118.cn

Ruby: s.index("x")
来源：https://dg.zhonguo6118.cn

C#:   s.IndexOf("x")
来源：https://kd.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://rk.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://gj.zhonguo1118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://lh.zhonguo4118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ct.zhonguo4118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://pa.zhonguo6118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://ey.zhonguo4118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://jb.zhonguo7118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://bh.zhonguo2118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://wn.zhonguo3118.cn

[E06] 替换子串
来源：https://nb.zhonguo7118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://cf.zhonguo5118.cn

PHP:  str_replace("a", "b", $s);
来源：https://le.zhonguo2118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://tr.zhonguo2118.cn

TS:   s.replaceAll("a", "b")
来源：https://us.zhonguo2118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://sh.zhonguo8118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://ga.zhonguo5118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://hl.zhonguo7118.cn

C#:   s.Replace("a", "b")
来源：https://fa.zhonguo1118.cn

[E07] 按分隔符拆分
来源：https://yn.zhonguo4118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://gt.zhonguo2118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://gk.zhonguo4118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://uo.zhonguo5118.cn

TS:   s.split(",")
来源：https://qp.zhonguo5118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ix.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://yd.zhonguo2118.cn

Ruby: s.split(",");  s.split
来源：https://jn.zhonguo4118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://wq.zhonguo5118.cn

[E08] 数组按分隔符合并
来源：https://ma.zhonguo2118.cn

Py:   ",".join(items)
来源：https://eq.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://fr.zhonguo2118.cn

JS:   items.join(",")
来源：https://re.zhonguo7118.cn

TS:   items.join(",")
来源：https://or.zhonguo2118.cn

Java: String.join(",", items)
来源：https://qv.zhonguo1118.cn

Go:   strings.Join(items, ",")
来源：https://oa.zhonguo2118.cn

Ruby: items.join(",")
来源：https://zu.zhonguo4118.cn

C#:   string.Join(",", items)
来源：https://au.zhonguo8118.cn

[E09] 去除所有空白字符
来源：https://hf.zhonguo6118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://hd.zhonguo1118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://ya.zhonguo7118.cn

JS:   s.replace(/\s+/g, "")
来源：https://mw.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://rm.zhonguo1118.cn

Java: s.replaceAll("\\s+", "")
来源：https://rv.zhonguo3118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://lc.zhonguo6118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://rs.zhonguo7118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://nu.zhonguo3118.cn

[E10] 左侧补零 / 定长填充
来源：https://mn.zhonguo3118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://gu.zhonguo3118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://lw.zhonguo7118.cn

JS:   "7".padStart(3, "0")
来源：https://sf.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://qg.zhonguo8118.cn

Java: String.format("%03d", 7)
来源：https://yk.zhonguo8118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://iv.zhonguo6118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://ty.zhonguo1118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://pv.zhonguo5118.cn

[E11] 反转字符串
来源：https://gc.zhonguo2118.cn

Py:   s[::-1]
来源：https://hj.zhonguo6118.cn

PHP:  strrev($s);
来源：https://ew.zhonguo6118.cn

JS:   [...s].reverse().join("")
来源：https://tn.zhonguo5118.cn

TS:   [...s].reverse().join("")
来源：https://fd.zhonguo4118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://dl.zhonguo3118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://wi.zhonguo4118.cn

Ruby: s.reverse
来源：https://rn.zhonguo6118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://ju.zhonguo8118.cn

[E12] 统计某字符出现次数
来源：https://ym.zhonguo5118.cn

Py:   s.count("a")
来源：https://dp.zhonguo6118.cn

PHP:  substr_count($s, "a");
来源：https://xw.zhonguo3118.cn

JS:   s.split("a").length - 1
来源：https://oj.zhonguo3118.cn

TS:   s.split("a").length - 1
来源：https://kl.zhonguo4118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://aj.zhonguo6118.cn

Go:   strings.Count(s, "a")
来源：https://nr.zhonguo4118.cn

Ruby: s.count("a")
来源：https://wx.zhonguo8118.cn

C#:   s.Count(c => c == 'a')
来源：https://os.zhonguo8118.cn

[E13] 逐字符遍历
来源：https://pn.zhonguo7118.cn

Py:   for ch in s: print(ch)
来源：https://ei.zhonguo6118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://gw.zhonguo2118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://gr.zhonguo1118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://sf.zhonguo6118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://sm.zhonguo4118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ai.zhonguo5118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://fd.zhonguo7118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://nr.zhonguo3118.cn

[E14] URL 编码与 Base64
来源：https://nx.zhonguo6118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://cx.zhonguo6118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://ul.zhonguo4118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://re.zhonguo4118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://md.zhonguo4118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://nq.zhonguo4118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://gy.zhonguo8118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://zp.zhonguo1118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://wb.zhonguo1118.cn

[E15] HTML 转义 / 反转义
来源：https://ai.zhonguo1118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://gr.zhonguo4118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://cr.zhonguo2118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://jg.zhonguo3118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://cc.zhonguo2118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://bp.zhonguo7118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://wt.zhonguo3118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://rd.zhonguo3118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://hy.zhonguo4118.cn

[E16] 数字千分位
来源：https://zq.zhonguo5118.cn

Py:   f"{1234567:,}"
来源：https://fo.zhonguo1118.cn

PHP:  number_format(1234567);
来源：https://xx.zhonguo7118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://to.zhonguo6118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://ni.zhonguo4118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://un.zhonguo3118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://qt.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://hf.zhonguo6118.cn

C#:   1234567.ToString("N0")
来源：https://so.zhonguo8118.cn

[E17] 首字母大写
来源：https://cz.zhonguo4118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://ct.zhonguo5118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://ar.zhonguo1118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://uw.zhonguo3118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://ut.zhonguo4118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://qr.zhonguo3118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://xx.zhonguo8118.cn

Ruby: s.capitalize
来源：https://rz.zhonguo4118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://uh.zhonguo1118.cn

[E18] 模板占位符替换
来源：https://ry.zhonguo8118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://rq.zhonguo8118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://ry.zhonguo8118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://qh.zhonguo6118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://lt.zhonguo1118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://ob.zhonguo4118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://rm.zhonguo4118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://md.zhonguo3118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://um.zhonguo1118.cn

[E19] 多行文本按行拆分
来源：https://ah.zhonguo3118.cn

Py:   s.splitlines()
来源：https://eo.zhonguo7118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://gh.zhonguo5118.cn

JS:   s.split(/\r?\n/)
来源：https://aj.zhonguo5118.cn

TS:   s.split(/\r?\n/)
来源：https://mf.zhonguo5118.cn

Java: s.lines().toList()
来源：https://yi.zhonguo8118.cn

Go:   strings.Split(s, "\n")
来源：https://aa.zhonguo5118.cn

Ruby: s.lines
来源：https://tg.zhonguo2118.cn

C#:   s.Split('\n')
来源：https://al.zhonguo5118.cn

[E20] 判断字符串是否为空
来源：https://ku.zhonguo3118.cn

Py:   if not s:
来源：https://sq.zhonguo1118.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：https://jj.zhonguo7118.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：https://zy.zhonguo4118.cn

TS:   if (s === "") {}
来源：https://dc.zhonguo4118.cn

Java: if (s.isEmpty()) {}
来源：https://pk.zhonguo3118.cn


<!-- 参考信息 -->