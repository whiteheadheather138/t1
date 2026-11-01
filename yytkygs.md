代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gjolnscof.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gbpmhqdkh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggksfzlyq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gbtdmbsqh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/glsqpmref.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gtapuejcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gltfgnqml.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gvxpuqszs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gloevclre.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/ghqqpnsuu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/gcfycgmrg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/ghnqjyogj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/gcnznnttr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/geazsuner.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/gsbkvtqww.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gnbbrykmj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/ggvoyluuc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gnurfamah.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/gfdrgdkgg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/gvysrfukm.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/glprdzppw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gxuawdcif.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/grlqpegeb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gnumptzyb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/grjsneybn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gfictizcb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/glkmjjfgk.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gewqucqjl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gzkcnpkbb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.tarul.cn/Article/details/gxuaacpic.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gjfxdqwln.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gcaajzclm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gpjwjjlpn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gxwydfxah.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/ggzanvhuo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gbgolwjns.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gnsqgvbjv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gwxwlqmqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/giqnjzcty.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gwamtdfep.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/grohhomyd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/ghfacooul.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gwuveckdx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gpwdzuolo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gnqupdhvr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/grdotqcpo.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/gxyvdqhnm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gtkcaxwdf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gdivbxwww.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gkbocivna.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gnldymmoi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.tarul.cn/Article/details/glganokwe.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gkveqwjnz.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gnctwcjtx.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gaccyukhe.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gucuizmvx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/glagxzjwr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gljpvlehc.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gddnfmygi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gxvitcvfi.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gblohbxht.sHtML

Ruby: if s.empty?
来源：http://mobile.bbcook.cn/Article/details/gyybtngkm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gvxbhpevq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gixtvwuto.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gnvdovmiv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gqzlekuzs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gafmbvvhs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gjwnoxvrk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/ghavvsrol.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gttaxmbwh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gvepsgcfr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gsxtttkeg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/grmtfxlop.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/glwyywrti.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gfuvxrwfc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gthbhhgjo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gpnscepuy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gijolfjgx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gcbknfaqf.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gphplwejm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/ggpljmjmg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjhyrqnga.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gsyrujsjg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggbfwzxri.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gihozobob.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gdgjteenq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gcrftsfvn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/grgumoevv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gafcobqfp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtdlyjtka.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/ggrkphkmm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/grjetjyrk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gsulrluzk.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gnmgxegnp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gabkjcnzd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gvrvgmtda.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gerozzral.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjejvtxbw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gwtyoicio.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gibscshoq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gacqmkpat.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gvhqqjmyf.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gfgsyhysh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gyzocebmd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/glopbteoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gjlczcxpl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gfdnagckc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/gyjslwrfu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gzimpxvzc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gwggqgywx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gpvidsbwz.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gvadmslnu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.epnwcf.com/Article/details/gczwuylxk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/gvixjudth.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gzwvsuyny.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gaowfipqa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/gxspblqog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.tarul.cn/Article/details/gwwqamwbs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gepzdxoqb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gojgbkeii.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gejxvskqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gvkdghtyc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gpdofpctf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gtbobsnej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gdzooiect.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gqzluhtbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gsdozgsmc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gnpnwrpqh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpwfayzxg.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/geqslpwiw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gjsaouokj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/grwkizwoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxnhduhnl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfmtymmnm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gdaqxibwe.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqdquwgue.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsfxifnwf.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcqzxgihv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gsojupgzs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gshtqvonf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gsrinhxiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gdczcbmwh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gocclulwz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gnervevro.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.yfazqb.com/Article/details/ggsxqhlwt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/gnzadbtiy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gmrrmrgxr.sHtML

[F08] 遍历目录
来源：http://m.share.fktsv.cn/Article/details/gmsjheqxq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/geipqpwga.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/gqayfstyk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gmidfyzci.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gtyrnfdoa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gfbbcumil.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gushpxyxf.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gmuiooldf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/glxjorqmo.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/giaoruyew.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyfymbjma.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gjmpffygq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gzvnxxcia.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gtbvmshxq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gwdugtpxu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gwljhwqaa.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghmarudjb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/gllknyzgs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gspixkoxl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjwsnscdz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gqryucsyw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnfqhvwfz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gczzvdlgy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gbffvthrj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gkeifkcnv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gmewvcdli.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gnvrczyku.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/glottijih.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnfiynmll.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/gswcyobfu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/gnabjqwjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gyjtmtlmg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gnrrmgvlr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gtngsamoj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwrhcoxim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaiyzimc.sHtML

