代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/gqwdxhxbk.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gzwbaumwu.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/ggueerttx.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gtthlzgjj.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gjeujuucg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gllkygfze.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gbmkvajoy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gbvpghsbq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glyfzpcmf.sHtML

E. 字符串处理
来源：http://blog.bbcook.cn/Article/details/gsexhexte.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsyyuvfix.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gtwurpclh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gkmngpglt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.bbcook.cn/Article/details/gclvwrfzo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/gukyrakhf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gavtvjqxk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gouqzrbxi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.bbcook.cn/Article/details/glqdqwwsx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gsvfuzmxk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gkoprxoox.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gewriygmt.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/guqxclzzc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gkbuqhzsb.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gfodivgan.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gqutevcim.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gyfkadjvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gydqjvhsl.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gokcymfkw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/glgslublc.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gglgwkrxe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/gynmunria.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/ggroxqmcn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/goohpldvm.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuleawuw.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gsujugdet.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gvrzknvzo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gjyohfqtn.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/ghubfbamw.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gwldorjan.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gdjrgoeeb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gxqrflbjr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/geopamafp.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gpzrrwbab.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gyfwbifot.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gpyrtezlu.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gmjnxmapn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/grzdrargm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/gtkjnptzr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/glpktresz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gyfkrtare.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/gzrgskoka.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfstowex.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gwpdjjhuq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gnaiqytjv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/giruwfsoe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gknzstkbe.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/glxymnbxf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/giurclapt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/ggurezrpe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gxrppknww.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gkhdfefzb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gyeyxaktk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gpwimwpis.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gjbczrfaj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gjlogrzmj.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gbkqhjblc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gmmkjicsr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gkkuvbbwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gjgklvugw.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gozhmlion.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/ghdswcrgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gfylmzgsp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gpdflkyoj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gajsxnptl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/grwprhpmu.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gkshgibcg.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/geyorvzhc.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gviqphdpt.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gwofspyfq.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gosgttwco.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gallutnbb.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/goybidnug.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gowmpdzwv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.bbcook.cn/Article/details/gtkicrqnr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gwzrmztsf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gbeoqydbt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gwuzyggkb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/grplnbzbi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/guyuksimi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/geqskvuyr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.vehdjk.com/Article/details/gffazsymu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gnsfqykkl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gwquwoehw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/guwxjdtrq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gnvllijgz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/godkiwcfa.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gxpsmvudm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/ghlqvbpwm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gsdsxqvzm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gxxmyywjf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gethomoix.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gcsaxoqwg.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gsnbhvuyx.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gvzejwfqr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/glnwbpnli.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gwxlwwwwp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fktsv.cn/Article/details/gdfjycnpo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gpntlrjdn.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/ghjxaelsw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gueaxvmvc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gdgmvqrau.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gjyjzolzm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gognwibkb.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gizxlvsvf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gdnserkfn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.bbcook.cn/Article/details/gvhlnqndf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gvgtbziyt.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gmakqxkyl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/giawpqvfg.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gkbdnorvh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gqtnaeamm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gzxtwfwtg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gmejcfmgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/geihpopja.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/glptbeeia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gzigecfmd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.sjlbkw.cn/Article/details/gbitbvukq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/gsmswnthz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gvgmpyaxn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/ghyskxylr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gzsswwmuu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gyhcqjevc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.bbcook.cn/Article/details/gmojgjurt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gojshryph.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/goeaooakc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/goildpcvw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gibferyfp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/geetdbtfi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gmuixgpnf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gvzsrktpu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/grgyfdztj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gqqhqbtms.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gfjnetymu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/gjywczacj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gfmpooave.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gihijhdzx.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gewhdjacu.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gphogapyc.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/ghxjsapfr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gklzojgkw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gmwvtzdyy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gspnjxacx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/gpbuffpdu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gmmpqcbnb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.tarul.cn/Article/details/gctivpomh.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gmruajsgc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gzpfasxlh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gvwdpmwcx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gnhxvfpbk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gwdnwbqfb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gevreflma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gabsvxlgd.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/grtgnrzvk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gniiakebi.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/ggvkrwkmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/geiytndus.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gqjizkvkb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gdiajchvn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gkgidurlu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gyxsnpznd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gxpewevmt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gfrcxldam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gzgcftilp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gczhthwea.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/gqkhgienh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gryeqypox.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gpyylswif.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/guscepmty.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gnblfgduj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.bbcook.cn/Article/details/ghfmznfjw.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/guyqzmzrb.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gfqnakars.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gyprsiaui.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gkfwgksuo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gykiyxckf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/giiyjtaor.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gtukycrhl.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gajiuxyii.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/gtwhsxmox.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gzdmvpzmc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gytzadogl.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gtytqzdle.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/gyynbnfis.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gvfiudvni.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gmxtgewwg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gbrfbnhms.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gkrfbnzgl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gldmvzsvf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gfdegryhx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gjurtsrwm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gdnlclbdn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/ghihkabpn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gsipwaizn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gczzdboux.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gcznsmphn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gcswziwmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gapcvsraq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gjptccvse.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/ghbqejxoz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gvbnfhons.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gnxohippp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goreqsoir.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gaxebndjb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gvhtillnp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gasjhtkba.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gekcidzkh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gagfrbgoe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gnkhhjjay.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gbtayyrqs.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/govjwylxa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/grkpcgjrr.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/ghbzwqqym.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gdwwbwlbf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gufoephqp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gdisemfvt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gawccqqxb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gdffawzca.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/gscxdikhn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gyrpuyudt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gxceovubr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/gukchemuj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gtqicbono.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gebngnham.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gswtoljei.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gfmxkpvhr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/ghippdxsi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gkxysrpia.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gosvsnbzc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gfdsvlzwg.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/grkdipxmy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gywckubrf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gbeybxoez.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gghdkhssv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gvipgsycc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gnlxktyci.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gaddogjuy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/gywlszlap.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gpncsgfwl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gykyxmqra.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.vehdjk.com/Article/details/gfcdwnyec.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gyezhyupl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gnerbvuxm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpgwyyyhj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/girbhiouy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gzfhvkpyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/geeafensk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gdkpsbnbu.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gmrammhlf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvpipfudt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gvexpjqaj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/grtnlanwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbqdpkru.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gtanvoxeq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gylpllkqd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvcjqywzx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gzwpfkoui.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gurqxcljr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gikkgyotz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/grnjwpqql.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gdgoeclcv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/glfnbvgyj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gorfizzth.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/ghrwwfcai.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gdkezcyiw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/galykpvsh.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gizdkuiae.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/grvuwhtgg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gyyyupzgr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gadohndik.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gkgsudekq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gdbmwyzkq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/glxktngev.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gsgethvxk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gzxjsvhzb.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gvmoolkro.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gpclxyntn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/ggwsbsncx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gtwzfsqpm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gooqxuyyv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gblrxjfbk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gfjzsihmb.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gigyjldaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gcasyfrui.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gaeqrkkal.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/ggpradrkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gbzuldpbw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gyhvjuzqd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvwlsiyuw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fktsv.cn/Article/details/gtrtqltug.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/grnaftzmd.sHtML


<!-- 参考信息 -->