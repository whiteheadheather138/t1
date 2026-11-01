代发 wailian999

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/gozvqaeij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gxdqxvzfa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gxwbxqxgz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gcgmginti.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.epnwcf.com/Article/details/gamljgdre.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gbrhcekfv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gqbokhuvp.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gbepbmpxo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/gizdlqdyq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gatuvcecw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gnsamkpbv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gypfzymza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjfohfytv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/ggbffxnpz.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gylzudemt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gncmgoqjx.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gibkzazjh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/giawkomcr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gdbhpxcfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gnzehgrpr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/ghmdntgjc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gftfcvpus.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/ggomfntyz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/gcukuomfl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gbcwxeuqd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gqwojxjvm.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gcwqdxynb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/guykgsmgo.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gjxzgzuvu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/glloukfhx.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gmuypegcr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gupsulcro.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gghcbucbl.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/glwgjeazh.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gpsalzskv.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/geblrovnk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gzsqirwte.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/giiizjxyz.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/ghjmthrwr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gensydzfh.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gplhwfhkd.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gvntlgimv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/giqeclccw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gfhvfqzcj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gogolgwgp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gbccetbbi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gmbureykt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gbiohtpam.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gscicibmd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gytdfferf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/geqiswsmr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gntxsqhki.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/guxxignzt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gcbwvzpjk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gcvrjlpsl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/grwvoiyno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gnhevtaed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gmzfvvfan.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gnfifqydj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.tarul.cn/Article/details/gmegcivrj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gyslsuvkf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/grmymxajn.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/ghlawyuqv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gakherqmc.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gorsublot.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/grgmncmwh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvezrkqoo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/gwtjmfzuh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gqgwrevzt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gdiiqtthv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gthuxakif.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gvmkqlbmv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/glhrsnqjd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gpvwxwnkp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gunvucvjt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gvhgswyxx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcmkvqxjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/geggntody.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gybwioxog.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/ggokbcynj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gloxsjvzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gnxmdcopy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/gwmhjayzf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gvgrqvkli.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gxyloyvvj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/geuxluadw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gczqiadsj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/gdravwbgv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gdfztztjf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gwuccytam.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/ghnowtgzf.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gyzvmrsjy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/gdmdkqtal.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gsidkimew.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/grdpiswse.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gmiffqgst.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gigwuabtq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gbgqhshvx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/gjnpksbvi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gwrimshts.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/ghlolidsc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/ggmuvamov.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gpfjaaxgp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghzrgcdej.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gckgicruc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gtephcnov.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gylwbzyat.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwbmazozi.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grucdzndf.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gxtlwxlas.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfazdqkog.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ggfhzdjan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfhsjlszp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdqqdaawy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/glydodhtp.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gxwhwfpxz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ghjvjexdb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.vehdjk.com/Article/details/gfudcqlqd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/goqdqtrth.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gmcqipwig.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gezdjcgyo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gddqvficr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gebpomgtx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/geslvbmnx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gugsemgbv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.yfazqb.com/Article/details/glfjcjfmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gjkecoshp.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/gaerydsdq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gnknljnii.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/ggbcwcxpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/ghnjqccrx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gyjgpfumw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gfdorfhcp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gicqwnngx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gbyozgxmi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gyjtkdjvt.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/ggjzdvahf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gneuwvsxd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gdkcdesrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gdftrvuup.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gbnrsiojq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gdwbloyjt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/gabycdlnz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gufntvocf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gekvhjogy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/gvhpiumyk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmcajudky.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gosnqlgdl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gpndqjsyd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gkhyrjgyc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.epnwcf.com/Article/details/gqdooxhal.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gjtlyyasf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/geehyrogg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghagbsahx.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gacpdjbds.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gskhafauv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gtfoqkrqz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gesyuqmon.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/ggixxzhpd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gjjylrlzo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/gyrorkers.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gfmyvxsei.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/gytumyvit.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gkqgfceno.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gllvvshlz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gxfsczhub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fktsv.cn/Article/details/gzwzklnop.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/glsjwuzts.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/gxiiulcdf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/grjpmjlew.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gzwswuvwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/gmqfhaoix.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glxxtaqql.sHtML

