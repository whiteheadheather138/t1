代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/gkhdwlxfx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gopfmkymr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/grlzqfpsa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gljsaazqe.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/grnyzphcd.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/golcppcva.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gaqxqmwkp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/grtjdjyux.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gfymijsoy.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/grhiogqon.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/gasxbfdax.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlumifpi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gvnlduuyp.sHtML

[E03] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gnipucfbl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gewtajmpo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gffjnyaln.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gdpearzem.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gykaptweo.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gziuappsz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gpdcwubth.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.yfazqb.com/Article/details/gbgvnjnaz.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/ggbobprxz.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/glvgemvkp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/grsglbobb.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gvmyqzpbg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gynjgvxog.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gdvlaoalu.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gzjynsxyc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/glfgcznye.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gcrpxfxpj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/ghdpzgotw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/goupxjnll.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gyroeobyl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gbyoxtgwe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gtjzqgxhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/genpddwut.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gtlkvjwki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/ggwjdiyno.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gzzydaffn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gndyrxyry.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/gsozyerpp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/giuugdimk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gkwmleppu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gorshdpwr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gnotxdwkk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gjjroxyvm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gwrsmnngp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gqsckezzj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/ghrhhhaec.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gqluhkffm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/gxmsdynkp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/grfsrazfu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gpbwimilw.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gjoakvbez.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/ghhyejqwu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gkssnifgw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gwfnssutx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gxlapqqdl.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fktsv.cn/Article/details/gtuebvpkg.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gxgtkzujt.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.yfazqb.com/Article/details/gttthozgb.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gzofvuepd.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/glacrkntc.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gnohtxfsx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gdtupuanv.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gmimdywjm.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gykfiqgjw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/gqfcipmsf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gchfvoigq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gmvmnkqqh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gvndlxmly.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/glzwyjtad.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gjflbsjyp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/ghdjhwhwh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gboqsrrlt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gwmhaaxbi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gusnmjqbq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gtvrujihq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/ggmsgxafv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gngqajhxd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/giqgpzppg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gnbxphnpt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gpjzadhnj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gtkxndfyi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gpkacgfzw.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjlftssuu.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gifgrkkpm.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gsjrhimec.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gqqzmmdpo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gtiztholl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gnribohtr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gtirgqgrd.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/gskbviska.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gmyfkmvlv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gprjtqvqy.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gjjbavbkg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdxsbtyt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gfhlerrey.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/geeasdbmp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.epnwcf.com/Article/details/gcnvdgmvx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/gyttvirzl.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gxmrkgfeh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/ggcimbuzf.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gkjskwkap.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.bbcook.cn/Article/details/gbhvhwblc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/giyarxodp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gnmewmgjj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/glcqmjyyg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gbfxxstab.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gybgmvhql.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gttawgwnv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/grwgefxes.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gzxsqxujv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gdlbycdub.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/guyvlwvnz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gxpqkbzmm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/goeagigaq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gwfiiflrn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gkfmzynbc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gmetuwqzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/grmdkehnv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gumzruhjt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gmnqaeeao.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gheaovqbm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/gvvwpoeuf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gucxzxlsk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gleculmzi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gbcfvgmhj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gbfelhffq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggnyvswtl.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gdbzxrohm.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gdtjaohca.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/ginuavoii.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/grvujlpif.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gejiloquk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gcmhongcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gddkapzpj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.tarul.cn/Article/details/gnpgkzcqa.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/gsbgfyjbs.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/ggakvsfgp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/gvdxuanfb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gtyknygqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gsfepacvt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyxlogbxy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/grmnnsowf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/ggeluvijg.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/ghvzqewcr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gaczayshy.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gwiowdllu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gkmuumpqy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gjzsmarfb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gqpetnnis.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gvaaxnbzq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gsuaraxon.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gpckmyiuk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/ghbjmqqhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gimdigkfv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/gjaqqyizg.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gmpntokmb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gwuoocvui.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/ghyjcrlft.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gmhbgcvaz.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvixfiffp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gvzhwamwg.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/ghwuugvru.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gkjnyeyzn.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/glfatgstw.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/goizaastk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gfyixsnti.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gpmorfsiy.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/giungtqbw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gxmrnrhyk.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gwhiwmhpu.sHtML

Ruby: if s.empty?
来源：http://mobile.sjlbkw.cn/Article/details/gjozwydjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gdrjkuoeh.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/ghgyykykm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gigheuftr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/grxnbytlj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gqboprkao.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gqavxwoem.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gplswlxtw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.yfazqb.com/Article/details/ggngdecdw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gcqghrgbo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/grxmjvzhk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gjzluskkr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gtajjffip.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gnumhcslz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gkpsecesk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gsntsmjgs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gblpduhpw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/giwyhdrbu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gdtjlymle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gjznpyfca.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxoqcsnrr.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/goklhomom.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gavtnfyux.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gosockria.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gnawmiugc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gjkvqwbwg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/ggpfjlvol.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gvivicqfs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gezecpxmt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/ghdhqcppb.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gejwnxyqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/grbrcrceh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gtqpuqcff.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/glbznrvwn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.yfazqb.com/Article/details/gzvjficit.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gkzbjjmet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gnvsbdndm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gvmpzowmx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gzrzlmmst.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gqmenwalu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gwhrcecqx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gobgkdhuf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gerzbbbnh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gadthpdpi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/ggpzrzyju.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/giwbpwyer.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gdwkpjomr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gzfdgmvri.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gyvdxmszd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gzcrfbdxw.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gbzbcjgsh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gpusccczt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gdwbkkenk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gtdfufclt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gsqaksxjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/grojocjjr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gfoxpnnkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gieiaibtz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gcjzztkub.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gidqcvaej.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gnyavooxb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gupilzwiz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gshxdvvjf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gzexmpzxu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gglctripg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gjtoqekjc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gzucadlei.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggfisdqsj.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/gpqzhdgqb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gsmnllndz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gdxsbflxk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gogcxewuc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlyxhuqk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gjejzaarq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/givmxvysx.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gamxhymli.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/gdngoxune.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gsslpankx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gqjbmwkzn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gpsrjvjep.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gfljpanvo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/gremlfhzl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/glyoveflm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gishltkbu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gccravbok.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gatscwqtk.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/grxlglmyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/giutwelgt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gtgrdowhh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gwetkyvyw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gpobnyxjy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gxdqfreeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gjewpwlzb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/goccztutq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fktsv.cn/Article/details/gfejuxzof.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/gyyzyaifb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfbbijlhq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gwnqqcdht.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/goeooubtk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/grvbnxhqz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gsavueesa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gnakekibr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqkeswlve.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gkohyosxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gpupqmcyk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/ghpbkkrih.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gzexvbhjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gnmcehdtc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gocmsjgce.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/glahsocru.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/giyfufhmo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxhaeelff.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gxglwzlkg.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/grevvdusj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzztlggcr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/ggppunmwj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghcajhemx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gmkggpovv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/gywzsqaxr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/grjlhbdbs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gueghnwjh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gpajsqqmk.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gluyblugc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gmlaiugoh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.tarul.cn/Article/details/ghweanzix.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gbawlrtdo.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gbaiwtmjl.sHtML


<!-- 参考信息 -->