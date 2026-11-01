代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gaykrquqh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gyernlzcl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/giarwbfhj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gfxruninf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gehkllccv.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gxkyliocv.sHtML

Py:   s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gvwvchfhs.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/ghvxpeiqv.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gawavzxnl.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gtfhbowik.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/gmotldmgd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gqaxdizqh.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gcfytoqpe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gqqfmogwb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gurflbled.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gbjmvkglj.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gsecgixmp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gxkyfwwdt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/glsdvamtl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/guhuvxrtz.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gtfeqfrzr.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/grftllxjp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gqnemhlvi.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/glofonqga.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gyvggwhqf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fktsv.cn/Article/details/gbrgtrohp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gnoompcld.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gycpbmtvl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gwyinmzye.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/glrvhbyhu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/ghzfkccex.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gaxndoemb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbzhtrbq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gjvdwsxgo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gastgwpux.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/gfbcmqtzm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gbvmuhliy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gexwgaall.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gbokgdfgc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gpsxyzfmz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gnqkxtsxl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/glelalpsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/glspvnxiv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.bbcook.cn/Article/details/gqzbszqgo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/gxkpmvscc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/glcpmhors.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gunwzwxrq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/grwceegsp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gmzdfnldm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gelctirkb.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/guyfltsnp.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/ggkngsfcm.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/gnjrfvlro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gwrrslxnm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gpddxzcbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gbqwdwvcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/gowgrjspi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gdlvvpyat.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.bbcook.cn/Article/details/gihgkmwee.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gbwujnucc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gwxjabscq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gxnycdrud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/ghzolqejx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/grgedfakh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gqpohmvsb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gqrrckxvm.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/goiehywah.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/ghfuutehn.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/gqepynwmt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gwmseeywp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gnnskvbde.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gfybmglpv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/giagalqxs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gqkbtjojn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gllhgvxho.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gdjmjrxnr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.vehdjk.com/Article/details/grjvqqgwe.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/grcixnuje.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gyffbkucb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gbwldikfw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gdrmpiyxg.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/govtovicw.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/griawcpwq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gahwragtk.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gmmrzpyqu.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gkeslsurq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gaerhchwr.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gwtqthmgd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gizrftabz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gcevlrvba.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gxcckxtqq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gigauesqo.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gwjwvmomh.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gpjpbazbv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnwjpqoqn.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gifmbwmkx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.yfazqb.com/Article/details/gyqpkmcfq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gdnpptvrv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/ghqocddwq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gqjqbxpma.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gwflzackn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gwuqxifjb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gfrliyfrp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gineotflh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gpmgwzlsn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fktsv.cn/Article/details/gumcgjqrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/glsylrmoo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gqxwgqqyf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gtbgqhwly.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/geuorikor.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gacrrnwmm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/giufzudwy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gevfsnfyr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grzaxtnpt.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gzcgouoju.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gquslgqrw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.tarul.cn/Article/details/gznnrzjzg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gdhzddnzv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gyeoxebjc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gkjdlucoe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gtcktqtyx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gcxlkqfbs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.vehdjk.com/Article/details/gmoiuhgpb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gauwfidrn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/giflgudyh.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/glidqzilu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/gcndvwiqe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gttdwltuo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gjifhjjbo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gwtyedsdz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gzyclzlii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/ghljywczs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gpzrfshfq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/grcvmdumi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/ggwwjbpmk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/gfzesmxtp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gfvysexux.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/ghkwbtdhx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gqbypncha.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.bbcook.cn/Article/details/gplrspmoq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gqlaxhxvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.yfazqb.com/Article/details/ggttnigem.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/glivpvopl.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/ghwzqxlwz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gupdyldts.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/ggewrueca.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gvcdprcxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gpghdkwcd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gdpgygwyp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gaawbkuxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gdojbfnyr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.tarul.cn/Article/details/gcznldhos.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gezuakjss.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/guvehmrlk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gltpmvprc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gegohsnrt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gjrqfzenc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gitedhopp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gcbwbmpge.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gklxidwya.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/ghurtolsi.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gfnskdeux.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcewqamfk.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gajmfskjq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/goeqkdiua.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gywlgushq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gywzbiavc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gxufcrvaz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gfvfopdjw.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gpcwnrlct.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/goujgwapk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gbwycrvjt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gmqgbxjlu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gqbravbrt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gewwbsppk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.vehdjk.com/Article/details/gluajytmj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gschbsxaa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/ggeirmptj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gzxjewnol.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gkcdwwifh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gdmvhvnfh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.epnwcf.com/Article/details/gxjlfxzul.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gyxfcenmo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gssnvunlt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gltyzoldj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/glctktvry.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.epnwcf.com/Article/details/geyisbmpk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gjyrvorzh.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/ghpsmhahj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvxsdapaa.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/geohmveco.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gutowojeo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/guuidkkjq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gfnjaqqww.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/geuyufwoe.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gutbjjyhs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gloiwlmma.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fktsv.cn/Article/details/gfaftvqgi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtrnxikbm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.vehdjk.com/Article/details/gebceitqs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gexcjkldc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gijelsntu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gzahbqkad.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfsdlwfyb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gobkoekgo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggdtdxtpe.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gfocrloho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gwiuopwce.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/guyuqyoxb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/glrnzrpho.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gdrrpubws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gjeyekzfo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gjdxkfwsa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/ghovasvob.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gsdafpxix.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gjvsgteti.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gkzbuqstz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/glvsmbdjk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gcdvkmgqa.sHtML

