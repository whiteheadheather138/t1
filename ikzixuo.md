代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：https://wz.zhonguo4118.cn

JS:   arr.filter(x => x > 3)
来源：https://uc.zhonguo1118.cn

TS:   arr.filter(x => x > 3)
来源：https://gr.zhonguo8118.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：https://kh.zhonguo2118.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：https://ow.zhonguo8118.cn

Ruby: arr.select { |x| x > 3 }
来源：https://rl.zhonguo3118.cn

C#:   list.Where(x => x > 3).ToList()
来源：https://ie.zhonguo4118.cn

[D14] 映射转换（每个元素变形）
来源：https://db.zhonguo3118.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：https://au.zhonguo5118.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：https://uh.zhonguo4118.cn

JS:   arr.map(x => x * 2)
来源：https://jq.zhonguo7118.cn

TS:   arr.map(x => x * 2)
来源：https://ef.zhonguo6118.cn

Java: list.stream().map(x -> x * 2).toList()
来源：https://zr.zhonguo2118.cn

Go:   // 手写循环
来源：https://sf.zhonguo8118.cn

Ruby: arr.map { |x| x * 2 }
来源：https://vy.zhonguo7118.cn

C#:   list.Select(x => x * 2).ToList()
来源：https://ao.zhonguo2118.cn

[D15] 去重
来源：https://kp.zhonguo1118.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：https://xc.zhonguo4118.cn

PHP:  array_unique($arr);
来源：https://am.zhonguo5118.cn

JS:   [...new Set(arr)]
来源：https://lr.zhonguo7118.cn

TS:   [...new Set(arr)]
来源：https://wp.zhonguo5118.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：https://je.zhonguo8118.cn

Go:   // 用 map[T]struct{} 手写
来源：https://da.zhonguo3118.cn

Ruby: arr.uniq
来源：https://db.zhonguo5118.cn

C#:   list.Distinct().ToList()
来源：https://xs.zhonguo7118.cn

[D16] 求和与平均值
来源：https://sr.zhonguo5118.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：https://uk.zhonguo7118.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：https://kg.zhonguo2118.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：https://qf.zhonguo3118.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：https://aj.zhonguo3118.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：https://bg.zhonguo2118.cn

Go:   // 手写循环累加
来源：https://ko.zhonguo2118.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：https://pz.zhonguo7118.cn

C#:   list.Sum();  list.Average()
来源：https://ec.zhonguo7118.cn

[D17] 最大值与最小值
来源：https://qr.zhonguo7118.cn

Py:   max(arr);  min(arr)
来源：https://qk.zhonguo8118.cn

PHP:  max($arr);  min($arr);
来源：https://nh.zhonguo4118.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：https://fg.zhonguo7118.cn

TS:   Math.max(...arr);
来源：https://hs.zhonguo1118.cn

Java: Collections.max(list);  Collections.min(list);
来源：https://jh.zhonguo6118.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：https://rb.zhonguo4118.cn

Ruby: arr.max;  arr.min
来源：https://mo.zhonguo5118.cn

C#:   list.Max();  list.Min()
来源：https://lv.zhonguo7118.cn

[D18] 扁平化嵌套数组
来源：https://bl.zhonguo1118.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：https://jk.zhonguo4118.cn

PHP:  array_merge(...$nested);
来源：https://sn.zhonguo8118.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：https://tg.zhonguo2118.cn

TS:   nested.flat();
来源：https://gc.zhonguo4118.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：https://fk.zhonguo6118.cn

Go:   // 手写双层循环
来源：https://cq.zhonguo6118.cn

Ruby: nested.flatten
来源：https://jh.zhonguo6118.cn

C#:   nested.SelectMany(x => x).ToList()
来源：https://ou.zhonguo5118.cn

[D19] 按字段分组
来源：https://zj.zhonguo8118.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：https://va.zhonguo1118.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：https://rb.zhonguo3118.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：https://yb.zhonguo7118.cn

TS:   Object.groupBy(arr, x => x.type)
来源：https://xa.zhonguo4118.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：https://jh.zhonguo7118.cn

