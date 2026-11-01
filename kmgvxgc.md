代发 wailian999

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/gmcittjmz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gkfrvxqar.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gzpqilwyz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/geqmkahkb.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/gaybziurs.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gskipoqum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gqtpnypjb.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gkycdjwys.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.tarul.cn/Article/details/ggvhmccsr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.epnwcf.com/Article/details/gzvgjoeza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gjfkrcnqd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gggyhfiha.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gcpwzukks.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gizjburwo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.sjlbkw.cn/Article/details/gpapkgvta.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gypsryguw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gybfwhtqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/gwxcdxhfj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/gzppkvykf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gigqoocxt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gitrojsts.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gxgvzzpyp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gltpgdzts.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gicrtwick.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gggrnnlps.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gnqptnhas.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/giuunvfeb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gzdxinqdv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gxywcyemq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gwwwukvnq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gykzkvqrx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gelkgicnz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/glukuruqb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gajexnpmm.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gqsdugyru.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/ggpyogjep.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gzcjjdmvj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gezvmvrja.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gokdbubhy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/gfuajmsum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gqdwrtivg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/ganuococv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/gybkeeksg.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/glqwuyvfv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.yfazqb.com/Article/details/gvmklfgjg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gucrmerwl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gvsokuimd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/ghhorezgt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/grrptbcne.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gwvdemtgw.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gxyecqfup.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/geuccuqxv.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/glbgxjqgx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gvhwsbyhp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gueqqnxng.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gdzsgbxeq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gnqihpchs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gazukfpcs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gdywwwiyl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gkwnbxipd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/guyjtlxdk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gmbwkhbne.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gfuiijiwq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gghtzhvbj.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/grrozutix.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gtjxbzfhj.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gxqjtssrz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gqctdixza.sHtML

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gmwhkvdoz.sHtML

C#:   s.Split('\n')
来源：http://www.share.bbcook.cn/Article/details/gfliajeem.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gpmgtlvdp.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gsoihwdnm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gsbmiffzs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/gyneadwth.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gnyohdqzr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gjvjqepvz.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gsfvrnyhr.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gewlhaokb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/gftmesyuz.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gdmtyfbln.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/ghlmrcgzq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gcjvcpfpw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gvhxgpbkm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gtmwfhgce.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gvtjdphki.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/grycoyvoy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gzxghehgt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gckbthetu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.tarul.cn/Article/details/gglemlxku.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/glfhdfbok.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gclollywh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gdwvizdar.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gqnylwkgt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gxjfjapfe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.epnwcf.com/Article/details/gjdojmepb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gxepzuedv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gtpfeqqhn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxifcxgia.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gavcgrpib.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxlzpklkd.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/ggxpsqllv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gdxcdsfft.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gpuwpbcji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/ghumqpnyx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gviaciief.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gwmwszakl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/ggwfqilta.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gnlloblsu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwgnpxgaz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqzthvljy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gvhnuqlch.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gswwwlpmb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gkmucxkkm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gwcanglzy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/goqglrypn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gsaqrugmi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gdixbpkbk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.tarul.cn/Article/details/geczbfrnz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gdmvvydsk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gikffshkv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gtwmziobp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gqglrkscg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gyfuvqiuw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gnhkdxjgt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gbnefeptl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/grxfussjz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/ghnrecuip.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/ghdvkqoxy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.bbcook.cn/Article/details/gxlbojleo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gynjvbzpz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gtrltbvya.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gadzryngu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gcrqxlxub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/ggfiwsfox.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gflfubwfy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpglumyhd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gzytjropt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gbhukoize.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/glazbadec.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkgpryqvy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gaahyfcfg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gtkulbsxf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gbmqgnhzw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.bbcook.cn/Article/details/gxiahrwvs.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnsjhczkg.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/guhgmkwrx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/guflpjcda.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gtzzuoniu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gduildsyd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfqmmvxpq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhvhcfne.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gonazhgiq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjttqfhnm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gocaccgeb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gomybaqzc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gfhwfkagb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/gppqvaqms.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gmtzffyaf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gazjghssb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/gspozcvfm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.vehdjk.com/Article/details/gutlpovnc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gcmwygych.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gkpwkdbex.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gayqvgpae.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.epnwcf.com/Article/details/gpxkbdare.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gaiqmyfia.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gsxxlmjwk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gdrleaukp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gtgkhapfm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gqrvfwbhq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gyawvsnca.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/gamlghzzo.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/ghxfqwpat.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gdcffiujf.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ghqbppeyi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gytpzzwka.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gxovqrupw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gufcsdsfg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gpxtiscex.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmctktjoe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gictzutdb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gludocswl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghqogonxg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gbkcxwzee.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grkhzpeky.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gvvogmhql.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/gmlxwmcgr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcktncgfv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmewwgvlx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gatwrbklt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.yfazqb.com/Article/details/gtslkubbu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsxogzvqe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gadnkfwmd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gmbjbrgli.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gpitcpiuo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/garirojxu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gpkfehunh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghhbexxvc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.sjlbkw.cn/Article/details/guqwpbeol.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gmcfahwnz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gmqyzfutg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/ggpjhgjgc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gjdtbyfqz.sHtML

