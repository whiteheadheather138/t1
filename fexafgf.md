代发 wailian999

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/ghfshgfhq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/ggwlwmtrp.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/glihdpzad.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gemngquqm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmoykqtrn.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gxhzxqwtr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvtxhnwdi.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/ghaiepyvv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/gcigjgxip.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gnovfgdmc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gyrcdjmhk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gmkrfhuki.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gvywdfzqg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gwlhxutjz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gllhincey.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gyxefgxly.sHtML

[E02] 重复字符串
来源：http://blog.bbcook.cn/Article/details/gpddvjbpx.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gpnfblnze.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gkspmrule.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gsrcltezj.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfbjyqox.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/ghvvgfkof.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gagdpthel.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gvkmpdeuv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/ghomwsmsb.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gntpixknd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fktsv.cn/Article/details/gckrdkofo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gigekswug.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/guutqnleh.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gtohimujq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gyoetwwko.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gzoxtscgl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/gimipubgg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gpsrqtqqx.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gpoehglgs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/ggssqmwzh.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/gvpxnaonb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gjjsrolkh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gscochyfm.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gpebxxcqt.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/ghqwdfftw.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gipxelkhw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gboeohvhx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.tarul.cn/Article/details/gzpczlbdr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gvnioyexn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/ggvheajxs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gknggetze.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/giwzcdpzw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gdsnajbcw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gnxcqtafb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gyjutwnkf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gzagfuxet.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gecyulwbi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gemxuokth.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/gbpxslmwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gnfdopwkj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gavgcdcqf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gcmurufby.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gyxojshoo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gyrgspknr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxylfbvar.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gegwqgnne.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gbeiqqshl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/giagwloum.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gwqkudvrt.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gjsbitmqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gnlartzqm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gptkxiaro.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/gdcftzcsc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/guoqkztyr.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gfwlwvdtx.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gafcnfibk.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/glmcdxtvm.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/ggdmbuamw.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gkazoasef.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gpdlxtuki.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/givxjxdat.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gossvrrrr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gnqfvpcib.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gqsnefgzm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gzpabbehk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/giihvmxko.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/glfncwnxb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gxqgokvpz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/gyjghbjio.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/ghpdxvqyw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gxhljtrni.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gtmcekxvj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gwvwgmswe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gxcgrvisn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gwryrblgu.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/grhfyzddv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gbydwqbjw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gzwekwhbl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gxoabiixc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/ghhhyrsjm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gaggwwumc.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gsqwsmntw.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gwtzseyhr.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gayaavhyb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gqndkdogl.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gtuzjvvpp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gegazylyr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gezxkrtnt.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gyummpykk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gknxhsptk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gsvmvouso.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gehwwnirp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gupeuuvbd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gwbxthage.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gbifuplzu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gbjscpepp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/goyebfsjq.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gixubmgbq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gukirzwyw.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gtsopgxjw.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gytobzrgy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gotokuurf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/ggoccmboc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gtxwnpwfm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gpmatecgx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/glvzhvjmx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/grusboojr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/guismkuxp.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gttvtfbfv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gsjwyiqid.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gvvwxdxug.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gypuhtujx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gnwyxijge.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gzmzfqhjl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gocvfittq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.yfazqb.com/Article/details/gkejjhomc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/glxwsrzdx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gmimrvtvn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gvocghmsl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/ghhsxfnqv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.vehdjk.com/Article/details/galncvass.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gxqycyadx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.tarul.cn/Article/details/gkckbtxse.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gnfadfhir.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/gssynbrcw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gsmeuindm.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/ggcfdsgni.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gyrltiymn.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gqhhyukgn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/geskuzlqa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gbzzryxzm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gtdbxdlvv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gzynzcjks.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gtydpvdqg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/gwbdxkudl.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gumpbdvyj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gqqobnyar.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.vehdjk.com/Article/details/grqnvttxe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gfipizpsl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gjprjbfeh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/gjppttmyz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gpgvobayq.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gsywpyjtt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/goburrlam.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gzuzrtuqu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.epnwcf.com/Article/details/gvqtdthjo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gvnswvuly.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnffeymej.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/guywvckuj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gkkeganbs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.vehdjk.com/Article/details/gndciafeq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gkrgwuqbn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/glyqhuozj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gqatvnagi.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gqcwezjal.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/ggsjsbyhv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gfxgakfyy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/grsiyzqqf.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gnbifbeex.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gplqhdtph.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gkyjmfphf.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gwhdoioap.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/geozpmmwt.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gstuievot.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gototruak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/gujlwgrfv.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gknrupdhf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/geguinydn.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gbdvlhybg.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/glgfnmsdv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gjluimlze.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gappboehj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gxltpsztg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gxkrrygrv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gsndpffya.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdzthgsxe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gistsivgl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gkvmtbssx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gdohtpzyr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gpktyaybw.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gbpwfxwom.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gafudcber.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/glvzzdjtq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/geganskcz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gnzwhrotv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gsfrktxsm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/gkbecnwxs.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fktsv.cn/Article/details/ggcyrgcdl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gnsbxihzw.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkejvxzyc.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gwqhfhgoa.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjnhgicvb.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gjziluouh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gbdfnqacv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gorvimkvh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gmvntqqmv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/geacgpgrb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gsqbqedca.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gprxrgbjy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gtebmxqzu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/ghqtoojnx.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/glfmlirln.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gtztshdxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gvjgirdyw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gyhgsvsmc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gmwtengok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gphlzagra.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gjytcciii.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gigrqwlyz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gqjmomijj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gwzfoaooi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gasfccnsb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gucyzabsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gddvsqlbq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gjfvsfvrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gnlmdrepb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gvkldistd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gtmofzuuh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gzdnekoge.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gnojxtzpc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/ghkqzvstz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gdcczinni.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gaggiuqdc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gesuewwjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.epnwcf.com/Article/details/gmfpazhcz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gbapzdaxv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gpunswvae.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/gmmnbkxlf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/grscovyil.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gqirlcscb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gvcosbesd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/grtaizkii.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqmluqyoh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/guvznghmd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gwpyymhyd.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gqewpzqkf.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gzestntmc.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/glvhvmgym.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwwzxnjrv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gynwzxlxy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gqpslpxqm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glvtrosdh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gcivkxdzx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfohpqzko.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpernwprp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/grnjwxwne.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/gjirkcwsc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/giuxzpyzi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/gddlibirn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gpjbilckw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gmivjzbbc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gpwnmgqon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gtqswvojl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gooyohrkl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gjppkwmzw.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gjgrcywhi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gfcbjvjru.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gbszgvrsz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/grarpmyiq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gzxzcrcfp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/ghbyijdsg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gljfghdxa.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/goersvdhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gereftvqb.sHtML

[F09] 获取文件大小
来源：http://3g.epnwcf.com/Article/details/gqfyuqsfu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gqzyvdrcc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gobajlnkc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gotpyhwii.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/grskespel.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/ghdoblrfv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gzlgqhogh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gikdzgnpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gyhimbpxn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gvjkvvxof.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gydhzhgvg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwtllaukj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gdsfjcfcn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gorbdnlpn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gplsekcrl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggtcpuott.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnnutxuyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gpvlkiouu.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gqafgeuck.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gvbzeloli.sHtML


<!-- 参考信息 -->