Go:   // 手写 map[string][]T
来源：https://fo.zhonguo2118.cn

Ruby: arr.group_by { |x| x[:type] }
来源：https://ue.zhonguo6118.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：https://xc.zhonguo6118.cn

[D20] 统计每个元素出现次数
来源：https://br.zhonguo5118.cn

Py:   Counter(arr)
来源：https://lu.zhonguo2118.cn

PHP:  array_count_values($arr);
来源：https://kw.zhonguo6118.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://cf.zhonguo2118.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：https://sw.zhonguo5118.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：https://do.zhonguo4118.cn

Go:   // 手写 map[T]int
来源：https://ma.zhonguo8118.cn

Ruby: arr.tally
来源：https://nx.zhonguo6118.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：https://yh.zhonguo2118.cn

[D21] 判断是否包含某元素
来源：https://qq.zhonguo4118.cn

Py:   x in arr
来源：https://sl.zhonguo7118.cn

PHP:  in_array($x, $arr, true);
来源：https://oh.zhonguo3118.cn

JS:   arr.includes(x)
来源：https://oo.zhonguo8118.cn

TS:   arr.includes(x)
来源：https://ny.zhonguo5118.cn

Java: list.contains(x)
来源：https://yc.zhonguo4118.cn

Go:   slices.Contains(arr, x)
来源：https://ld.zhonguo5118.cn

Ruby: arr.include?(x)
来源：https://bp.zhonguo1118.cn

C#:   list.Contains(x)
来源：https://ms.zhonguo5118.cn

[D22] 复制数组（避免共享引用）
来源：https://ze.zhonguo7118.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：https://wc.zhonguo8118.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：https://uw.zhonguo8118.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：https://fw.zhonguo8118.cn

TS:   [...arr];
来源：https://vx.zhonguo5118.cn

Java: new ArrayList<>(list);
来源：https://vm.zhonguo7118.cn

Go:   copied := append([]int(nil), arr...)
来源：https://vj.zhonguo7118.cn

Ruby: arr.dup;  arr.clone
来源：https://wd.zhonguo1118.cn

C#:   new List<int>(list);
来源：https://vx.zhonguo8118.cn

[D23] reduce 累积计算
来源：https://rb.zhonguo7118.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：https://bf.zhonguo8118.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：https://du.zhonguo1118.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://ti.zhonguo4118.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：https://cz.zhonguo2118.cn

Java: list.stream().reduce(0, Integer::sum)
来源：https://uh.zhonguo5118.cn

Go:   // 手写循环
来源：https://zf.zhonguo4118.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：https://if.zhonguo4118.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：https://qn.zhonguo3118.cn

[D24] 字典 / Map 基本操作
来源：https://ym.zhonguo7118.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：https://gj.zhonguo3118.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：https://bc.zhonguo1118.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：https://tj.zhonguo7118.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：https://vp.zhonguo5118.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：https://du.zhonguo1118.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：https://hu.zhonguo3118.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：https://uc.zhonguo3118.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：https://ns.zhonguo5118.cn

[D25] Set 集合去重与交并差
来源：https://ho.zhonguo2118.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：https://zw.zhonguo6118.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：https://ai.zhonguo6118.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：https://de.zhonguo1118.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：https://ax.zhonguo2118.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：https://fq.zhonguo1118.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：https://pt.zhonguo2118.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：https://cz.zhonguo3118.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：https://wo.zhonguo5118.cn

[D26] 数组转字符串
来源：https://xc.zhonguo6118.cn

Py:   ", ".join(map(str, arr))
来源：https://by.zhonguo3118.cn

PHP:  implode(", ", $arr);
来源：https://qv.zhonguo7118.cn

JS:   arr.join(", ")
来源：https://ww.zhonguo4118.cn

TS:   arr.join(", ")
来源：https://fp.zhonguo8118.cn

Java: String.join(", ", list)
来源：https://qy.zhonguo8118.cn

