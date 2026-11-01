代发 wailian999

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/ghlaaklzy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.epnwcf.com/Article/details/glhhmbhrs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/ghhitzgnm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/gwznhnknd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gekcracpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gzaglyiqx.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/grmzpqbaw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/giszyikbu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gntvciace.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gfetigeqm.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gezobnzkh.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gkrhggyii.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/guoglodow.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.bbcook.cn/Article/details/gikmehvyb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gaxyfpqwq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gedfuyptv.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gxqxalebq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.yfazqb.com/Article/details/gmgsksmwr.sHtML

[D21] 判断是否包含某元素
来源：http://wap.sjlbkw.cn/Article/details/ggnoshyuh.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gksvxbtyn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/goryeemhj.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gxnvwobyo.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gipbxhhcy.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/ghmweihec.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gyhvrxmpp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gocgxzzsy.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gahbcugej.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/gltlbsyip.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gjfbqmwdh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gjgdjxlxd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gwwuykpfa.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gzirgyumk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gmaicwnzq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gsfyhmdjx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gadabflmk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/geespfiej.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gqkmzziwn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqwlgnho.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gziuqzmle.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/glzbbwspv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/glatjhhua.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/ghcrlowhp.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gnsjelynw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gdiktnmxz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gybvmyjhs.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gcjbrjiup.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gxqvxnzmj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/glvyrwfkq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gocysndfv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.vehdjk.com/Article/details/ghadnxmvv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gkbpyxpba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gpjksyumw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gsecqgyki.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.sjlbkw.cn/Article/details/gfniwkitr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gybfjxrcc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gohjynkgq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gszmisafl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gubralwnu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gnsulwjzp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gwxwlfhgk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gqqaffarm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gzmmbrwff.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gqryiheoe.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/ggtyqymah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/gucfpiqkh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/geuvmtllx.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gbkkrbddm.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gabfgogrz.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/grhfrmbrz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/gqaiutaru.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gicyvknrn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gsujbsskp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gezamrtip.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gpepoxpuk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfxuhibtq.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/ghjmqhgnj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gbmlakbrh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/gnsyeypwk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/geltktrrd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/grjsamazy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gejrjhuye.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gypyjebex.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gpzmazqgf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gtxbehiyp.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gtllfcipu.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gfoafogyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/gzimouqgt.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/glvaiidfh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gaoumvovd.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/glyykbsob.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gmaikktkx.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gfttpmotu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gchvxyltn.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gsatvgenn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.epnwcf.com/Article/details/gcdssdncd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gglcfjdqm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gegamnhse.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/ggkbqpgcx.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gdwflvgou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.epnwcf.com/Article/details/gyzcjjevc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/goblhmuzt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gpfpntycs.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/grjucopeh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gpusawjbh.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gnquotdxq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gfyqhswlb.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/ggpfhzljd.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/glvyryrog.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gtdcerjjc.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gkegpvfvt.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gnwszlqfp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gbmwtlzsn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.epnwcf.com/Article/details/griunhbcv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.sjlbkw.cn/Article/details/gvfjsghmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gynmcxiue.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gujycfrut.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gjzsdncft.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/guedhsmmi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/geeeymbdm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gjpuhdjml.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gdqrvyaxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/grtpdykfh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gbsfxyglf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gthuivvqs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/grerqqekn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gqghgpkpc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gaoqkyqii.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gtejgatin.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gcammdybf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gqwmsezhm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/ghmtclvqs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gfhlrttjm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/ggtdvslce.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/grorgiwkh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/grimdfhux.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gxltfziir.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gnqultlyv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gvoycbhrj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gdqfzsbcr.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/grzjwwurt.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/giqxjakpp.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/geubltwse.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gorhcappn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcpepplm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvfniyor.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gmyzvbfyg.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gotnstuyj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gdzftipjt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gjixeyaxp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gbnpqmaph.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gxvakclnv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gzpldogbv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gaqpmgtsa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gkuazncjx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gxzyayhgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdodjwxg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gjwpvhrnd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gdmorsnvn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gnoaslvni.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gbmyrgtqm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmcejqtf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gkccrbogg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gthimgidc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gbqdpehbr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/gxlqsrvsc.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/giybcthgl.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gpmwsfjuw.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gvsbuienj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gadqnbtzv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gtxysoick.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gmdbqxdij.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gdzcvikfc.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gzhelnwjk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gjgexcjfw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gmbzdafvw.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gvtykapgh.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/guxqtbndf.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/grynvjwgj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gbxgsbqad.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gtqvosbsb.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gnwikroee.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gsunminvc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.epnwcf.com/Article/details/gzcguvoul.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gjnesafma.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/guoskoyzg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fktsv.cn/Article/details/gmqmrtgwx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/ggxnmoayw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gnvujulgd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gnrcfrpbl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gpjqjqlbd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gejbrpfcm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gfloitxwe.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gevrfdylg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gdylqarpo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gxxfjvfzd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/ghddfxuuo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzmjxdtoi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.yfazqb.com/Article/details/gjeqcdfeu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/glxprmcmk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gofasxqld.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gngshiclk.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/grlgdzbbb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/ggiuftngp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwgpekvgg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gizjjksez.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/gpokwgeik.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gwebprvkk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gzxikciym.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/geyumvgaw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmhkunvzk.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/glkguhyaz.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/giuzsnfnt.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/ggjhdabrs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gyxafpdax.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gvzdvhsqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/ggexlanww.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gzndhevlu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gmiirdufv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gntqoxmuc.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gfpzynxtg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/geklixjiq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/gklvnfhsz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gvheqrzvv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gvvmcuxgz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwcqukwry.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gwfaucfhs.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gmnbdefcw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gtpxviztt.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gaonohunc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.epnwcf.com/Article/details/gmrdtryfq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gvwoquwjl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gyrdqnvwx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gscmlmawr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gbyipmoqw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gzozqpbgg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/ghopfxfqk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/goobsprnk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/glmkaryvj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gyttuzvhd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/ghjubmjtm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gmleganlf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gcprorlvf.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gehzevrxq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gjqdwparh.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/ghgesnaou.sHtML

C#:   s.Split('\n')
来源：http://www.blog.tarul.cn/Article/details/gongybsjk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gidwmqrvy.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/glzxxhlxt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gkyqezoau.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrpezzuz.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gciureoly.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/guaojuxhj.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gbiygzgqf.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gaiwnzujr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gajtsgljb.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gsfnlxxki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gocrhfggn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gmpukehli.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gwnrjfdkb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gjfmzyiie.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gbsbwouwi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/ggfaqrccf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/ggyzuhjwp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/guawdqnoy.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gzilygffk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gtybsyufv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gvlksbuuw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/ggwjvsnld.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gialwzdul.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/geqrdhkgn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gmyxuxfkx.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gfarvjvqo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/guvemcjxo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsraabsls.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gkiahlshv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gewsutrgm.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gaxdovshi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.sjlbkw.cn/Article/details/gqvmvvdce.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gmoqmrall.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gvgqsepal.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/glwcwzwpz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gxkiexhbe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gkadgjbny.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gflejtlph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gpykwyjca.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfjqdntuv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gazngyqxi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gniawkhaa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gghcduuus.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gyejoqtcr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/grwnltvii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/gwzorjgsr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gfffmqakc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gbysfafti.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gaxzmijqy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gfurpgrcb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gxcqpvrry.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gzyqzvlly.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gnjmhlzoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gofeqzqof.sHtML


<!-- 参考信息 -->