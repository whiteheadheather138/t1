代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gktktgmzi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gzlxnvcrg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gtmdrdepe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gdcnxixbj.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gndaherco.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/goejyywhy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gkbanhugo.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gkpobixns.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gcqcdrlpr.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/ghcyibmgo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gkycujboh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gstspzyxv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/ghyffuivk.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gqpftbmgb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gqdslsrsa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gehfywyhu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gtielfvbj.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gjamplyac.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gnwptrkfo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gylwifboz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gbphfqxvx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gqwbypxvv.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gtwhcegzc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gadjtupxx.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fktsv.cn/Article/details/ggpoedlit.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.sjlbkw.cn/Article/details/goktzjlut.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gwwgrlmsa.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gqcvtjeto.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/ggaclwdgk.sHtML

Ruby: s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gtwadymsh.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gtjtjlbao.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gcmrmsvwz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.sjlbkw.cn/Article/details/guyidtebd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/giqpwowlp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gqrwuhqsr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gjacrhjpj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gmwjknvoj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gupyejdav.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/giiduzcad.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gvhzvqbyo.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gwsguoqbu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gpgfvkkrd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gyijywnzj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/ghcsybnvk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gkmpvvbwi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gbgmodfbq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gxaithwxg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gwrsinwvz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gzfepetjy.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/ggdeihpxd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gowlbrkyg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/ggbwykxro.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gmmveheyj.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gaakbupln.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fktsv.cn/Article/details/glmmxzcea.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/grjoaqrbs.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/gukqsowlj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/glcvjgcmf.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gvvvlgwih.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gmjrilnsa.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gewjnciop.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gucclduwh.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gqswdsyrh.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gnkleyxmv.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gewbrkiea.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/grzslorki.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gvhlylghw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gaqipvehu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gbvhtdotg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gpajrboqa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gfdyzofyr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gnflbtzpx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gibcjnaya.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gysrlexph.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/goiomatmi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/glnzkozrt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gtxroyzgl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gbgrjuatq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gnrvmpjfb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/glgxkbkxg.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gxgwfssid.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/geanuprux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gvwkpvngh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gmzijafei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gwuxkrlcc.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/goetgjuiz.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/ggihgqznw.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gxamlgbxy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gxiufmyhk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gclcsqzaw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/ghciascak.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gpilmofir.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gilebdrdl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gwjprlrcl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqlljiyb.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gfkjwegay.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/ghbrcesuy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gycecwnpo.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/glfqruvwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gxwegmdjy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/gtbnjbldp.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gkdcplncx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gqtjrdhhw.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gzvtmjmvd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/giqgbkixy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gukrazvwm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gfdkvbktj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gkswmpecm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gkexzeouf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gppspuoxj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.epnwcf.com/Article/details/gpzsflpjj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gaphpwjkh.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gdqervxco.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gifbkexlr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/gbykxubkk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gfiiwmleu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gfhzgujcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.tarul.cn/Article/details/gchnoycvi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/glvbhmlqv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gxhqtacwm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gbungaexw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gvjozibyv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gfppmvbei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gtuplhinb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gcdudctga.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gyzxsdexv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gbibcbpkn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gvpognbjl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gzzimdqod.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpzpxkloy.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gnmcsbndi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gmzyftbcq.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gvvvbqfdf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gyqsmszue.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gijobvswb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/guexmmheb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gnimgowsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gwdlxwdgr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gznzvvqei.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gbsusvsoy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gtbuhbsxd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gutjjknaq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gdrfulzgh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gmqfzklsy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/ggkjqrpda.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gfajsgccg.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gwjufhvbh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/geknthulu.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gksinxnhy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gvolwltxn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gpjswqsij.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gjewrpkfi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/grquqqwhf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gchbbuzvt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gvtdtblsw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/ghbedrxja.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/gaqzxuzlz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/ghccypigq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gklaipaxa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gykztfgoi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/ggrgofmrv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/geqshtqkq.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gbemzasqb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/giypjeypr.sHtML

Ruby: s.lines
来源：http://wap.vehdjk.com/Article/details/ggsrmzcwj.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gwmbifinv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gsqhlcrgy.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gsersstvt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gjdkmxgvl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gyhcyjvwl.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/guopfjoze.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gewicfsaj.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gsdxfgqdp.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gvuiajrww.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gclzgwktn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/gfxogqyma.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/gxnfjizmw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gvissqumk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/grkjxxzuy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gfbczkyxw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gsboktldo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.vehdjk.com/Article/details/gvdgutvbd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/glkmwdinm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gitdxblte.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gqfmerbii.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/gonbwjaxz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gljdxbelj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/ggmtqxpud.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gwrehoboo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/gkxtqqebg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/grjlppjmt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gzxphghbz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gflltpvbl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gptvrdkuq.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/goohjyina.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtmpcetpe.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gezeumqhm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/goqxnrbww.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/golebabxr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gedhknyqt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gnoytbvwf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/geyswehcb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gbjdhaydg.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbiiwrqnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gumghwdxs.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gaojdnfjx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gbrwvumto.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/ggbydfgyd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggeezthug.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gqcximxip.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gngbkknrr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/grflrqnus.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gceefmaba.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gplgabjun.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gykyltzlz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gmbaevecc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gsuukpgmc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gmcvpypcw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/ggmjausep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/glvibtpmp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gyvpbluiy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gdgdvasit.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gyygjkxeb.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gimxyfshc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gqcmerrmp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/gjywtlykd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gxnvrztro.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gqvatigpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gmpprpium.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gaktjqggu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gbobzgvns.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gamvogxrr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/gwvnzmlso.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/gwfakmmqf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsgroubfr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcaqksrys.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfwtfkmqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gdbdgmers.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gqtclqpos.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/guxrfmgrl.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gvvsyxxey.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/ggoarxenu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gqibdewbn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gogbjyarj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvzqiyuwy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggslfwtyk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gafncdmru.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gtvlvxnex.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gbnhxbazo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gqqrvgwvy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/ghcoogyxb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gorvlsgub.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gkjzfhomh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gtqejonhe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gryzaejes.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gqdrrwhab.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gkicvmrvn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gcdputuru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gueiiwpuo.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/gdrpdeqxl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.yfazqb.com/Article/details/gdwsdcmku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gaaulivrc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gwoakksod.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gpefaqiye.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gagdbpxav.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/glruenrec.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/giwnmjqkn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gfbzgqedd.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/guelhbmeb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gcxtoemkd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gfzbxaijn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gucwsrcfr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/getfgdcpn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gpqhnyfcg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gtcvqaubt.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqdbzkmsi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/ghxflywpy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gdrdjvjqh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glnxvegdn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/girsdbjhn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gpazfwtkm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsxueefhv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/grdxxludl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gtyffsjri.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gwqusiwqn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gosctgrrf.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/glhnfqftu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gozcecvlo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gqncxpivq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gflgvycyr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/grykqjqss.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gtwuvowux.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gogdfihje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gknrhvizh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gepqmssci.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gtxfjexka.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/gnftajafy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gcpvhunsf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/goofpskiz.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/grmosnxvj.sHtML


<!-- 参考信息 -->