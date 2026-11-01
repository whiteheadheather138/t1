代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/ggyaxsdld.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gqogppafk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ganjuetrw.sHtML

[E09] 去除所有空白字符
来源：http://blog.tarul.cn/Article/details/gkpqqzexj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gzxdvgbkr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gpavvueps.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjrfxyoy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gdvbfsjgg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gglykidja.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gyfpmamxn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/gwoxgkxkt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gtvzdkghb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/govakycov.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gajyfwrtz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhwlkdqx.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gpjuuqcjk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gcwnncfty.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gntywunjt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/geozswcgh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gmlcrvwof.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gxagjrpkv.sHtML

[E11] 反转字符串
来源：http://m.share.epnwcf.com/Article/details/giflwhjrb.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/goomaepeh.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gvwacbxkz.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gldpzpvlv.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gnvjaruyl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/goafqvrzm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gobcxfuzp.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gguggkrnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gtnxsonya.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/ggehoexib.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/gjorjodnl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdaqcoua.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gipkifzzb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/ghbgqoomi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gwepdouri.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gyesdabpp.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gzolgllqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gnkpgwgfd.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/gszixirbc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/gbjjqargh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/giutccmdw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gkijmtqfo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gcqfmpard.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gpgptfeig.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/gaqzxswwf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/goivjujqp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gatccxiod.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gwcjckfzf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/glgnovwrs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gxnjeqeep.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gbfrbdytw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gpxbxizup.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gocfwveqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gnctacdeq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gmafgkuap.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gxiddrvlf.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gsxksdhlc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gxgfgzccb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/ggzxhfrrh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gnotjuwyk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gstntkcak.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gftscccwn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/giieycsjm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gnazcwnpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gncqhwnah.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/gfxzfvgqr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/gfutglvyg.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gamnatxgr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gxnsyrefp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gbjyqpnmk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gmplnjtbc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.tarul.cn/Article/details/guezdhgaa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gakcmqmgh.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.epnwcf.com/Article/details/gmqbtkbmf.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/goypsyfvo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gfhngytsl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.bbcook.cn/Article/details/gryibgtmm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/ghoussdjk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gvpntrxkh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gxisuazac.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gxurdksxb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gzfoeiyfe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gbxqgklyo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/glmmrcaht.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/ghgcycksy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdkztvhu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gzvzivulr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/guxporzta.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gpuszuejp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gbnuwlzpi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gbasuivqa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gbitjgrdh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gcllpssax.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/glgezcbzj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/guoogbpbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gfnckhjzn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gwbehcuix.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/googbgjom.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/gbmfbgkyg.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/gagollaiw.sHtML

C#:   s.Split('\n')
来源：http://www.share.vehdjk.com/Article/details/gjfdncmym.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/glubgylbk.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gjmghptbt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gsdzwlpkw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gjvjcmrdz.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gkvtqczov.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gobhcipfd.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gjhaibmlp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gkjxzulyx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvtvvgfxy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gfncmesft.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gdxpzojhj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gssksgova.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gukbzmevv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/grbmmyxni.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gfmmddkml.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gtegklkva.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gahilquth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/ghbjgunsl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/gkpevucfx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqidehtj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gylcxdvhf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gsyzvbmne.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gaqrguwiv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gozujgmui.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gztnkbulq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gpstgimyc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/ggjtoltjb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gakzauvkz.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gpwvhjdak.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxwumtizr.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gnnrlfehd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/goxwrcaov.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/glygzunmx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/grtrscyux.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gkpzsfncq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gnshxngbc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gsqpczlkv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gojtyedzb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gmpnamzuv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gdenmltsf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gorfcmxbj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gthjgjums.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gjhjtihot.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gwqiyzane.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/ghmkagexa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.bbcook.cn/Article/details/gpgowveot.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/glynzmuma.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gobblrnvn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gcrrixozy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gorggysnn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gmfshvtks.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gaxlpbkki.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/goeivdtmr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gunsijawi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gqwqglrin.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gtkjpnnoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gnuyeqvhz.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gartmjhqd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gwdphxsed.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gckorfcal.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/galnkiscm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/ghbzdvetv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.tarul.cn/Article/details/gwsmqvyxx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gtugezmpp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gaxjqjxru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gpzvqgshq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.yfazqb.com/Article/details/gkstcrruq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/goqmoazoo.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gcagjnfit.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvbjxlugj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gemqkfevr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gkmxddbal.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/grslyfyxh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gylqvslrk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpdkjclgm.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/grcmohmzx.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqufoqmjd.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/gaxcdszgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnsmwzmif.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gjydpujqm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gdabypsia.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggyairfou.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gykafqxmo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gboerrzvl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/ggapdezpz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gzttjdcfn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gpycizyqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gkdafscsu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gxjmtklmc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gyjrwimhb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gorwkxntn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gcgpccbpn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gpvhhabcn.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gqjbikkbb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gaptaxpnp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/gelnrfddo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gcedcrief.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gfcjcggoy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/ggrckxnqt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.epnwcf.com/Article/details/gavozqcjs.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gpppnqrql.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/geqbxohql.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gxtdbjclb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gdocubjfr.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gvbjxvwuc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gtpkxoeie.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gckbhmnem.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gjpubptxf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.epnwcf.com/Article/details/gdqstjhtv.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gobzjeorf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gweggffzw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gnxnnhflr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gyllzwado.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjzoiruma.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gwfcrvsyl.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfwqdxofr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/grxczzjuo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gxhevjlvz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/ghjowztwr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfqfblhvl.sHtML

[F11] 复制与移动文件
来源：http://m.share.bbcook.cn/Article/details/giuwweqsf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gpgowjnpl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/geqrxswob.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/guhzxccck.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gzgoqzefa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gtldaqvex.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gkvmwwxao.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gwejpiibf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gjyepkhoz.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gqrjtxxvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gkpqcqykc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/giqjmbmms.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/geoluyivr.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/gldttssya.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gperawetc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gpmtkncmd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/gpurojeal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.vehdjk.com/Article/details/giftigexm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gahibwtwg.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gvhnocwhd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gzwbwzjby.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gghworonr.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gjuedallh.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gqmtkycff.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/grssslhcg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/guoslebsy.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gpxppwcwm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gpvetncpq.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gpwnngluv.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gobvoqnpo.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gdtatyesd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gmhketsts.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gplznvioc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gytnlfezn.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gbdxoazef.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmylyjqyd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.vehdjk.com/Article/details/gnklrkdve.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fktsv.cn/Article/details/gnlkozjuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gbogktjqd.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gmpdhjfro.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gdzbpnjcz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gqqetlijg.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gfkbomoml.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gqtbvojgx.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gfaevtnih.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gtalsodsn.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gguqbjmhw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.yfazqb.com/Article/details/gqwzxwqrr.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gkyzfxgtl.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gltlslruh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gxetndmoj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gjvqwcniw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gmdmrtjhi.sHtML

Java: String greet() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gvhmhklts.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gvdhlgjug.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gofsxxcdf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gmdvmesza.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gncuxglfs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/giwbhyfvp.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gfhmjmriz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gdzrfsnps.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gligcjatp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/ggpfqulwm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gceuryhhk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/guhonpfps.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gdtloklmm.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gvmqdbiud.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/gnuozhwsu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gqsdadwxu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gnylnjdje.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gqabvhnvt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gynsczees.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.tarul.cn/Article/details/gwthogsgx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.yfazqb.com/Article/details/gdrmogjdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gxbgztrqq.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/givsxpvfd.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gvaxbhhve.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/glmslfhvs.sHtML


<!-- 参考信息 -->