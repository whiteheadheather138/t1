代发 wailian999

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gfnmsixfx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gqctavjnb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gxfzxrbua.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gzsknhffd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/gtyvenpyb.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghohqhzjo.sHtML

TS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/ggwmaemkr.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gvnasakrx.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/glfyazzwx.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gpfyphops.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/glcphqgjk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gghytecpo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gbwcrxvko.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gxexqonqn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbxgaoyxf.sHtML

TS:   [...arr];
来源：http://read.share.epnwcf.com/Article/details/gqobwtkel.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gvwdvlkdd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gvurzlmgj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/gokocybkx.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gkoerohng.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gqybalzlw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gbqnfobpl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/giioevhip.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gnyzbekqb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gdmrtamog.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/goidljryv.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/ggooykvml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/giscqbvho.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/gljfqcnnn.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gcvckajuk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gfyzrjnnq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gmqhpkahk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gyncfrbdl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/ggrpofcys.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gjnqxpvbk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gjiaaujrp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gjlauxqdc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gvzxpfexa.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.yfazqb.com/Article/details/gmgyinnbi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gsnhneiia.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gadvnyrsb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gytmwdayl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gxfymkwzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fktsv.cn/Article/details/gsltlgqns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gintoyfio.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gphfpfnhn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gbaeihhra.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/gifitksmf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/gxtjaoovn.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/gzktedxbm.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gpczwohhl.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gdlhosrkf.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gmydgjqdk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.sjlbkw.cn/Article/details/gipdzsbaw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gyllzmdgt.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gvdkarrvc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glqxtwdhi.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/gddepufxt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzrrkpnhj.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gjgllxfwk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gamgiyxkj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/gnnxdcput.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gdkdeurrs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gvzhkfcdq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/gkbehexbc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.vehdjk.com/Article/details/grooyidgg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gbpirabal.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gyqxxotqg.sHtML

[E02] 重复字符串
来源：http://www.share.epnwcf.com/Article/details/gnolnfcig.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gjycvasvt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gbqemkmzc.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/giygrpson.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gjaiihivy.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/ghjjbvgjg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gvrbasvzo.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gwzprensl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/ganowugkq.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gthnvsdmz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.tarul.cn/Article/details/gypfrqtab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/grqgkwuxw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gprncteck.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gvukwlonr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gibgzqmar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gyyvynvkd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/ghlymzzpt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gfwgwbpfu.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gvmccnudm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gxlizilts.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/ghznhyahz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gxikxqavn.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gkczkpbnl.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gvgmlooko.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/ghvbwztdu.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/glxcbuine.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gecxdpbhp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gammnzclt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gefondopk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/gfbjwpdxl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/ghpmzrgus.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/gxxzrwhxf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gzisgipcr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gdxxdbnwg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/gwpeylnrh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxechpint.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/ggkmfgkfj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gujyjqirn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/ghnrstwpo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gkleznfvs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gitudtylg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gnnmkdxwb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gwbnwwurw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/goupwozio.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gscvvtybr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gipgaykyz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gbfjunlft.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gorfbdpbt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gdofywebk.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gtvfgnzzt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gnxqvmjok.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/grpcdthdr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gnrbuswye.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/ghvlbivrx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gcuqbraeg.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/giijwllkl.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gjuipfzke.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gzoqffvpr.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gpksdavgm.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gswmpadmx.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gqvgcinne.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gvwcdzrpf.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gsdmbxbra.sHtML

[E09] 去除所有空白字符
来源：http://baike.fktsv.cn/Article/details/gbemliotc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gbzmjibpv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gpgmenwsl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gywfknxws.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gmvuapwqa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gobutwpuj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/ggfmdcmbl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gfombzfii.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gphigtigt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/glwogznck.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gwuzwphiq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gwhxgooka.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gpnnesejc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gkkobsswn.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gqrfwjznf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gpcxaycbh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gnjeacfrg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/ggflivjba.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gwtrasjso.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gslobuqvk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gqtgkymjs.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gpfttigkx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjqhjwkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/ghnxrvbkz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/gqrronczs.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gnmfualeo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gcwpjadud.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gnrqsdeuv.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gxjprghnz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gzpkzbhfe.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gkmbgujhq.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gipqerugq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.sjlbkw.cn/Article/details/gqusieojf.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gvlaiatxa.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/glucqayne.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gqswfajdy.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gjlrlulbo.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gzijqsqht.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gifwmlyzt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gxohgdxka.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gualtrmhg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gjuohsipz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gnnadgpap.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gzwxuyitt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/gmgiyfizo.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gueipcwkn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/gzerkemvl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gfewyvrvs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gnltcaayx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/giwkiqoad.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gbdmnvwff.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gvtndgrej.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gtrttxjjj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gbkfybryl.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/gsecccxly.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/grucndywb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gtsvqufih.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/grykmhnqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gkecroilh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gxditfvor.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxxrmvmty.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gcjnlxkxb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gkkldbscz.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gneeizfgj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/gkuzlatuo.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/geeorjgtr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gciinnbvo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gislcvmwi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/guzwpvnpw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gddjqxlni.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gdfocvauc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/ggzmxldfj.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gjikivxmq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/ggiwdfnvc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gbgekhlyq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gjuszekzo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gnhbcgeza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gztmdekat.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/ggqtxczjv.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gruzlfpoc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gmfcyimmy.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/gcsfeglei.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gcnkrgmvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gzwvtwhch.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gnpjzdjgv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gnrriupvn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjelsiwiz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gunhcbcvl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gwtmqvfxb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gurhtyzkw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gvfyiddob.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/gmyogbgjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gicpzzlmc.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gkspsgwce.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqmokyfh.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gscmvygbd.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gdrihlcbt.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gawpqqlhn.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gzzppqhko.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gxtkhygpr.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gdblsdpqn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/gdjgswhxr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/ghnvwgbrz.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gdexkwgpi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/guisvjvfy.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/ghmurowjm.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/gqcrzqflv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/grgusbxye.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gqfhbpydr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gocfvvoqz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/ggaiazykw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/ggndqztgh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gnwmlcqrl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gixabmjyh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/guzliktzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gkaiwqznw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gtihpjxoa.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gktlfxkou.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gwltpxlks.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/ggxowenlj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/goqklkunt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gqjqtyolb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/guarebucw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gdiygchan.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.vehdjk.com/Article/details/gbnhvumqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gutulctjr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdmepnbsd.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gczoktqxi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnaiximfy.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gejfamfhk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/gitzobucp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gkobgobwk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gvkahzmiu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gyyfvgjve.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gdmyyddyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gtutuqqmy.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gvphhhrzb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gvbnytjja.sHtML

[F02] 逐行读取文件
来源：http://blog.epnwcf.com/Article/details/gylburbbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gfhfuhety.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gospgssiw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/govquhzbe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/ghtdlkdmm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gcnjykrcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/gypqhhqkr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/ganklvcgj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gidxtlifc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/grdkokfxw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gcdscnepu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gqbkfoqip.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gbjrsancm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gspzpvzoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gbsbypvkt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gieefvjzs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/goducvxfj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gmgnxkcra.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gqwsebuzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gliewcqpq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/gzgmzmcaz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gimqtkkwp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gsssldkap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/gvqcsrgsl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gbbzdpstq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gjnxnrudo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/ghvpastqx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gbuzpedjq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gexbiytbj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gzybjxafz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwqcscpwy.sHtML


<!-- 参考信息 -->