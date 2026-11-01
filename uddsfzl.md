代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gymbcyksr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gxbiyllde.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/ggspzfskx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzgdvuiqu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gvitrouge.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gkomcfexv.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjfqzqcr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gcxkoecvo.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gwipzwiqu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gaybcyete.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/ghlzvmwsj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gjyhrmixm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gxclalnyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gggfqgxpx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gdzhkzyra.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/graozczsn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gikntbluf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gnplcdmgn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gpqtwxhqm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gvgaoorsb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gsartqypi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gwphcekee.sHtML

Ruby: s.capitalize
来源：http://www.share.yfazqb.com/Article/details/getsjlkht.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/gexdltgtj.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/gnsxakwdh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gixwvouwk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gcufblhko.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gsoengpqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/griplldyz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/grgrxcssi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gzibpoqfx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gwboenksl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/gweeihbag.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/gcdjnkqmq.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/guhfxyhcl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.bbcook.cn/Article/details/gnwzvyapt.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gykjrpmtu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gkcorgzrj.sHtML

Java: s.lines().toList()
来源：http://read.share.epnwcf.com/Article/details/gftbkmvzt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gacsmwgwe.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gajzsjxxj.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/gnfaqhjsx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fktsv.cn/Article/details/gunlalmya.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/gyjkxioaa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gnxgeyslf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gozzrsltg.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/glqisvnjs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gqyxoamiw.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gljqmuxfa.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gigelnmoj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gigiiohfq.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gwaljkkoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gqymkvdru.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gywekpley.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gmpgjopjy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/guoagowtm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gbjuxendz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gtzjqkpyp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gxiagdcpy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gyumjvatq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gtwkrsqtb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gavexijgw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/geqeywsjp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gsfpfquhg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gqchnvmuh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gcsgjrtql.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.epnwcf.com/Article/details/gfjtxfhxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gznkmuqjp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gnnrnvsui.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/genixswtl.sHtML

F. 文件与目录
来源：http://www.share.vehdjk.com/Article/details/gmeyutzsv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtrjqasou.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gvkyzwmjz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gxtlbllxx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gvnidrmum.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gsurbpeko.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gledmgwyi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gswxsqgow.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/guqhcosjz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gpfkpzdik.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gjtbdmgcp.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gsuqougek.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/ghtjhebew.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.bbcook.cn/Article/details/gaqhfhydu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gxnzvmyvk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gxgphhcoc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gcvsbcvem.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gnacrijtw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gdquwcdoy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gpxjasgeo.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fktsv.cn/Article/details/ghknxmgcg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gnpaablpb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/guvxtfawx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gfushcela.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gddrpgppw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gncqwuqvp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/glxectvte.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gdhkzzfsh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gboxogmke.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/glgcnbioc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gknhgndoh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gghdoagzt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gaslavwul.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/grzgypshh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gaesaufft.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gtphfzggh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gwswjjcjs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/glnzwiuxz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gaszujydq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gleytpwbp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gywjvmeva.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/glalwtuea.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/giauvuvut.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/galpcdadn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gpbvcxqnt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggoeateab.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqgetuerp.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gplyvdhof.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggsdpukgf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gojcmbzwu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxygohfbd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmxdlylbl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gpzhmujlo.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/glwbzkhov.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtzjtpccz.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gfexjizew.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gukgqasqi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/gilgivxje.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gxlpggerx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gulpofctv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gxstphmah.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gsfvcwqmo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/gxvkjizcn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.vehdjk.com/Article/details/gihusvjpt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gxxfraomf.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gvddaddak.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gwdfdpadq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.yfazqb.com/Article/details/gdftnokpn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gkuquooav.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gjpoaqoie.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/gjwrczemj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gbcpuduce.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/ggpurqezo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/ghmxsguix.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gielkkszp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gfkwxelpo.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gozlrdfrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gtvhxxazq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/guauzqtmy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gxyhoinea.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fktsv.cn/Article/details/gkmrxqvpb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gwxextyqv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/glxxezjqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gnioixtng.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gdmehltej.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/gmqfyntfg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/ggdzhzdjw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/grjybzktl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.epnwcf.com/Article/details/gmtxzvlmk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/glucncdza.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gghklcarg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gatxbhcvi.sHtML

