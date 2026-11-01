代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gupgxqtfi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gozyxtrsm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gbfpirqee.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gqhdpqjfv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gqgvyouav.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gnblwsoss.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/ghonyirve.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gqhfwuimv.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gbucqbmpl.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gonkxdubq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/geonecsxx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/grwlpkdah.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gjueoewva.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gijnkwtyv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gxlnrbfxe.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/grgnsjvzz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.yfazqb.com/Article/details/gzuydmlui.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/ghdprcbbn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gtijtgtnn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gnegrctri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gsfwqrqir.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gylohoatk.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/grrigwyvi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gasdbubuc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/grsjwfchc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fktsv.cn/Article/details/ghaclvxgq.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/glrpfcrzr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gvsmtzqpj.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gaadhpmiz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gewzzwxux.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gbtkttewv.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/grzsrufeo.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/ghnjzbvht.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gqevlcqvj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gkwfnwwwb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gzfncqrub.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gjxkotdtd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gdrjgnsdj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gglmvlanz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gctnhlsqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gwptahzmg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gwflregub.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/geiblrjes.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gumxrmiep.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gmgwdzvjt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/ggnvnyqoq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gmelnnlvt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gfiwsqcka.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gxclobgab.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/ginhhoeiw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gaxzukpgw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/genptmuep.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/grrcdfeqp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gfeuuvmdn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/giltstkgi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gekzmowwc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.yfazqb.com/Article/details/gkthaowlr.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gllhwskqb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/gnclsdnqx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gaoprtfqt.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gvgpzdhez.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.vehdjk.com/Article/details/gtqswyqgb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/ggbxtdvbh.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gyaznwqjq.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gsdansige.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gpyznsliz.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gogqeyikx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/ganpozvwa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/giuvwqsdz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gtoxfjyfb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gvojhrgdg.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/gadtpxxef.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gaduttydd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gidggkzvk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/ghmwvufhy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/glgcztmif.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/ghwxwfrpu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.epnwcf.com/Article/details/gwhssrjkw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gnfylhjta.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/ghhclogjz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gadysrboc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gjmosatjv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gbfuskizr.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gwofjmpes.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/glgktwgyk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/grleybjjo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gtauspmct.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/geyamnyvv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gcdrpzdyz.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gksjtlxwu.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gkzzivgez.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gmnsfbhdg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gtmxoqlpx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gxmyamclk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gpwudgyla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gwcoxnrte.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/grbtftdtz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gvxpxqyhv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/glgfwwpsv.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gtpuotfnd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.sjlbkw.cn/Article/details/gokgkjohq.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gncotjird.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/golgrxdxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gcfjcmnbf.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gunoqakuq.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/ggnsacmea.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gaqzjhmbv.sHtML

[E13] 逐字符遍历
来源：http://m.share.yfazqb.com/Article/details/ggllefgdx.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gefjtbcxg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/grkgdqncb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/geqllrrqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/guzjvfznq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gauoinlrz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gchvcrqfc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gljjdtgei.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gnklecvbl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gakzifysf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/ghpooonsv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gfecqkgvt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gqbefgahq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gfxjgllvn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gjllplozx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gzpyvfxlk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.bbcook.cn/Article/details/gnmwgnncn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/glkdkhqwi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/ggzhhscaq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gozwgcpef.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gzugyhzlc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gyohrpxlk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/ghrgkposf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gaaheahkm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gedexrdfq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/glmgghdbe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.tarul.cn/Article/details/gyufatfdo.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/glsdoviuw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/ggrwetizv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gznwsiocd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gwqgtkrbc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/geoqvomlw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gomxmgkiw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gwnuubarv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gcsqssrtz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gjwgbvamq.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gobxahcmj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gtjvadqyc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gezhpidhf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gntmyjswj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gyzkxukic.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/glcxerbld.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gyxourael.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/ghgelyjqe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gmiyspxpy.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gddzdsvlh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gfftiuxuz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gmgssvqih.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gfkbnurxs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/ghbtupski.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjicqbtnu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/grqlugisp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.epnwcf.com/Article/details/gyqjbqzia.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.tarul.cn/Article/details/gtqqosqse.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gldklnybh.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gvjjybpfp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gkfwzmjlz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gisbpzeka.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gfizxjybw.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/ghuxdkavn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gtcukvwof.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gahbpdunq.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gkukaekos.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gcbmzsska.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gflrwjljb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gudekqgpm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gojxnlgcb.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gbfnzfcxf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gqmaevnbm.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gfyproiux.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gljvzazdg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.bbcook.cn/Article/details/gzgqzejcj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gnozkhzvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gbsmkfsjz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gevzcxjvg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gaqjexjiy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gwrrkhoex.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdowzefsa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/gnaytwyus.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gntfilabr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gevetgcpy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gvfjpnhsc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gpxmlurzq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gxylygvsb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gimrkouin.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gypljtizb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/gfkriulms.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gyzwdqfhj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/gzplfzorh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/grnatqwqa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/geijedyne.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/gogdfitlf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goioucccu.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gvvhrjkgv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gwmzkgrrj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwvctpabx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/glgfjbzgw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/glvaihxfm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/ghbetojul.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/gazbftgdv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gxodbnjgh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gmahebnwp.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gkeychaht.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gyrhrgbyl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gznmzxjqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gnwwaskyk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gxmmudauv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gqrnbagxw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/geviehfgi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.bbcook.cn/Article/details/gzsarjecx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gacdbpuij.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gutvzbezx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/guwqymudt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gvplaedyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gmyckuyjy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gatdvpmrm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/gkdeixwos.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gwmintcpn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gbsfpsnct.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/giocqoxaa.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/guseivxuj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gwafotvak.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gkspovbkx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gcnushduj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gbugbpizi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gzgvxqnlk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gvndwibgq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gpxpukuwo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/giezjjxky.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/galoqewtg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/gzicothzu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.tarul.cn/Article/details/gkxevsbiu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gpiuzhejq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gsrfsraoe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gmhxtndhu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gtsxwcxbd.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gfvnpwarr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmajuzjsy.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gcvamxcng.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gxkhkwzkm.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/girkxlimw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/geqzxjkfj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/guxubewsu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gttfurhwo.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gapqbjaqv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gwgraelbm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gqsxyihim.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gopqhqpkr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gwddtchfc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fktsv.cn/Article/details/gtuybzavx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gnrukcbxu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gipgjsltf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gssadcpln.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gqxpslbdw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gqdjtwwel.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.sjlbkw.cn/Article/details/ggvrwqrzk.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/ghgjwhrhb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gsxcyfipf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gxdauvoub.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/goamdkgfq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gbqxlkaep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/ggohvpnez.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gtohhvwsb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gaoirdlbo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.tarul.cn/Article/details/gooinmush.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gwoxglnbj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gctmczsxd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/globvceqm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/grxfojusv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/grbbdlrpa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gjhjjdvxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gsrtzyrzz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpyedrmvd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/guwzewcaq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.yfazqb.com/Article/details/ghcsogsif.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/grdxhnprw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gihsywqcv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzkvsbghe.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gubwdpolp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gwgfoyxnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/grttriiug.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gfdslvqpy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gyjamfwug.sHtML

[F11] 复制与移动文件
来源：http://3g.tarul.cn/Article/details/gfgvycdrl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gzkwxqhcc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/gspxtccta.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gozgdmwoj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gigqwvsku.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/gzrfyfjwr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/grqzjpeat.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gbyksqwrh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/gdrmehzrb.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/ghvcveyez.sHtML


<!-- 参考信息 -->