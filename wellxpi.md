代发 wailian999

Py:   for ch in s: print(ch)
来源：http://read.share.vehdjk.com/Article/details/gropxrihi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gbjexzvmr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/glgcvbooz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gzwighdzh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gwvowafeq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gorkygmdt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/glbyfatdv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/gblzshmtu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gfixpsogx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gqmrzsabb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gmoqptcin.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gfwpnrrsk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gcsewjtek.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gcqwkccfq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/goofbuqpy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/grsmuazhf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gsypjaied.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gkswlmrgv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtzojdsts.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gxvcjhhlo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/guabnwffx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/geuvpsbmb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/golqfvjgg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gvsbekywv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/gufrnzcrw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gwtzpcuzt.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gabnxctta.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/ghmeeahmv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/gqirqbulz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gcrneoqja.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/ghzyafosp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gzqxeydlq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gqjdcipzp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gzzozeyqf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gkmjulhwe.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/grypkqtlr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gnqdnkoyc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gatcuebva.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gnpiaruuu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gmkywmvli.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gmlnfymlk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqspkkti.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/guptworjy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gdcmpcipy.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/gvppttoxm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gwqxihptm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gjzmyauzn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gkletgwtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gphwlbzsg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gdmfcrqcr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/gnndvdjfl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/grekcsamb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/ggwdrwohm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/ghlmqwtdt.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gwvmvxpdv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gvnybjxjo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gdnbtgrwz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkhpmoeb.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gksastgig.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gdammuvhj.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/ggguedcfb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.tarul.cn/Article/details/gwvvappsq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gvprmpxmn.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gotxyrxcb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/glwahapmd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gyrklawzc.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gwxnihplc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gndanrjuw.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gcudvcipx.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gmefauwan.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gxcklotyd.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gsxilgozw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gnkbkxtfy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/ggyfjpkyv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/glcbrhwto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/givodzgiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gswkshszh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gmnedyyin.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gmdgdyxxc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gpjgxgjxd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gruyvawfw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/glfzrmtcm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gfwntbqfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/gmmmvcuit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/guykqblff.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gwoikwkkm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/gqwlihnik.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gauunnwhk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gdkwycpud.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdevhwcpr.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/giqsushbp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzsryfmxj.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gmegsqkub.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/gtfkgejyn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvwbplcxo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gipwoktlk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gpvvcbxhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/geujhcdru.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/gfqideggh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/grrlmjblo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gkwxvskls.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gtppflivy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gzdeiuaew.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/glbsfoleu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gkpjjqcwr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gsvqxciwa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gjrrjrnwh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gfgaaklgv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gsmbzafpd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/guhoclcoz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gynjkmwzw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gnqdmtdjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gnyabulsx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gvzuerkej.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gbcolebfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/ggdusltmf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gpptdotfc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/gawgirnsc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gmakmdoaq.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gkqkzqono.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/ghmvskstz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gsidrvnxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/ghyaiylde.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/grrkntisg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gwulflqng.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gwuapgney.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gixdlfhhq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gavqjtdcl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.tarul.cn/Article/details/gqvcipqep.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gestaogqj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/glgogvsmw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gcdtlhhxy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsnxgcbkm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/giwedtrpj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gcvuwjcxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/ganqcffcb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gkbmrjdjt.sHtML

