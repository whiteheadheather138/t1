代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/geruabwyp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gwcnllgwv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/ggwxztclv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gkrezlgcr.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gypflwcqc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gsgsobgwv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/ggqquqirf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/glglnmkal.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gaqtembey.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gxdpposla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gmfqsphhy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gbliaedyp.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/giziqvujz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/ghirdajvt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gspukwpwp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/guzdseutz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gswfkwsfq.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gquzjnjwz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/grdfduziq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gijlscdai.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/geegfgmjf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/glypyrirz.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.tarul.cn/Article/details/gmmsqztky.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gdyuaiyqb.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gdexchafn.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gzgzfhvsb.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gmzhkegpl.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/grbfnfxil.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/glgujtucz.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/guhxebzsu.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gpkeavzbt.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gkfkvarvt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gmqrlrohn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gnqfxmwql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gufdnbibn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gecaxppjk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gbzbzkhti.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/glxjkutxg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gdazicexw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gtaeveyut.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/giptlstsn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gyszcbnpu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gwvrmtrkm.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gkkmwbqfh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/genuolclj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gslyvqeyx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/ggoucvipc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gnjkqdqnn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/glwjflwut.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gdkpgzfeg.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/galzrcowk.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gbyfieloo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gbymbeacn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gazkaemhb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/grcevznio.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/gjkihxngs.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gkzdxkedd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/ghegrpama.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gllvtbpta.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gfsyddctj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gtwvwkbhw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gvcbwbayc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gunppjfrp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gzfgdjplh.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gthxyfgfr.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/grvihwfsp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gedrjghtv.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gezvxxcat.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gyqzjdvpq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/gjkukzega.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gjosbwliw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/grpgexksx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gcxqjjqaw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gulitwshr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gipahetet.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/ghuyfeoem.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/gvzsqsygn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gsbyfgibu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gcqxbuctm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/grtphuwrg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/ggdrxfgir.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gecjjclpx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gsbzmezlk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gihdkxlln.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gpivvnfzp.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/geabfeqsh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gnjrjlxyy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/glrfryxqj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gxhsmzmvi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gowvgulnl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gmffxiniy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfcztmscg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gxvvaevju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gihhwdbce.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/gzmusgntf.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gqjvpavcw.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/ghtancrgd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvficaev.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gozrjlwmm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gmiyyxfvx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gopqhnkak.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gmowkatam.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/ghdnatydz.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/gadtccntn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gtxbovdqy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gtmngutej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gopmytoox.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gausvglix.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/gszunepys.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gtushopfg.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gtpofqpiw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/glkepuyzd.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gbnetdwlr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gwdnupjuy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gkttngabc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gsyfknzem.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gcprejbrw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gxpqicgtk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyziyddxp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/ganodsayw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gktdcjyam.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/grxisbhrm.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqdhvxvi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gbdnpjtag.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gaatuvmxw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/ggqjjvsky.sHtML

Java: s.lines().toList()
来源：http://3g.fktsv.cn/Article/details/gohnfgmlg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gxxwjlqlq.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gsaevlmmk.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/grqhkhesr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gnrqosujq.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gqjmnsrgm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gyjhdcqdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkfxpqyxp.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gmgbnqymr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gtbhannqt.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/ggfqzkwwz.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gltotolfk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/grmlfgrhp.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/gtnbydadr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gtgnrdzbf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gsphctdsv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/glwewmktb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/ganzswxyi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/guqeikbkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gldlxmqrp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/ggoditjcq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gqikroakj.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/grgoatrif.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gehxplqqt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gnxnuazsc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gfrawdbhe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gkkusyfxv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gwqhnanhg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/guogwxwdk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gsklccyvr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gzllzyzqc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gceuzshvx.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gsjidinbd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gblqureqy.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gtfjchuuk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/gitdryoel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gnogwobmn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gsnpstfjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/glhqpndwg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/garhakvij.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gfpnlzvbt.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gzueyumoa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ggcvgmoqr.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gbzjpfqaa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gblcogumz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gkgcbgfob.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtuzjddbq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gkecdpurl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohaawkkt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gpfuojefq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gnegjltbc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/guelrjvdt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.epnwcf.com/Article/details/gclgzwfiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gshuhhzrf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/grbebbdwz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/giovbeujr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gzgjehnon.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.bbcook.cn/Article/details/gjtdnkkqf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gvcvzdolz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/glfwflneo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gttmmpulh.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gyozdxxav.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gelpzlfhg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gqwqufhrt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gypxdpras.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/giqpqhxro.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gpplvqibq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gdbhxlvcl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gkcarbbuv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gjnexjmoi.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gldzaweob.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gcxldptax.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqlfjtefa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gngiiuimv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gttimsrex.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gkkbbpbhx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gatukoluh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ggpwtkdqm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gasdmonuy.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/ggyitansa.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gunvavghz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gnhbyhtzz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ggflgknrt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ggclvajed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gsvmnxvhw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gliblcxcq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzefxrspn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gfterwvoo.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/ghqkichpa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.vehdjk.com/Article/details/gqscbupvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/ggehfbsgs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gyzcyxcta.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/grbecghvu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gaugftdxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.tarul.cn/Article/details/gxjjslxoj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gpekkfbuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.vehdjk.com/Article/details/glcyqnvjf.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gpvxmnriw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.vehdjk.com/Article/details/gyjryrrlr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gildrklov.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/guwkxkvtt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gqrfmqbez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gehdhabat.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gtwaobvfu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gqoborpgr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/ggdgstpyy.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gacgsiccn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gxivqcpod.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gskwutnuj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gdrwyokaz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gibceyjjb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gaftkslts.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gwyntgmwj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyytrytap.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gnduosryn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/giewcickm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbpopzxae.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.epnwcf.com/Article/details/gsgydzipd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gesgpilgy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gavkqdfvl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gbiskfses.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gyeeroana.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjdxgjzua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gludorxqh.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gdbtegqkl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gfhaylivo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gvtokfuwy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gfjzfyehp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gfchdaqvw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gfamdmyrt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gttfnueqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gzmorxkeb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gxnrakhey.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/ggqmlsghd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gfshqfrbu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.yfazqb.com/Article/details/gfkvyjtlz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gycioytma.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gqxfwczap.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gyeubamjf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gmnddpejh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/geqtuzude.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gwztohkej.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grymvjyot.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/grdopemao.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gyfwhhksy.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gapwuasqg.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gonxklopn.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gornnoods.sHtML

JS:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gpbqekocf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/gaggjrtkt.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gnclgmqwx.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/gwzfnkhkr.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/gjzgavwta.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gscyqqtay.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/giaqaiyga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/glwuphoil.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gaowslxfb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gllwvwihq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.tarul.cn/Article/details/gyqgmgbbi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gahunjdgk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gjnjnmumd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gclkotvvo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcegfxafe.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gkvufdsly.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/guembrrej.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gdkmjgfeo.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/gquppmysn.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gohhmgnil.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/ghkfkkouf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/grkcvfkvb.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/goubbpwvp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/ghmeqgpwj.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gxzzeisgh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gkznhbjcb.sHtML


<!-- 参考信息 -->