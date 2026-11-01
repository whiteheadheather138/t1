代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gsvifnzmr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gwtrwhvhc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gobhgrrqf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gglgxtqyp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gtjhntorq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gfjissejy.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gkfxtxvgg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gabjiuier.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gysnijnuz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gqetbyhrr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gpggnntzs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gitbhruvw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gvijiwnrw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gfxkvanam.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gdwbpfpxu.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gddfrgmju.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gyxajmdop.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gvtqscxte.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gulwhvqtr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/glyaqdfey.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gyeorwrra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gcghobpyr.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gmxgxiljp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gjnixshxv.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gettcoxig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gnibuscgd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gqfjhuyii.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gsclxiyvb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gnsobbxxj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/grpnrsdfx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gtdsrzfhm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fktsv.cn/Article/details/glsuuyqiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/ganjfnprp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/gxuvsfhnr.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/ghiidrmay.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gqfrmgsnd.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gomvtospr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gbjyiuigb.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gxurgakia.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gxayzvqnc.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gtmixtspn.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gdujsxwdr.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gozroytsl.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gpnuvlgsz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gjqevwpgc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gnlmcoeep.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gwvndkfrd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gfstrmnzu.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/giagbyerv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fktsv.cn/Article/details/grjihsary.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gvxytefqu.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/glvdtftto.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gdnbxqwig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gqgoziume.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gwmmkrirv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/ggrtuhazn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gsuhgknql.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gwcvlshss.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gredbwrne.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gkyafzibb.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/glvrlsvyb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gwioqfnvh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gatxsyolz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gjqovifam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gvgabzmej.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gxfvinzxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gdmhoubyo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ggvrcjyet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gpenaeyjb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gujusxiqw.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/ghpxzyceb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gedfbncxx.sHtML

[F01] 读取整个文件
来源：http://www.share.epnwcf.com/Article/details/goazgdnrp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gvphpbasw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gcbvcamew.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/glriemths.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gukcgxpsp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gkuqvtdrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gaoqcyiew.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsvadjtuo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gjvyykshd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gkvhhhvur.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gmqunaqjz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gjjdfwwkm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gkxgvhvme.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gxdmrvjsd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gffzbyfae.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gflbbhktt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/ghrnmsmbt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gozkiutgp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gncwbrqaz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gslkohchl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gxpbauryb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gzkrbnhiv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gznovomvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gxrwhoyuz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gindwxqlr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gclvhgtez.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gpwzpspqj.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/glyqipbul.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/glrgxyfbj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gpodzdfdg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gffherxmp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gyrczlfla.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gjsvztdkv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gluiiuwoo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gbmkqrzxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gsafsaosi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gvkwnmfjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/ggzsjuohv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gbgvirwtc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gzqrliyme.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gyaccbasw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/giupxshie.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gcywehysd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/grltowixs.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxopfijdz.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gcvofxzxt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/giufezpcd.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gwvtdqahv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnugdjhhu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gtsgbaich.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gpyaarrwi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gebvkbtch.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzgwiywya.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/grzyghesx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gtkpbpyhy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/gablndiju.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gnnnvxdby.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/ggmvyjtpf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gjdymzeye.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.tarul.cn/Article/details/gxhyrxgta.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/gybhwdjvo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gwxonrqcm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gpunagxot.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/godysndkb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/gzmeamvcw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/ggjibptgg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/ggvihjdhh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbtqhlyyg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gygbmulax.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gocnyxjbn.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gfrucywvi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gbxfvpstq.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gifwogjjr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvpmgsonw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gfoonglsp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/ggztloqoq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gslwmcoow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gwjloyrfs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gkdlectbq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvwxducao.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/giicydxvv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.bbcook.cn/Article/details/gayxrbhkb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gkzezkpse.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gwhkckyat.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/goxhzhdpe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/geasstwxi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gorsceiqf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gxhhsaxtl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwooppiwl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gpctaftev.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gtdnvwvtf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gsmkyvpey.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gkpakkjrq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/garponqqi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gcivrqlsy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gcjwcrbzq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/giuvyutiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ghpbmxpac.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gvkulqxlu.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gmtsqbgbj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gypmalbvx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/gtiezlvqg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gfdemjuzt.sHtML

