代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gjanpmovn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gtgcpxrmt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gaatngbdw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gxicopbdc.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gqyjdxuzh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/gzonwlhiy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.bbcook.cn/Article/details/gyyxypvys.sHtML

Py:   x in arr
来源：http://wap.yfazqb.com/Article/details/gvovuusli.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gaabpgbgh.sHtML

JS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gmmksljyo.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grcgwgugp.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gzcyqsqak.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gsbtnrgah.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gangrcvyn.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gunnlzjna.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gjurlpeve.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gayifxlrw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/gotmtddae.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fktsv.cn/Article/details/gkeznmkni.sHtML

TS:   [...arr];
来源：http://mobile.fktsv.cn/Article/details/gwmubnpyh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.bbcook.cn/Article/details/grwiwuziu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gthbdcyta.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/guuivqfdv.sHtML

C#:   new List<int>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gvmwrafsz.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gfswnraxm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gyqumqvpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gzzrsloxl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gzfivgtfy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/glujopdmb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/ggutgxsbg.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gyslrmchv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/grsboxjbb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/grlsvifht.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/grmdwwqsy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gfdqafihm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gemstcdkx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gchpkfmvc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/gzehgpkyk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gsycvkhmo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/grdntlrng.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gsykvhzja.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/grrukqlza.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gtbvanmbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.tarul.cn/Article/details/gchfqqwia.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gsyvadzpu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gzvlosrrm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gdbxlbffp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/ggfnblcqq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gukrnripz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gbhdwkrgc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghqkejwad.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/ghzxoiupz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/ggrocxrun.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gvecspviz.sHtML

JS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gelcqitab.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gvifcvbkm.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gzspqejyw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gbvjfxgus.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gplniikxr.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gvrkuyuxb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gohozarmb.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/goyghzayi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzwvlbdqj.sHtML

[E01] 拼接字符串
来源：http://blog.fktsv.cn/Article/details/gokexeiht.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gxixxxthl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/ggjasbttk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/ggbaievwx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/grgdvtaga.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gvqtmobbc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/givjkegxy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gcmaoudqs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gvwtigurs.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gebaiuexq.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/ghakublot.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gipmpfkoi.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/ghcgbhcvb.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gymwokbux.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gspszephi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/gduahisze.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gmfiqpmzg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gnyvqsjmq.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/gqqdmuwwr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gkvsmbqjs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gphxqxxag.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/garldmjtj.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fktsv.cn/Article/details/gapefbqxe.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/ggzyimaqj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gtbtauorx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gjypftiwc.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/goqqtcbae.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gphuauxzz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gdzvvrkec.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gbdilumwh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gakwnshxf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gfszimbxd.sHtML

Java: s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/guaouuama.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/ghdvrndnf.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gzcfzftno.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/goiocayyy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gqjunrwnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gphadnmoq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/goxbgzbbf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gpaadllfw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gzwrrpila.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gtezfeqoe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gezbfngfn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gxepzcwth.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gexdyrzhh.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gyickpyvy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gsttxkdnv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gppoyyotu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gdpzbgepx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gziturfxj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/giuiuhqky.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/grasztbqc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gfhcpjxph.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.bbcook.cn/Article/details/gazxmmufg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/geyxaftvb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.sjlbkw.cn/Article/details/gbvmoided.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gwzqtlotv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gtrkzvmco.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gghrmzrih.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gdaglkork.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gtpbftksl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/goprfwnaw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gavxnpwij.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gebgugrcc.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gadfjwawd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gkyylnuqq.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/ggptvnjhy.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gqjlsehvc.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gmawhytkl.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/gpghbsbsi.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gfmpsxtqx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gvifffsus.sHtML

