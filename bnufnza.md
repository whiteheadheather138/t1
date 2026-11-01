代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gzkrenmgw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/gzuaxjwwt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gkwrphsqt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gspcymemr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gctkwzfdh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/guibkufsj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gncgzezqa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.sjlbkw.cn/Article/details/gvqtmbjwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggzjjfrpy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gvbnqyxpx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gdwrdnrzh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.yfazqb.com/Article/details/gcyothogf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/grlxqdsgx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gnvcmkcck.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gdhjyibmj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/grarcubeb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.vehdjk.com/Article/details/gmfnozlrx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/goginaxif.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/glabdyesp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/glcndfvxt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gjfkccbbm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gadlctnpw.sHtML

[E16] 数字千分位
来源：http://wap.sjlbkw.cn/Article/details/gpfozdqbq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/ggimesbpw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/gygbvngfj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gwkgrciog.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gktxbcmuy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.yfazqb.com/Article/details/gkljjxpar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gpgslyxsr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gltjjvyhb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/goytyvtyu.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gsmnaazet.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gpqchzzil.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/glntyihgb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gchaqkzdr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gkbfksclb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.yfazqb.com/Article/details/gvpujalyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/ggmaptrty.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gigcgftjf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gqvvbosvx.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gemvhpsll.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gwezpeysm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/glhxpsags.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gnmqoencv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gynsdcepm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gzefftorx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gnnlgkohy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gnzlnqrfm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gfavcfirn.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gvolwrnws.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gdgvaroqj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gnzfgkqtz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gltiydnnp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gdcmnkxki.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gpdytpehh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.epnwcf.com/Article/details/gooprxrss.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gwpquiupo.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gralbcthp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gyrknbbdz.sHtML

Py:   if not s:
来源：http://baike.sjlbkw.cn/Article/details/gztayjlov.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/glyjokclq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gzkbuyamr.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/ggwyguskw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/glfpmtdyz.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/glpqrtngr.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/glxppngyu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gwlpushwk.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gjfexmhbv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gzowdrxfz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gqwbxnuga.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gntoyfqcg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gtqwrmbjz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/giobxaqak.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gqmilbkfb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/geughqdke.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gwlmdcktm.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gyrvkming.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gvuhdypbc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gukpjzddh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gnomatulc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gssyqkgtq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gaeohuicw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gkqjgxpml.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gznakkovo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gbcavyabg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdcijezul.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gochupbat.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gruvibiow.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gypyjjurf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gczyafuyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gzbmzutzx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gxhmbynjc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gcfatkvnw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gmwzmpxpk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gklztxbtr.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvugcfsle.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzuqywcbd.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gjwlptnul.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gjilkhfwh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/gxkitcedx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gfgcagodr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gpsceqdue.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gbrglwyks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/glwlnelvo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gsmmmkwnq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gmlyvcgpn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gmogqgens.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gpksrkbsx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gitdzgnpt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gtinenpym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/gewgkfynt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/grlssltxq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.epnwcf.com/Article/details/gzlxufmdv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gtaouecjd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gydfjwmex.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gsdrrceyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/glcwvadrq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gfbmtihnj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/guhkclffz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gazqpprhm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/gwzedfvbv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gsqitkavi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gpavujamq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gouebrdxf.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gvvmeoczu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gnsfurzpk.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqekphngs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gxtxtllzs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/giwwmsabv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gbjqvzvlt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/grthbjdwe.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gebvjbbfx.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.epnwcf.com/Article/details/gkuxjsask.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/guriwoxwi.sHtML