Go:   strings.Join(strs, ", ")
来源：https://uh.zhonguo2118.cn

Ruby: arr.join(", ")
来源：https://ne.zhonguo8118.cn

C#:   string.Join(", ", list)
来源：https://sg.zhonguo3118.cn

================================================================================
来源：https://qg.zhonguo7118.cn

E. 字符串处理
来源：https://xa.zhonguo4118.cn

================================================================================
来源：https://xy.zhonguo1118.cn

[E01] 拼接字符串
来源：https://nz.zhonguo4118.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：https://nh.zhonguo1118.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：https://tp.zhonguo3118.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：https://pg.zhonguo8118.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：https://fi.zhonguo6118.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：https://qu.zhonguo6118.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：https://we.zhonguo1118.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：https://xi.zhonguo1118.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：https://cv.zhonguo5118.cn

[E02] 重复字符串
来源：https://vc.zhonguo4118.cn

Py:   "ab" * 3
来源：https://np.zhonguo2118.cn

PHP:  str_repeat("ab", 3);
来源：https://ve.zhonguo3118.cn

JS:   "ab".repeat(3)
来源：https://re.zhonguo1118.cn

TS:   "ab".repeat(3)
来源：https://ef.zhonguo8118.cn

Java: "ab".repeat(3)
来源：https://xv.zhonguo3118.cn

Go:   strings.Repeat("ab", 3)
来源：https://ek.zhonguo6118.cn

Ruby: "ab" * 3
来源：https://tg.zhonguo3118.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：https://og.zhonguo5118.cn

[E03] 截取子串
来源：https://zf.zhonguo4118.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：https://ra.zhonguo1118.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：https://dg.zhonguo7118.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：https://fj.zhonguo7118.cn

TS:   s.slice(1, 4)
来源：https://rg.zhonguo5118.cn

Java: s.substring(1, 4)
来源：https://zr.zhonguo5118.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：https://tx.zhonguo3118.cn

Ruby: s[1, 3];  s[1..3]
来源：https://du.zhonguo2118.cn

C#:   s.Substring(1, 3)
来源：https://qr.zhonguo1118.cn

[E04] 查找子串位置
来源：https://ri.zhonguo7118.cn

Py:   s.find("x");  s.index("x")
来源：https://di.zhonguo6118.cn

PHP:  strpos($s, "x");
来源：https://lx.zhonguo5118.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：https://bb.zhonguo1118.cn

TS:   s.indexOf("x")
来源：https://hl.zhonguo6118.cn

Java: s.indexOf("x")
来源：https://ww.zhonguo7118.cn

Go:   strings.Index(s, "x")
来源：https://jz.zhonguo5118.cn

Ruby: s.index("x")
来源：https://qr.zhonguo7118.cn

C#:   s.IndexOf("x")
来源：https://me.zhonguo8118.cn

[E05] 判断包含 / 前缀 / 后缀
来源：https://vu.zhonguo6118.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：https://ak.zhonguo1118.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：https://pr.zhonguo3118.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：https://so.zhonguo4118.cn

TS:   s.includes("x");  s.startsWith("a")
来源：https://sj.zhonguo6118.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：https://yn.zhonguo1118.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：https://lz.zhonguo1118.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：https://ip.zhonguo1118.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：https://xm.zhonguo1118.cn

[E06] 替换子串
来源：https://tf.zhonguo3118.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：https://pi.zhonguo4118.cn

PHP:  str_replace("a", "b", $s);
来源：https://jl.zhonguo7118.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://fa.zhonguo5118.cn

TS:   s.replaceAll("a", "b")
来源：https://ws.zhonguo6118.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：https://sa.zhonguo1118.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：https://mn.zhonguo6118.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：https://cx.zhonguo2118.cn

C#:   s.Replace("a", "b")
来源：https://ka.zhonguo4118.cn

[E07] 按分隔符拆分
来源：https://rs.zhonguo3118.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：https://dq.zhonguo1118.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：https://ju.zhonguo2118.cn