[E09] 去除所有空白字符
来源：http://blog.vehdjk.com/Article/details/gbxlazzpd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fktsv.cn/Article/details/garwdjnex.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gessqcmrx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gaupkvfic.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gynsuzthu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/ghzxplsnp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/ghjlpjpus.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gfehosila.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gvcwuubjr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gfqjgcikb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gswanveae.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gbrpgoakf.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gtijiahrw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gwlrbhosl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gikgndfvs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/graztwjcc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gpiccwwjw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gsutnefkz.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gwzrjuseh.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gogueprrv.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gqfrkeyyn.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/glfukazny.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gfflnxews.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/glrzcuqva.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gxyxrcxwj.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gaqnwkgjl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/guzxenenu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gaoxhpyab.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gcorxdgwg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gnvhcntej.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gtcycrosp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gxmqvvyxh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gttcusrrj.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/grwuiweoi.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gkrgxhxmf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gokwbjxyh.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gvndicjwo.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/gbobnqclz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gdmyzjerz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gmzkatnpw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/giciuprdt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gissouisq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gygrychfo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gkihnojax.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gbfnmembk.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/gatqkhhll.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gymbsxkfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/goyazkdqq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.sjlbkw.cn/Article/details/gdtokdvgc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsajmcyfn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gngdhphzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gvstkhpha.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/grkrvmort.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/grbhkwfks.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gnrirbrwl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gpiwytklb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwdzyjai.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgeevncv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/grffeuzjt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.yfazqb.com/Article/details/gbdddenrc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gbhlyuivt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtawzfcbd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/grhypjeje.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gjahnrctv.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gytatwpyg.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gecrazrux.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gzfgftkoj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gnaacjmiy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gbbvulleq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/ghuejogrz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gdzatnnaj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gucrqixqh.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gcnhmortc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/guehtifrt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gzojjmpbm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gyskdefso.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/glpgmdivj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gonrruugc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gopgxhyzl.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gapdymtdh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gpvqzthrq.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gvfkuhikn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gwulvggpn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/ggxrswmxw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gbmtiocsk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gfgtkayvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gdtzwdmqg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/gmhudvrpd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gcdnommpc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gushukkro.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gkbdgsaae.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/ghkzdjdrh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/ghijlgbrz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gfdtyvzaz.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gtkdmpgbz.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gjbrvibpd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gqibxfvrw.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gdlysijzm.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/goizgtvvz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gbzumfjnm.sHtML

Py:   if not s:
来源：http://m.share.yfazqb.com/Article/details/gjgtanfdg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gxfrtycuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/ghxpybojl.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gmfsdeixu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/glvyldwly.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/geltasara.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gcerqrobf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/goefvkjmw.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gsmxxudtf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gpgpbuxoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gnybzycez.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gotxpgjgi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gobuihpzb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gqdhhgtol.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gixhwkhxr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gdilcpriv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/ggcurdoiq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gdltsnxuk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gerivklsg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gayycitby.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gmmvcoszg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gwsdctkgz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gzqscxhtf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gpkbwkjjl.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gsaonezox.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gofzyqtbw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gssudfndd.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gtfsvobgt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghwjevvdb.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gmvxqfmuk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gpoosxmiy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gupvryqkp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gfyotumrw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gdkyvundj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gjgzzmdfv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gmalvajsm.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ggkfdjjxk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/giujqjdva.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gqnsqaxkr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.epnwcf.com/Article/details/gmgayhbvr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gkjkpzyio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gpnybqizq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gxwkhvnbz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/ghfhnlqbc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gqkeqxesg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gjbchkdft.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gmfahojej.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjctoxsg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gclhqjptf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gbngbqzxo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gtxbsajdw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gkiidcssj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fktsv.cn/Article/details/gmutcirxw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gqitpkzrv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gqipucnnu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gkslybxcc.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gsgnhenks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.tarul.cn/Article/details/gijwhgvog.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/guegveecf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gmbtrbqhp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gyslmokqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gqlhdcsng.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/ggqjyoxif.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/gareogsjq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/grlfokrds.sHtML


<!-- 参考信息 -->