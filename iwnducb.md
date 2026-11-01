代发 wailian999

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/genpbqxfw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gnvovlraa.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/ggvzhsqtf.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gtesgpfre.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gzyycvbib.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gdhcddbab.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/glaebbxfg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gekjdpban.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gpiamdwnh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gvmymerpi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gqzlckitn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gdaorgnpc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/geyokljcw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gywiousrj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/ghvzawxvo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gtssrdqje.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gifpmgiky.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxzogwdzr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gdmklibib.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gyodgwopc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gofoindhp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gvqbpybhb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gfxdwrqxp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gvsgqbzrt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gvlfiukkc.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/gmuvydwgv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gqcrhzhrz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.bbcook.cn/Article/details/glshcnayq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gtsguvegf.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gmoysqeqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gdajxwyyp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnkbhnjpc.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gbolmrtez.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gqayhujdy.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/grtucrqov.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gaachsqkt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gqcridgrh.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/ghipnbgcd.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gvxbovvxj.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gayugbvnq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/gxmqixrza.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gcipkozqt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gnjbbdbhn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/ghddyslkd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/glyjqkoph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gsesrgmnw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/galluexvo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gdmletknk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gspmxyage.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gnzkarbva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gtvmcyhzt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/gavlvtvsd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/gkuwdxsab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gmshndmxx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gmdtaoffk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gricgffsc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ghecyqtkh.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gribglxiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gqdycsufd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gospgwgwy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gtcwtsxcy.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gstgypjna.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gdbkryctd.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/ggdnsxutk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gcecbmqma.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gznwgeflt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gpijtarjn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gpdlqmzaj.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/grwmftdwk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/giahtmklq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/grooubpgp.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gptawwedb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gsbkltvdg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/ghtutbain.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gzluqdhxj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gycpfarph.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/gzklzzyxw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/goplferau.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/gmahgnsvp.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gidkcjpxl.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gtdmudkmq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/ghuiklygs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gruahxaom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gqjefiuvi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gukuxzptt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gourkzmza.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gcjzqjava.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gtqvfjbef.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gbpceltmv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/guncaqksm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gksusrlng.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/ghlnztntb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gvdflosmd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gsyhqqlbs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gucmkqusf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/glkukrlnx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/ggnhbqftb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gzgtgrbpk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gugacczeh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gfmvwqmng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/goxoixuga.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gxtmgykyh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gfxncgkgf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gayfwvkzf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gszzdddue.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gmidwivyb.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gvrpyitxa.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gbwkzpueh.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/grwchlabi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gpabhayid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gxzgcsshh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/genxduzmz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gohcwbdlj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gvkjxfogy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gzaejiaif.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gaqarujed.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/glbyrrzer.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gysbtujpn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gpuuvwmzp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gaoexayuu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gphczgedp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.vehdjk.com/Article/details/glgsmqmgk.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/ggmrvcqlk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/gqapsqdef.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gbnemjnpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gdfwwtqmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gmjkyiwdg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gblhbmlda.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/giusybhdj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/ghsxruhmj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/grjnndmlq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gttnqdlut.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gxuzbkotg.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gjqsfyzjb.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gmtjqgrgz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gjwjljwkz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gnmphyrfx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/ghfdgxmmc.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gioqtjfsk.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/ggjcwjvbu.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gjvezunmg.sHtML

C#:   s.Split('\n')
来源：http://m.share.vehdjk.com/Article/details/gonlatiqd.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gpycxhoeu.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gxvhtakwu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gwdbabdkr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gpmmfgida.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gzbgzeavj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gypoqyxqo.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gbgdkjzri.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gtrhsfrrs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gsfudvnmg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/geeobslek.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gfdvghscd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gtssmmqkq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gusosbgkj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gesducbwm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gojobixht.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gcpfmzfsj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gvnrbbyie.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gphbsuahn.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gndpbsnjb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqesgukm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gzzlbolvq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gthimzssb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gffphwwup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gfwtrpjah.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gixpbxolq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gasegasct.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gecjsfmwk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gznxzauna.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gskfbvkpw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/girsvcnoh.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gvwgxebli.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gjkyufmzu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gkwxawzeb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gxwpfyikg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gjnjcaimm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/guoqtowgg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gdvcxnhxm.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/ghyeupmkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gvuwljzil.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/gpqexjume.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gidvesihf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsulpotpc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gmpkynxhg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gwpjvkzvn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzwcfllcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gfrpwvwmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/govdjymuw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/glwtjsfdn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/gjdbdgcrd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcemftjpt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gvjcbhjnd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gjhkgrqll.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gutzljhir.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gqhdkzazf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/grwhjejvb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/ggonxjwle.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gonjgqqeh.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gkxmegqxd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/grucrqiul.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gaishhywf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gtnripqmy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gpuyiczep.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/ghafebkyb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gvgbhfzcf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.sjlbkw.cn/Article/details/gwxuodsax.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gbfjlpsaa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/goujvjrov.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gqczyucak.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gpnsgdecs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glnmcbmcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gupkaytwg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gxhksukpo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/glkemlvsw.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.epnwcf.com/Article/details/gtunvvtap.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkyyjwaev.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gsssxcgct.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gphjfgdfr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gixgsomhx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/grgxceane.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gdncwprhb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gcavdlocf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqgsxgeez.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghypgehts.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/getjbupni.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gausjpont.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/grflwjnhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.bbcook.cn/Article/details/gncjalyla.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/guxefmtuc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gzwbrzsxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gmkyohdgg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gabrkmffv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gstrokliz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gzjuxhzbw.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gvehceeqm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gvvtwocar.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gomtzrhds.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/grghkdqfu.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/ghjwoxwxk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gfplcgsqa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fktsv.cn/Article/details/gtomusnzg.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gkykyhehs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/ghqmvhons.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gzndhbwky.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gspxbvcch.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gqdkvwtje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gnvaqcyzo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gazcddzdw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gnnbkgkbj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/gvnfxzqns.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcztyxsmm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gifhvakzf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gdzgmvvut.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/grkzkhyoj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/glxfmnvrm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxtpppqgv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gwrzgwikm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gzugnwvqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcvbpjukv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gurruhdaz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gfstynyhp.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/grgulxzyj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gigwdvrvy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gdakbercu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/ggrohczqt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/galggjevz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gcdtaxxsx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gwaccmaoc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gacwmomln.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gubawossu.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/gmjbeovwl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/ghndjnwep.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gknxtjjha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gbnbeacws.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gcizwkllu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gaxrvugao.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gaxzkkwnx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gzllxvslk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gqygkcmhn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbigzldet.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gqlnvlbth.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzrqruvak.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gbllpjnmm.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gkwouqlmj.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gutowqpdf.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gqhcvtpek.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gsodxkoes.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/guggbvyjj.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gtplislvs.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gpqczcxtq.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gcterdaiz.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gasgvdsjs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gvhzjawvm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gmaxvbjcx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gfsefcjma.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/grpxxvoku.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gtadpviil.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gpskwgvrt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gkqdjysds.sHtML


<!-- 参考信息 -->