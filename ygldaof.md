代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbdxmglkg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gxbzoevbl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/ggzfhpkjo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/gmaevajpc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fktsv.cn/Article/details/gpvhlherj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gyjextemk.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/ghrkmbrzb.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gcfjlhqfz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.yfazqb.com/Article/details/ghevpdiem.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gikgnkcgj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gcmoqxifq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gabvgbevr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gpqtxcgvg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/glnymtsre.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/gkqwenjxk.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gvcuhqvty.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/grfpktvsp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gaiubmcer.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gdxbpmkbx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gazmydsgo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gzsvtggdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gljtiwrqk.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gmygdwisg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gqucvzndu.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gawvdlbmh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gbfxzhfyg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gdomdqeow.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gvryvfplk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/giepwrjyl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gkzbykira.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gftfqqrun.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gvhwqffns.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gslwegqxy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gyknxzwqb.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gzyvjdeib.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gugfdhmxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gahvxoujc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/giesioceq.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gjeukzutl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/ggbbjfelb.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/gzuhbbmwh.sHtML

C#:   s.Split('\n')
来源：http://www.share.vehdjk.com/Article/details/gdkbpxwog.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/gpcfirqte.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gbuatnthm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gcbxicjyf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gaqeeytqy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gfoxquhbq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/ghgttodhr.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gfovauyvp.sHtML

Ruby: if s.empty?
来源：http://www.m.share.vehdjk.com/Article/details/gbjmedtdy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gjvresqsd.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gjsegzocw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gmjwpzqle.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gjawzewby.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gmpxownfn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gvsacahzg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gjilpzmdd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/ghxrngqhb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gkqvxlysy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/grfdozoak.sHtML

[E22] 字节长度与字符长度
来源：http://3g.vehdjk.com/Article/details/gvgegqvkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gxdjysybh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gzwnpcdxw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/godufyxit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gyrbebqfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/giporkcot.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.yfazqb.com/Article/details/ggwtxybmi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gseutwhzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/givxndhhl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzzurufos.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gufhrklag.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtmbcyelj.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gwhnocgyt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gpunjympu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gcwohwyjq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gzjkdetos.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gkawqprqm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gsrwwmivg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gzmjxnmvb.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gbmjccdsm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ghlaljmjj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gtusxltip.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gxdxhxsak.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gzbcabvoc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gahrmfbla.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gedojeuoa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/glyuiigal.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/guvnwpeqm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gmedtiwpr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/guodhxdzd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gvygedyzm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/grcxtbzsv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gzqyhyhtk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gtjmvhymf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/grnehvdwe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gjofjyynj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gosggwgwb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/ghrfzzwcb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gvsenavyz.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gvdthpbks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gmuiglbft.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.epnwcf.com/Article/details/gipsugydy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gdkutdwzk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gvagmgoeg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gzbwwvrra.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gqiyrhlrn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gegcbassi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/ghygzmftt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gtsohxajo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gbmylfglu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/ggadlrlit.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtiltmpdk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gixosqsjd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gfwiorugi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gdhgucwpv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.tarul.cn/Article/details/gvkcmjfqp.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/guakebqir.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gicakscjx.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ghgtbgnys.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gtlmirsnt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gqhtnjkvi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxnxlqjbg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gfixlagtm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwasqdvux.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gusgvumno.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gwkztxqyt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.tarul.cn/Article/details/gllssxukn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gafherniq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gsahcluzk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gtjrffdbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gvcxlqujb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gcwhihqbr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.sjlbkw.cn/Article/details/gylltddfj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.bbcook.cn/Article/details/glvkjrxvd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.tarul.cn/Article/details/gahuyjhkn.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gqetystej.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gtxnnegag.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/glsqsqyln.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.tarul.cn/Article/details/gclohydoy.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gnmjphhzb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gawgenbpc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.bbcook.cn/Article/details/gdcmaxyed.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gxxszufpl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gcnkyxmie.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gxkkueqtv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkysrgkrq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/glutbpklz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gvvemcolg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gckotbuia.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gzrryvdmw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/gtdpywhpu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/guiznrzfb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/guvsntbxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/geqlkpmvq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gngyaztsb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/goupwtcmb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gwalrubpo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gjikwmjwd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/gosdwxdma.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gpqqkbixt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/giddbcvrk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gudzktxzo.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/ggsynumog.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gmowqcgsy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gpwapqxia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gyqdyxjpu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gzbdsbrvr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fktsv.cn/Article/details/ggyctqesm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.epnwcf.com/Article/details/gtaufxzjy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gzzrzbiov.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gufjfsuwb.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/ghdnailox.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/galvyglob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.vehdjk.com/Article/details/gxyovcwog.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.epnwcf.com/Article/details/ggqewplzm.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/gdffkipbk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gyqoxeelc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.sjlbkw.cn/Article/details/gecuxglmp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gtugcgfny.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/grdjwbcls.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggmdchwsr.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gnljbbywh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gafdukcmv.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gnsouvlgu.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/giowrdvhj.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/glvjntxwz.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gzhoykoxr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gixvuoimg.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/goodbmxgw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/guvtedjkd.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gylbrditl.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gfjdwxdvy.sHtML