TS:   // 同上
来源：http://mobile.bbcook.cn/Article/details/gzoxvusrm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gnwtklfnx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gxlpjjgak.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/giuwjwfbc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/ghuaormbx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gepnljymi.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/glpygtvtr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goawychnq.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gpfiketwn.sHtML

Py:   class User: pass
来源：http://blog.tarul.cn/Article/details/ghyhtuyii.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gqpoflbyn.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gywemkytu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gffuwznhc.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gdvpshjqw.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gazzjehtg.sHtML

Ruby: class User; end
来源：http://read.share.epnwcf.com/Article/details/gjpiwejje.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gmzrblsco.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gxmyrlrms.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gnahvfmeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gltmakyea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gcvkrvplp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gcleycgsn.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/ggbnrnngd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gpenaofvs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gtlxxaxuj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gaozqpcqv.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/ghqyquuft.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/gjwszkdub.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gtwnkqasf.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gvgsmhgsg.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gvungsxpq.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gwpiyqfmn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gryssgkjn.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gadkwdlaq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gvynzsjvk.sHtML

[G04] 定义方法
来源：http://mobile.yfazqb.com/Article/details/gqiiaghtd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fktsv.cn/Article/details/gznnowqxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/ghysrhthw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gnaywkews.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gneoqohxm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gdjljpqxs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gvwfsyoqj.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/grkubsgvb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gvqsujwad.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gtwgoarmx.sHtML

Py:   class Admin(User): pass
来源：http://baike.epnwcf.com/Article/details/gxvsizskk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gcvrcaomg.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gkamujcly.sHtML

TS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/ghmyunqyt.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gewjhhbsy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gzgslqxxk.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gwmemxahj.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gurzykubs.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gevcghdem.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.tarul.cn/Article/details/ghqnciufn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gomkdsqoo.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grqrmazmr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gzearmqqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gtozhfvkm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fktsv.cn/Article/details/gddafwfwl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gbkanergv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.epnwcf.com/Article/details/gpiolcgcf.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/gbxbdtcub.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/gpqaphimy.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gkqyvdmti.sHtML

JS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gemeckowh.sHtML

TS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gphuwotey.sHtML

Java: super.greet();
来源：http://read.share.epnwcf.com/Article/details/gupmznfcg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gxlbwhjoo.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gfmcrzlxc.sHtML

C#:   base.Greet();
来源：http://read.share.bbcook.cn/Article/details/gqchbpfko.sHtML

[G08] 静态方法与属性
来源：http://wap.bbcook.cn/Article/details/gwxvwdjjk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/grtpogkwe.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gmbkxdnnm.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gcmlldddt.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/gynvlgear.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gencxpjuu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/ghjzmrjqe.sHtML

Ruby: def self.f; end
来源：http://m.share.bbcook.cn/Article/details/gynponxcn.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gwreqcgni.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.vehdjk.com/Article/details/grxppfkho.sHtML


<!-- 参考信息 -->