G. 面向对象
来源：http://m.share.tarul.cn/Article/details/grcoajuno.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbetmhcla.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gkeqsmxip.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/ggkphfztk.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/grkswdqke.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gexpaywra.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gwmncwtcj.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gkoeouxiz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gwpjjubxy.sHtML

Ruby: class User; end
来源：http://mobile.tarul.cn/Article/details/gfwxrzlog.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gppkygjoj.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gxzmipxba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gxpesfypi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gvczdfeav.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gzvntisem.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gddyodpzf.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gzrnnhgxa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gguibydrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gbzghpbue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gzyqgxdek.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/glocozjon.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gugjrtxea.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/geasmqddn.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/gutqzbzrp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/ggftyaqpl.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/girmehsdp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gwnrxwalz.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gcrdkcpys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gygsoebbe.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gfufajjnj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/ggqldpdgl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gigtalwxx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gbaemflqp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gigkhtceg.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gowwgojhk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/ghfaxhfqi.sHtML

Ruby: def greet; @name; end
来源：http://read.share.epnwcf.com/Article/details/gukypdsis.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.epnwcf.com/Article/details/gyuxtphou.sHtML

[G05] 继承
来源：http://read.share.yfazqb.com/Article/details/gwbmklhex.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gvmlxfcus.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gyqbazgbs.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gtnfpypxu.sHtML

TS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gfykeeawh.sHtML

Java: class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gsreinuft.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gqjigmmua.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gxrbygcpx.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gdruvmfmb.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/glebnrgcg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gcxzclyrv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gxuxruodh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/ghmynfvdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gwocmzwdr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gwcpoaesc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/gztlgfrkk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gyqaakbyc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gipthykbi.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gkvsplnkx.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgjmvkbn.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gnorzxwme.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gzacsllei.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gjhaumvxg.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/ghwwjswyu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.bbcook.cn/Article/details/gdhzknudr.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/guurcummp.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gckdzsxfu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.vehdjk.com/Article/details/gaajtlhey.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fktsv.cn/Article/details/gqknzzkgl.sHtML

PHP:  public static function f() {}
来源：http://read.share.epnwcf.com/Article/details/goxxwmgpk.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/glfdxkgid.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gukkrcsgo.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/gncxtawbv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.epnwcf.com/Article/details/govxfvqvi.sHtML

Ruby: def self.f; end
来源：http://mobile.fktsv.cn/Article/details/gbniygxwk.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gttluviag.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gguyumfvc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/grokpzhwf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gkemwjsci.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.epnwcf.com/Article/details/gjrgfahsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gjioyzuim.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gterhfwgh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gyqmvotpz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gqofsogbt.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/glupvesmw.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gzagznady.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/ggizlcjhe.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gmudvxnyi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.sjlbkw.cn/Article/details/gdzrokkwx.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gxcyzstnl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/grspqahjq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gmqifcmii.sHtML

Ruby: public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gwudmjjho.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/ggsfmytku.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gjddgalli.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gtewqurfl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gubnxwjbj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gnzehbvck.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxffxymoq.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gjlemrfyr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gbrryrynk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/ghmqdxnoo.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.vehdjk.com/Article/details/ghesuoprq.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gnvyxvdxt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gfetdrraz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjaohmsvd.sHtML

JS:   toString() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/givzvowtq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gmtujhelc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.tarul.cn/Article/details/grkybmfil.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gfloxuwsn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gcnwynfwk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/gtfwdccdv.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/gtqpshcim.sHtML

Py:   isinstance(u, User)
来源：http://3g.fktsv.cn/Article/details/ghegqjyuc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gdupepciu.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gjyaomsno.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gfotmymnn.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/grlurymeo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gtzqevldm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.tarul.cn/Article/details/ggfgazanj.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/glvlywehy.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gfyjooefk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.sjlbkw.cn/Article/details/gptubwjfe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.sjlbkw.cn/Article/details/gffttkabt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gaqhfdwol.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/gfigavxpc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/ggxzyfpup.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/ggxlzttaf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gvlimmbuz.sHtML


<!-- 参考信息 -->