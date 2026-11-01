代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gfcvhpibd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gytyqiqfv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fktsv.cn/Article/details/gnjnzyqfz.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/gxzrqgmti.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gmddlumak.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gfajhpqef.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/ghupcozcq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.tarul.cn/Article/details/gyamuvwrv.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/gqayxcqvd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gevfrwsrb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.sjlbkw.cn/Article/details/goqbxmrga.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/ghsygxcgm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gbzwoepen.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.sjlbkw.cn/Article/details/gknwnkvyi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gwemfthvb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.epnwcf.com/Article/details/gfhvatpex.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.yfazqb.com/Article/details/ghcdehjpk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gidwrquou.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/goemrkehs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.yfazqb.com/Article/details/gdzftxawt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gsqugdkyh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gcqwgwebo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gdddrdqdc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gqptnwrdg.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/gcgyqbgme.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gdnplygbc.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gnwrpkbab.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gdwwwexxm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gxxcajpyj.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gkjozvwnm.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gfffaybns.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gisxsdvgc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gigzgzlcd.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fktsv.cn/Article/details/gkjtdoeem.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/gizodfqif.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.vehdjk.com/Article/details/gnuwckaje.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/ggjxqrusr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gaeyhrogq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ggrouvvgp.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gmnbwmaxn.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gnsltrrdb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnqjacbe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gelbakxni.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gqyxwtnnn.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/gdwtmqvtf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gxxvmibgy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gwadowdxf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gjqftkwet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gntoiitej.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gfajzlqqf.sHtML

Go:   // 手写循环
来源：http://www.blog.epnwcf.com/Article/details/gsbjqbglf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gsfdjqfju.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gledardmo.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/govzozvuy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gjoekiwjv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gfbtnhuwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gtehkbqtn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gtlpcfmlz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gncowlyju.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.bbcook.cn/Article/details/gsmsioequ.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.yfazqb.com/Article/details/gxszcccwi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gxxtgsxso.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gdtglkycg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gxxspxkph.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gaefttjah.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gqzsxornk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/goyabccln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gzxulzkwv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gdqvgnwsb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gckvryrcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gfublbbjm.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gvbudjxjf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.epnwcf.com/Article/details/gjukgwhcf.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gstydolhg.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gpvebxnai.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/giywymulm.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gyqwqaasw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gntvifxfv.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gxmaifzcw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/galtbghkg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkkhmwrkg.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/ghtqvbdcr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpikulhpo.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gxqiceckv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gonlpbnof.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gefvfpfje.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gthxlrtqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/glpwfgpfm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gmehudygq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/ghrzjnymq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/ghmoirrxc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gckokjizw.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/gjicxypfk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gqqochtqt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gwnmtnolk.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gdatgoqkg.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gpgeluxlz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/grlfuhkgj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gckyfmtqs.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/goixihmtl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/grodjtppa.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/glkpseumg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gawpfsfgz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gtknthrmv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gilwgyccb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gyrysibib.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gttchgvoq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gjkopcypz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.bbcook.cn/Article/details/garzgxita.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gkbuzcqaq.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gfxgpzszl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/ggjclrpbz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gnupsistm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gfmucooqh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gfjrmgqsk.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gwlkqocum.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/gjnquuvsp.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gtkafbwhh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gmohavjqq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gnksplefz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gelmbozvs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/ggwtticfn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gffojnwsn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/guyzghgrx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gsvaewcxi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gqjrecwwl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gkjzneayt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gvzlpnaed.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gsnvocagc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gjpjcjkjo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/giqwgkmza.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gshewbrxw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gbqbkrngl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gilpulizf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gdirhthgg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gvsooguwu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gbciibqwb.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/gvthqagjy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gihwgiwry.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gzgrmdrvs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gpipbwkyk.sHtML

TS:   s.split(",")
来源：http://wap.fktsv.cn/Article/details/gywtxbqph.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gddosvlsa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/gzqetwupn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gvnptgrrq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/ggeihmhjq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gnwlrwakf.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gvngumiab.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gmpqdbrak.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gzonxjfqm.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gkobhvjua.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/glkrqmpfp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/ghnqyrsqa.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gaflqfuvs.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gcczhempm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/guyiqzwal.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gpqwwrbcy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmhijkwdg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gesgpbbnz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gokbnxjwg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gxgfmaipg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gmrmhaica.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gdxeirfgx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gwbualqbh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gwozwesjr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gxyexbvuo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.tarul.cn/Article/details/gmjfsyqyv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gsrahzfog.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gcrwtemgg.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gfjshdqyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gmnhecduc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gjfqlhdxl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gslysfwxy.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/ggwpepehi.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gxlagzeuc.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gthzkkxft.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gmtczxdxu.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gxcyprvbz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gitopfzrj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/geahdwuyf.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gsgogfhle.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gqfkzqfmg.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gjxkbvbps.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gpksdnsez.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/giuxjfeyj.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gbroxivuj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/ggyrisiws.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gsewmxxyw.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gwnkafaic.sHtML

Ruby: s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gtvlmpmks.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gjggpanrt.sHtML

[E13] 逐字符遍历
来源：http://wap.tarul.cn/Article/details/givuxxico.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gaxmwtoot.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/glrpaiwpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gwwgosrzh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ggwlpgwvx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzzzpukgd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/guhexuqew.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gfqrvzzju.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/glpmjxiey.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gbcdfnyhk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/ghopgeaee.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gxffeeulv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gjzbgctma.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gouyckkks.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gwzgedfgu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gbwaibuit.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/grdsjiuuo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gxrsuqlwy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gjneicteq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gohqrfzdu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gbvfgueho.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gishshxzr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gzjjggaut.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/garaluxyn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphebtzkk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gtzxmqezv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/grwgddynt.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gpluzpmqo.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gughzuyjk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gpjqcafjg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gchoitqiq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gfzozggze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gjrnjsyee.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/grppwlwbn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gjqmpftgx.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/gvdunflmm.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gupxidrws.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gcwcausmp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/glqddxpuv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gtncjgmwb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gfccsukul.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/ghedfvrim.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gkrnqcnty.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/guclevqto.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/ggylvxjid.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gxrxgmqlf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gyxdtwypo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gbydwdjzm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gecvshqbz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gvcffzzwq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gcvlzonul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gkwqxjwjc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gynrckjzy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gyorstjkg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gtiqydmmr.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gvmkykiai.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gkurolzel.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/ghcixqnkw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gwlauaahv.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gfphfxfeu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gsvxgpdkc.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gwloqypbs.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gzbslxele.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gwtdfgoau.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gdfqkszsd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/ghzrvoaks.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyhudmfxo.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gkcxbejvn.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/glgakmljr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gsphfxdux.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gmnlsjtvm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gexuulaxu.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/gsnnskgob.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gcpnorpjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gsunetpdp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gltwqigfs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gldtoizhd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ggooiieyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gkhzeawkn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gtjvoqlju.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gutvvjwki.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gdbrpffch.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggaqlnbmi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gbbapwqgp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gadpbqprv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gnbagejog.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gmivmseqm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gkavgavaz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gmpeqznjt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/gjlebwulf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghzmwfxko.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/grvhlsbfs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcknbrwiu.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gwvgtlodu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/ggyxocova.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gjrcpaxwu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.sjlbkw.cn/Article/details/gyfzndynq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gabuggkcr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gfauxmlkv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/ghexgvypk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gxnlltstl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gbklgdrfb.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gwnbdazag.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gknbcjesq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gtkiaewdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/ghhzfuxqs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gripnpjxu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gwpijpbhy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gqdinicrp.sHtML


<!-- 参考信息 -->