Py:   os.remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gegjnbcpp.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gfvsxixua.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjnxiopaz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gueumeohr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/giigeeadc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvsbkjcnh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/gmbdxgvse.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gxwypxiat.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/geaxxgvkq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.yfazqb.com/Article/details/giawtygwc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gmecydamh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gbdgtlidd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gahzucjxt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gregyjsnq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gbwlqmakd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gxnkxaoap.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fktsv.cn/Article/details/gufqcczob.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gukfkniid.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gmqjeqevd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gliaqgung.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/ghmepuayb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gtqepmajt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gbgrvgszk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/ggfyprqfr.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gcsdopplm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/getetznsb.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gjrampgpt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gireuqumw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gennovyjm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gwazbeyon.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gdiaejqgd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gndiyrwjg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gyglrirmr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gsherelwq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gffgqflok.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gaxnadunl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gkyxocldk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gbiiismzy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gioikljyt.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gdmgqgjzc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gkoxjashb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsvokmkwk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/grxphkdab.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/glbettahi.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/guomwehbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghsdbyaiz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gherzsuns.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gedxyqatd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gkvhdqpxh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gekwepuox.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gzaxvcxgv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gedakuxac.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gmwuqnjmh.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gnovvwpvj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/giayajdfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fktsv.cn/Article/details/gahijnydn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.epnwcf.com/Article/details/gxqxfogwk.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/gcnmjkuhw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gaxwojgat.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.epnwcf.com/Article/details/gawqeznaj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gzhlaqwqu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/geososiyl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glajcpzjf.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gypcsqspi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqdacnzql.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/ghbqkrxdg.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gsucumzxd.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/ghabsbwdg.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gokfpknfi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gkilovegp.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/grkbujnkr.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/gddmmmsxp.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/gpyrvcdhr.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gprmszkyk.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/gcrpwccjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.vehdjk.com/Article/details/gtsmmteid.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gdbnfxvug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/glarfccpk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/ggfxfnruy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gzbhwycdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/glgvmsuxl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gtutnrmqw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gxotpftcu.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gdhyuxept.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/ghdrjuocl.sHtML

PHP:  public string $name = "x";
来源：http://blog.epnwcf.com/Article/details/gozzfpdoy.sHtML

JS:   this.name = "x";
来源：http://www.blog.vehdjk.com/Article/details/glrwkbjtx.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/geijgsegc.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gyrzdgtuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gvtpozffk.sHtML

Ruby: @name = "x"
来源：http://baike.fktsv.cn/Article/details/gajnqwnmp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gfozxwhaz.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/geveffwue.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gkqrqlseh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gvftqwtlv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/grsaesaka.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/ggvcicafr.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gqpbxiuey.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gkzyqtuuq.sHtML

Ruby: def greet; @name; end
来源：http://3g.vehdjk.com/Article/details/gqgdhwpye.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gxbyexcbd.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/grvybqjqh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.sjlbkw.cn/Article/details/gusoaynet.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gqhwawrbk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gckldzbiv.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gwzavzwof.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gucwcxiaj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gyxkrwcyb.sHtML

Ruby: class Admin < User; end
来源：http://3g.fktsv.cn/Article/details/gufjsdudn.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/grxigyerz.sHtML

[G06] 重写方法
来源：http://m.share.yfazqb.com/Article/details/gnnguizdl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/guebjuiez.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gthukqzgt.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gwcbqhkjo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gtxeqvuiy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gghibwgom.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.bbcook.cn/Article/details/gqooczwcm.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/gatiezddl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.epnwcf.com/Article/details/gjrycakad.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gxvsbqsfc.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gwvuxtwxn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gpcziyzub.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/ghduqiwjw.sHtML

TS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gukrukzaj.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/gkdnehets.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gustxrzch.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/ghnexkioc.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gioexmbeu.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/goppyhzvc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gqvxkophl.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gcgbhcrvx.sHtML

JS:   static f() {}
来源：http://blog.vehdjk.com/Article/details/gsvcchzhk.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/genlvauhe.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gsasbxqns.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gxkyugyzi.sHtML

Ruby: def self.f; end
来源：http://www.share.tarul.cn/Article/details/ghwozabhg.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/gdaqbhike.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/geccfcuqw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fktsv.cn/Article/details/gehqkrqpf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/geqijyetz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gmcvhvjhy.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gltikrawn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/giribyxqm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gkbrguoqw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gqbwxsddg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gfbddjivl.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/glcvanhqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/gybssmoso.sHtML

PHP:  public / protected / private
来源：http://wap.epnwcf.com/Article/details/gcjxqmcvt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/grjwasoms.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gcevlxbbk.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.vehdjk.com/Article/details/gdyhbvicv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.vehdjk.com/Article/details/gvequlwxc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gdqpstswe.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gdzcshaex.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gkxfcpcfb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gjkqnthuc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/givolobpo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gllwpimlm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gbzzsrurh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gmrxsppiy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gnltgvhid.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gtbpujfyq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/guryoyhcd.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gugcdmwld.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/giqxvsugi.sHtML


<!-- 参考信息 -->