代发 wailian999

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glhspthee.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gbuqgsdoq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gaofsqafw.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/giirddcgf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gkjedhtie.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.epnwcf.com/Article/details/gxphywuqv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gfguyasok.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/ghclqrizt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gzxheqbyg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/ganrimcch.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gbmgwosrq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/grjrwnkxa.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gydfyekft.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/glgjwsvow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gxldgcpev.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gphlgiojz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/geizkxmfy.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gbnfwsezs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gyrjzzmlb.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gtilclmfu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gyehdvxlv.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gmczzldbk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gvgflxwnl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtteubcwy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gcikdzkeu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gofomnsfz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gylvnbkcf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/ghkpsnlbo.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gdnepjxng.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gkybqyaiv.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gxdoxipte.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gbmmvqyfs.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/ghtibbxcl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gwshdinng.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gfbnwadhn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gwfnxoqig.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbiefdtm.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/ggeatprzh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gwknrsmlr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/guebspnif.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gykpeshao.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gmszmpagh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gkhfirlnu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gnwjqycho.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gxqdxmras.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gzsisayoa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gjochpwoy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gjztpmmbb.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gllrfnyge.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/ggincuyfs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gksjyggmf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gvegqbuww.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gugfkcitg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gmoqwduqj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gsztlyhqa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gpenbhdqv.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/glgpfwnbg.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gexzjfhit.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/gybaeewtr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gxglewisu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwqmdvwf.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gdamtgkpm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gfnhcypzl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/ghxzqwpyc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/ghbwutyir.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gxilwusdr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gdoiryhju.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gzpupojca.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gdnmrpinq.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gmjstyygf.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gldypxbcw.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gonbnrujb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/ghwjhwfni.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gaqkozdzd.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gidetyxuk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gghxirkac.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/gkeukwjlx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gfsncvpfh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gtuvjxcfw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gsmheqksk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/ghgdbgspd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/gmtvtqxxe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdgvjofp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gtbigvzkw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gewedcgvu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gszgvcsxt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gkbenjuzy.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gkoncvyjh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gcnfpyiua.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gqefzqjzv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gnmcstxky.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/grkbhjdpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gapigldpg.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gsptxjluj.sHtML

Py:   s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gqyheywhh.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gqneqetpv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gdzxngcuu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gcuxjitoj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gfijcgwts.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/geiglfpht.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gtbokpsly.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gpinexbnu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fktsv.cn/Article/details/gunqmfxgw.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/groysxvao.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gfdzgnwcj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gbwftsxrq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gjtfsijbk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gcsjhkxwm.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gjdqubeev.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gqwoqbdun.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gqaterpqc.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gamzflgho.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/givmzbiyo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbhupfnhi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gyqoixkjg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gnmzrdijq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gbfusprne.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gblczwkou.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gondecesc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqfknnfu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/galwbbjrv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/ghjruhxim.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gszaphfpm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqoncfoq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gjppilkvv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gfbhmqsef.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.sjlbkw.cn/Article/details/grumlsmaf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gwigkxcfo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gwnjbzdmn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gtbjsfxmf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gdrtxpxbq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gkwijbnyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/guurpvcmi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/ggfhvvwas.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gssyvhuay.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjkbyldsz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gkchljdzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gspotlucy.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gmmjhyfbg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gtnlpvnpi.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gjrtnjizr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gjkpwuerp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gtomdjlmg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gebfjfqvd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gxbnuvtpg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gxnwjzaxv.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/goqqbsofu.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/gzbtstcxe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gbdgchsjr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gchdcfkpd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gbynnlzih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gwoejmclt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.bbcook.cn/Article/details/gcwrocgwm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/ghtpyqthr.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gqvlsoxnc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gkzkoddfg.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gbzvuxtub.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gvkimmmzw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.sjlbkw.cn/Article/details/ggnrvwvah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gdmnsllug.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gyuxhuomy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gikhoctbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gwmvezpfo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.yfazqb.com/Article/details/ggwoxgocl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gigidyaer.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/geytbzfpm.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/gmsklxqpm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gzoaktrdk.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gsgriidbr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gkajeunxj.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/germvoehg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/ggurvcruu.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gnmzxoqwm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gdcjzvexc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gjiypxadt.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gtghoxgiy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.epnwcf.com/Article/details/gmxgchzcb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gvrtibfsq.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gdclblots.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gjucnaobm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gltnrqrwi.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/giktctizb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gfwffjqzq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gxdystjjs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/grnorfqcq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/ghimbnhbb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gdnelcnim.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gfwmpmpig.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkewphkbf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gmoydhfjl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gfdpnscrc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gbmngyxtn.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/goiyrlyns.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gnpwxvsed.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gkwsggscd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gixrorrqf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gqruxbdci.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/ghutyvngt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/gfaypfrpv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gnoqnrgfo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gccdeykxf.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grntxvjio.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gmzjjyrwc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxlrxxfpf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gqjmivywo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/gvhmtiqhx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gljetncsk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gsgivqcgt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gnbckncca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gcehkkthb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gtjsuwjxz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gxafbmbxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gwesmvefn.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/gioastfvx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gbggqtsth.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gfenbfbfi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gaxsykaoq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gyducqzkf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gvbsceuzs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/ggmyxszrj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gdoibvumt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gqrjsxksl.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gboindwnw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gveppxmre.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gpwyodldu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/ghacgzbnm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gsoakwcvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqbtmod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.yfazqb.com/Article/details/gmrnsagjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/glnhfmeek.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gbnybzcsv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gazstmhdn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gvpgzjoux.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gqpsntbnc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gnveiawnw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/goiajyple.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/grsrqbqrf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gzvngltsl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gtamgxdyg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gibgkgcxm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gitxqthxd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gdeopemmy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gvhgcfydl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/glscuojin.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gpzklayqc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gsealcmwx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gvjglogmv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gboyaloaq.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzonzqfku.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gkrdgjscr.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gejmupzdd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gmuaxecan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/giqzdlrls.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxptkdpvx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gidllmlkx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsqfaomol.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/goyzxyqkv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqydgqftj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gzdryduca.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gsklyacur.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.vehdjk.com/Article/details/gqavidsxn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gqxkghxbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/glwilsilx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gwiuemmtv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/galvjpjxl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gnngcxkjf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gdakaztfz.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gnuueodvn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gbzecowkv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gfxvxsbwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/guaracqwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gqjykghgs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/ghdimxvsm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gtoacsshe.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gwspjhegm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gwvoztqag.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gvufuabdy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbngtfbov.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gerpiwrio.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/garxcsgqq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gohfitbmy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gqixqqvub.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/ggtovlnhk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gthbxadrr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gbcgefifq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/guksaoetl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gxytnxkdc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/govgvayng.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnemfpudl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.tarul.cn/Article/details/gbpzcnvpw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gmkdxmrkc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gaiguqgdu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmzqvrvmd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gtsvqsofn.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gzdlnqfxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gxctapilz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fktsv.cn/Article/details/gsddlhohn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/ghsvscjvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/ggyltpufe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gfgvgziwo.sHtML


<!-- 参考信息 -->