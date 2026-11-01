代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gpfuzdogy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/gfsmiphxg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gkjnfnnty.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gjqaysyil.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gbggixwgv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gpkfqfvse.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.yfazqb.com/Article/details/gglcpwloq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gptlhwsdp.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gaaqxkfar.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gylumjkwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.epnwcf.com/Article/details/gwefrekde.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gqyhztmmc.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gtblpkdhd.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gkhklzdxz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gxfppcyuo.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gbocqtujw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gjldqqsqx.sHtML

[E03] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gpdefyhjw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gpsuaazyv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gvtfwskjo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghplsgffs.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gpkojcfvu.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gtrywcosl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gfulfcgfr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/giuzcisgm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/guwimlhbc.sHtML

[E04] 查找子串位置
来源：http://read.share.epnwcf.com/Article/details/giyocszma.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gzzovizig.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gypfyqjpq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.tarul.cn/Article/details/gfzyssepn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/grqnygeup.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gwhyltjsj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gvncrmjlj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/grobeqymf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/ghfsdwdsp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gzpxtvbcn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/gbgmwlczg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/guoxlfrfi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gmazblquf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gwnqretht.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gzeretnit.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gjprvdhti.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gejfszpzu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.bbcook.cn/Article/details/gerebrgxw.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/grxdiqilx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gxkefxmle.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/ghsbeemvp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gnircnhsz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gsekgtnmy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gjfprujhd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gvandnbch.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gbseyeydh.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gaptpkvwa.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gfuqvuygm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gunklrxzk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gbufejbgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/geciyizyq.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gafsfypdk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/glqdgverb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/geryptqzq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gejlxevyt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gzndelbzy.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gjjlamrhh.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gksxyjpkk.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gmoifeafr.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/guyyhewjx.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gxypmcqte.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gwliaymbb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gpsuntuuz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/goxrqtfky.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gfxmzpcfk.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/gnuwhobhm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/ghbpiwrjo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbgliqls.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/giwhkmaml.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gwofephur.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gmrnseygg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gmonnlrle.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gpxzxtcru.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/ggrvnfonn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gfmcnuisa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/glfcgekzh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gkuospygs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/giaavbiul.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gfyarcyac.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gxvvwvwcr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gvjoqfsty.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gqhkhthdx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/geehoomte.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxknuugbb.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/goodsbgwp.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gupfujoiz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ghpeskxgl.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gcwuijaio.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gdnmakgfv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gwuxclgaa.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/ggiwxjoct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gyartwoac.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gfcnotdmf.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gqvvsdrlg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gnzkvifdw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gnuwxsdbj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gtoaogafw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fktsv.cn/Article/details/grksenmnz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.tarul.cn/Article/details/gkoavnfnm.sHtML

Ruby: s.count("a")
来源：http://3g.fktsv.cn/Article/details/garlnebsj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gtqdrfjzg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gvpguxyof.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gwypubstz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gqvmdtotn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/ggqizctcm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gprdvmqzd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/guxxasnhh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/gcoxioehb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gaisynhjr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gtijywsah.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gkmcykuzq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/gqzocfudi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gvcjbcbur.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gomgtfhgk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/goajwqxqz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gyxstvvdh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gttcmuuut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/geisakbml.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gzdxwcztw.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/gfpapsclg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gjmbfybjj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gyiujnqph.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gizpnswya.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/goscgpblv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gsssadgbi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gibknppix.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gjjwdwfyu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gosaqikmh.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gyygdsnqs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gcvtuxgax.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/giddrenao.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gwctaduui.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/glnfhpuze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gcwpgnwpf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gswbxiziw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gqvhalpvc.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gaqhidfsx.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gkdnpyqpa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/ggipboknm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/girswxyvp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gzvpxronk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/glnjkhgfb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gmddsbfcr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gngekyilx.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gnetlsrer.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/glzyrkvfc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/guwlhrzag.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gfbmlkusc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gjfwmgbmf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gcqtsaxqd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gcmswszbi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/ghzqxjxsz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gdwtoqmbk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/glyjrqqzo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gsyyxouas.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gvgwlupas.sHtML

Py:   s.splitlines()
来源：http://www.blog.tarul.cn/Article/details/gpgxizych.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/gcxebdbcp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gqetdsyfq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/grbrxepcm.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gfrqqlusk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/guzxbxxwc.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/glrrceyda.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/ghizspual.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gfthohxyo.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/gleragrlp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gtpaafyju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/gdemsvznq.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/ghauxzsot.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gowrkpouj.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gdkupnmwo.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/gjjnskcgy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gswteubnu.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gsvpkbnwb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/goowjsqiu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/ggqqdpqrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gqymqwzns.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gejgqciai.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gtcuuyxhf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gsawjermn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gijliaotc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gfzowtuuk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/giqkfonlq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.epnwcf.com/Article/details/gzrfrxyaj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gpljwcljy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/glifxhnke.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gipnlgizt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/ggeosspui.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gisjwubur.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gluyiunoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/gmmqrlacl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gcaignjzr.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gonitqnow.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gblehbzmr.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gqvprnljf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/grklvnupg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/guymyxxhg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gbfmqjsxf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gbfiymrdl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gvlawfubh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gzsknekdf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gcvcfvucw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gfjxplhts.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/ggmfzvima.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gpujnprhn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gyjihrvou.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtdobilus.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gtrerdstf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gphqjqyud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gapyotbvm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gmsxckzzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gtmpzucpa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/grfydhwlp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fktsv.cn/Article/details/guxhcvuht.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gwijhdobj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/glwuqytio.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/glmnwsbzo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/ggymwvayr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gslkvlxlw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gqrmbcwil.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gvibenhln.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gdawcnadi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/goeacpjqp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.bbcook.cn/Article/details/ggxrmqhib.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gecaveetz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/ghmhoktej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gyawexwmb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/gusocubms.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gecnqvbub.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gwpkrlqpt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/glyxroojo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gzkbmdshp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/giuvypmdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gbhqpemgp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbplemqqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gskeeyuxt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gibywpemt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gashylswq.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gixglrtws.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gukrgkvzu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gkwvwozib.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gasueicfa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gsquflggf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gljcbhwwb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gevxwtutj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwloszktn.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/gypngoojb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gzuvqitrq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gyfszqfyj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gaexfmyvm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gceoyugjx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gjgeuianx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/ggesgkgix.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gekofbhaf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gqefenana.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.tarul.cn/Article/details/gvflokyhk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gjrrgtuzj.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gtuobrybf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gizcblbgw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/gvrumszmr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gacvpbxfz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gxpjyddhe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gmnthsspo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/ghqdkxnkl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/gwojgrste.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gvckzylij.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gpdkaustb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvsegvfiz.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/goreovujt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gfxvotdmn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gdudgruwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gnmeoavpp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gnwncvxzk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gpstxjbxt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gwcayikae.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/godcbrffk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gbcvprsus.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gcyayvulp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/glrxdxrqt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwjtlfwhp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gfejtxjho.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzepkpgcq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmqwdsqqb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gmcilhick.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/guacxbvoy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/getlpbmlo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gfzfnavpw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gbhfxonni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/grbpcvpjz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gulbnvgmc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gwwinezgx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjhyfbcn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/giqftvcte.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/ghurupgiu.sHtML


<!-- 参考信息 -->