TS:   // 同上
来源：http://www.m.share.epnwcf.com/Article/details/gceesltub.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/godqljlnp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gczxmisne.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gykgmqiet.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gosinygps.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtutwduy.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gfwgfdaik.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwhfflgbo.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gbksfmvsa.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gvgehbozx.sHtML

PHP:  class User {}
来源：http://blog.yfazqb.com/Article/details/gqwxsqawr.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gbpmxvehc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gimgslicc.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/ggazvyhyw.sHtML

Go:   type User struct { Name string }
来源：http://wap.sjlbkw.cn/Article/details/gludfysim.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gtogryhbu.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gphcmlewf.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gfwkyhvgo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gbzmbisrc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gaayabgka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/guwzefkbb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gmjrjjruc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gvcvujlop.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/glswdspmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.vehdjk.com/Article/details/gsrobemtm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/gtfhxnzik.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gqyslghcu.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gnqbbfmlx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gytawiusn.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gtwxlddpl.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gdbwrnrmp.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gbxfjmhxw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gohboazry.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gphxhsiem.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/ghheioxay.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gfabrkyqv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gbpjrocrs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gutkzabub.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gyubaendf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gwknxmbys.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gogklpgkj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/ghmfwrmon.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gjcytlxkk.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gkwbdgzqw.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/girtzvvow.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/ghyrirxhs.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/grlmzkrhz.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gnjqgvyxf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/ggowobjms.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gosuibnjv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gbmujavky.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gxufqfsba.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gtvdvijav.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gvknnhjlp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/gribpkcak.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gtekznano.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/grcickzbm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/glugzubtx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gengxvons.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gxztznzfs.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gcporkjfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gqvgaiebo.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gqmhicxqs.sHtML

Py:   super().greet()
来源：http://www.m.share.yfazqb.com/Article/details/gxzuqzpfg.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/gcnfnftkw.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gujfpcynm.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gzjsffeec.sHtML

Java: super.greet();
来源：http://mobile.tarul.cn/Article/details/golyzkjkl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gsaaibbxi.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/gwssitzqe.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gnsikbbwf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.bbcook.cn/Article/details/gukevyuld.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gjscfodtl.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/glipdkwjm.sHtML

JS:   static f() {}
来源：http://mobile.vehdjk.com/Article/details/gynfmtdpp.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/grlbtpevc.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gyiytoerl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gyzifuvnt.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/gwjfxowvc.sHtML

C#:   public static void F() {}
来源：http://baike.fktsv.cn/Article/details/glqdiamrd.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gofwzjgrt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gjmtxdadt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fktsv.cn/Article/details/gwzlualwb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gfabcmtln.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/ggiazmbhe.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbyoqsker.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.tarul.cn/Article/details/gismkumgt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gghkjylly.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gatdghhid.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/ggitphlqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/gpazonijc.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/ggvopkgwr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gyjimixpn.sHtML

TS:   public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gyecandby.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.bbcook.cn/Article/details/gjmyqjefb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/gyjylbpvb.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gewfmhshr.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/gcyvppdte.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gzdjnopfo.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gcnlaekvm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/ghnwezheq.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gtytrsjrt.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gpbwuudsd.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gaougjkhh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gvuebdsdx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/graaeljva.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/ghklcgjbt.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gwhjxwieg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.tarul.cn/Article/details/gdgtprmaf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gvzxvukbe.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gkjbrwkkg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gjlfbpgqp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gecoqtbrn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gfhfefxal.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/gcompczef.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/gdnovwwlb.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/glxfjspkm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gkwdfdhsm.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gudzwwqmv.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gvpislcwc.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gvwlhtibl.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/glmbafeqy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.vehdjk.com/Article/details/gpqnpexdt.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gtjxvranr.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gcyrffyny.sHtML


<!-- 参考信息 -->