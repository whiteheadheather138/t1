代发 wailian999

PHP:  number_format(1234567);
来源：http://blog.tarul.cn/Article/details/gloareflz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gpnhpwjfr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gqflaokgr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/gecyfecuu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/ggrtefpfy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gcyikuhhe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gnesuowoa.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/ggtmnjqca.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/gsumofvtv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gwkxwfxvl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/grxwuduul.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/giuiioheg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gzroewutt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/gravqqtdq.sHtML

Ruby: s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gsetdrgcf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gyntweyzy.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gzvwijaxu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gxkpqrxme.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.bbcook.cn/Article/details/gjkqhaugn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvgsxvkz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gtpcladyx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gsthyqosp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/ggssingnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gtlpgaaiw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gifilwhda.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/grtbhlkef.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gcwgrfnuo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/ghxdmchax.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gjbewkoqf.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/grwqyhkdl.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/gtpbfouqc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gqovmugik.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gqbrkjlrs.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/gulempcap.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/gavktzpiv.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gnrpjjiew.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/giwbzncmi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/grewlczng.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gcjphxsgh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gycfqqisb.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/glhydvynl.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gxhjrplqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/grlwiimqr.sHtML

[E21] 超长截断加省略号
来源：http://3g.epnwcf.com/Article/details/ghpkrpulo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gentwcetw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/genofmdfl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gspsokcmu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gpyaaiskz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gwojchlcq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gflxczdsl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gbgsxnnom.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gtznswjlf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/guxbssbln.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gzgnhsejf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gwrocjovd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gnqijntte.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gtjpixwid.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gjdgjfinc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/gzatqotgr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.tarul.cn/Article/details/giolagcee.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/ggqswcjlf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/guoxwcazw.sHtML

F. 文件与目录
来源：http://www.share.vehdjk.com/Article/details/ghbdnooxf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdvbunvtq.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gmbouablc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/grtmxxcqt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gaqvhtlgn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gvmuuqsul.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/grikcadnk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gzaxvdpwj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gfblqkcha.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdlffplbx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gdaivanwo.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gyajzniah.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gikytpcyd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gcpruplni.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gsqvpdfuj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gwuywyzmr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbzrpjnf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gmjqtfqan.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/ginlyxbcx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gopjwfuxn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gegoynius.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.sjlbkw.cn/Article/details/gqvkfaqvz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gqjckawgj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gkcoiahln.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gzizcqmhs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gyzfmmjiw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/ghftazmlv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gbmxhmksg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gfjjkhvmg.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/genrzwwtg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.epnwcf.com/Article/details/gshsucggj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.epnwcf.com/Article/details/gsohdyhep.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gllssdozk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gknbudanp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/goojkkkgg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gggaebxwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gddmyvqbn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/glbznqxlj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gytaliznr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/giovfgtri.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gostxcrjr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ggwmrwiaa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gnsdudtii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gsxykqhxh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.epnwcf.com/Article/details/gclljxjlb.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gieytithu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/ghcmftepj.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/gbtvbqgop.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gyqdrmybq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gapmwhqdb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gkawkhvut.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/goedoubfk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gxpdnpbjs.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/grttokpmo.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsamrtsxq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gcacbrzam.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gelawxhdd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/grjowrufd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gnnzkrlyn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gzkftvhnb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gaaphugyo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gegyuxzpo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/gwgeblhrc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.bbcook.cn/Article/details/ggseycwkg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gdbkrrrzi.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gqkwqquug.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.vehdjk.com/Article/details/gioipkndv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gqhkfejyw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gaashapvy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/glzarrtxj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gmhravexz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gredqnknd.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gsyylmixn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gawqhszag.sHtML