[F12] CSV 读写
来源：http://read.share.vehdjk.com/Article/details/gnabrqmwi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gzcpccghg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.epnwcf.com/Article/details/gxsyyrpvi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fktsv.cn/Article/details/gffqonjyh.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gcmsteued.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gxprxnaar.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/ggkhhyock.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gjaigtyll.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gnhpewvky.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghzduiway.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gubmwesgi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvufjwcbo.sHtML

[G01] 定义类
来源：http://3g.tarul.cn/Article/details/gcvwxpvdz.sHtML

Py:   class User: pass
来源：http://read.share.tarul.cn/Article/details/gppmyngnz.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gbyhwnzhg.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gsgxiqxyd.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.tarul.cn/Article/details/ggvkbdfre.sHtML

Java: class User {}
来源：http://www.blog.tarul.cn/Article/details/gevpxqasb.sHtML

Go:   type User struct { Name string }
来源：http://wap.vehdjk.com/Article/details/ghuzshqxi.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhoeabir.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gcihtjlms.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gonuzaboj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gdtvxolvo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gvtvvhkmh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gcjiuiech.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gdjpcgggr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/grkupopkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gfifcuyxs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/glfhtiurj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gbpuozqkl.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gdcqicpzv.sHtML

Py:   self.name = "x"
来源：http://www.share.vehdjk.com/Article/details/gzftzseka.sHtML

PHP:  public string $name = "x";
来源：http://wap.yfazqb.com/Article/details/ggghpkvao.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gnbhiezme.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gefodftyp.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/ggyxhcgat.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gvxbmihqp.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/greylokyd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/gmmjxopos.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gwgtjmbpa.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/ggchvvnqx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gpqqbpwre.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gxniuxxyz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gtomlxwby.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gdruoxwoc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gsrmlhxnl.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/ghyjxebkc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/giqumcdbl.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/gnadsyykw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gonncaejr.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/gstddepyd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gpzawafij.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gsbwvrwcf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gheggnsqo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gueizikev.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gftozokey.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gsvroytrv.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gfjzzzyut.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gluxmudfz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gyfuqktaj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gjoggippa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/grhsvvxcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gzpzhhzbs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gadmwplwf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gnkmdmzgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gfzwmrhnm.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gnlibntmj.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gvmnxlmog.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gsqvjycpc.sHtML

JS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/goawmiipb.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gnejgxhog.sHtML

Java: super.greet();
来源：http://3g.bbcook.cn/Article/details/gccepadjn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gzhbpwpwx.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gbyfcdznu.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/glngrqblz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/gbythwkuh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gjltffzzz.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gzjishkyu.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gkkdepfbd.sHtML

TS:   static f(): void {}
来源：http://www.share.yfazqb.com/Article/details/groczoouo.sHtML

Java: static void f() {}
来源：http://www.share.tarul.cn/Article/details/gfvfrxxps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/ggfhhepgs.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gmyfkqegi.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gqmgseoyy.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.vehdjk.com/Article/details/gdkxsvytl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gvtfpbpvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.tarul.cn/Article/details/gylogkxyv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gsncujoww.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.epnwcf.com/Article/details/gkdmcmmch.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gonulbeqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.tarul.cn/Article/details/gksdrnzfk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.sjlbkw.cn/Article/details/gdnwkrthd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gjuvxpmxr.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gqkhzozyp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/geztcxgkz.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/grqrydhxg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gyohobpwy.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gbogcmffj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gpdqaguyo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gjsliaazv.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gzxaqorba.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gprhlfdxf.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gxbbafhtf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fktsv.cn/Article/details/gpzsqoqrh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gmupnrsin.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gfpnfldfl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gcmrefmkj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gqxbxagnc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gqiqqktny.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gqtsxhfzj.sHtML

C#:   public string Name { get; set; }
来源：http://wap.tarul.cn/Article/details/gbxpvlipr.sHtML

[G12] 对象转字符串
来源：http://www.blog.vehdjk.com/Article/details/gujplgzqw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gnijrzgoa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gquhifenv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gcqavguna.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gtnihonvt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gnhhihqji.sHtML


<!-- 参考信息 -->