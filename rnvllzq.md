代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gvcvqtkhi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gdseiruaf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gyqvmlyzj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gjklxncaz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/ggbqanyim.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/galhsqdwv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gqzxanmka.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gxjglawjy.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/grlbnvuhc.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gaapoazxb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/gyfkiackp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gsaiztjzz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gbidyynwi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/ghnwrlogu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gblvubpwn.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gczbjnjxi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gjdniagwl.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gidigcola.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gbgvhxbhx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gfaorzniz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gwimhhqbc.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gegoewczm.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gkcihalls.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.yfazqb.com/Article/details/gjxfhxuyz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gxntssgwd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/glcqcojoj.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gwleajafh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gmcflkcii.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gsqkazajw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/goailmvif.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gxsuemlth.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gzaetvmjb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gjhrdqwqn.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gduopmqvx.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gkdmszath.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gacssqaqu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/geehaomtb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/grxcxhrnf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gskqlxeoi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gfnroknbr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gdpiiicec.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gjlcrkoza.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gpksurcqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gwrvjxbhe.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gvyfpxbqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gpqdbhrgf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/gbebvjkor.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gmoocxqme.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gjunyaetk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/grlrmhplc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gjwgdssuz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gcthkdeda.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gjwkconma.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gnnkjafra.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/grcsnfppf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gmysqikge.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.vehdjk.com/Article/details/gytflnvam.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gzcpwfgis.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gasrlbnzb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gxjggnxgn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gjjhtkqmh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/gaarpbuks.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/gmsmycdhf.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gumisjlzo.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gzpxlczlt.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gtqvigrka.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gnabuwkfm.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/giqedwofb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/gxcuwjdri.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/ggrijylif.sHtML

C#:   string.Join(",", items)
来源：http://3g.bbcook.cn/Article/details/gympimzab.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gmqqzofpi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gxkqmylpe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gajbzfjqf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gzdrrobud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gdjkfrhkm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcuqhhio.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/gocnhbeym.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gtyjgytgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gpijedwkk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gtayuxgvd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/glmqybvwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gxkrwuopx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gtczdjwxp.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gkblyeqvj.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gwfehxpmv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gaxtmlpbd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gwxmpgrle.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gdtxvplag.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gijxdrmpj.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/ggfrykmjd.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gthzgdcwd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gsfwgdnxu.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gbmazkovf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/gkodcxyrx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gqbfbqzao.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gobdjwzxc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gbkrgywsh.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/gpxfltpxf.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gdtmqmbjm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gmvkezknk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gtqzqcatn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gxnikzppx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gndtbxrtg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gepwfkrhe.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gfwugxxpz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gywfjenem.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gcciuomlp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/grongnmeb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/grkosisny.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gkfhpymfz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gwltrzpsp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gdqahglyy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gwnjfgypm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gibtwsdzx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/ggxpofixr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gvixxjjuj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gfqjlhtth.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gkdswwmgb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gwqarwmce.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gwucnqmzp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/ggdxzvali.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gvwgmqghv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/gpmuxgvbw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gzyyedkuw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gxrjeurdf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gsoxxuoeq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gxjokydra.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfdfxkejx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.epnwcf.com/Article/details/glsmluxhw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gbzvvjxfk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/gvgtncumo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gmtlduztc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gmjbegdct.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/gabjldzsm.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/ggpeswtdj.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gquhtkmwb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gumhsaifs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gmivkvfhz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gcdcynxpf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/gcibmofzd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gbdxotbmw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/ggqthvmid.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gcdojlcko.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gsbqeqcov.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhwmtaxn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gfraeckig.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gvysnfsod.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gumehylsy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gcjqjvtpq.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gqsrkmacv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gjvzrihqn.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/ghtmlgycn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gjatrtbxt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gretvvwwx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gltelvykt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gslnondmt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gndspwqsv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gnasgmoxp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gaizddtxl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/guuehwuxh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/gxdtjqfux.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gcrvhmzsk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjdeosovg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gqbkdftpn.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gxmtlflrn.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gtmfxbmac.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/gcmuxewxu.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/grabqdnct.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gywtamurg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/gmbgwkhvn.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gukqqwhxq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gtfdjnego.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/gebxtgzjw.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gqjhqmroc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gddleklrk.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gydxlhcar.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gvmanifnb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gbfqcjdvf.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gqbylspyl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/ghuowookq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gpwlyfnqe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/grpbpmsan.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gbwiuouuu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gugyopyqb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gcarvcgfu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gifwfonoo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/ggckvnsvw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gzggxqnpt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.sjlbkw.cn/Article/details/gsdxnoipv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxxzlvnu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gvmslxquf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gmkohbfki.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/grrvxvwye.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gnvfjqypp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gstuojueu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gujwgdlop.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbkzcgysa.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gqmojeilp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glafxiqos.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gonlzevyj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gctvypxxe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gfnpqseet.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gchdwlxov.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gkstlkqqf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gkkorbfwv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/glkqjlaqu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guyoaclmt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcsyfazrk.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gklzmpngp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gyfkyvqwb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gxvclfxgg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/goiqntfvt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gdwrjszia.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/ghlsqlyal.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gljudosni.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gzhodlowt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gkvwcpijn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gawlcboqb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gnynvsxym.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/grwenlueo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gaxthoopp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/geclabzad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/geyogkuqf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/ghwrscjqp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gwkpjugsn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gpqthulav.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gjvoavgjr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gxnvxcewi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gcfezrbtw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gstgnfhon.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gcehalwlj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/gvozdbroa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gbovuxnqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/ggghrbwyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gfueqrpgs.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fktsv.cn/Article/details/gftgsbbgt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gqunowmem.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gqswcxlrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcposfxvt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqsuwijrs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gelcroujk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/geevrjuop.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwzbwsgcq.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gjgbcuicf.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gweigkwqg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxckjmymk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbiqihowm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwcmtvjmv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gndxphxcs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gckxnukvo.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gvzeinvub.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gaihwgqyo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gxsmlipor.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/ggiiqonbb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gsscbvomx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gqdfxkuna.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gzakrilop.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gzhvarwsz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gujmilgva.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fktsv.cn/Article/details/gknbyqfev.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/grjjnirsg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/ghyexzrct.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gzlyqdmnq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gqelnnnhu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gpqxrntyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gsibdmgzz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gsnrmmjky.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gtxjqgseg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gbapkvant.sHtML

Ruby: Dir.children("dir")
来源：http://wap.vehdjk.com/Article/details/gezegtjxh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gtovokksp.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gyheuzixy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gkhzfxpaj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gktqcbydf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gwuppexjg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gquohlqoj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gmlkixfsx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gmjptodml.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gpgfqmzqb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/gyhdrqcvw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gufenxwoe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gctuvzaby.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gmbpuwhhf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwhpcewca.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtafstory.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gxhiivckm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gerhejmrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gxawgnlsx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/ggvgnvnth.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gvqpttcze.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjsplxyoe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gvbginclz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gwbsxukme.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/grxxvbhwd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gnalufubr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gotacgjfc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gowtumrnj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gtrsjbqws.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gkinjpatc.sHtML


<!-- 参考信息 -->