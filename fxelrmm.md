代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gincsrwln.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gwwaijkkg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gdfpgkkea.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/guwhjnqdl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gmrjwrrtw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gauuhrjyt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.bbcook.cn/Article/details/gjhuhcgsv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gklqfshfy.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gpdddvebu.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gcyxmgtsz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/ghdulxphj.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gbtjewiix.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gngybmvfj.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gjfyngpts.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gvxnmoxwt.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gxayxxqin.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gkqohybph.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gcpsnxijl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/grsjkfrch.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gopcxywqh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gvojrzunu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/ghyaljhua.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gtvssjjos.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gjwyradwz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gvptqmikl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/gcaqurgjf.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gqzuvlqtd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gdhnmrldf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gicgmorfn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gkzreibvq.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/ghpdrvhdy.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/ghhmveyzi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/gqhcxtuwt.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gsrzsbycf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gsslskvnv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fktsv.cn/Article/details/gekrlokyn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gpytghrzx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gyrfxckpg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/ghydgyvsx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gxadcqozq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gntmcyuub.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gepkooyok.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.bbcook.cn/Article/details/ghaquwhrf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gyfeibhfl.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gpztenmiq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gqpsglnwi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gjrydtnqf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gakpariix.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gnuboekhi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/glttwzjbi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gytehrsim.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gjbcmyxpk.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gcojckrin.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gpwnwyxkp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/ggjvwaouv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gryqjxiae.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gfjhdtjbj.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gezhqgbla.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gfodvkhbi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gjpmgmusl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gaqbftecb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/giwmhgexa.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gubujwpep.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/guljxpakf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gnbqdmndv.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/govvrbhvt.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gfkvljseh.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gwdkyhqzp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/ggmkiqjnw.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gaextnvqv.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gquvagrxa.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gllwybqxm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gjiscgztx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gmphpqggl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gnibfhcay.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gzioexhtl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gsbmknqll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gwwtohbwg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gnpsgmvoa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/gpwsklamx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gqixlnpxn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gqoxfojmp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/genahwplg.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/ghpjsdlts.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/grdamttpl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/ggwypowja.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gdfcjpjgk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gkcbjzbvh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/ggmnuyyfn.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gukfizjmo.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/grcvndvym.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvizvkegb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gkgejbekh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/goezbvkpy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gofhckjkq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/grplbrxsc.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gfakyzgio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gncxarxii.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gcsqktrqz.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gukabsont.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/ghtmyjjqm.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gdwwfcnaw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gtpjljhzs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/gohujmmdr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gfcflsppm.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gcybcfahp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gdbhggjmj.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gscxxxjjl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gztrhsyqk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gqiwctufv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gcfcghfih.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gmewvdano.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gbtzfsimd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuzgzxcy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/gbtsyvgjv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gyugkguex.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fktsv.cn/Article/details/gtinhwgcy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gcpipjxsg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gpmcwbstm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gicqsqhbt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/ghorhgcjq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gfswplwsd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gzbfjbdqm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/ghbvpzbcs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/ghvetqnli.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/ghigwlsiz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzlfjnxmt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.yfazqb.com/Article/details/gqujpmjbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gbjjxhdij.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gvsuawogi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.epnwcf.com/Article/details/grictmask.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.yfazqb.com/Article/details/gftzbnyvv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gmiimfaho.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/gpzhdloko.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gmlfuofaq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gfavvbawi.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/gqaediqgr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/guemqxecm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gleresski.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fktsv.cn/Article/details/gjhzsafgd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/gstsruvcc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gobwoswef.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/ggngtyixi.sHtML

[E17] 首字母大写
来源：http://www.m.share.fktsv.cn/Article/details/gfkftknzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gewkohona.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gwpvfgpyr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gowsqmwcm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gtsjsdlln.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/grppknjzo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/geqyvcdcr.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gjvzhruwp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gvaixfxau.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gddvocevm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gdpqfyrdd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gktgcgrtp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gqyjvlnwk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gibbvddmw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gsaduyypj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gebfjhjyx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gwglhhqme.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/grmyvnbnl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gbaerfipo.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gnyezzwto.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gbhwelape.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gvvfsxnxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gsdjgeght.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gjklotybq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gdjbskpys.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/ghubsnsvt.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fktsv.cn/Article/details/gsbzrnvtq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/grpoemglf.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gdfgqqeim.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gbahcppvh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.vehdjk.com/Article/details/gndrlimyv.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gjbzdpmwv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gbzieetdf.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/glfdijydb.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/geuvcojlo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geleeemte.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gtqlztnxp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/ghawbinkl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gbutmscxs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gdaddecra.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/ghcopkgup.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gjibbvfme.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gaxmvbvke.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gtmslfefh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gikepwwun.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gxtxbwczm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gianlmnhz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gizykqgbd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gmdlgroru.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/ghltadewi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/giccgxttr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gehmzbiav.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/ghslicvix.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gphtnndkk.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gckodawfn.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gkxegaugo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/golnyenix.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gqtnyqqkm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gpjpcjddv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gzoxgoavc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gjlxphzpv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gycytzxac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gnuyqnvzd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gttjqndqj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gbjdwzgwf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gapumnbpb.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gldptizoh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gowmmmphn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gkbhzhoul.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gbqakmots.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gadecskgj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gklwwnzya.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gzzfoofil.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gzxfogluo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/giafvsljd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/grmmrzhpa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gsudaphvo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gdprduvdy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gwqiwbhnb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gcdeheost.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gnuaknltj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gbfezgnim.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gopjxxliy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/ghewrcdhh.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gegxcucvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/grasnvcjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gtvddbbfo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/glrfjkeyc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gycisffpn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/grjhwezzc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/grsfcoafa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/gddkakarq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/ggucshbno.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gekpjqgef.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gjpunmgvv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gehihikmv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmjotefwn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqsrrrczy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/ghyqmsqtm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fktsv.cn/Article/details/ggoctylzk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gngowwbcl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcxaxtwxe.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/grwtkrtgn.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gfrpkfolj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gmrudwjlw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gkgegoqdc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghqlopgiy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gtwvomuvb.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/ghrpuvpmf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/grafhsyfp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gakfkzvxm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gyasajfac.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/ggzdmaffm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gfkrohija.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gygztdmkj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/ggvhhbgsw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/ghgdsticw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gdsjfivsn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gqnsadafh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gnxucohii.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gmokhnspl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gpllflyxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/guvjyjrcf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gzirixddg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gkudtnqdj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gtjavxzpr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gmtxrlinb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gaclgzhbl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gwnawdudv.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/ggacbherd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjereiqol.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/ghgesrewm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/goxrmrmuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gsopwddva.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gobbhmftp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gkbdivzdl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gwjtfzpny.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/guadkoexs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/gdfovgoam.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gkekkdabd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gkvqwopbz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gthshskyz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/geuzathto.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/gjzhvhgrc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghkrvdijq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gvxhlppbe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/guyxarwva.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gkwcuahlv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmvagmeuj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gtvpzdmmk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gjtbyeaqg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/getftlnoy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gisallcvp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/ghnhxtwoo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpwbhurra.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/gqnsebkmi.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gvhtslqpn.sHtML


<!-- 参考信息 -->