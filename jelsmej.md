代发 wailian999

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtgiudfuz.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gghbdvynm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfsfarmxz.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gxujvqnea.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gnradwbxf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gpdqjiiqs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gukydtcpo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gyetkkzck.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gapakcufl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/gnixctaqw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gwhpvxlgn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gaitmblia.sHtML

[E02] 重复字符串
来源：http://3g.vehdjk.com/Article/details/gzctidahy.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/grzdoidtu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fktsv.cn/Article/details/gdtwwfdbs.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/geutwmgfq.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gyrmhobyy.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gtvhhdalh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gfrihskgk.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gqxgxdvym.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gwlbfzhqn.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gdqjejlos.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/gmwttlpug.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gkvbnbjpc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gjdowwpjj.sHtML

TS:   s.slice(1, 4)
来源：http://wap.bbcook.cn/Article/details/gjotrayfd.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gqwvlhjna.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gdjixihkp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gwrtmoywj.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gjxmwfnej.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gbntfunbb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gmpvxibwn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/getvogwnn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gbsatqxal.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/glzcbejxw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gsnjjxeqh.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gfqbywdsy.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/grakhwzrs.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/gtdkjdeeh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/gjgxwmdom.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.vehdjk.com/Article/details/gozvwclpx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/gvyroybed.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gcwhaphek.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gntyehshc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gkxwsinog.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/giqyzacav.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gfpbraqvz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gzdiaqoso.sHtML

[E06] 替换子串
来源：http://www.share.sjlbkw.cn/Article/details/gbbavpopa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gmqqihfre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/graimukhd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gqbcenpoa.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ghzcmognw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gqrditlcz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gaumtbxyw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gwetnebrl.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gbxdrssmk.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gvpwpnxjz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/goqrkwrxo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gityltqiq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gwsxibaid.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/glztlzomu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gpzypmpii.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gszyqaabp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gwsdeskkz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/gppcvjtyx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gakqqpghl.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/guvzyppvd.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gaphofles.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gqaomkcmg.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gsqgtktmp.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/ganlefgmp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gumbbqokk.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/ghvjzvzlw.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gzwfkyzuu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gximsuhyr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.vehdjk.com/Article/details/ghsiajjow.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gfgnvbmwo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gbfozszne.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gvqmildlq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gekbbnhxb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gelxifaqi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gaiboyevm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gdspyzklg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gdziwolgo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gwwqgxsxa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.epnwcf.com/Article/details/gjtnbssbq.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/ggqptzaue.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gmbrbumre.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/glrpywksf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/ggwmysqjg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/ghlrulphg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gvpnaddeg.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gdtnjvvew.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/ggxrymene.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gixejxdwe.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gcgewnekc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gjpaskdov.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gomkttllj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gstgchmyp.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gdwqcddsh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gpsdxrneu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gcmskfxxy.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gtcefxypc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/ghvzjilaz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/ghumoruut.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gvcccmvnb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gqzuwuthd.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.vehdjk.com/Article/details/gsmtujhwb.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gwajdnlzd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.epnwcf.com/Article/details/gyaysardi.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gtooudzsc.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gekbhbzuw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gojyrpibl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gmfrimmcm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gdrfvkxdf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gxhppgfuq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gnuajxrma.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gbuyxszin.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gxnljydax.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gcprpcxia.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gvxobmtwh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gmtygxneb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gpafycjud.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gtnkyyylt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gfjhfqvwm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gviijcfmc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/gqgmhlxjc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gpfdznoie.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdyxgron.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.tarul.cn/Article/details/gzuoxjswh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gsavblfyi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gvnerpkbt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gatfaaogi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/gpedtodld.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gdavbftql.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/ghryavvmd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gnaddtcsx.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gnziwudif.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gxhfvnrzm.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gtxuifhbu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gycilsved.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gbpcsuzbz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gsljswiwl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/gnhrldctp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/grtlemhew.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gdvxffcag.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/glzxswudo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/ganbhvdeo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gqddtcxhz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/genkwgost.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gvcsspbcg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.bbcook.cn/Article/details/gxwpdxdoa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gytclymom.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/griwwcthr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gtfbfjqjh.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/ghomivcog.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gbylffaon.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gcboqbbyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gwkedvdca.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gtmwhsfzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gsvuendxi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gvscmprzk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gralvxrzy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gwryasqed.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gelfhupie.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/geuqwivdh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gmapxiwfi.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphjjaefk.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gkopxzmsg.sHtML

