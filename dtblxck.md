代发 wailian999

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gtvyebihy.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gsaevnsqt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.sjlbkw.cn/Article/details/gsrdnhmyf.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/ginyrhect.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gzwqxchvi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gftwjfgjt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gzubjgyqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gkfjvkifd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gqgvdvflb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/gngojsdwe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/ggmyjybpv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/gdcwoytsm.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gblfxunoe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.epnwcf.com/Article/details/gkrlbrsoz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gleschthl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.tarul.cn/Article/details/gslqwxjxx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gyfcuotzn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gbmlipgyc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gykcifexc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/gtzsqkghd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/ghykuxelt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gjoaxkwcg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.yfazqb.com/Article/details/ggqtarwya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.tarul.cn/Article/details/gdumxkjfk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnzvpoxdr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gpwimbvnl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/gvdqwjugy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gafyrpslu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.bbcook.cn/Article/details/goasyykth.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gnvzyepgs.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gdijdgibc.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/ggdavmkvy.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gpvqkwrrw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gewttntaf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gceqkwxzm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gaayeaslj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/ghjlqzpti.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/gxvzmpvos.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gvmmtavls.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gqounvlpw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gasqrnomk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/gicpbkevc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/ggmrcakww.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gouzwzmpq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gdeilouto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/guuklwnvf.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gvvrhweig.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gqarklxnp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gkxmjguhq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/glcmbegfy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/glxyedfqf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gfryddnqp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gitjbidjk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gyaazbjft.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gmxwxhdqa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/ghrtyzgfs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gxhizmgdj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/ghetuffww.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gbhkztwly.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gzhecgynv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gozapvwit.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gyqretnfz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gmnuyklfa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/geuxqnidk.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/ghrlkotxl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvfsuoco.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/grrnmtwsp.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gvalgibvl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.yfazqb.com/Article/details/gyppyfvqi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gibvchaxu.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gqlwsqhub.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gwilotpna.sHtML

Go:   if s == "" {}
来源：http://mobile.vehdjk.com/Article/details/gvssdgqvz.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/godzpcjjf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gwcfgfybz.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/gehzrcmcr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gnjvetdbr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gbyqajwkh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gkibberks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gbxropxog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gyefmxvfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.tarul.cn/Article/details/ggwbwaiej.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gqxwsjupi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gpyceitqf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gxwqzuuma.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/gdozlpren.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/giykmzrsv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/ghrynnniw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/glfqpxlyl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/ggeukvmog.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/ggqxjcmid.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gvqrrksip.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gmeoazcnv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbiqmdola.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gukifclus.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxguxcybz.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gjhkhxvji.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/gpbomqcpz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gslnhacbw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gvdfwsiyk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gesnkoqqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gvoyccfnl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gbjkecnmp.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmvuqbguv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gwjhemlxz.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/ghtvoqzar.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gmfxwjdax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/ggsuommht.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gzllmjqkr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gktnobfno.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/ghviwoqmv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gqamwmrfw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/gozheunnw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gwvehlgrq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gmvvcpnfl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gvuehmctd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gdjbuzjcq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gpchhkgxr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/glngjldal.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gnystlybh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gzxtnkhum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gsgyglkyu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/guufohjek.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gshglnoqb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gplhjfcqq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gncfsswlu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gmoihsnfq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gzuuylcoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gwruofpsr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gsgyexhkz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.tarul.cn/Article/details/gkvlzeaax.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gzwvcvwkf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gbtypbhgq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gwkflucel.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gycxrlkwv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gfnkrevjz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmpmaakny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gnmnkvbsy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gfvolqyvz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gkxhvkhli.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ggmbfflcj.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gbfmaortu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gomrkzvww.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gxlupafjr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gysrpwocr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gvyskxbyt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gamhmojwl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjcyosmxb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gnlsktdhv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gbduhwlut.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gxqzvfrow.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gfxfviiib.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gepsbscdh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gzidxjyfk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gyuuxhtev.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gegudbhon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/geijcchzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gxbeaqodz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/glmaoupdm.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/gxnlvjlbm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gffzpzqov.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gobpjedll.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gcvnkzfdf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gknmldtfy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/geedpbkif.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gjvvrssfd.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gntpapfmc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gryuaiejt.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/ggzjduuto.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gktfwlikt.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gceefzfzp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gocnciggm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gspucmiyh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gccylqcll.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/groyexrdx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfuxwpiqw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gabxqqdap.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gceiskalm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/guucxraqx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gkjzewzry.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjfrpgkkq.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gazcbfoow.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gmofqthwx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gmxrmqtiw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzgrxcyzo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gduyfuqas.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.epnwcf.com/Article/details/gxcycaypx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gfnfuevtx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/gvuueqzwu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gdbjdpgzu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gibqopszb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.tarul.cn/Article/details/gpswmalwc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gbpavyzmr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxhtlrmk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gnmcszihk.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gqcwzijqy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gktgzornx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gdpludoej.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/glurietfr.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gbhvwprxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/guwpjloxy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gjzqfvexg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gijguebal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gkaffmiuq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghfiroxtu.sHtML