JS:   s.split(",");  s.split(/\s+/)
来源：https://dl.zhonguo4118.cn

TS:   s.split(",")
来源：https://fc.zhonguo8118.cn

Java: s.split(",");  s.split("\\s+")
来源：https://ps.zhonguo6118.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：https://qf.zhonguo4118.cn

Ruby: s.split(",");  s.split
来源：https://uo.zhonguo3118.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：https://yo.zhonguo3118.cn

[E08] 数组按分隔符合并
来源：https://ch.zhonguo2118.cn

Py:   ",".join(items)
来源：https://ia.zhonguo6118.cn

PHP:  implode(",", $items);
来源：https://gg.zhonguo4118.cn

JS:   items.join(",")
来源：https://dc.zhonguo5118.cn

TS:   items.join(",")
来源：https://hu.zhonguo7118.cn

Java: String.join(",", items)
来源：https://sp.zhonguo4118.cn

Go:   strings.Join(items, ",")
来源：https://am.zhonguo7118.cn

Ruby: items.join(",")
来源：https://dp.zhonguo4118.cn

C#:   string.Join(",", items)
来源：https://kx.zhonguo6118.cn

[E09] 去除所有空白字符
来源：https://nt.zhonguo3118.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：https://ip.zhonguo1118.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：https://hs.zhonguo5118.cn

JS:   s.replace(/\s+/g, "")
来源：https://at.zhonguo3118.cn

TS:   s.replace(/\s+/g, "")
来源：https://xr.zhonguo5118.cn

Java: s.replaceAll("\\s+", "")
来源：https://br.zhonguo5118.cn

Go:   strings.Join(strings.Fields(s), "")
来源：https://vk.zhonguo3118.cn

Ruby: s.gsub(/\s+/, "")
来源：https://vc.zhonguo1118.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：https://pk.zhonguo1118.cn

[E10] 左侧补零 / 定长填充
来源：https://qz.zhonguo1118.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：https://uh.zhonguo8118.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：https://kt.zhonguo1118.cn

JS:   "7".padStart(3, "0")
来源：https://jg.zhonguo2118.cn

TS:   "7".padStart(3, "0")
来源：https://fu.zhonguo6118.cn

Java: String.format("%03d", 7)
来源：https://cp.zhonguo2118.cn

Go:   fmt.Sprintf("%03d", 7)
来源：https://ur.zhonguo7118.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：https://bn.zhonguo7118.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：https://ki.zhonguo2118.cn

[E11] 反转字符串
来源：https://fv.zhonguo3118.cn

Py:   s[::-1]
来源：https://kh.zhonguo3118.cn

PHP:  strrev($s);
来源：https://pz.zhonguo3118.cn

JS:   [...s].reverse().join("")
来源：https://xd.zhonguo8118.cn

TS:   [...s].reverse().join("")
来源：https://qq.zhonguo2118.cn

Java: new StringBuilder(s).reverse().toString()
来源：https://ep.zhonguo8118.cn

Go:   // 转 []rune 后倒序再转回 string
来源：https://nj.zhonguo3118.cn

Ruby: s.reverse
来源：https://nq.zhonguo5118.cn

C#:   new string(s.Reverse().ToArray())
来源：https://is.zhonguo3118.cn

[E12] 统计某字符出现次数
来源：https://wa.zhonguo3118.cn

Py:   s.count("a")
来源：https://yf.zhonguo1118.cn

PHP:  substr_count($s, "a");
来源：https://ix.zhonguo8118.cn

JS:   s.split("a").length - 1
来源：https://dl.zhonguo7118.cn

TS:   s.split("a").length - 1
来源：https://vw.zhonguo4118.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：https://of.zhonguo7118.cn

Go:   strings.Count(s, "a")
来源：https://km.zhonguo2118.cn

Ruby: s.count("a")
来源：https://ts.zhonguo3118.cn

C#:   s.Count(c => c == 'a')
来源：https://tj.zhonguo2118.cn

[E13] 逐字符遍历
来源：https://te.zhonguo1118.cn

