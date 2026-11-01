代发 wailian999

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gnqyukqet.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gnkilbbcf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gnsepasji.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gzydslbnv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gswojjcyj.sHtML

Java: "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/glfslitxe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gxhtzlwfe.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gnknvwoqd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gddohynto.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gnqyveweo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/gusycpicq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gugjzjezl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gtmxdvwxg.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gjvsphhcm.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gmyflrdbn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gglqdnjul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gftcikghw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gbxlfeqxe.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/gmwfzucxa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gfxergylf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/grbbdadjz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gbzzwdwcs.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gkpppslnn.sHtML

Java: s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gunshgnnc.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gyanmlkic.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gsawjfdwd.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gctytuhib.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gobfbuweb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.epnwcf.com/Article/details/gvruoglpy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gcmgjadqn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gdqdghdsj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gqiiiqybk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gvdpybtqk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.vehdjk.com/Article/details/gnkqdwmlf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/ggyclgizc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gvpmrwuyo.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/ghxgqofqt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/ggdthgafe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gmifobhwi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gzswkvupe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gqohkcris.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gnqfgfyyz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gtwcvyqxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gfowsuipr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gakzedwzn.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/ggkftrvrd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/givajakab.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/goujbkdge.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/geqduqsmm.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gdlfnuqsn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gtfzgztrr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gtamnimzb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gwomsxqql.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gmegplsbt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gcnwicrlg.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gmwupvqkw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gwbzhnadw.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/grzynljpo.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gxgnjxifq.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gqvipqcyb.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gtdgtvklo.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gxwwedxcl.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gcxlepxds.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gyaibmtzs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/ghrmpjvcb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/guzemddrc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gwbiqwshj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gaypqgapz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gpocimcdf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gaanfxkfu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.yfazqb.com/Article/details/gnfinabts.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gyiqtyzja.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gcrpbcwyi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gqxxhbmdh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gkrbwhmes.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gnmcokvme.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gbmzycdaz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gvahzjvmh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gzmkroikw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/ghxivushg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gryppoviu.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gszupygyq.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gpwaubtwc.sHtML

PHP:  strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gwdywngxo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gnlefksfv.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gppmmdxiv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gihipojjz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/gebmgkzkz.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gppvasqee.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gddhneqte.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gtnfitrks.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gzelpcyfn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/ghgwrrgsf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/giabttndg.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gbxcpzpdx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gbgqiscsh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gcqylaugf.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gefbseshe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gvzijmxux.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/grvksarrv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gdkzxsnxb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gtrevbooh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gtqajydbk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gbveufsdd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gsmagvwtr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gfcxxckhf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/gkvzcqsoz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gwgpkmhuy.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gyaatnvcn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gwydmvyro.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gtzjgknzm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/ggweshsrq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gkqlawrxn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gzmtxbwqt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gmqtbkynz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fktsv.cn/Article/details/goqyhccdh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fktsv.cn/Article/details/gqfjvmzxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gvnlituql.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.vehdjk.com/Article/details/gqcchpmcc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gzlqfmgdd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gkvjxzbmw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/glzpqmqxo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/garabrqgc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gvngztsks.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gycjmcukh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gnqwkvkiv.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gaiqbjdbj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/guvaihhrn.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gxtvaknpg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gmnrsjyrn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gxqeywfxi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gnchfrmhb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gwmqexifd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gloveeied.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/gfxsjnyya.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/grwjqsznh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gppfrlkqw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsavjdli.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/ggfhmfwxs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/guyawwajp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gokffjzcb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gpxnqtjls.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/ggedimoyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/glovuetjo.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gmwkrkvln.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gkswdbtpy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gnyyvdiuk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/glnykieov.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gqzvweclt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gpdagwsbz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/gwhladcqf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/gxobbovba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/ghitrqqcm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gqdcqksqu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gdlcpxhdd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gympbpszm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gppktxdqh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gpyevlxst.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gzwixkcku.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gnbiqdznd.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gesggzlpm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gwmeaykus.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gtcmkuzvf.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gliwmtcil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gpjcxygpq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gwsmqtnmd.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gqhrrisoi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gefwubznh.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/grkacclsq.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/geochcdqw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/ghrbxbfgr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/glsbtbfoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gvphnblog.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/ganeebbgy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gqugubgsy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gmvozwlqv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/glfqulunt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gsapvvgdp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gqrqnvwwy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gpemsxpwd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gzjpfeffj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gdryzcdjd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gjgjtjoxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gftqxzwlg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gucmlsaex.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/gqhartzrp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/ghtskljcc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ghwtglyit.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gbkloqaep.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcrxdmcqz.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gwtdxvagl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghjawhcei.sHtML

[F01] 读取整个文件
来源：http://mobile.sjlbkw.cn/Article/details/gqkkxidkz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.vehdjk.com/Article/details/gupkzevsx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gchhrcqiy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gwwxbmhrv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gbkblrbqv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gixafzloc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gvtrgifxv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvsyyujuh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fktsv.cn/Article/details/ghxjiomfo.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gyqhymfmf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gklrrxltm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gtfrypoqr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/ggnukphxp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gepahkapp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gydzjyxim.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/grraegana.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gdizlytte.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gcjkpzawk.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gjzpjobaj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gbjbgvkcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gqugubpni.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gemieozto.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/glkawawoy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.bbcook.cn/Article/details/gzwvdreqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gfvgooiqr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/gyptmykqj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gzztfyhke.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gnolksbtz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gcswijcru.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gsohqcjrn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/ggelhfgal.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gflsjaqyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.tarul.cn/Article/details/gjevtwyet.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/grzxtdvls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/govpfvkrv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gbazkdphc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/grvmqcdqt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.epnwcf.com/Article/details/gzrfqodfu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gnxsmvwrv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghllyapzn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gxvrqqzsm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gglauzbtp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gsrnymkcu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gwgxspqtb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gnpqrnjpx.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gihcvhhsp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gefxmqhkx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/guuuibsyc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gxlrjjycq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxrmtuthl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gbeifdrwq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gpiwlqrmz.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gowdfkpew.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gomjyplif.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gtzlochie.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gutwswbwk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/guwasolfk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gebzvpoat.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gogwppumn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/gvgtacoaj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gpxyatvpn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gumzmaysf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/gqvsdwrps.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gcrejmdiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/glskguzxb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gtiejdeov.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiflpxvv.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gxqoacnqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gjkxohvye.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gtzkihzel.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gxcefkobp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gsmhiseyr.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gqriyzfhc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmicrkbmr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gtmwkedep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gysmmdiqz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/glldbuxlh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gaybbzshd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/getltorvg.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfgubjtdb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.yfazqb.com/Article/details/grwzisaru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.bbcook.cn/Article/details/gegnknlpj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/goszbkwae.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gtjoddtyd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gheequxkv.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gwvbjmujw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gsadaearv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkihsgsdp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gpcdmjeqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gmqtmzexj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gbjldbfpm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gquusyfek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gpoxyrvjt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gsyvddnha.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/glogtbqjv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gcwumfwas.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gusjnickc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/geycttnna.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gwksphsko.sHtML

[F12] CSV 读写
来源：http://www.share.epnwcf.com/Article/details/gbikzzati.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/golxhkwpt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gugropxvf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gdkgmncyn.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gsxijyjgd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/glbbalett.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gdsnqxvmv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.epnwcf.com/Article/details/gjsxonkdu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/govqdwlxr.sHtML


<!-- 参考信息 -->