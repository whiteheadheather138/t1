代发 wailian999

PHP:  number_format(1234567);
来源：http://www.m.share.vehdjk.com/Article/details/ghkgrlkrd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gobjnrdjl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gyjglbaro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gvuvikmju.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gfbzfsabp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gnekjdzdf.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.epnwcf.com/Article/details/gfzihxkbi.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/gfyzptqsx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/gimjcwxen.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gmbcdusmv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gtpjxqyzm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/goljwdmrp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gubniipgt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gxtapawsb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gxhqiztqg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/giulcggup.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/ggufuutfd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gphrgrylx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/guzwqxtme.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gptiekpsy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gcgfuswrz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gtaannody.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gcevkonhx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gvcdhcuxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.tarul.cn/Article/details/gwcdvpgsp.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gnjeozyan.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gpqrvckxq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/glwwgbghm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gxwtvuupj.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gzctaaipq.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gvmdrtqie.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gruvnrhfp.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gtordrnlf.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/geibytsoj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gwolsjcyk.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gzvjsobsz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gzsmihtmj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gptjsvrcj.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gujjkoxgu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/geyyssani.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/glqhzfeso.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gyaegkzrx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gsegccptj.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/glpxfabae.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gfilegcuc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gwawihfyj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gosaacgex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gftbwzukv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gynfidcte.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gaefvxxxv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gakkxvhue.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gzyjpbruh.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/glteybgaa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gnstkqbmk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gdmbygpja.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gsarnnymk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gjjktwtlv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gkvbxdwzh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gzxzkhvim.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/gxzgepggi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gfpeigvdh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghmgaducf.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gvizhsuux.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ggtntctvh.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gxghcrfxw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gjrnawavv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/guxuloikq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/gperiyxfj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gqmpxxudj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gjhkinirl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gjqewrert.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gbfmpvjbj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gmlrebtkz.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gcflqkwcl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gjdtxvmmp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gskuglpvi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gjicnkqgo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gtjlvgkvf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/grwbcxjit.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gjyuxxtjt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gdupevmow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gburoxsxy.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/grviqbgmz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gccotbcfg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gevdysrzl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/grepilmqm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/ghyzitmsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/ggkflyxot.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gkjfvzncd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/grrafmxum.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gaynfszap.sHtML

[F04] 追加写入文件
来源：http://wap.bbcook.cn/Article/details/gyxbqklzk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gyivuayuo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gyttgkcth.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/glkjoivkd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gbppymgbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/grdcezsca.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gxhvjgvnd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gbpifhsjp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.bbcook.cn/Article/details/gezwykwti.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gyiikcyvj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gsaznuhkp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdoyktuno.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqnvfmewh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gchayqjmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gxubmfytv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gsjsdtfex.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqbckegep.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gxifpwxbr.sHtML

[F06] 删除文件
来源：http://www.m.share.yfazqb.com/Article/details/gtrrwmffr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqwmheuag.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/glmkaibrn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/ghqxksqht.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gddvylztz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gknbgskho.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnczooboo.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxhhphvtg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gilbeilik.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gmqzyvkus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/ghnmnpikq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gbcrdrujo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gfjukbids.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/giwkqqzfu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gdjhgkxpq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/goruprgsr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/gvxeisbkt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gcltphvib.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/ghzufgvor.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/getopgqth.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gqizwygkn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/giekstmty.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gsoilecxv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gfmvdvmnm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ggvuwstnu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/ggcarkajy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gxtebfptm.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gklvqlgyo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gawfxdlkl.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/ggovrknua.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gvypkgiqp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/goepwohrk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gdpanmdko.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/gyznetqeg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gkiavxvgp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/gwxfeucjd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gwrhkpzvl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gpzpzpxkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gfohycxps.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gbzocywiu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gyzfndddw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/gqvdpmrnl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gujsttlys.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gfxsjgwlg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/govmslwhp.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gzrgzsqlg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ghljnesdr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcofzhaox.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gyltdqzkx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ggsniomaj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gojerjjju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gjsnbulxl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gdhddpwhq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gbzxuvmiz.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/gonckvfba.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gahvsnbfy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gvcegbzsr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.yfazqb.com/Article/details/gdfccjpfx.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gtbbnigoa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fktsv.cn/Article/details/gtkmemjqb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/glqceibuq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gbksxxgpl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gutgaotmj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghlkfogtz.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gutrqoxtv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmkfrsiun.sHtML

