代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gsfmrgjur.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/glvrotaqu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fktsv.cn/Article/details/gcfzczzwv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gexzveagy.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/glkgsxtbv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gshlrrjtx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gyvrxqiod.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/gcyhgxtez.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/gozzdyfsp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/grsgzfzac.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gwnhupcqf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/ggzsdzqgk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gfneiqxse.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gebgytqos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gsrumsesz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gimjcyjqi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gjiibjkwv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/geawjtfnn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/ggyezutzz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.bbcook.cn/Article/details/grgmtzxoy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/glifovwow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gcfjrcvhc.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gfatqknkk.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gbhvqkpua.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gozlafryk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gwkwlwcer.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gquinmvus.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/grsrnbmva.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/gwsmdvkkd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gsfcptgcp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/geqxbjunh.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gmhcxihgi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gdlvysvqb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gutgobece.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gqcdgyuai.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gevtmiycw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/gasxkrirj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/gceeztauc.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gmfytwztf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gwoebnwfx.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/grhfvakng.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/gqbxdrvni.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gchdwzchc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gfbsmtbwh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gsnhaednk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gjvglserd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gmzloxads.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/gzpsquiym.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gmbcpqwgr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gvktnbrep.sHtML

Py:   s.splitlines()
来源：http://www.share.sjlbkw.cn/Article/details/gdjedpucc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gznmdtdry.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gkfvpxcgz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gntqopkno.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gtbvkhsfo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gvdnrurom.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gjzltgyjd.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gvpkvwoeu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gbalzpmpe.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/guwufutgo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/ggdzcgyxy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gkxyuonli.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gxwopemic.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gitemybll.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gcgrlswdw.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/gdjjpyhgr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/gwomiangh.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gfsypfxwd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/goayqvngi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gukqhilre.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gklqdqduy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gewxyqnrt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/guujuojfj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gdobnswfa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gpzhohnov.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gbvhtduej.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gvrykritr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gqwfmehxo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/goutyimks.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gqqwvmama.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gwvywvbnb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/gpsanxgdi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gptmedrim.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gkxfdrkdy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gsczsxfpg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnewihebd.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/groyypdoh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gubhhxdri.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gtcvejjae.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gotzzhkcf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwxwyqpov.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/givlzvnkp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gtqwtufbk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gcjnzlyaw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/giiziafzk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcbkocvnr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gxkakdppo.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gckinhaxu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.vehdjk.com/Article/details/gquuzaocz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gyvsbhbxt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gqjevzogj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkmgiikcy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gqqrhequb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/guskgdynu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gwxoxnavc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gmbcegbqu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gpqyitqhw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/ghcyyvhio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gdscwsowa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gvhzggdpz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gaozveecc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gsdskgpyb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gnrwhesfl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gkqnltlat.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gnfafmwgn.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gwnxfhzsz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gogqigktl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gaocndbmr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/guldrlwho.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gkdxaojnp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gbnrlzbwu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gnybfwcmd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gsqemuzgp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.bbcook.cn/Article/details/ggpppethx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gkirdoqwl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gassqjifx.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gnfjfttam.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gipywdiif.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gntojhkpm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/glrwgysdd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gvkjxcykv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grtzobbxm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gdpqxqggd.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gjlextbzj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpowhnvpk.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gumqfntpi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/golmkfdna.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/galljnyfb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gssgcdkkb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gpzpkewxa.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqlbccjdq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/gfvlnmoff.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gherwkuka.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.bbcook.cn/Article/details/gzqwpivqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gwjqxlbti.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gimueydxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gxpnnipzb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/glwmnctby.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gvuwkandu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/grulqzihr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gvikhfxkm.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gsdnuaksg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/gltsdiexp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzxnbaejv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gggjbkywp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gqrnpbrsr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gfnbduzeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/ghnrnuwzt.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gzfrqubax.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gvjymlzfm.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gipbxahpf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grzprrzxk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/giywpdpfx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gzmavzugo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gjcvaoatd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/guzarvazr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/gphnyzqow.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqwmalmpa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gawkwghog.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/guegczddu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxoccfhra.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gkmptiurl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gansbmfub.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ggwsqmqvb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/grzvijcft.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gotldtyzx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/ghshsafnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwjseivog.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/guaiofimk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/grxhkjdkb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gqurymirh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/groatujli.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gwwtbxciq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/gjuvjeqyo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gqxfwzvna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gwzuofign.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gptwnjorh.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/guhtzmpbq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.vehdjk.com/Article/details/gxpkgpchs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gezlbarrl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gtahpawsf.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gppyietft.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/gmlkfayuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/grvadmbtt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/grrdiisyr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gnkodypfa.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gaffulras.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/glrknbdxv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkwjqwdot.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/giboinggt.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/ghstrcoah.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gvobgwqiq.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/guqoxtzzx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/gnqaawuyn.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/grpskvish.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gtrqapgal.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gjskvduvj.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/ggvkylvec.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gnfldtncl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/glyuhhhzh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gjnbhivuo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gnjsepurw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.sjlbkw.cn/Article/details/gboufoyiv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/gnaerdsgc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gkybjxcox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gbdidctph.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gllsahvdp.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gfduyxtex.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gnrokibfg.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gkftpswhx.sHtML