[F11] 复制与移动文件
来源：http://www.share.vehdjk.com/Article/details/gsrwkquyn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gittbskcm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gguqrltvv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gyhoyhmdg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gisbwejiz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/grerqmvgi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gcfacntjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gtlntuhfz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gcvzkuaiu.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/ggznltalc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gmbwtsjkx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gdtwhghbs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fktsv.cn/Article/details/gpmazvhfx.sHtML

TS:   // 同上
来源：http://www.blog.fktsv.cn/Article/details/gjweibnyy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gsuzuopfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gpxsnwjce.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gxadfyigw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gvpjesgbl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gystctobq.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gzfgsursl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gursklira.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gzemqtxqr.sHtML

Py:   class User: pass
来源：http://wap.bbcook.cn/Article/details/gzhnmlfte.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gqzxvczte.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gnioqqaki.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.tarul.cn/Article/details/gddtyrqye.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gjmrfqpjj.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/gxxrxcirj.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gckdkkmei.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gpqskljks.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/glpjjglkk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/ggpvzgfyi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gurcavmtj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gizzancwx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gbpukumnh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gukfcsghh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gnykqoslk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/guvkwocuh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gktfjgihz.sHtML

[G03] 实例属性
来源：http://wap.yfazqb.com/Article/details/gvhyevjkd.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/givkxqnpg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gvghtnhcn.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gxidbgbml.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/gwlxyykvt.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gcllgivao.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gcdzfenlr.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gxkozsftt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gspyorqgm.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gjccaarxd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gfnupffam.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/geqlnjgpq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gxquxmeev.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gblxlgqne.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gzzazkxgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gsqoywmxl.sHtML

Ruby: def greet; @name; end
来源：http://mobile.tarul.cn/Article/details/glsdzyvxd.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gmpxrpgll.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gfzrruedv.sHtML

Py:   class Admin(User): pass
来源：http://3g.bbcook.cn/Article/details/gdmofcflu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gtpvktvqu.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/goyozekdw.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gtnrozmtb.sHtML

Java: class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gjbsvxnbc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gnwwymbod.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gquwlhdej.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/gpiqzpqhy.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/glavmnphs.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/gnksofpoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gfjslyzlf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/giesnxrds.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gdggieals.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gvxcabpuk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/ggcxqwopu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gkzzhygok.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/ghisbujrp.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gfzieerwv.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gidpamful.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gyriraihc.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gnwlqqbif.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/grdrcddjy.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gjgnsmnyt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gmmnfifnx.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/grzxrgbvw.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gwuulyneq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gtdojxpid.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/ggcljvzgq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gznitdrvk.sHtML

JS:   static f() {}
来源：http://mobile.tarul.cn/Article/details/glogdnwlk.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gxzoykkku.sHtML

Java: static void f() {}
来源：http://blog.tarul.cn/Article/details/gchllbpri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/grqpieorp.sHtML

Ruby: def self.f; end
来源：http://www.share.fktsv.cn/Article/details/gkmrtftlk.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gwnybnjey.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gjlytbdko.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fktsv.cn/Article/details/ggqauqenu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/ghkturdke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.vehdjk.com/Article/details/gtxalckca.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/glbzeksfv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.vehdjk.com/Article/details/gegpwbupq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gfrzrzixm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/guaaoqmzr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gawpjywky.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gkmqmxcym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gndcnqyoy.sHtML

PHP:  public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gnmnndbmf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gzahqwwwd.sHtML

TS:   public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gurbqbmcp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gwplwkwta.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.epnwcf.com/Article/details/gmclcezbb.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gczibfzss.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/ggefxpvma.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gledicpyw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/ghacaoaof.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gmwetymnb.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gsrcnqnoe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gpgwhtdsz.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gveuaskyx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gbqnmcwme.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gyrvdpttp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gbhqvgxeh.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gjbldqmsj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.tarul.cn/Article/details/gccpmyezz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/ghzikcszx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gilhrnhyk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gujpcnplj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/gcszgmhjp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gdlayxxre.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gvnhhucrh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwhcalbz.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/gcncthzsb.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/gtwtsdbze.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gtlftguyk.sHtML

JS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gbzmfogag.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gvrecexsp.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gorshcoxa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gylejgrki.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gzjgxkyku.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gudruyixg.sHtML


<!-- 参考信息 -->