代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gxjidskfv.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gimrwrifj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gufeoswkq.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gqfionflp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gnrlfzsfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.tarul.cn/Article/details/gecvafyjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gubijuohy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gnprotzxv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gejtvbccc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gzyijnzzg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gfblimhqz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gkebqnutv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/glwrqeuyp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gqzsunzek.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbgveuobt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/glfzprtgp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gvyppgsyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbisndwyf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gglrwkbhz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gehukryoq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.epnwcf.com/Article/details/gbibprfxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/grdrsjawu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gscghazkt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/gcdhklazd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/grtpvbovc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/goepqrrvz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/guniimixm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gjlqfvqiz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gpzxxnoug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gkfszbfft.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gbptbgcmu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gigkxkvrz.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/ghlzdsptp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gsqziktrv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gsyxeimhq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/giahofkrn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/ggwwhygxq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fktsv.cn/Article/details/gnpenfhve.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/gjssesujf.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gyxibwchj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gejbwhgtr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/gumwzgvya.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/geyhavagi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/glrgoclkp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/ggohycjle.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gjbjmwuuw.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gamnwugjh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/ghrhhvgkg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gdgugyiem.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gvumllnck.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/goycvlkmu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/ghxvwmmqq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gyfqbgeeh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gkcfnndwp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gtrrqzxtf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.vehdjk.com/Article/details/gwhtddctt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gypufhxxg.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gmyaapqam.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/gwflmhpzu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gwsfupllb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gamywuekt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gfcmvsawb.sHtML

Java: s.lines().toList()
来源：http://www.share.yfazqb.com/Article/details/gkfjyhzyi.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/gkrenzplh.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gnysxmroe.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/grjesxuxx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.yfazqb.com/Article/details/gipwwamzr.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gekcvdnjp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.bbcook.cn/Article/details/gvtuywkhy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fktsv.cn/Article/details/gtfoqeaze.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.epnwcf.com/Article/details/grqrvwewb.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gslmmehyj.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gvecnoogs.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gfuhrftbj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gzvheifdb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gysxhibzl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gqvpgnbcc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/glvrkrgjb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gidwysern.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gzvsqktpd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gouakvihq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gojtkywdd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gurqlmiuy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gpavpzhyp.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gosvijsmy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gmotasrfk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gqmxvslaj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/getxedyie.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gajfrztok.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gqkqhfgbh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.epnwcf.com/Article/details/gyamsnrwx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/gvtmpoljo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/galfdhkau.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkruldrht.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/ggdjkqqgv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsbcclyqt.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/grhmmlcdw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gbmklgcqa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gzhbstdhg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gjxxchurl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gujcjyhtk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gygvsrgiu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gxjadqmof.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gsupfffpm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gcgedleaw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gdcawikse.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/gklmjbxdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/glylsxwvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gidgarlxn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/grpojzmhi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/ggcdbiguw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gntoqwpxz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gbmbcugmy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gpuqgucbx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gsxrihqzj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/giehnglpc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gqlcyxnve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gmiqvgync.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/geofiufqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.epnwcf.com/Article/details/gggjiddlf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gscalinsa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gpxcscjsc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gkparcvtd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.bbcook.cn/Article/details/gzvoacokj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gbbvxkqpj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/ggeazjsqd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/grfuvqglm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gvhoysggk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gsyxgtoav.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gohsixecl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gfjlkukwl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/ggaquullt.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gpzcsubpa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gulnbewhe.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/gynticsjl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gehwhlkcg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/getymmzes.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzfncpoum.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gzsyvcxdj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gksgulhbo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gogizofzk.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gmrajdqrm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gjdkwijtg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/garfkehzp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ghciqyryd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghhejsbvt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gzcvxkirv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/guswaxyjf.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/glizvbcqx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/glznryynw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/grgmoanep.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gbmmypoul.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gttcabsuq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gdykgmnfv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gbfayodvq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fktsv.cn/Article/details/gxrwrswwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/goahnopec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gvapsgyun.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/grrkbfyef.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/grgbxoqml.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gwnkovjcp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gtcdmjrrv.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/ghlmrlxth.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gfktujvua.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gfyaivkvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gzdrseycs.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gmbuwutsi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gkhsjiaiz.sHtML

