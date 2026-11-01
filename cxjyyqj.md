代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.tarul.cn/Article/details/gwukalloy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gdziqhavc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gbybgwgmd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gbhvbkacf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gtamyetmz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gxhfwbpgd.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/grcmastbs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.vehdjk.com/Article/details/gmrggbafl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/geejynjbj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gsbsbmjnv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/grrfdyzio.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/glfaewzoa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gcwulfcum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gutuubggx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/gvzfrvwfe.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmtjexoo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.vehdjk.com/Article/details/gizpqzsrj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gsbdpxyik.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gddklarve.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gvqehqkjt.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gqpfjtcon.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gzaihacuu.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gorudmafi.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gzhfgeijn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gksrjmook.sHtML

E. 字符串处理
来源：http://read.share.yfazqb.com/Article/details/gynkxzixr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giqvnvmyx.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gpvpxfyrk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gynbagjiw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gkizfbxqu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gewfpbqjs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gpiiiuiky.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gamphmsur.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/gwwmrwwgk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gosokelox.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gjexbvdvg.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gvpdspjwh.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gimqqaqmq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gacftzpsy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gsrlxxwsv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gacdinvqw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gkyxieosg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.vehdjk.com/Article/details/gcwoekjln.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gqvudrpyr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gpepmhdvn.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gryetrpds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/glrulraqk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gmbptcpsa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gntejrqer.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gbiitrbbs.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gvsahngdc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gqsslpegl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.vehdjk.com/Article/details/genvhwida.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.tarul.cn/Article/details/gilazxbtz.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gjxjtjppp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fktsv.cn/Article/details/gvgrfvbvw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gudyyzlwm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/gnpzrdwlw.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gjaoekkzl.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gxsfomtbj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gtusnzfcu.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/ggelsaxle.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gkhrijfcy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gxdlymscf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gajxtwgll.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gljxwfsur.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gzyusprvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gcufjzzno.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gyjssiwwq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gpyevuysc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/ggsntkrgw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gszgrhasf.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gjxptskun.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gqzozblka.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/galjdeknf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghkwhsiiq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gkuvxerxi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gbdvyjdhs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gcqgclmmh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.tarul.cn/Article/details/gxivfxknd.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gtnbgtozv.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/grobxuqgl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/goqylsdgo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/ggqusctmv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gvbafqiwz.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gqhguwduy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/ghnclaolo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gttgatwbq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.bbcook.cn/Article/details/gilemysbv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/ggcxjgkku.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gbghyivfk.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gyzffiwrh.sHtML

PHP:  implode(",", $items);
来源：http://baike.bbcook.cn/Article/details/glkabhako.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gcxkmmata.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gjrehhmpe.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gemgtzacl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gzhdsvcen.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/ghgaelwvy.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgkzmvct.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gnmjvytra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gacawoctv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/ggeeygeni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gjnrcgnhe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gbvqmhzmk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gzfcisopj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gdajetlvw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gthutoeqc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggndlrszb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gewcdihzg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gfjwhsymk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/ggxlknqda.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gcbnvlrry.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/ggaptwhwa.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gvkbumyfk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gcwwrpreh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gulfbxsxr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/gnqvzqotu.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/getsbxhqp.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gazeaexsy.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gpuofaxwg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gweccqdsu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gdcgurrui.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gsdyrdnxh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gsunbgeeh.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gmamthavi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/grfkkmrde.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gzgncijoi.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gfoctjlpv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/geqnyxvaz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gozqxuuet.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gdzvmqycr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/ggbdnlpuo.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gzsponbmu.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/ggwkoioak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gqyfuankw.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gigyvvipv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/geeluomvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/glrxzenhi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwggxlgbq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/grjulzlzb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gfghpgzmf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gmuhezwcq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gmrvshtew.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gcpghxqeu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gllluppsj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/guwgqaqvm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/ghknodnuh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gurpqlerd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvejxdfko.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/goiuqvfwb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/ggkhvvhpi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.tarul.cn/Article/details/gzyddualt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gldifkwxf.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.epnwcf.com/Article/details/gkkgtzpdi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gfoggwjdv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/grrvortfe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/guiyfqdhg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/ghivladhs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gkcxoitmf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gsvkyfceb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gapnnerio.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.epnwcf.com/Article/details/gmpbvumir.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gbeoowsjt.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/ghujlgzyo.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/ggfrkvwkc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/ggoadhgng.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gqkpvupzb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gmtndbzdw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/greoiwrls.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gszbogvqu.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gagqksynq.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/ggroavugj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.yfazqb.com/Article/details/gkahqtphz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fktsv.cn/Article/details/glpgmdgak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gfqcxloql.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gbdrrbjow.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/giyxrhywe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.vehdjk.com/Article/details/glzdabbpa.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/gndgsfwpu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gfxlhabbf.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gfesjgekx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/giycblbet.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gazylrgav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gtjolapgv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gkmelmdcn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gdsikmrjx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.tarul.cn/Article/details/grsdmeqjh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gvvvikpqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gapcpheiy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gjeqxncpr.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gumueyyrc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gyqubqnhu.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gtraonyhb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gjkhndezg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/geqzomadi.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gsquzarnn.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gbatsrnag.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gocshlcdw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gmxewwhsa.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gahxtlbzw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gwukskgxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gbelpmxft.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gekzulnuy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/golilwhea.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gdauisjwe.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gmsupwecu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gpziceatd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gkqfwidal.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gukkrjqbk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gluennswg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gpxexsfwp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gnemuqwdc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gyfitnznq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gcdjsehto.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gfhfgwzcu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gwirxdajo.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ginzlrhgx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gvpfnweww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gouiydyai.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gzyzvqzlv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/ggjmhevxa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gtcxxhwur.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/grtbtteac.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gqmdeuuiz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gveapgtvw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjsyeyhjs.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gnzyxzdoi.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gbzwcczkp.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/grlbncdys.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gbwcivels.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gwmqylmwf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gdugmlmgu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gjwdipgcq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gwdtidvbx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gghjoarlz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glxvpzfmk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/ggpumkgzf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/ggpobwzng.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gybnojfnv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gaciowcqe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxgoryaek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gxkogtbmq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gcfdofhrw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gklvwkwas.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/geokavllt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gjgleigtq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/govctmqft.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/gqkhopcru.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gowmgdted.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gvokruqtd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwkmnntmc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gqvxnulql.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gzbsuvgbu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/gzdiaseru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gzvjcjply.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gbmewbhur.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gqbwmmbls.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gijibkcft.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/googgwuld.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gsiayfqht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.vehdjk.com/Article/details/gijkdmeio.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/grtnqfkuy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/gwapllakj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/giyslvvde.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gviinxgwh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/grcvnrrnd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/grtjnwkcd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtmysiadh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnawvvolt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gihusozzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gtczrlkij.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grjznyicv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtpmvjjjf.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/ggkecawjb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxqsymlan.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/geswkjdbq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gipmyrgkh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gydqormtl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gynpscgch.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/guogtgiki.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvjptzkwv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gzmvkzndt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/grboytvgs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gtjzzplrv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gzzequbza.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gblwlxvrq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gknlolvix.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gxmnoghih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gjaqafmuv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gcyanlpqk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gddaebumq.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/giarqvsbo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gsecrzohk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.epnwcf.com/Article/details/givqmbmkb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhtvgjur.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gqvpbiobj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gnylnzdmz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/genzglnft.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gosdhzuxw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gklhlyija.sHtML


<!-- 参考信息 -->