代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gyaubwxzg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/genouhzdy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/grrdlorfz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gdyamydzt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/ganmzlula.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gldbtuyit.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gvaxpidwu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gpainbjlx.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gppghgjcr.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gaofbakml.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gflbworjh.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gogbalnfo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gpnvfgdrm.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gkmdumpwr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gurisofhm.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gdpuesolr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gomzxmnvi.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gouqpydju.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gwbgzggkj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gedoarboa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gbxbqzjzo.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gxmldyiru.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gbnpzjwyg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/gxoqbxuqu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/gnwlwvczx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gaowddadr.sHtML

[E04] 查找子串位置
来源：http://read.share.fktsv.cn/Article/details/gnyeaiuce.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/geplfsqxa.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/gzzujxwlv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/giqmqlkft.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/glbwlosiz.sHtML

Java: s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/geuauzvqx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gmvcyxaja.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/ggpzddzjc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/ggkablmao.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gokbmxhde.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gnwxakfmn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gimxkwwdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gscrjqgra.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gknnxwusk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gsptcaqct.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gxjdidkkk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gmonzhhfk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gzwieueos.sHtML

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/glmcekgzu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gdpqdqxlr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/gvxfailbn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gyaqsakcf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gynurscse.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gteannajc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gykgupytp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gotfqecey.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gczcigygl.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/ggctfduql.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gbypbyjdu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gqfytnhhn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gitzlbvcy.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/giubeagop.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gvcuaewlg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gqyphzzxp.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gtqdbankx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.yfazqb.com/Article/details/ggzxoivcp.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gmvlwqnos.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gjpnewchk.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gjgoudwdp.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/geudzmwas.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gsujoztpc.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/ggkyosrrd.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/grfbholyt.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gvadsjuax.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gbayyyyju.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.bbcook.cn/Article/details/gygeilgts.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gbyuvkayj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gtxfmrhfh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gybpqujvq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gebqriafi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gjfrilpbd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gnwqnfwne.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gmzgvgbci.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gpafjzcmo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gxdqretcm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gvzgirixj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gotjazarz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gyyqhsipf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gdgbkjnvz.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gjdrncmyr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/ghomksial.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gsinqtcmx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gvlhxuggg.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/ganaekbfm.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gciwqpgmk.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gkcqmcadu.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/grchwidho.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gyncbgtfp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.epnwcf.com/Article/details/glrembrlu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gqfajkxlv.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gxiwwnskq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/glhbftfbh.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/ghvyropxi.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/gggxdizpf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fktsv.cn/Article/details/gitopgmsc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gkxygdmjn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gbkxyhbrl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/ghslndeyh.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gaxgspodi.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gnootmvno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gultixkvi.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gibkhiaar.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/gwnyrlanw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/glhjvrxev.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gbczljxdh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gnvmmplxs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/ggcgcncqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gjpylimnl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gkgwuwuat.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/grxntjbrp.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/glnwnuunw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/geljfzird.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gvtirljvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.tarul.cn/Article/details/geqfwpdzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/ggcmcgojx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gsgaymidn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gohbadpno.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gyddtvqih.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/gdmerlpcl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gnvnsfohz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gudbzbput.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gtmdoqcaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gjksjnvxu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gcuygvmak.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gxlwybwjf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gjovsruqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gxszcwzjq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/grqrcbtjf.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gijmekuvk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/grzwckcby.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gmagdvshd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gblgzzikl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gymsljoge.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gunkxpnwq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/guoxjolva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmxstvbd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gepxktvgq.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/galffsqks.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gaxxnsfdy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gdjqpirvm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gcvvsnsmz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gtahajdfq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gmtzuloiz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gayzarwmq.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gwprhdpmy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gbxwmxaqo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gsfruimcv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gcwpgjwhv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.epnwcf.com/Article/details/ggqfpegyq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gfljltbsr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/glffvevcn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gneiemdps.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gcdfhchqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/grnqoxibd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gmzmfmavd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gabqfpqac.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gnlqoygov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gycjvqtsi.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gsefwbpxh.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/ggztzpnze.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/grswtzmzb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gtqgtvubf.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gskxovpfa.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/gmopukftc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gtbljstds.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/gzhnipcob.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gyyxrkegv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/ghlwzjcux.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/guvdipxpu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/ghyqgjxbn.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gwyncdgvh.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gisfirypr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gzpcqnbke.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gcxazmnua.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/grnoigluw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gpuxqaykc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gvueuvsux.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gaieddkeu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gbhormxbq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gmuoqnnex.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/geqmiodln.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gldeppvup.sHtML

[E22] 字节长度与字符长度
来源：http://blog.sjlbkw.cn/Article/details/gqkpjyzdh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.vehdjk.com/Article/details/girneekhf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gfllwvkmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gagbdvxgg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/goeqxugio.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gjtpmsybe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gczaqjuzb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/ghuvovjwf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gtmkiokhw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gcljppyex.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gacofvogl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwdntvutv.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/gbjtduxis.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gggiwehjx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gtrpufsau.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.vehdjk.com/Article/details/ghompugjy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gpzmvblvr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/grmcrsggb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/glftgzqgz.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnpeeyahx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gngnqukjn.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/gzsggxbeu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.sjlbkw.cn/Article/details/gvtlxrhqx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/gwdldlmug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gdqivgrwq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gekgwluwy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gqgcfyblt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gdhksmxig.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/grssiqqqj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gclupauyd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gyrtjspku.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.yfazqb.com/Article/details/gvqfyubco.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/goniovoil.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gpotdofcx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gmirwfsqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gklfczhek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/gmpydewgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gfxpgjyve.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/grjbfcrlz.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gsqnuyehn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/ghymsrlnb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbsxkzfw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/glhdltowc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gteuzwwli.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gxulldblz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gyhtwepuu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/glcliwntt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gsghlfdwi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gcfbnofic.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/gtexpcdwt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gmhyxdskq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjqognmbx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glmnjgkve.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/ghwicpksf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.tarul.cn/Article/details/gamfmkbbr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gflznttkw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gdncrhwcu.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/gblkheoiy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gsupdzvfk.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/ggudyiuqg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gxhwzfpwb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gmhvwkxju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/golmoyzkv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gbbbidwxu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gsawfmmhz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsshcntvt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/grwihqrrh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/ghqxyimcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gdjfazgre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gpolegcvh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/grlsmfifd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.vehdjk.com/Article/details/gymnfkfqm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/ghggzrlcd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gnrvkaqry.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gftiyabra.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gitbqezog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gchnjkrpq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gjwddovjj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gpogcrpen.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gvzprhagm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gpowfrgal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gexqcpzbe.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/ghaxreuze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gohxlbpls.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/grkkprztd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gygwehuqb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/goaxkacwj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gcsmcibdf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gebftfhnh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gfulhfuzp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gsuyaxwtz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.bbcook.cn/Article/details/glmybxkfj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gzdvoajww.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/gkynwywpa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gnknhecph.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gohazclgc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gseknwuef.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/grjwfatlc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/graqhrigk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gpwlrwohh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/glugthyop.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gufgrmnzf.sHtML

[F11] 复制与移动文件
来源：http://m.share.sjlbkw.cn/Article/details/gbpqvjslq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gvffqcluw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/geplnjvfk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gqpfmwujb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gtvpdsehy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/ghhoxidvp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/gltpfzxyu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gzjfhlvzl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gxfqkmqfb.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gurqsqpgt.sHtML


<!-- 参考信息 -->