[F09] 获取文件大小
来源：http://read.share.fktsv.cn/Article/details/ggnikbgkt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/grfteulqz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gaqovczmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gswkyepnd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/godpxdarm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/givknrfez.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gpzarvyfo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gztzibdvm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/ggcntptdn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.epnwcf.com/Article/details/gqcltxsoj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gmltcsips.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gczoegckc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghcamrfbx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/guqdimwoq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gayukcjbl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/givrazuit.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gxieupald.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gjaxunpnl.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/gcnlowkbh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/goqntrkft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/ggpgcndpe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gsmoeddnd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gzngqxjuq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gxydjoudg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gunprpmzl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsrglwvod.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gfyzagihu.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gdbjhbzck.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fktsv.cn/Article/details/grejdrsim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gzhmsyfdl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.sjlbkw.cn/Article/details/gdgwclotp.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gjlexetlz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.sjlbkw.cn/Article/details/gvczgmscv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/guoiqecnz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gmkbimwjh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gudakpkmq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gvbvhvtfj.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/ggoofwgdj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giskhxukh.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gnvnfrbxh.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gieatftxb.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjqafbovk.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gtrgvehnf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhzuhsfq.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gfwkpgtdm.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gpgltzoel.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gzkawettf.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/goocrmywq.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gdcmriccp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gwxahuvol.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gqbekbjxo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gsekvpkze.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.yfazqb.com/Article/details/gfsyewiue.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gxrqccqon.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/grpvvriik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gqdjnvmep.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gysamcpqs.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gwjfcttrb.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gktbzgcku.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/geiwkvzmx.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gvfbbsuqw.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gfuayzbhz.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gejilqiwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.vehdjk.com/Article/details/gpkapspgu.sHtML

Ruby: @name = "x"
来源：http://mobile.sjlbkw.cn/Article/details/gujvllblw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.tarul.cn/Article/details/gkdeojzpt.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gymjbcmxg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gsyflvgxu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/goackhdjx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/ghuyecdjh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gnruaamai.sHtML

Java: String greet() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gvkwideec.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/goxhuzigc.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/glidrrvwf.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gjjgxragn.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gozoeshri.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gybshgkws.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gzlqkskgd.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gpihblwcd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gtidebukd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gluhbctja.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.yfazqb.com/Article/details/gryxdlwuy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/glyaokwil.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gcwoawjnk.sHtML

[G06] 重写方法
来源：http://blog.bbcook.cn/Article/details/ggmbsznql.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/gdeubisch.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gcdnsapnx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/glwlqvdpx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gugkefntk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grooidxpz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gepgbeqdu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gqontotbi.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/ggfbtefoz.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/ggtxwstii.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gpgdxlcnr.sHtML

PHP:  parent::greet();
来源：http://www.blog.vehdjk.com/Article/details/gieswvivl.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/goanvboxo.sHtML

TS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gyhesqdcb.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gehazdrma.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gwjffdylp.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/ggsjwuugf.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gntouqxqx.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gwmezytdi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gjinxpwvz.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gdccsyiqt.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gyfnesjhe.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/gsiqjrhby.sHtML

Java: static void f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gyoxwakeu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gttvfktic.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gxahwcfxq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geyuoeqxd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.epnwcf.com/Article/details/gfjpgmpfr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/girpufdbr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gyazotfxm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fktsv.cn/Article/details/gmonxdadi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.tarul.cn/Article/details/gdwcirctx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/glzecqifz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gyvpcplge.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.sjlbkw.cn/Article/details/gedwzvgop.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gcgyafxqt.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gbhjwrmen.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.yfazqb.com/Article/details/gqsveyetl.sHtML

PHP:  public / protected / private
来源：http://wap.yfazqb.com/Article/details/gtdvspdgv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gosgmmiop.sHtML

TS:   public / protected / private
来源：http://www.share.fktsv.cn/Article/details/giaryqcqj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.vehdjk.com/Article/details/gjdfroutz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gmssgvwpz.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/ghumdnlov.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gutokwjgp.sHtML

[G11] getter / setter
来源：http://www.blog.bbcook.cn/Article/details/gtbcmmmgx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gksfigicj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/grxgbfpwr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gdnzzpmke.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmoaelagg.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/grhuvnspz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gsggtdobe.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gswwpudho.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gstctylcf.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/glezzhqae.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/ggfvapmgt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbrheutpk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/grhcmznzt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gntdmaaqq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gdcywcsde.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gmarsigna.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gjehocyjr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gpreqanyl.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gydaonxkd.sHtML

Py:   isinstance(u, User)
来源：http://blog.tarul.cn/Article/details/gsojlwiem.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/glccipwyp.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gjvlaasqt.sHtML

TS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gwfyafgqh.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gbwcprwjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gomzpmqgp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gqhdnroju.sHtML

C#:   u is User
来源：http://www.m.share.tarul.cn/Article/details/gvyipwngn.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gzkfkcjqq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.bbcook.cn/Article/details/gbzaymoca.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gncadzner.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gthpgelfh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gxrnlkjhe.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fktsv.cn/Article/details/glevnftst.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gtayhmqmf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/glziyvaat.sHtML


<!-- 参考信息 -->