G. 面向对象
来源：http://read.share.epnwcf.com/Article/details/giwvpfpcl.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzxjbwakl.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gqmrljupj.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/glkuvltgn.sHtML

PHP:  class User {}
来源：http://wap.sjlbkw.cn/Article/details/gsbrjkvvr.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/ghfgtzwwy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gecjbtvgu.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gedavkagz.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gmrjiiilb.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/genmakiey.sHtML

C#:   class User {}
来源：http://baike.fktsv.cn/Article/details/gdjpygkqr.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/geymnjaad.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gsuamzewz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gehplqqkh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gitsfhzcw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gngxnvhxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gmiydnahc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gvdcdmeek.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gzonplfnx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/geumcejlu.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gdzagawnr.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/gyyfymkzn.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gngajczzq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/ghsawqpva.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gzvbinccz.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/ghyvfytlp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/getokvcgi.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gzweugocl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.tarul.cn/Article/details/gsjkxwegp.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gbwkthkcp.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gdnvamwpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gthddyunq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gcdjhvsez.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gebnebzwg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwzcjnrqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gleztdsqp.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gwdjqlviv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gefwjkpsq.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gqnazifhj.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gbspxwuvi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gtvnxkmva.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/glsxaxysm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/ghwiyxvwk.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gnecwyenu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/ghhvyqaog.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gtetvtoqf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdvasermj.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gmdbiwwel.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gktdpzafp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gzvjrkmma.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gcygadnbc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gqrptbild.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwlqzwusy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/gaxeaoujf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.vehdjk.com/Article/details/gqdeakwxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/gttalejba.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/giensjock.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gtotsjovp.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gzyxohkuo.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gfxvqszgg.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gwjvwrfqq.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gtmvajlqz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.bbcook.cn/Article/details/gargctoei.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gnepgcqyj.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gzsivxwbb.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/grivtgntj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gahkhhwim.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gihpimpri.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gveraokhu.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/glbyvfbmw.sHtML

Java: static void f() {}
来源：http://wap.epnwcf.com/Article/details/gagjtavyd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gttqozhky.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gpzhkqsit.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gxxnpnjbl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.bbcook.cn/Article/details/gkwlyqcvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fktsv.cn/Article/details/gguztxwid.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.bbcook.cn/Article/details/glqflbnby.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gpoeahscr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/greshewja.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gdiusdjqt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gavfdqjga.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.epnwcf.com/Article/details/gbmhbmfom.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gugxqnbhi.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gjgwlsksh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gowpzulev.sHtML

PHP:  public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gjdqiyzgj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/guolwdhyc.sHtML

TS:   public / protected / private
来源：http://blog.vehdjk.com/Article/details/gqkeghrtd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gkimtvgnc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gistfnqin.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gpvqndtyq.sHtML

C#:   public / protected / private / internal
来源：http://blog.fktsv.cn/Article/details/gfuamjgif.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/geukdplqs.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gwovavrah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gwrrypjvc.sHtML


<!-- 参考信息 -->