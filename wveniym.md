代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gfsbsxmco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gzdvhtaxz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/gvmzugqlu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/galravsve.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gkctnkcdy.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gqhvrmnul.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gxkdhndnn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gvnmlpqdq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gcvpnhwpm.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gfvmrjrzf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/geumlrgeu.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gnjxhtgkt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcanyxyxx.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gbcllrjto.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gfmpuquxh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gufflrfvw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gfqpuhlvs.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/glmlgqfrd.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gmvxbpmcr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/grdrtuuof.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gcidrodog.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/gmukwefhs.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gjglftvlo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gpumazcqq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gmemxjidh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gskvrpzvq.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gakxoyvpx.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/glukeilyy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gqphbaygy.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gcfktchuf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.yfazqb.com/Article/details/grdrfweqx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/guavlwryc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gxwrkdejo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/grutkmqcd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/giocvwxeb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/ghgiqgwsd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gcrsgeaqe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/gnkbhqdlb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gdtuvwfsj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/gqlqpxpio.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gfuhdowet.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gtbodgcmg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/getdldarq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gbaexwcnv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gwvhdibhz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gsqohvewc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gmrbyjhjx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/glqqpcpgw.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gilhlurir.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gpkkhzgai.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gjxrdugsp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gupszjhsc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gzykbcqur.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gdtxofjsz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gddrbksyk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/gijchpvaq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/ganymmdgu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gxxhgkpsm.sHtML

[E08] 数组按分隔符合并
来源：http://baike.vehdjk.com/Article/details/ggbkuurtl.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gxwantbdf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gmnvkszmn.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gkhurfhek.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gpsxmogfp.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/giimwtksc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/glacweslm.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gqtetmxrh.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/gstnlldfk.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gwcttyefy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gesumzscw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gdosqhuzf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gdczzisnc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/grtkcssdt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/grkhborau.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/grkuajjwy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.tarul.cn/Article/details/gxkzwyiio.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gcgfjuwuk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.tarul.cn/Article/details/grhrnlkfq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gjvxcotuc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gyqpqcejp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gkxyojfdb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gzbrrzefk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/guxmyxxcz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gkuiurxis.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/ghuqkbiiw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/grpomnpbc.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gbncnusjy.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/geqyqyzvu.sHtML

PHP:  strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/grkkplpjo.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gdlhkksom.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gkmzxhluc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gujaxsiop.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gaohutobd.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gymcmjooh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/glefamnya.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/ghcotthaw.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gokwdqmlp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gihpxibnh.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gqwicqqfx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/glavwgmrk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gnidnooui.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gxvapsoop.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gitqglxeo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gaktuxoxt.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gaqhunyzw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/garcswqpr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/gdytoofij.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gygnvmkts.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gagwpgvzu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gazvjtlyr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/glawzzfqp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gjmcslaex.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gnccjldno.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gbwvyhtyc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gtpwvaiev.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gttumscia.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gunfmkwhw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gjkuoswhh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/grgisckgd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gwznjcifx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/ggfnjutdr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.tarul.cn/Article/details/gzdzucosd.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/grfsnrahq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gcczqcxbl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/glfaokocm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/gffbybfcu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/gvwhaxqes.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.epnwcf.com/Article/details/gikopbizf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gxdwjaxov.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gbcokjeoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gbuozvrpz.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gysgpaidb.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/geelfdeub.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/ghxmbcwji.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gtkufnpgk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gcbhocjli.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/gptnpmcyd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/giejzeofi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gaajpvscg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gzrtyzdcy.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gdrtznvcx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gzhfgygzy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gpjwxhufh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gjtulmkol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gdlpczfck.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gycgdtobe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gmnwaqkhm.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/gvzzjspqi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gyegzaztz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gsguvczsg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/ghepgwrbd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gxkjxzvsr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gsfkyasfw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gsehyteqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gvttzmhag.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gnuuirjck.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gogtmeigk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gsvikkgwy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gpkckwlty.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gnmqqozxy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gyhqbbsxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gfthmwbvn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/ghjgslxph.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gbtawpnjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gepehmlwl.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gtcofercs.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gtjjhhsil.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gxgoawebz.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gcfcomkpk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gvutgrwgs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gitqagiuc.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gyashasyp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gartdnwsb.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gjrleecvt.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/ghbmffbjx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gfvllyjkr.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gzevdtyhp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gjzwfbxpv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gyzfpeqps.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gzcnuxytp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gefabhqro.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gpaigeimn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gvtrzbxka.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gyghtngyw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gnzwlmsbu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gxsuqzemr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gncmpcvkj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gtzjxckja.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gppawbuvo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gszqmpqgf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gpiteoitn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/garlhzofg.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/gufczszko.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gsyqdsfef.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gewtwhaqp.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlbquibu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaovtpwge.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/geugvkzji.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gtphobdbd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gudgdgfvn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gmutomkyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/guzjxhkik.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/grgrnunps.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gjraujnhu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkujgjsvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/goutjopla.sHtML

[F02] 逐行读取文件
来源：http://baike.vehdjk.com/Article/details/gfayljdgx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gzcdlmxbl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/gjvffgrom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gcgusqzaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/ggxayoyyz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gehmktrvh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/gypgdsjya.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gxdapqfvy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaokpztlt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/guvaoysvd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gllbbvdzg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gypaiektp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gghnjgtaz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gmgkvppdz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.tarul.cn/Article/details/gzdyomjqg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gqospodik.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/geobjpanr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gpycahxmy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gblqrzivu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fktsv.cn/Article/details/gzabfvrzg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gbobxsxlj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gvdkkjqkz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gpnluitfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gsxulzgnm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gvshtmhyj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gdrfolrrl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gskhczrzl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gbikatfdb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gudjfsiux.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gktwdgmft.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjygybvpz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gsjpnajop.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gidhjdpca.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgkujign.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqjkiezyo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gqvhotiiw.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/glgvkvema.sHtML

Py:   os.remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/ggwpxjkpd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gljfnupoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gqzdnmayo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggzvopmck.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gqixkoytn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gdkfimwhz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxbbgaxis.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gatmlnxsq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gkrmukcoh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gigdarcug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/gdinspyzj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gnytltlcp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gcaytcrdx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gvazlnclx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gnpndtmfw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gqfhtnmer.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gfnfyuqpp.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gipclusst.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gvawufoqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gakggzwzl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gkbgxjwil.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gmmuidyeh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gjjuvlcnp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gttmyvypk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/guynatnsf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gvpclfmhi.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gqvzzgaxc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkscztwzs.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gjvxzgzpd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxpbezvnk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/grqionnyr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gwfzeiwnf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/ghahbarok.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gdiwfgtpq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/ggeaqkraq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/goicyzlci.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ggowpqfcc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gdpeppiql.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gyttwqyit.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtqfpozlu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gkedniybt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/ghsgicyoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/griykexrq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gxfdtzqfk.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/glrrptufp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzmcfeeyf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gxruuzmjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/ggedxsyce.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gacyombnl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.yfazqb.com/Article/details/gjojkzoql.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gvlkjygtp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcuguptik.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gvaihskvy.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gfuxmlauw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/grxmdhiul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/ggmjlmbru.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gbhgpyhon.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gcnvqjwjs.sHtML


<!-- 参考信息 -->