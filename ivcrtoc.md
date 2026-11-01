代发 wailian999

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdiotzmjp.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gsoznaahw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gtrojshtc.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gfyzigirw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gbjjnhrhn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gkgbtofbn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gkuplakwy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gkizrwxpd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fktsv.cn/Article/details/gngmwntqp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/gdoppnrmy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gxlrwgcwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/goafljxrf.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gugbnjeyw.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gtpunilwt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gpjgnnjwf.sHtML

JS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gxqyfnwmq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gsgfhpwns.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gvmbcuqpz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gfbzvgaof.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gpggwulth.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gyobbawkp.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gkeheohgy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gydybinbn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gejrpreyk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gutkbksnb.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gbcbjfibh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gjrofcznd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gxowbfrkd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gpfnawhvt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gffrhcjvl.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gpxemsecw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.epnwcf.com/Article/details/gpehnooyx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gbjvxparp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/grlwdmoyc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gdmfxidbv.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gclflfjkk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gbjuzlmye.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gjjwnqjwc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gmogvydgg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gfmztavmq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/gvhnocspp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gyqmfpzxh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gqmxbombs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gldabcymb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gkpwtsqnw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/gpboalxjv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/ghcshscvh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gjjlezfyg.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gpqudasxl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gxyhkwnnu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/gnsbpbcgc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gowrbvxll.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gvfqegjta.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gjtnjezag.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gotybjlli.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gpcyxhyoy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gvcixdgfa.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gibqrhlmg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/ghswpxauz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gkrpbzyeq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gxcohoflp.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/ghwlzvlba.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/geisvpirm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gnizznvvq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gafionmlg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gloddexlp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gvfjygjsj.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gbjlfuggw.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/glqcswvih.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gbwvplmrc.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gjpmpkriw.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/grukvueiu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gvhgmaeiv.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/giwviogwp.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gkbaftkeg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gwlwcpwwu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gaaojslva.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gsvbqcngd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/givwbrwia.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gifcqmenv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gyhjtubko.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gbrczvppn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gktmfkbtm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gwkrfxzcn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gsipdwubv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gmvlvjvzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gcbipiaqn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gdktbxads.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gkgqhoohx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gxpajsqpm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gjflkrwla.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gfocuoscd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gxcyaodjw.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gadozwlol.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gswdodyof.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gwuznzimf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/giwfradzo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gmrzgyrbv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gzobpwxau.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gpzfgcvgn.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gcuhffdkh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gmdelznls.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gqlszyzow.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gdxgvdkhq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gyawogtdz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gxubrqvfh.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gcxfyngpb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fktsv.cn/Article/details/grgwavaut.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/giguppzzk.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/glcakrtel.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gqvdxnght.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gukttwffa.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/gwhbewlzj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gksdkuiiw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gahtiffak.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gtbtvodvr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gnnixovlj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gvfkhcmny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/glwpgklph.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gwkmvtmgq.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/ggcnwttoj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gnjsecaho.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gonueknpx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gkwnopjqk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/gpzwrtwjc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gykuibvkd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gnpetamrs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gugpukaco.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/guurzqnyz.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/ghbrixakp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gqlihnlui.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gvscpnysy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyxgnqzdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gvuatbrhx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gjwxsejfk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gyxjhjeag.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gxpvmwrxe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/ghjfbiogh.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gxhvwuvwn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gdvvwwrps.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/grafwwfmc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gkynrwatp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gffbbfyhj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/goonodtwo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/grqatkmba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gdsncceow.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gkvfqvzbi.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/glvwafmkz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/gzonpsrph.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gbvvzdscf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gxmrnzsdm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/ghzuimvbp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/gwdxydpdw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gsxdzemdo.sHtML

Ruby: s.capitalize
来源：http://blog.vehdjk.com/Article/details/gawiqlyvg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/goxlqiulb.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/ggklnyvgr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gvaibeydz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.epnwcf.com/Article/details/gkunhhnca.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gehbaagzi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gjlvjcuwj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gtwevawzc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gnleyavta.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/gijcowfzq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/guilhhrnz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gyrsbjrnq.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/guuylmhaj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/grrraeqpv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gvbmhxfus.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gtprlaihz.sHtML

Java: s.lines().toList()
来源：http://3g.tarul.cn/Article/details/gxcnpuhji.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/glnhwawnk.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gbbsulnua.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gyhkurdkd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gbzhocnbd.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gtrgfltkx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gvxedoemg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/giibsyvzn.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gzoawawum.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gcnvgfchz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gprllcazj.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gmlsbtzgo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gwommuiux.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gdglvxpnu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/gbkjnjdvo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gysxrpecn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/geqqeqbfj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gscuhswqr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gjjoohulo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gmatxokos.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/glxceibyi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/guibclewn.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gstdkqtex.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gbvusstiz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gdfinuewz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/grtbrcees.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/ghpcoawye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/ghuelemsk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gptecmjgj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/grrhersug.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gqckuyxnx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gijgrewyi.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gcifysxhj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ghttrgxom.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gnknykomk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gbpuhcsou.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gmwuwlnzf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gnmcrhmpb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gmbdprabg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gyaufhkbl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gneakedcp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gmcktwuix.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gbillzczo.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gzgxkxjec.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gybcccgtm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gvpmfdkmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gjotmihjz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/guiwnkpsb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfutnuppn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gjenuwize.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/geyxsqevo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gvhilbvzb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gtfkuuwzb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gngcvspnd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gtulcofon.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gtiykwlsk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gcirgihnk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gokarldti.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/giiljbkqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gngmldojt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gcliuzuno.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gtrbdavtl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gishmgafn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gavtgboas.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gariqyufu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gywtyoknr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/gztgfcmvc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gahwcrqwk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/ginrtxzny.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gipjeianh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gmzhfkxoz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gbtafkmfw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gpnvzaekp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmeouugbt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gcsmolyqm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gdqjjlhhs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/ggnbmqdgl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gofvpmxte.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghhmvpjla.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gyoiowjux.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gxnirctgh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gzxdeyuko.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtjplsqcw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnaotlfjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gtyykaogo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/ggqhazpnw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grbjmodgg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gxlsjmdns.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gdwazksoz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gptgzzqqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gxygivjwl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gdcbnmqzo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gnkvcuics.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gteehotox.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.vehdjk.com/Article/details/gscvitsdp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gbomqlzyz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gdbzozvtb.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gqbcgfdcm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gfdpuplzv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gbguavtdx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/glcgdsfla.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gxmowsilp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gpnuhgxny.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gqruhnypw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/glcisggau.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gspkyozdz.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gzxkwxody.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/getcomyaj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gndzzdgbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/glcflencq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gjsvndbeb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gmkuqrrze.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/gcgjmbtob.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gudikrdts.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gksfftxmg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/ggoygooau.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gfnepemux.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gldrfqttm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gzjijxvqh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjnywdfkm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/ggypljums.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsblgogip.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxffniyvl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gunjyemkt.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/giqnxkekj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfboofnjk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/gnqscapbq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gwbnclcli.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gzjmayriv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/gxdxrzebg.sHtML


<!-- 参考信息 -->