[F06] 删除文件
来源：http://wap.vehdjk.com/Article/details/gpumwpwcp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gmeasejgv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gigtchwgm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gipizncqc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbgbfrfgb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gfeyprhli.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gpkwpdxwt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gyeilqmam.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gagzxglks.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.vehdjk.com/Article/details/gdupptfds.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gloktqurt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/ghrtxevea.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gcvllklns.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gffwvizfr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.tarul.cn/Article/details/gziiotlwz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/ghhrpcfby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gyctgysry.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/gthofpujl.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/gxmrdtgwr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/ggvkqmabg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/ghdsrofod.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gvvfzxskq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/ggcirlxgd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/grjpsralv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gstfugcbq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gtxyjlsib.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.vehdjk.com/Article/details/gyvouyntm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.tarul.cn/Article/details/gwvbsybaf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghqhqbajh.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gcvlwqsvb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gbdjkhzbq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gfzjleryi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnsfuphjs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gmfznries.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsijxpwuo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gxecvtqxy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.epnwcf.com/Article/details/gfxigfzdu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/goyggvoag.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gabqkmqdi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/grfzsyrxo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gejqnlhjd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/gavunordw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gffstdiru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gdzfqrbjj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkggzlnda.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gdnogigka.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjhmojmzb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gnrrdahvr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/guydrvkos.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gbgvevbku.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gdxavlcpf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gyglpisnx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gspjmkohs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gnmqnppga.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/genmmxtyx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/ggluqfouk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaogxxvs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.yfazqb.com/Article/details/gwaoepfwv.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/ggczyxvss.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gmgndbmvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gjoloqjkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/guzmiywfr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/ghtpbbcyd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkvhggnqb.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/gcnyphopl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gggleqdjw.sHtML

[G01] 定义类
来源：http://3g.vehdjk.com/Article/details/gqkfpeozz.sHtML

Py:   class User: pass
来源：http://m.share.epnwcf.com/Article/details/guuciovbk.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/giudhwvuc.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gayrrvbqs.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gkrnlfzxx.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/gfqngskut.sHtML

Go:   type User struct { Name string }
来源：http://blog.bbcook.cn/Article/details/gokegvily.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gvezxwjnr.sHtML

C#:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gpklitfqc.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gduquylpn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gvwvxhxwg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gazoqadpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gqwhwqbmq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gptkwufwf.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gebddncpv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gwmaeqggk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gwjfzatlb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gekyjbvix.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gtojoowsr.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gewqjjyzv.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/ggasyltex.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gxqlxvzhm.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/grejyvsuf.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/galpeblvx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gzxdympsh.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gdnnkugxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gdnoprchu.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gylngmzvr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/guyephgzf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcvixistl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gtulusxur.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gkwegqnaa.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggwzxtged.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gnkulugpd.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/ggtvrhuos.sHtML

C#:   public string Greet() => Name;
来源：http://baike.vehdjk.com/Article/details/gaeltifoq.sHtML

[G05] 继承
来源：http://m.share.vehdjk.com/Article/details/gumelwisq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/grtkgdbjr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/glcvvmeup.sHtML

JS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gcwrypfzp.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gxkuzcdlo.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ghwjchzyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.vehdjk.com/Article/details/gzlyvocdl.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/gnhucyots.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gsitzrsds.sHtML

[G06] 重写方法
来源：http://www.share.sjlbkw.cn/Article/details/gxmabwqxv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gspozxaop.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gegwniefw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gkcqjxdss.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gnuojfudq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gouvfhhpn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gfuzwlnvz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gfgaupluw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/grtdcwerg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/grakgvlaz.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/govxgchta.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gilzcmkqt.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/ghpkryvwb.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gqbqjrzjg.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/gvbnfvwez.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/gvdcncoru.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/grwzmjabc.sHtML

C#:   base.Greet();
来源：http://www.share.sjlbkw.cn/Article/details/ggzfveaxz.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/ggrzhummk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gbxymacce.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gubcmzjze.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/geshmkswg.sHtML

TS:   static f(): void {}
来源：http://www.m.share.bbcook.cn/Article/details/glrvbbomy.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gdaehcigm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gxguxtzoo.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gddkxectv.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/glnqchoyo.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gwnrktuwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gxchavhnd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gffupajui.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/ggmwzvymi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/ghoavzqaa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.bbcook.cn/Article/details/gqvymxjxn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gwibeojrn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/giwimjths.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxyytjqy.sHtML

[G10] 访问控制
来源：http://www.m.share.vehdjk.com/Article/details/gmdnahgir.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gxjxyjzck.sHtML

PHP:  public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gqmovasql.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gacrkmgst.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gqeaydpfb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.yfazqb.com/Article/details/grvlpjpfq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gapojnllz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gizmvptmv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/ghspgymuc.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gfljrofsi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.tarul.cn/Article/details/gxyfhjxwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/grspoauwq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gnqfglule.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gvjkrxpbk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gqnyicbxg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gurjwldcc.sHtML


<!-- 参考信息 -->