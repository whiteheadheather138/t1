代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gwhgaawin.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gjinujtxk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gtbebinsb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gxstwheti.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gihcwzpbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gchkluhmt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/grdbbffso.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gxmczbgfx.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/ghoqwrzra.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/ggolfkjmx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/giiphlolb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gqzkpznzq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gynkniokz.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gsucixtyq.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/grhhkpzri.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/ghkmqhkrf.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gakklneuo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gfadibxmd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gmlxibejq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.sjlbkw.cn/Article/details/ghkevcxli.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gfxtqvllm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/glubouhfh.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gaugrpamb.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gkuwvhtal.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gibedyahu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gdnsgogwj.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/glnjsecai.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gcvvazwfr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/gdviyjmrn.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gzgxqyoxt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gxstyrmvs.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gwybeepxh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gkbsjcvip.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/grdnkreix.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/ggngnjipe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gdjnkzeik.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gykxbanuw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gcbhnzffa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.tarul.cn/Article/details/gfmkvmssf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gfxmofxqn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gyivvjarb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/gpppscaps.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/gaexnhpsu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gqexdxiok.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gwxbwunsj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gjzeqxzql.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/ghbmvdbrf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/gftwdbyyd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gfvifkbci.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gzurygdtg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gnqqtpctb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gccesyvky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/garhlpyga.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpgftrom.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/grszomuzw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gkraqznbz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gqvvtyfli.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.epnwcf.com/Article/details/gphdtfzwt.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/gxkgyjehn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gaogaigev.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/gzozrxtzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gaxeuxoiu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gvpvwzetq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gjtyfhmxy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gqvkfolkn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gixaoiwct.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gmodngaty.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gnjickmcz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gtvvifnvb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/ggvmqfzmd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gzwwvjchb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gfdhiohrt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/gpekoxomz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gpbiqkpoq.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gqpvqpgzq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gceoswqjh.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gatylqkvf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/gusrectey.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gomrbjuju.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/ghhtbbhen.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gyazzxurl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gpxgncofv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gifaaphuf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/geeitcfdc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gmpfdwyfu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gwlgkuqxr.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gluzkktnk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqbygqfas.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gletlcmmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/glibnzqbm.sHtML

Java: s.lines().toList()
来源：http://blog.vehdjk.com/Article/details/gfgpyfjly.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/govfdrpgg.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gedekfgtm.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gsfoddiux.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gjxnqgdoe.sHtML

Py:   if not s:
来源：http://mobile.vehdjk.com/Article/details/gakhivaia.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/guridzlah.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/gicffjajx.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/glevnboxd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gseutqdls.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gtrwffyjg.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gvlcigjco.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gkpumudte.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gevkqdbsm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gphfrsfxt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/grhsatrjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ghmzzgrwt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gwcgrrytf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/giqjuriom.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gpfyognmm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gztsfaoft.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/godvflwgl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.vehdjk.com/Article/details/gdsaacfsk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gjlpmwbak.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gsahalukx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/grvvqaalf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gvggtejnz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gkcqczlox.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gcpvqnher.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gzonazxun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbslrjbie.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gixxvxlri.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/gsymcrkfw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnjvewoxh.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gmxelevzw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gabhoitgf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/ghqqvklwf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/glfnpcgxh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gwgqtfqys.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gzywwpphd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gbcfeuhvr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gmrdirdnk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/ghprfmbcw.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gbddhgpho.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.sjlbkw.cn/Article/details/gjfwkpwvh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gxlcwsoys.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gekzfznbs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gjynxknmb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gwrwitelu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gujznmees.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gtueulysv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/guvotszva.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gwfrwkgxe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gfihezbob.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gqikujucm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gmpvpdcaf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gyawjhmmg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gxinthtuo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gqjpftuzw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/gstrzfkzo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/geaqkrlsz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gsjkqkrec.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gcdoktuvh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gmtpcjeqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gqmcpscgk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gaibrlkac.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/gcplnvfdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gxtxrpctx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwixufyl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gvvlzaojw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/givboilwh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gkdgxipvg.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gnctiodtm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvrtyenyl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/glsfiebdv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gkyascvat.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gzufphtyl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gaiswfhra.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/ghwgqjodo.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gtgqdhwql.sHtML

Py:   os.remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gikevjgvd.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gmqqpezmc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gqmzzgsjo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/geiwpyots.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gpyrcucim.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gaqpiynoh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcytnkqyo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gnfuzjaqk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gaotsedev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/grqoenajz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gdqjsfjhu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/ghgzmtyia.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gmjnayhsk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gymxnlnmm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gdjchrsxc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/gndhswxad.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gawrpbtyz.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/ghtepxfwb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fktsv.cn/Article/details/gtxieibik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gzjqwqxky.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gzhilpgya.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gfqaramrw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/ghpafetrt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gsqxgwaiv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gxbigmftx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.yfazqb.com/Article/details/gmhklryed.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/ggnryscgv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghtnkihrt.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gyldkqvtg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gqvugunql.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/gxmvstsed.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gvrkgmcnl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gwvdcapqb.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxqcdfbz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gvscytpzx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gdbsgzveq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gobssgvsj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gaawytghl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/geluqtztm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gtuqqbrim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gecymglqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdiivdspz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcxvhkykh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gouyzlfiw.sHtML

[F11] 复制与移动文件
来源：http://blog.fktsv.cn/Article/details/golflgrbn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/glsjlubar.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gbymaespa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gouduwoxc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gjpundczw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gutqhrobd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gotxkgsws.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjumifgjl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gprexmtwr.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gycfnbehc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gqjxitrsa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gmoxgjhjk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gzunpwkal.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gxpwqjezc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.yfazqb.com/Article/details/gdqycmnvo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gdsusdutf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gieimyxsi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/grkgpmgdc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxuepnhoi.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gjnvuabbt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwpndavzy.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gpllgrjig.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gofpgonff.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/gsjttyyyz.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/ghrdzyuvf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/guaihymcj.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gudainauf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gyfwrmafg.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gbxrdwpve.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gwcfjzjjr.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/gpmdciotd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gskgbmkvy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gxteeaqob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gbxgauthc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/ggcpksuny.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gbeytxbzy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/glzerdjlb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/gikngnwht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gfdfequpc.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gnicrwcuw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjxbncch.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gfehrlydl.sHtML

JS:   this.name = "x";
来源：http://m.share.yfazqb.com/Article/details/grqzjwntl.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gmegmgobf.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gptearbjf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gqfzrfjoq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gszxxvqyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/gyqfweaci.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gmbvmihqo.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/ghyhgsspy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gpyesmlfv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gutyjhhzq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ggguvpwsm.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gtxcsrjvp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gadxokyie.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gjjzljgxl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gwhbibjcm.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gmpiwligt.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/ggiwpdxxc.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gxyszbeqt.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/giwqmmnci.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gyakppoje.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gsywdfgjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gzimnaasy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gluyrzuix.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gvmedlluj.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gcztcnphl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/ggaedpsrw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/geuhmxbwa.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gazmlynzc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ghspkfwgk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gvlvryxxg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gjomnkynt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gyajivxuz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/ghoiesnbf.sHtML

[G07] 调用父类方法
来源：http://www.share.sjlbkw.cn/Article/details/ggskzwgyp.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/gipkiukwd.sHtML

PHP:  parent::greet();
来源：http://read.share.fktsv.cn/Article/details/gkuswnqtt.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gairapfjx.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gyczlyojh.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gqxszlndy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/giutjmymc.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/gzetdztxy.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/gmjrwjdmu.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/goztnyqjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/gwfmkpqzl.sHtML


<!-- 参考信息 -->