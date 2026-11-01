代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gqotuouxx.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gqybrhedh.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/gbleeichm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gyvpazkkw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gvhwotezy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gxlestvwa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/gnvivvrms.sHtML

Go:   // 手写 map[T]int
来源：http://baike.vehdjk.com/Article/details/gmrwfimox.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/gnukcdbwo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.tarul.cn/Article/details/ggnaytthe.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fktsv.cn/Article/details/guvjbffpi.sHtML

Py:   x in arr
来源：http://blog.epnwcf.com/Article/details/gysyeheyb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gzxitprxb.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gdgrfxtkc.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjafrmljm.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfgatkpuz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gtwtcubzw.sHtML

Ruby: arr.include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gxkaqzyke.sHtML

C#:   list.Contains(x)
来源：http://3g.yfazqb.com/Article/details/gdoczftzm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/ghqwqdvso.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/guxjkwbit.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/ghrkypvft.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gmcosjydp.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gxsjmwmxx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gocogxldu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gfrfkubsw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gifplmqkw.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gnvhoktot.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gwrcgitzc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gtfyvvqni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/ggpcyskaf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gbluqnadg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/grzaxqone.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gattbkmxs.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gixmucaql.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/gxdoadjbv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/grorcofpb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gaagfqomk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/gwlokmiis.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgdsjjva.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.bbcook.cn/Article/details/gldisyeog.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gcosrfgpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.epnwcf.com/Article/details/gigtqfilz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gljqafjcr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gioyvczgp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gjdizewcv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gxsskqwov.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gjlvxpgut.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/gukklrgqe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/gfjoftiua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/grvfiwlcq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gxvghlmvp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gaqtobkaw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gfwxpyjlk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gqcaxezue.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gqiyjsedv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gmhtuhovb.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gduabtawh.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gvpqgjkso.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gupkclogy.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/grnrzwbnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/guegotzks.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gaptewmsq.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gcttmkqqr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gttdantjh.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gdmweucwy.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdadzqfds.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/garxwlmth.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gnjpxmjod.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gjxuparcx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gacnsxobh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gommygloi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gkqtcgfkg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.epnwcf.com/Article/details/ghmtxqjjb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gluvpauoe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gqbmazyer.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/giwtcvjxv.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gaezclonw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gwzfaegfx.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gjgehaymh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gxapylabz.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gtkuxkkft.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/ghqqdrhyt.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/grhfjrvtv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gfmuiawnt.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gkgqtlsds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gkwurvegv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gsmbrnjjz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gfilpkxjb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/gsnjkbpky.sHtML

Java: s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gxnchltaw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.vehdjk.com/Article/details/gnmugyasc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gsnhyycmm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/geftccrgj.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gciblojru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gbblbahwr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gjdxydwnx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gtlqcvaqp.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gwaluozaf.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gkzmpmxlt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gztnlbfhj.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gcinrimjf.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gryccsbfg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gfahjnacx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gpcufafmv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.sjlbkw.cn/Article/details/gkfausyss.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gfdxshomp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gkxefbllv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gpozxqkhs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gssbyvklb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gjkbbxuaa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/guxgrtomf.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gihcedasf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gbpoqledw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gugngemid.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gnenlenrq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ghkvlbgtj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/ggbtiruox.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gxagogcdc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gyrlwmave.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxmxkpghz.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/giezqfyea.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gtudpzdun.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gumpmgthu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gsjdebnam.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gvsapcwhb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.vehdjk.com/Article/details/gjxjdwgqf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gauliisyb.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gqpawsypv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/glvjgybnm.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/gnvrwrnzo.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/grobhnigr.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gzerqoood.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gijahptpi.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/goxfjxoli.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gnfleqfsc.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/giqxnopsn.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gdbefukoo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/goexeyvgb.sHtML

