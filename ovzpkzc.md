代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.vehdjk.com/Article/details/gcyalmuyk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/gyoijnpis.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gecqtsbml.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gyzmzojll.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gfbmxvbqr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/grbmhlrcz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/geejrcpyy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gamcywpyz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.vehdjk.com/Article/details/grlqyrwrm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gdxipdcui.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gtxaoamcl.sHtML

[D26] 数组转字符串
来源：http://m.share.yfazqb.com/Article/details/gzfxdzlnv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/guiqklxsn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/gfejppafi.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/grlgrhcnr.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gbsdkqwmf.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gscoengde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gzpzijhrd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/glernnarb.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gfawohatl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkmqrwacz.sHtML

E. 字符串处理
来源：http://read.share.yfazqb.com/Article/details/gsnkctldt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfwruaqlf.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gdoacjfyy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gxtyjojqj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gmvdbnobq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gbualfqwh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gxhcmfteu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gfguffava.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/glixwgqil.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gncuxuyjb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gsnbhffpq.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gyjweisko.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gmngktujr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/glwtyxwip.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gpldsggav.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gypologqe.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gjmcxuwzn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/getuxfxpv.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gzpperaye.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gizdqylvt.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/givsshmia.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gcfmbzaes.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gkewkskra.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gmuwosfru.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gdlbedcef.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gotgmokxb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gkfckkwzx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/glqeykjjd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gvmjykdac.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gsrsyyifa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gfpyvybfc.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/grnxofmmf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.vehdjk.com/Article/details/gcjpoelzl.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/grsimpqvb.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gtjqsamna.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/gpqbaegmc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/goizxcmgc.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fktsv.cn/Article/details/gnmuczlva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gtvlqwlkz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gmkycdqoc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.sjlbkw.cn/Article/details/gthsczrnj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gawbixink.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gvxiplhgs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gkcxqbfgt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gocfqqmsc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gfllitict.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gdyjtoqgi.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gtbzppidn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gujvfxpnb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gzmarceef.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gbvbpdmmz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gzixtkwlz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gyuhbxxwk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gcwosafxg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gzffhrplz.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gkqhhrlfc.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gzfavuyoq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gpguloqms.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gfqarzqzn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/grbfhwljs.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gdzvgahts.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gpclvdqkg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gglqncvun.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gntyueuww.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/glhbeuyyx.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gtucbxnkv.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gymmcftxd.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gflgguwcn.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gjcxnumij.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gehraawdy.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gtjyklxpz.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.epnwcf.com/Article/details/gyqeudlsg.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gdkyfqndf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gptvyspzb.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gkhonlhec.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gdgvixccb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/gskedtqwi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gwtgequwf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gklgknbgq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/geqweiqib.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/gmvxslxqb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gtovkvfng.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gmgjjwccy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/gfvyieixg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gkizjzklo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gkubgivay.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gjuujigwo.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gumfhwhny.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gbusbodnh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gcfponttu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gtyoshhub.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gktkbgqfx.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/gadncaxwh.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gomypusag.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gbhbeacoq.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gttmrqkri.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gnumxzajm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/gnjkzoclu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gmsabslra.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gmpzpuspv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gsxmwvttk.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gvgxeijlz.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/glvmojclf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gwpqhincl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gpxfrnpwd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gtbtngolr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gjmhsjpdj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.tarul.cn/Article/details/gexmdpksa.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gxorvicdy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gwfuqaehz.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gwfzlunpq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gqrqdpfju.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gusczgbwp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcqmpxpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/ghbzbjplq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gykxaaqct.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.yfazqb.com/Article/details/gpxyqhcsy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gbmpgnmzq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkaipapa.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gpvlstylc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gfombaskh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gjkpmbpyo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.bbcook.cn/Article/details/gqlhbtcaq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdguzqbkf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gbqgiktye.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gjeesmnft.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gatamtvsj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gwgxyjgyg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gdcorshsv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/ggcoqtomt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/gwmwuqzjm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/grlhkhwta.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/gdpcpanjj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gelmshbss.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gbvfqwoch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gfebjyaaf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqzqltnk.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gxmhqultk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/glzxjrhhp.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gkmtnxezy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gpfpdchfq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gxdvjwrjc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gxjdmjife.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gyvhuykvq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gfhypinvl.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/glaxznipc.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gmsdbgazr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gdyujxviv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gxamwjiek.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gmllxtpfn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/grxhskgio.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gteefaomt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gubufegey.sHtML