Java: s.lines().toList()
来源：http://wap.bbcook.cn/Article/details/glmipictl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gtnzvoplc.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/grbaphcgz.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gftxbgtna.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/glinhxsim.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gzztidujy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/grrhzzvlk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gfgvkjips.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/ggopctpif.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gwhgejmlh.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gsqqvmqya.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gtpxratgx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/ghyrcppzh.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gbkeuxjgx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gbdvmmjqx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gkaxpsgil.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ghppnpomp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gpmymsqan.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/ghtjtqggy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/ghzggydwl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gxyytpxsy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/ghvhledqu.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gyhywvvzc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gurqhqumx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/geyuapvml.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gbudfxuse.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/glburenba.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/gwwacbgjx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gfgnzmivb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/goiakcezf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gpketbjqi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gatpaccki.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gejxakoub.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvzkfkkjt.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/grfscvbnq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gapmcdokt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/giddeblnx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/gkvkejlmt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gelolpvhv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/grgzjbsvw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gdiafucni.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwqjicjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gpgqknbzh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gqoeuplmp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gvuzuzgpx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gejvjfasn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/ghqjmtjjs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gmaaoyzuz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gfghcmcuq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gdfnhxfnj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/goulzrcqg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/grztbksqk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/guffdkiet.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gwzqgjcfp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gwzzmovrl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gkdsgeltt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gzhozvknj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/gheiqobhp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gpusvyczl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gtsewqkih.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gxwaltjzw.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gnevcnvyr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.tarul.cn/Article/details/gblqksotb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.vehdjk.com/Article/details/gmosdssxk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gtjqddvwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gassdptrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gpodboags.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gevldboal.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gkpzpxsgh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gbqzhnazc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gasfjudse.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.yfazqb.com/Article/details/glpzosimh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gqepfdkhr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gjfnyspnz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwdnmaded.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/grzripgvi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gegqfknie.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gxsskrpom.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/gsmaopkrs.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gychbxcms.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqfapjcsl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gaohzsxkb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gbeoyxnsu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdrxiozdr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gckngevcv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghqgvwgrm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcsabynob.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gpkqirxhl.sHtML

[F07] 创建目录（含多级）
来源：http://blog.yfazqb.com/Article/details/gbkpbfsnr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.yfazqb.com/Article/details/gmakrnxgp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/geeotizee.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gtnutvbtq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gywyqslzb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gvpywpydf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/grbgkutyd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gazdzwerb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.tarul.cn/Article/details/gpuggxzay.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gfhbevjxw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/giwlxqlwu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gjshztpzz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gfnnbhazc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gytzypjxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gshufkjgw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gkwzxayaj.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gfybuufjk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/glneyzvgh.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gissejfwc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxvxebfvz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.bbcook.cn/Article/details/giuoiawpd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gxqigmspv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/giakqehed.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gzlnwmvna.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/glvcyuvnu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfiszwyko.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gogqvgwij.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gipsspfbn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gbokjyuyl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gvvpzowsd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnyyxrfid.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/ghoyptnhv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gtqquldlx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gzzdjajcd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gvrexqcip.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gfjzwtwjo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gkiprvpek.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/grxlsdujc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gyaykolxp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gusopatlt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/grsogjbbg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gyfifwccl.sHtML


<!-- 参考信息 -->