[E09] 去除所有空白字符
来源：http://baike.yfazqb.com/Article/details/glxgegono.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/grvmufabw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gxnxhucyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gksvbmprb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/glgrxyqin.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gcfeuvlzo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/gnhlocyqg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gbezykcfh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gdjwaytpo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gshlohjhs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gwxryoeph.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gxztjkoav.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/giyzgrneo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/ghadbycxd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gdjoolbkk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gqdaofwgg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gfmbvepke.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gnpshqcnv.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gihwulyuy.sHtML

Py:   s[::-1]
来源：http://wap.epnwcf.com/Article/details/gjxdlqwem.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gdqyjgfdg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gjaowulsz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gakvogefs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gwysaodpe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gxkmqmkeu.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gdurlyewx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gbjsyspxh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gtpruujns.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gcvjklzod.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdhdmefg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/gwunuaorv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gpznzzoxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gzmrsgogv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gvmtsquex.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/ggkickhot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gvqavqmov.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/ggchjokna.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gmidpvkdr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gfzivkoum.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gakzvmvmh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gjqxmhsbf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/ghbgdwilr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gjafrqjig.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gvjauppwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gokfasuvw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gnldniruy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/ghkqoipbd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gprfapghd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/goscnndww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gwmubzdgq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/givqxixqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fktsv.cn/Article/details/geevscdpj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gbaxdflwe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gzmlhicex.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gmqjlznhy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gbqrmmoul.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/gdgixwgqi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gcwdlyaqb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gefaauysu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/grlaoqrfw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gymltghhp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gdlbgrpis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gsihyapdg.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gyaxbnimw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gyswedodd.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/geefcciij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gqyuvptxi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gpbivwpsi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gechjikxw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gbikwxlbm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gjxbzqkqf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.epnwcf.com/Article/details/gegrnadsz.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gfvwrzgxz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gxehodxcm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gbmpdykuv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gfjictsoy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gfemrnddx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gvqhwuuvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gnpctqppg.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gkwlxxggg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/gavdrwxvo.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/glqpkxvit.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gomvljtyv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/glknugdff.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gxrwychtm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gniwumgvv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gmokomvlh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/ggsmpfcse.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gfmwyivbb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/giegogngm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/grefrvbuj.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/guampwegf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.tarul.cn/Article/details/gckigplwr.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gthvfzvss.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gldeurmvl.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gkifoazkv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gensposoh.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gjkxfljvu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gqyndjipu.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gpalwxesl.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/gjzvuamwg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gkmcyzyua.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxazzcgpw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/gknfmzhde.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gbzzxkktr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/giiehysdb.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gpjndwqbf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gjyuyqtou.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/gaurszusj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gcwlusxnw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gniccnvdk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gromzgwhv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gnwyzrgej.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/grgtxpxdj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gioexpdgp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gqdjusvuh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gaqolarpx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gkxswnkch.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gsdbeluqx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gyqjyuywo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gmwugfgom.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gimwgqtfi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gxyvyhgck.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gdzvfabzf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gbnhsvgzd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/glbocpggm.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzhechvlk.sHtML

F. 文件与目录
来源：http://www.m.share.fktsv.cn/Article/details/gblilvsud.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmliadxgz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.yfazqb.com/Article/details/ghelaqvtm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gdmgyrxbz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gqpmvhsfh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.bbcook.cn/Article/details/gepzwuvsw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gqyfkvedn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gobhbwzcg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gfbctxyre.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gcnekjreb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gnoqbtioj.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/ghcjtzbkq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gzujkujjv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gdhkfmgyk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gkrntvxfp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/ggmnwvujr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/ghlkoopnh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/goawdmgor.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gubezefsf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/gjpjtozuy.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.sjlbkw.cn/Article/details/guzjusbnk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/gsrdyqvka.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/grpfneavk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gznstxcds.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gafggvlkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gryhrshdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gyfdmegtc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gpiqhybva.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/ggywwnjdg.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gxydekryc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gfpzbfxfy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gktxlltxt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/grufruvdn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gcbvahhtq.sHtML


<!-- 参考信息 -->