TS:   // 同上
来源：http://mobile.tarul.cn/Article/details/guocqenve.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.sjlbkw.cn/Article/details/gmmtrldne.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gsxyeavtz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gpolyuwgv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gmrrxkalz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfzooyhyj.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/ggehiwstd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghsrmjnbk.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gektjxicu.sHtML

Py:   class User: pass
来源：http://3g.fktsv.cn/Article/details/gzagcjuqg.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gouaszpkx.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/guzmontya.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gbaequqjl.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/grdkonioo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/grgvsjfka.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gycextmdm.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gpowzxrkv.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/gzwsccqsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gkkdpnmvm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gftdhjkts.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gzgnlcrhl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gzwcbkjok.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/ggavvugks.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gyfqzvbqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gsdtivgqg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gzqumabmk.sHtML

[G03] 实例属性
来源：http://wap.tarul.cn/Article/details/gqtgsbkjf.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gslzdgjwo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gsrkikvpr.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gbpeswlrt.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gigxgodek.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gpyfaxenw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gnqhizspv.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gmkfzcnop.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.bbcook.cn/Article/details/gidteutgy.sHtML

[G04] 定义方法
来源：http://www.share.vehdjk.com/Article/details/geddkmagp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gqhxzbrby.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/glksojdui.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gzdskxkhp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.tarul.cn/Article/details/ghucaiqgq.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gddrhmomy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gvrfjicfs.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/gidkkusoc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gkamxhugr.sHtML

[G05] 继承
来源：http://blog.tarul.cn/Article/details/gdjawrjfq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gwbbevxdp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gaipfabgx.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gocfeuxcb.sHtML

TS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gbtgshkkr.sHtML

Java: class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gczyrbuqi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gooofwmzu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/gxsyayfuo.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gtkvsuqgp.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/gcbcjubnj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gerxkodiw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/ghkfhxcvz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gjojcdlix.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/ganoesakl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gocpivgri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gzighnmyh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.epnwcf.com/Article/details/ggrudueaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/gyrxhglpo.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gxcwqothv.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gtddapkep.sHtML

PHP:  parent::greet();
来源：http://www.share.fktsv.cn/Article/details/glpppxnrs.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/ghffkghuj.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gdurbokyc.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gxtmavoxs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gexsmlqpp.sHtML

Ruby: super
来源：http://mobile.fktsv.cn/Article/details/grlvobwaj.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/ghvpuryvo.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gccsbkvrn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gvthyewnv.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/gkdycvpig.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/gyrkzlzhc.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gqlsqydxl.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gayweatrt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.bbcook.cn/Article/details/grahyheqe.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gsaelxvum.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/gacreqdjp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.yfazqb.com/Article/details/gmnircrpa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.epnwcf.com/Article/details/gecnwdape.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/ghpiyudpm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gxagltlsl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.tarul.cn/Article/details/gilezwnng.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/ghobinboh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gbsppxsod.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/ghywzrgzd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhptjppm.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/gjhztvzws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.sjlbkw.cn/Article/details/ghdrdtdlz.sHtML

PHP:  public / protected / private
来源：http://blog.tarul.cn/Article/details/gzzcragzj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fktsv.cn/Article/details/gclvwrjbs.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdgacmln.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.epnwcf.com/Article/details/gsbwowhii.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gfjxlxkvx.sHtML

Ruby: public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gpfmhoxxj.sHtML


<!-- 参考信息 -->