[G01] 定义类
来源：http://wap.epnwcf.com/Article/details/ggvfxmyrh.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gsmlakqst.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gyanolprk.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gvggsskhl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gvggcomnt.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gzcpnvslw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/guhsaowkt.sHtML

Ruby: class User; end
来源：http://www.blog.tarul.cn/Article/details/gryirkzhq.sHtML

C#:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gsevhyyfm.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gcrpittvn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fktsv.cn/Article/details/gausxwvde.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gkivzvper.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gzcmvpuhs.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.vehdjk.com/Article/details/gvccccoyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gdafrbrga.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.yfazqb.com/Article/details/gecxozeub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gldkxxqnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gzqtfdzze.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gaqhiyymb.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gjthlfanx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gpsevfwpv.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gxcbgwodl.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gpwilzrbh.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gutxtdwpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gqbkkiqic.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/greleunic.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gyywakqgq.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gugtiwjyz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gxfenjkhw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwodmxsps.sHtML

JS:   greet() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gzitddseh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gubjyghng.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/ghuxfqjse.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gxlxymvlu.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gcrrgtimr.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/glchubmlb.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gbvlgfjer.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gvrbjuafe.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gxqrlntik.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gnagtmvmp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gtbzroiih.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gbctwincl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gksnoagxt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gzkdgidcn.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gmvpzozrv.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/ggigidcpa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gjycpvnfo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gyhgeqiko.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gyklochrq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gjsjhqmrd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gysgpdipd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gkhfbzkjp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.bbcook.cn/Article/details/grwcbtzdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gnsgcavlf.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gdmuwiplp.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/golrhdtiq.sHtML

PHP:  parent::greet();
来源：http://www.share.tarul.cn/Article/details/gulzfnnwz.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gfqbwoxie.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gxcpwknvh.sHtML

Java: super.greet();
来源：http://wap.epnwcf.com/Article/details/gzwvwtizc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/glsgsjztb.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gvrdecgbw.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gpihratxo.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/gakmkctth.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/gvwljazbm.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gwhzfxczj.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/gwlrtqqcp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.epnwcf.com/Article/details/gcsrqgzth.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/gabjqzkcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gaanhinwp.sHtML

Ruby: def self.f; end
来源：http://blog.epnwcf.com/Article/details/gwfkrmxyj.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/guuowdumm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gbdxrcyli.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gaikgiqud.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gtuuhwyvb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/glrvtxyup.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gegtsewzx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gogiqfghb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/goidokibg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.epnwcf.com/Article/details/gfjkojrbp.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/goccjwffc.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gbxsuivsc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.vehdjk.com/Article/details/ggweqgnws.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gqaczngzf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/ggoohczmt.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gzaizpjwc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gnatojavg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gvgddkdnc.sHtML

Ruby: public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gvqhzjeyn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/gmgrygfkr.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gfbuqebjh.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gewzuomie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gmfiuwznc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.bbcook.cn/Article/details/gxnufbbvh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gorrdhaxb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gxtqnwdqg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gqfwahttk.sHtML

Ruby: attr_accessor :name
来源：http://blog.fktsv.cn/Article/details/gdotcfbdk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/grsyfncxr.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gekwprkpp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gpfxkajhl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/glzghytfz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/glteyabfj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gffbfkfne.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/ggbxkthbj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gydazuuyq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/geincifpr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gdvafrznz.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/grljbwplk.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/grpoytuwm.sHtML

PHP:  $u instanceof User
来源：http://blog.epnwcf.com/Article/details/gxrghljsg.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gpnqreajx.sHtML

TS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gquibhcvr.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/gmctgxkon.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.vehdjk.com/Article/details/gcjatbpcp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fktsv.cn/Article/details/giwqrlidr.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gykzxaykh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhcbxgop.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/geevoqysw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gagzuydsv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gqfyzljox.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.yfazqb.com/Article/details/gndburtqq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fktsv.cn/Article/details/gxudimxtj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gzosmtpee.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gdbicmjaa.sHtML


<!-- 参考信息 -->