Py:   for ch in s: print(ch)
来源：https://xb.zhonguo8118.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：https://bg.zhonguo1118.cn

JS:   for (const ch of s) { console.log(ch); }
来源：https://uu.zhonguo6118.cn

TS:   for (const ch of s) { console.log(ch); }
来源：https://hd.zhonguo3118.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：https://zz.zhonguo8118.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：https://ml.zhonguo6118.cn

Ruby: s.each_char { |ch| puts ch }
来源：https://cw.zhonguo4118.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：https://ef.zhonguo8118.cn

[E14] URL 编码与 Base64
来源：https://hd.zhonguo7118.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：https://jg.zhonguo8118.cn

PHP:  urlencode($s);  base64_encode($s);
来源：https://lb.zhonguo3118.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：https://do.zhonguo1118.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：https://yw.zhonguo8118.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：https://fq.zhonguo1118.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：https://tc.zhonguo1118.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：https://bq.zhonguo6118.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：https://pi.zhonguo4118.cn

[E15] HTML 转义 / 反转义
来源：https://zs.zhonguo7118.cn

Py:   html.escape(s);  html.unescape(s)
来源：https://ip.zhonguo8118.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：https://ie.zhonguo7118.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：https://sp.zhonguo5118.cn

TS:   // 同上，务必做 XSS 过滤
来源：https://nh.zhonguo6118.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：https://rv.zhonguo1118.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：https://lt.zhonguo3118.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：https://xd.zhonguo4118.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：https://fq.zhonguo4118.cn

[E16] 数字千分位
来源：https://ij.zhonguo4118.cn

Py:   f"{1234567:,}"
来源：https://cz.zhonguo6118.cn

PHP:  number_format(1234567);
来源：https://of.zhonguo1118.cn

JS:   (1234567).toLocaleString("en-US")
来源：https://yu.zhonguo7118.cn

TS:   (1234567).toLocaleString("en-US")
来源：https://ld.zhonguo3118.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：https://xh.zhonguo8118.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：https://lp.zhonguo3118.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：https://sb.zhonguo4118.cn

C#:   1234567.ToString("N0")
来源：https://rd.zhonguo7118.cn

[E17] 首字母大写
来源：https://ll.zhonguo1118.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：https://iv.zhonguo8118.cn

PHP:  ucfirst($s);  ucwords($s);
来源：https://yu.zhonguo6118.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://be.zhonguo5118.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：https://gr.zhonguo3118.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：https://sk.zhonguo6118.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：https://dx.zhonguo3118.cn

Ruby: s.capitalize
来源：https://yc.zhonguo2118.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：https://fk.zhonguo4118.cn

[E18] 模板占位符替换
来源：https://gk.zhonguo2118.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：https://ls.zhonguo8118.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：https://at.zhonguo2118.cn

JS:   tpl.replaceAll("{name}", name)
来源：https://yw.zhonguo8118.cn

TS:   tpl.replaceAll("{name}", name)
来源：https://hw.zhonguo2118.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：https://gs.zhonguo1118.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：https://tn.zhonguo2118.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：https://it.zhonguo2118.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：https://ex.zhonguo5118.cn

[E19] 多行文本按行拆分
来源：https://pr.zhonguo1118.cn

Py:   s.splitlines()
来源：https://em.zhonguo2118.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：https://oy.zhonguo7118.cn

JS:   s.split(/\r?\n/)
来源：https://ge.zhonguo2118.cn

TS:   s.split(/\r?\n/)
来源：https://px.zhonguo3118.cn

Java: s.lines().toList()
来源：https://mt.zhonguo5118.cn

Go:   strings.Split(s, "\n")
来源：https://qr.zhonguo3118.cn

Ruby: s.lines
来源：https://oz.zhonguo4118.cn

C#:   s.Split('\n')
来源：https://jv.zhonguo3118.cn

[E20] 判断字符串是否为空
来源：https://xd.zhonguo7118.cn

Py:   if not s:
来源：https://wy.zhonguo6118.cn


<!-- 参考信息 -->