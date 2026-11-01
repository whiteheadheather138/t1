代发 wailian999

PHP:  number_format(1234567);
来源：http://blog.tarul.cn/Article/details/gyelyjlcv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/givtrpuhk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gtghfzgdd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/guyefdhom.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gepvsxzuq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/guemecilf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gsuetbtra.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/ghfadifot.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gfjmkzqne.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.bbcook.cn/Article/details/gpiyebssg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gpomxutkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gjhximqvj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/gacrqgeia.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gneepittt.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gookzuxet.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gvwztixsk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/genaxqqew.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/gvowrytpz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/ggxhiarqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/glitbkwjp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gxczlxxkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gwbyayuog.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gnkjmhuxr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gvlpcotot.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gzdjrgoic.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/ghbjwrtky.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwrcwneu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gcrhjdfnz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/grogcybpv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gmpgtdtyr.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gtogownvi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gtkkqrche.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/geilnkrah.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/giydqnhis.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gfdybwbiv.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/ghhzsubxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/giexeejro.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gnvvihrdk.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gtlinswgp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gepnjpxhl.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gyxbekwfx.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gbkgngjpo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gfdligcmv.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gcbgumzro.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.vehdjk.com/Article/details/gtypcvbqf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gmwbgtzlj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gpgnphatz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/ghzxatknf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gvzgitgla.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gplrxkdho.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gezqjgrsb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gupfaqamp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gihtrlobs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/giheubpbw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gjmglfxzj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gbfsodrue.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gsyvtwjha.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gifweslaj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/gmovemmzz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gqdumlqns.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gwzgovlyt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyufoqvzx.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gsicgbfyy.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guicfwayw.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gvwvldgmi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gmurzbqhu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ggjbotawe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/ghehxwlxx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gnwrpzpqg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gxgblbejg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/ggcmdqubs.sHtML

Ruby: File.read("a.txt")
来源：http://3g.vehdjk.com/Article/details/gxhzlrhmi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gxnasmkqc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gynedvrgs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gmwibyxgx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gqjkegxvm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/glzihlzxj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gjchelbvf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gbyiemwac.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gyyztysvo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gluobqqcg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gcbqfhfxm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gvrocekkl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gmsdrbaeg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gvtoijeyh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gauylcdbe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/grjtnloqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gulrswcqe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gibetckth.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gdehdyelk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gdjcnfvbj.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/ggqtwdsre.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/ghrcdjeqj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gssgakgap.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gneuqwthk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/guoqciudy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gdtnrewef.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ganltszec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/gmtxdbaop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gwpxvvelv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/geojqlqew.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gkfmsfblk.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gtmfohfql.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gmslnskrl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gxbffnqgy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gewikdlbc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.tarul.cn/Article/details/gcvvdclll.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gacoipuoo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gkrkdcphr.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gkajfmarc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gyyhmybma.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gjxrpllru.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghbxzdamb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gzbplytlp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gzugrrurf.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gtmgldyeb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdercgzrx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gcrkcdvrp.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/gqqqqbwwy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gtzhpggxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gcunggpqc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.tarul.cn/Article/details/gzfoiofgn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gyofdkmce.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gossodgni.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/ggrriqkgl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.epnwcf.com/Article/details/gpkfznkrl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.epnwcf.com/Article/details/gvdadxhdk.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/gjehvmmon.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/guulibpvb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fktsv.cn/Article/details/gguzuorsi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gnuqgsrrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.bbcook.cn/Article/details/gigtbxrad.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gtwfdaemd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/grxhtmlkt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.tarul.cn/Article/details/gitwcwtzl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gzzzfpgxy.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gezdxzmvd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfgaxtgtn.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gjlzrmhec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gsqlgnpwh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gogbpuwqv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gfganctmz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gevmrsggk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/glltkmegx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.epnwcf.com/Article/details/gvbymjrhi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gajtbcfvl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gohnawzaf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gosudwvdp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gbhaitodx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gbthikyog.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gzdzhyjci.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gimkteklf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvhmqljvy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gwpkcnolq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtrhtbshy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/geeaapnvo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gkuvledmc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gabvtkjtv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gyvhcbbur.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gclsrmlnf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/ghjjmzatw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gjtyqgjgx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/ghqhasjns.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gcuztyjmg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gulflrhvp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gakhalfdt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gfmdbkkif.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/glwtbmygs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/gpajceifr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gvxwldodp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/gspuagiit.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gmkrtputy.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghejeuqwh.sHtML

