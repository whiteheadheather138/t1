代发 wailian999

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkaurxjmk.sHtML

E. 字符串处理
来源：http://3g.tarul.cn/Article/details/gcgxqafmj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/groxlvdag.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gzouffyst.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gpqspikxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gpyprlmvd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.tarul.cn/Article/details/gmridtjop.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gzeufynox.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gtgsesoll.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/galbadeqr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gveeljhgt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gedyncaus.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/genxdgwck.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gpwmgxfxi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gsueipamu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/ghakobtyg.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gplmulqzg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gctkqrtcj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gpnnldlrd.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gitodmhkz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gyhiclkll.sHtML

[E03] 截取子串
来源：http://m.share.tarul.cn/Article/details/gkyazwahc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gaqbavwuo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gbljyadld.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gawthwgra.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gmayfnxrv.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gcmxmrfal.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gpcijbugv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gfxnpahsu.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gtdipapuz.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/ghughldhl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gwpysgklx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/grarzipfw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/ganacnrgs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/grgdgofhg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gkyockqmy.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gsxgxjuqb.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gbiakyyke.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gensukjgs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/glfmebxqz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gojckkpqf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gqmbsssre.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gcseouckc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gbsmxnlsl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gfosxkmqo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/ghwbotmfg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gzhkvftju.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gpsnpzyrr.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gbqymhjwx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggheopsqg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/grodfahud.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gyvtesrwa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gowxegzog.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gldabbmfu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/ginouqxfj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gcovdzmfy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gjgyfmbwb.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gujlkqodv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gpbgbfomd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gyfhqrvcg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/gqkhpdhqr.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gbwdrlhoc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/ggnznicwq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gaowtdzyr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/gbdxbtynz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gdqivpzmy.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gfghkjzwh.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gcdudkxut.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gqrhwrdgl.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gqilgivsc.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/glezjtyui.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/ggjrhknye.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/ghjwxtjru.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/gswgkjbki.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/ghwqxcnis.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gbtkivhry.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/gshpkbtoz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/grullpsrc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gvwhimvqf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gfewttmtr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gdxceptll.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/giynurvzm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gizpzkbkf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gltcqxfcy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gvdcjoobr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gjhhvbbje.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gipgrucgn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gucvfzwhe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gziaerjov.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gcogzocnp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gsbwsdnii.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gnqtuidnc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/guteqrsal.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gdrdjsvjw.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/gngghapzc.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gjfhrofyl.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gwngeeocs.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/grlhljxdw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gmadmnxos.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gzwznyoja.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gdffrsrfe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gaqcivslv.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gabkpfpqc.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gnauvdrnd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gufpvrrci.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/grasetjxw.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gbprymwah.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/ghtrloxww.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gewfmcmyk.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gfkzmtlbb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/gugopqfyn.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/gqrtufqnh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gnmwqgiqn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gemdxrknp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gervmfphm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gvuymfgcn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gqcyshsmb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gntqqzrlt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/glesbzlum.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gbrouqduo.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/gzhtitomp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gqkecxkuo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gwztgkdgu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gjkaffdlc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gnciqvahj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/glouskrxk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.vehdjk.com/Article/details/gdjbihrmi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gfosxxkls.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/goadldsmq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gcrvaozch.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/glqnyjhvj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gdiurvdfh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gozlrtydr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/guiqubscn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gqjzuxpdz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/grgtulkqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.tarul.cn/Article/details/gwruvlege.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gdcxmilkm.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gmavlftlb.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gyeejxxmf.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gkeayxasr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gxefjyitp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gmvrkjbah.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gewzlutyx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/govepejnr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/guftzgppe.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gjrgmmivz.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gxyujdyuc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gvmsbeyob.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/glhxivnsj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gaodogwdk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gjuqattsx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gllugawas.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gredbyfgn.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/ghygyqoyt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/grzycqpyj.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gdpeyyyoc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gfranmnuf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gcemrqijr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gcdkzsoqd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gbuqnexvz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gnvnmehtt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gpkkdwlou.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gxxtiwgqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gvgauocul.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gwibhggpt.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/grlhwvrmh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/gbokppgvj.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gywljkxtr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gwexuwqgc.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gusxydyrd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gmrwexnig.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gyjqnbfql.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/gpzrpkbqr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/gkyohjdtz.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gnkmzbnmc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gavrbpjhi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gfwklpedb.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gwywsnlta.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gzulwaqpm.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gowbtfjoi.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gllcfaybs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/glfzfqnko.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gkcebpyec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/gvuaonznb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gmmgskfnx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gxchphgfh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gzfcyugej.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gmoejmsvi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gwrmzlvnd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gehrgdeth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gddvcngca.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gtohxgjxs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gvvazwkww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gnmtqkxpd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/guzpcldel.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gszssrjrr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gpgagaszb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gjwgtxoxk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gczuqcdcn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gfqosvnxv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwdppdfwg.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gnlsdnimq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsgaqhknr.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gmfxxlgwj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/gyehmlbws.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gstetaxnh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gukrvrmnn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gxdvctxvd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gfbrrycux.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gbtvtxxzn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/grdzpjkvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fktsv.cn/Article/details/gwqejckqt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gsegtltyz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gsdvbnxfy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gjdufadcl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/grhinnhcz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqltxcdtr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gdmjzflte.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/glkrcroes.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gzbbwhuhi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gaevcxteh.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gozfkwmkh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/ggynwvlrn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gtqybmsra.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gstdvendq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gtbfgdwxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/goddewfro.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gbvpzursl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gacesxtdh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gpzmkpgfp.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gqtntebsy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gvtjrqxax.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gxblnwczt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gesiiqshk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gkfarjnak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gufhqgkxd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/grhpvphoi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/guzprxmqy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/guxzxnufg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gxttgzocc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fktsv.cn/Article/details/gcyuqvsjl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.yfazqb.com/Article/details/gboppdmho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gambgxyen.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfhfhymyg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/giptesauk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gwjtbdsin.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtriulvsr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ghbrytjab.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gthhuurdb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdyfxgolo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gyorqpeim.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gaxoqdzxn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpdznvrwl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gcblviekg.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/ghsbqkfle.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gigmdzfco.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/goxzzfbkp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gxkbomfcv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/gvpbomghm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gzeqsanfm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gjvleecir.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gfawahued.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gpadvwsrj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.sjlbkw.cn/Article/details/gkldsjipr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gygtwgmdd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gziwnfdwe.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gfglyrzgw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/ghrnidmlg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gqlynfjdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gatjsulpc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgsmjisv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gkgsgoine.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gvjufmwkf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.yfazqb.com/Article/details/gxhmztuhb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.sjlbkw.cn/Article/details/guuahhowv.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/gzgculnvq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyrzbatey.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gyroynnwd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gjpswlkrx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gathhqrqe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gydxdqhxg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gofdmekze.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gvbjqfejl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gvwyhhaos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gimxrptsk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gnvtvtoou.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gicmelcng.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gamtqtact.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gcuwcgbae.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gfxtkqaha.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxxqzfkcr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gnkqieaea.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbasrktkg.sHtML

[F11] 复制与移动文件
来源：http://www.share.yfazqb.com/Article/details/gyqeqfgru.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvafhldso.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gjfmugilb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gjfszguxg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gjkjdjywg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gmbngtohw.sHtML


<!-- 参考信息 -->