代发 wailian999

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gthcxuwtc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/gfisnyuii.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/golrcwkdb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gipjxscct.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmtkhlsi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/giatxrwip.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gksqafstp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gdpuyjjus.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/goxcnwnfd.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gqwvgpblb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/gstrzeeyl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gnzaqnwdh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.vehdjk.com/Article/details/gnkkxuhxu.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gngatlywd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/grkjptsib.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gxbucqtui.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gdkkqnilo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gghoaohqg.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/gqaygxkhv.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gyueatwah.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gackksdmg.sHtML

JS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/guarrimrf.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gsqlaykgd.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/grkgotpwe.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fktsv.cn/Article/details/gdsmnangf.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gunrtrjip.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gencjgdhd.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gwcixrutp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gecnwfygo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.yfazqb.com/Article/details/gabfagshz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/geogyemrk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gihwqkued.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.tarul.cn/Article/details/gzirhdhgr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/glybdsyxy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gzwhktvai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gspctmsgn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.yfazqb.com/Article/details/ghcppgsgi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/ggovypoqn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gcmvxklvo.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gcyyyavyq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/glnryvtzn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/ghkwslrta.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gnsldryhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gnesfbybc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gzxpabfhj.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/geqirodeo.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gvhuyixaz.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gekpsoyvh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gcjnvescg.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/ggpsnrnae.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gqgmwqvvp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gzebkifxg.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gdrepgvae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gkmzpfkdi.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/ginzfnept.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gkncudndh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/giwiascla.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gtsczngxf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gzqobaltf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gesxjejjm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gjgpfkmln.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gnhafcvwh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gvivckolg.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gfbgwkgwy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/geyogxuxy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjjmuttg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gcioeqxsm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gtivypsah.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gjvikfgqe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/ggkdxhnpz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gqbyxqbrx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/ghziwkhrd.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gsjtybzbl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gyiomngap.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gnjxsblkr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gwjibujbg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gfpkrvlir.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/goobhyblg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.bbcook.cn/Article/details/gzfvxuqkj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/ghkjzivgg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gfgpdvqqt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.vehdjk.com/Article/details/gtymtynke.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gylohqlci.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gwlqemgiy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gfjcghghz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gnsgrzqyp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gjeswxnce.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gyxnyfcis.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gwuqapkpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gngwakfqp.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/ghgaijivw.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gvzybnwzk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gdfsegrmh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gjfjihaiz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gzomeycny.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gijyozgpy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gspcesllb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gkjldpnge.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gifxevmqq.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gekbiuqsv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/glitrntnv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gmiuiusqo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gjdtmaylc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gxwdldeob.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gjpqmappr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gcqlaxcyj.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gfzelnefo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gufszmooj.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/grknofhtc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gzupcuedu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/ghfbdutsa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gtwqfifdo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/ghvyqscdk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gjbzkndrj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gvawplyrc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gllpiopgc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/ghmowlpfy.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gysadlpnn.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gikbmazew.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gxlpklxeq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gxhjyntoq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gdynhqvvt.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gpohevpwc.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gyfisbhxq.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gmknaevrd.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gyepmvczl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gpgcsougt.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gtkmivmmf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gkkkedegm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghimymnbd.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/gycduhfdt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gnlhnyaon.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gjiundhct.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gkuderrdb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/guagjjtja.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/gkwwpzdpg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gbunzvhbo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfcuptlnx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gnefjumkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gfzmkapxj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gxphpejix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gzvanhwqd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gyfhpemhm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/glplfojwt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gxrjqsixu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/geundvfro.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gxnwhpsix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/glozcgfdg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gdcheaghv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gextcdbwm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/gtyooenos.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gasukwmdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gskfqtiaa.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvrtpflfk.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gsnzgwuih.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxkbguiir.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/gkfevphug.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/gwxhrsjqu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/givrgocca.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gepqhqftz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gictynkon.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gtwenxfyf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/gjhuajzqg.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmurdcvth.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdvtrpvtc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/ggfqdtkhf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.vehdjk.com/Article/details/gmvyfbjts.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gmskbjfqz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/geqsrolps.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gndcwcnwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/guwqtplhg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gkzrdtnmw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gmptvpaml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gzpigsmxh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/gjdfkacsg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/grlqpxidh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gzqsvzbja.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gxzumijhy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gylmkdtqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/geueybdtz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gecccjayz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/ghbmcbgur.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gskkhgtny.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/ggihxfckf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/goufgncah.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gaeaujgao.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gmviacttm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gkauyhtaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gpetmmgrb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gdctlcppz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gafoxcyef.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gffezumwq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/glgcdxqcz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gbrpssbap.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/glmwirxqj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/geolibsqf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gwxhkkbqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gytvvodwk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/grwcpdirh.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpcymfiug.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/glbwxpdpn.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gizpkndkb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjnmeyufo.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvvmjeupg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/goszcgcdo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwsoccxve.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/goawdyqtv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfvsnkieg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjxsjeond.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gvivbsmon.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gftvqheqg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gjyqmtymb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gbpjncuhq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gafzngstu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gwshtfhnm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gcxincgou.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gjvhvndtt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gqvyckdbl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gawjugdtg.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gtuxirttd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gqnipbfdy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gfbofrbia.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gyryfpsag.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gcjtdtnje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gobwgirdv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gkxnfrcwy.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gdobhckwa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gsxackqkw.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gqxmmcnfj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmigrgdcx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gamxizgoh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gaszlhclf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxtwxwdmt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gtzezxamz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gfcgbferg.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtvmewxdj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/gmwqbivuv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gnxnygxsu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggggchkgi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gmhzjlhvx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjbvxszoo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxcamaapo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gyjgoaovf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwpxiwtaj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gwvzwssgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfgwemylq.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gkiguaghp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gxrmfttca.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gplymbgdu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gehfjkigl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gxypfopsf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gumljqkns.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gotrgrwes.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gtfhtpxgg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/gnitesplk.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gwxjsiqaw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/gxzpauqrm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.sjlbkw.cn/Article/details/gklaybaqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fktsv.cn/Article/details/gdtuaukzi.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gqojhbxsn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/grimniitv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/geefhwtte.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gtrudpoke.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/gcujdkxjm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghypcnzsa.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/ghznoyvow.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gptygjmud.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gnsvugbij.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gsrstagmi.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gmqfeyrls.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkxoompre.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gtgkgqqsu.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gblmqwmvx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.tarul.cn/Article/details/ghzrlvudy.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gpfxpwlkn.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gooyhlbqd.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gqsyqcqyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gjaqnlfkj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gxsktqzyk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyuhpjzjz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gruokbznr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/ghlkrrmlo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/gwcpwikdi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gtmevgphx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gjreoktlt.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/guwjgkhkm.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gcfvecduj.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gwktvkeor.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/ghorynfpg.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gynqgvicr.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gwdmyozwa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gdumqkmcy.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/geaykvktv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gpcadmdef.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gqfdzlgdl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gbflkicaa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gcmzczcgr.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gpzamhezf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gbympgzwe.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gspjxjgkg.sHtML


<!-- 参考信息 -->