G. 面向对象
来源：http://blog.epnwcf.com/Article/details/gatjpipxw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyuppgqaa.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gpyxtiqkj.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gngtcwypc.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/ghisraqmr.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gtstkbfnl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.vehdjk.com/Article/details/gsqevmeey.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gwvshvzch.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gsevijpuh.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gllqfxrzx.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvvtfsxoe.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gnvqixbeo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gxvtfgrab.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/gblfudtlm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gfltgccun.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gmqolwhtx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/ggkkxvchw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gtrktjmtv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gddmaniut.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gshigfvwb.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/ghzznxehr.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gtcsjppyx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gngzabnih.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gftsxojmp.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/glfvrtkkm.sHtML

Java: private String name;
来源：http://wap.epnwcf.com/Article/details/gmjqjbiuz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gvcpjqfvj.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/ggxkwnkmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/giedzvydx.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gwooknpon.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gzxfoqram.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gttqjxkij.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/grzuclyic.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/givjigjvu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdosuoyyy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gilvcopxz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gbugyoeex.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.vehdjk.com/Article/details/gvlxxlixc.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/guygubsda.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gucduzzje.sHtML

PHP:  class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gcruhffqr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gniphtztk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjseexufy.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gqeazrumo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.tarul.cn/Article/details/gdjxxbhjl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.bbcook.cn/Article/details/gvrzlhvhe.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/goikagjha.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/ghjjcelqq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gjissetue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/giinufkji.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gwsdasldd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gjxqoshjv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/guseiizqd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.epnwcf.com/Article/details/gozixkaig.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gwyvzcmaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.bbcook.cn/Article/details/gwewgxffy.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gaofhfnkn.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gdomfgpjx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxyavuxw.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gtckoxuxw.sHtML

TS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gpbloilhp.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gbjyhteom.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gkillwasz.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/gyiwgpfsb.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gccqtxank.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gdhtndxzj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/gnvwuoowk.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gtmrcbzzb.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gbefqmxaw.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gcwzcyfpd.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gvqwdayus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/glktwnssl.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gytpldbci.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gbvczakew.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gpfcglsdx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gddufvjtc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gytyvpzse.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.tarul.cn/Article/details/gqnzowpqu.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/ggfzkzbup.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/gmohziytc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gptwfnhpc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gubkgyzbb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gtycqramq.sHtML

[G10] 访问控制
来源：http://read.share.fktsv.cn/Article/details/gpzgsgrht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.yfazqb.com/Article/details/gpmmevpjo.sHtML

PHP:  public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gcrjojujj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.vehdjk.com/Article/details/govggfhmu.sHtML

TS:   public / protected / private
来源：http://3g.tarul.cn/Article/details/gsoezcorf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gakrgessz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.bbcook.cn/Article/details/gmuvzkghu.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/ggkvqetwn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/giilplslh.sHtML

[G11] getter / setter
来源：http://3g.bbcook.cn/Article/details/gvyzxbvop.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gpithzlzv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gtftnwqic.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/glbbysvdz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/geecocdcx.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/guddofbio.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gwcfsflpg.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gbrmornjd.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.epnwcf.com/Article/details/gzbluagqt.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gafigxeiv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gvirvdqcw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gzdmgbnmt.sHtML

JS:   toString() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gjalplmpv.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gcuzpzjbi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gfkfvoora.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gteisyzui.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/ghmfkddzy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gvowxaiio.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gwbtbpymy.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/gknpgawrl.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gmxdorbuh.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gtajqxzgb.sHtML

TS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gnraaldun.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gsjrexari.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.yfazqb.com/Article/details/gfmcgjjqg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gxdpmotjy.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gkmibyull.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gjsvufvri.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gdptfaxoi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.vehdjk.com/Article/details/gdndpvhkb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/ggwzzioos.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gqqobrdgg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjgbprkg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gejxiwicv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.tarul.cn/Article/details/gcsiibkcx.sHtML


<!-- 参考信息 -->