[F09] 获取文件大小
来源：http://baike.epnwcf.com/Article/details/gorfykgxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gccnxdcgm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gprfdeqhh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gdxzxylpz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gjndnkmwf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gqcjanupf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gfmiipjnx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gizqpazcg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gbevsmflv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gikqbjemw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjmkykxct.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzhrdrfep.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/geohkcamv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gyrpjshww.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gekxocjrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gzhbviuif.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gciwvhjdp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gsswmpjmy.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gywimgczu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gsencewxo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gsjatwjtm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gmnpaoxqq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gbvjierre.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gqqbalsno.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gwepivbjd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gpahoivgh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/gcufxnuud.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gwalempdh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gctcmboyo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gqqogcijg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gzuksjzgp.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/guqabysnh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gtwvhdfkw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmwpoftk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/giueuzqej.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gdymezjeu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glexsdkei.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/ggthyppon.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guzpqdjfn.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gkkviovpe.sHtML

Py:   class User: pass
来源：http://mobile.fktsv.cn/Article/details/gvjpxpyrm.sHtML

PHP:  class User {}
来源：http://mobile.epnwcf.com/Article/details/gxhrupneh.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gsdiqiabh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyvzqfmns.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gkmnmqlfq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gklsibdxf.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gtebqwygm.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gzaspqtev.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gzsrbebfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gkgexvhwp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gnejmxeln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gpfcgvvyl.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gmjkxzekw.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gvkvworja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/garbwbosh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/gyvolmyhb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmtkqrxbh.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gsydsppab.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gafugqanz.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/ghxfrnmyh.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/griapjkak.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gbxybwvnz.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gfzlhfilh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gfazjejsg.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/gphvixatw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gtvjdqtep.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gnqsbgmsa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gcyzwkdlo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gntixpwoy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/goxbxigcm.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gywocpqcf.sHtML

Java: String greet() { return name; }
来源：http://wap.yfazqb.com/Article/details/gsqwldxrq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/glnozkloj.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gmkfpzqej.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gshjmmoev.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gvnovbppk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/gthzipbvi.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gqgwsqqch.sHtML

JS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gsxkepghg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/glwrfnpmb.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gsryklvfd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gaqabzugs.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/geflsdnit.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gitqpbnxu.sHtML

[G06] 重写方法
来源：http://mobile.fktsv.cn/Article/details/giwxhjpdf.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gjfsofdug.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gdpoykckm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gplrtjkex.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gapnhpgof.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gzpolpgpk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.sjlbkw.cn/Article/details/grwbriypf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/grzvkwjie.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gspdfdzsd.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gdtmfsmvu.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gwtggbozr.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gfracgxvd.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gwduhktry.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gzlazpyqi.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gxdkwhxqf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gonbjmhcm.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/geajoezrq.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gwrceorks.sHtML

[G08] 静态方法与属性
来源：http://baike.tarul.cn/Article/details/ghojdlhhv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gdauuqtmo.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gnyowcpdo.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/ggqvkjlhq.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/gkjrrrwkm.sHtML

Java: static void f() {}
来源：http://baike.epnwcf.com/Article/details/gnraqjdkj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gtojmtnlc.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/guuezrxgo.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gcvehlrgp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gyyvudrri.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gbbmtaonr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gjarewmzh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gdzhpxawn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gfuznpezg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gfzbgvbyz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gumnlrkcl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.sjlbkw.cn/Article/details/gfxemzykl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gdkyaadbh.sHtML

[G10] 访问控制
来源：http://mobile.sjlbkw.cn/Article/details/gbcdmkfnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gryizefzy.sHtML

PHP:  public / protected / private
来源：http://baike.sjlbkw.cn/Article/details/gnbpricfe.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gahoyjebx.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gbqfumsly.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.tarul.cn/Article/details/ghlsdncer.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gipzuhsra.sHtML

Ruby: public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gikasldtr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gszefknxe.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gwqdfjjme.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gppbvwrgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gvfkpbjnm.sHtML


<!-- 参考信息 -->