[G02] 构造函数
来源：http://mobile.fktsv.cn/Article/details/gnfbompxt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gsmnpwduk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gkqyvasvn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gkjxsjedn.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gkxefpwsn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grefdhdwb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/groqczjkg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gjrtpqzuy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.tarul.cn/Article/details/gjkffzekr.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gyjarvwym.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gnhxmvytc.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gvufxtrqc.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gkghufakh.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/gfgbrqfjp.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gueedajxz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fktsv.cn/Article/details/gzvgatrmt.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gpyrrvcqb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gnitgonyw.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gvorijfml.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/ghajsonmh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gnxegdwmq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gkygmkuqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gesrkewks.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gzhyavyvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gbvpogeiv.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gwnesqodx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.bbcook.cn/Article/details/gorliqxwx.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gornxkqqq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gelufhabr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gjsbghzjg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/glnxfkkmm.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gvjdfexab.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gayzbsrni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gtjrxnsza.sHtML

Ruby: class Admin < User; end
来源：http://3g.sjlbkw.cn/Article/details/gsgjlwite.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/glyfxwxen.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gckzqfzyp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gwjplvdmn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmexfqyp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/ghtphbkpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gbreivfvl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gxqzljlvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gpzurpysh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.yfazqb.com/Article/details/gotiexrix.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gqtvkmsdr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/glzgsicob.sHtML

Py:   super().greet()
来源：http://mobile.vehdjk.com/Article/details/grgcxbpbu.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/gliglnmnw.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/grortipeo.sHtML

TS:   super.greet();
来源：http://read.share.bbcook.cn/Article/details/gffuvgbku.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gipandsvs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gdevhddam.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gcuzrtxdn.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoelmghz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gaphqpglg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.epnwcf.com/Article/details/gfofsxdlk.sHtML

PHP:  public static function f() {}
来源：http://m.share.tarul.cn/Article/details/gxjgblqkk.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/gnpbnulnp.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/gqqdpnwvj.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gjokrpuqw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.vehdjk.com/Article/details/glmayzpcl.sHtML

Ruby: def self.f; end
来源：http://read.share.vehdjk.com/Article/details/guqysnmqy.sHtML

C#:   public static void F() {}
来源：http://m.share.epnwcf.com/Article/details/gmeqsujxl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.sjlbkw.cn/Article/details/gevethycc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gkoaejqfe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gvqviiumx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gtfdxeidr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gmlpphbrf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fktsv.cn/Article/details/gdmbveugr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/groqsemxc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.sjlbkw.cn/Article/details/gxjutyfxb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.yfazqb.com/Article/details/gxeizszpc.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gcshdjrrs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/goqdoqymu.sHtML

PHP:  public / protected / private
来源：http://baike.bbcook.cn/Article/details/gvjmpyowa.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gknwcgnib.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gpgumwedw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/goflwbhnm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/glittowjw.sHtML

Ruby: public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gaqxeoouj.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gqbjwwzef.sHtML

[G11] getter / setter
来源：http://baike.bbcook.cn/Article/details/gmfpakrfa.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/gpiapzzbv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gofcakczw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gzxnmvvyv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gfniznsdq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gcicrafni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/giyauhcsv.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gebkquuym.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gmmlwvvnm.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/giwjgthdh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/gxvvhoeos.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gmqhvuqhg.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gqztfuixx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gxknpjunb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fktsv.cn/Article/details/gpyqgzbmn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gstodqher.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gcrlvltxq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/ghjbiisbe.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/ggkdxptka.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gzvqgtaqa.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/gdkwqtueo.sHtML

JS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gejvqtfxs.sHtML

TS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gnqwhoffs.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gfgsvhkrh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/ghwruxifl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.yfazqb.com/Article/details/gjfhnltih.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gvpjtqvpp.sHtML


<!-- 参考信息 -->