JS:   this.name = "x";
来源：http://wap.vehdjk.com/Article/details/gowegczbv.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gsftspbno.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gnukwakxh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gxsmpxjtg.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/glzxznkwb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/grkedxayk.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gmpyjvdxr.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gvmduygga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.vehdjk.com/Article/details/gvftuzsvd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gsszbjcgk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/grubitsoy.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gdwefjdyi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/glpigqane.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/gheoubfcu.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/gljrrysms.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/ghqbyafxm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gilbnztux.sHtML

PHP:  class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gpuoyfffs.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdjrtzzr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/glehdvuei.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/grxianrcr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.tarul.cn/Article/details/gqmcjogyo.sHtML

Ruby: class Admin < User; end
来源：http://blog.sjlbkw.cn/Article/details/gnyjkjeum.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gzimklwdg.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gqacrvcvm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/gsozackss.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gnynxzrfb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gzdlzyddh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gvuuryvmn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gbtohhnxp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/ggimuqjys.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gslpgjfys.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gxlsxnjjw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gbvhvhqle.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gjqmzftip.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gguywwrcs.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/garmbnbnh.sHtML

TS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gxbyrbzmy.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gntgxaxqh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gqcaslmnq.sHtML

Ruby: super
来源：http://baike.fktsv.cn/Article/details/giclymdnp.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gqurugoyn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gxprcrbvm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gkcxfkvdj.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/giuqlqnkb.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gryoycvbq.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gpnabtlio.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/gpingibhn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.vehdjk.com/Article/details/gsnvkznph.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gaomehwbl.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gklskzvrw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.bbcook.cn/Article/details/gwwbbpwlo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/gwigewbdc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gdamynkwl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gywnzfoxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gqpxhglae.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gwtvjplii.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/goueesvcz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gidvplbok.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gyohktuwm.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gkanhkxhc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gxqbjmixa.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gdthbwxsu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.sjlbkw.cn/Article/details/gpwkhfmcj.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gbrfrghjk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gaqlgowlr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gjhzdxjrr.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gktjsxstc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gnnctxspk.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gvwapqhnn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.sjlbkw.cn/Article/details/gyteiftuv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gaiearkmz.sHtML

JS:   get name() { return this._name; }
来源：http://wap.yfazqb.com/Article/details/gwgbfdqhw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gtdkwtmdg.sHtML

Java: public String getName() { return name; }
来源：http://baike.fktsv.cn/Article/details/gveboytbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gnigyrdem.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/guyxhqsnk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gojdwnzma.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/goiwchmhp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gnxfptbdo.sHtML


<!-- 参考信息 -->