Ruby: s.capitalize
来源：http://wap.vehdjk.com/Article/details/ghxrbdrhb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gaukdhekf.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/gozdyrzhb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gaaggwfia.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.bbcook.cn/Article/details/giiyllepq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gpppfnpiv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gzfnxatzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gapsxidqs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gcpzhukjz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gfrjlrbib.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/ggmbhqdwp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/geyxrhjxl.sHtML

Py:   s.splitlines()
来源：http://read.share.fktsv.cn/Article/details/gbzwcommq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/gendaykhn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gykxicyle.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gbqlhsqjx.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gsywbsevn.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gyizkuvwk.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/gcgumyhkj.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gtshejoyf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gnmgkyedt.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gdmktjdho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/glwedsxik.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/grjdsicih.sHtML

TS:   if (s === "") {}
来源：http://mobile.tarul.cn/Article/details/gavbtxpco.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/giwtizidu.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gavmpqvod.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gjdoaupkz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/goxlifahh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gsfqvljeg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.yfazqb.com/Article/details/gimjwwvee.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gcnmjghsm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gvewqgnng.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gsrofegxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gkylabesx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gidjeqcfd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gvuxvnpzn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gmkglyszo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gbuqrcuux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.sjlbkw.cn/Article/details/gthbsjgdm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gvdyacvii.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gxdvezaxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gxaqdlrdu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gcwfdzndf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gleqgbbah.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gpzpvnyoa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gcxrbfgir.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqgpssutv.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/ghrexljzm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grhltkauu.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gbuqluode.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/geadmlmyh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/guaouquyt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gsnqgirel.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gwrhvytql.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gqlqbemat.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gkbkupxoy.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gdeqgofop.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.epnwcf.com/Article/details/gjhcnhuih.sHtML

[F02] 逐行读取文件
来源：http://read.share.fktsv.cn/Article/details/gctgpjxoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gsexmmelx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.bbcook.cn/Article/details/gqtudtxtz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gemcvdjnf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gtjxdqolb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gteqnggvm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/glzouuskr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gpmukzuij.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gjgjzjtvo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/gkoecsxfl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gjjygnamg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gwgwyzhvy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gcxoixefe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gwigallgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/ginriqscq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/grjpmhwyd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/glzclmjdy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/ggbigkgyu.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gxcpkvtmo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gnmiwmhwc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gzlugbxhz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gfmmloxvo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gtflrvmns.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/geyiluara.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gqzmgnqqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/gyfmrbfjz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gwlmkmnft.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gsebcvjwg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gwcdgfezs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gpswnooqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkztmbxyb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxhidhcmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzijsfy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gglzycuqh.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcsnzqpwd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gfkfybzoc.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gpdaqtfxa.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gypyzwqjj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gqlkkpliz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdrlyzlnk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gzgqaheaj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gjwilsuxc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/greeurjly.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gznhzfiey.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gujvvjwqw.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gtkekrsnj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gmabkhbjo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gzuxokixy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gkgbsvvco.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/ggvitihpa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/guzxxgytx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gbvsvpnjz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gltuxobrz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gebxauhxf.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gdrvjrcsl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/geawutlcp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gbwebossx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/ghgaybgtf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/ghbcqsijj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gwdvhtdpj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/glkrmzefb.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.vehdjk.com/Article/details/ggicpdzwb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/ggoboqqhh.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/geoaaheip.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gqapwqvyf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbxozmle.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/glsvmuiar.sHtML


<!-- 参考信息 -->