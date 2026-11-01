代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gpxtsdlfg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gkpvuawyn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gpgfyrbna.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gyhfmhxdm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gcuidggmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/ghiwwqtbh.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gntphnevp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gyheizxgs.sHtML

[E18] 模板占位符替换
来源：http://read.share.yfazqb.com/Article/details/gkrfkwnav.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gpozsunet.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gyijedbhc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gsootansq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gymhcjxcw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/giqsaqjob.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gcpxwnaoc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/glxobmvhd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gyqrdzooh.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/gfqpcalwo.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/gtnifcopc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gdkczvwzv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gcyokhysj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/glcbwuurt.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gkpxlgiow.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gnxuxwaps.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gstvmdfbe.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gnacmjloy.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/ggyxviddm.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gbdutirsq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpjzotmc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/glkokzigw.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gwhcomrux.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gztjvjroj.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gkpienzeu.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gnoosfhok.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/ghmqdwwtj.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/goabeszww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gzooxczdr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/glpmogeya.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gumczngfa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/ggqwxraxc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/geacbmubr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gnolynfim.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gtbvwviln.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gnrsssxfr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gjmhvppqh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gbbjzocgs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gnfdrqqam.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gwlbwwwyi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gljpjrkcy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/goewgnjjh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/grvbznsdz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/gklzahwcw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gnvedblhq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqyumdlsj.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gubtwadee.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gnzectjkl.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gwalhenzi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gtzeaprsy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxrgeipme.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/gptkbykqv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.tarul.cn/Article/details/ggmnnuzji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gwtyxesgp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gbiryrlbt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gruuaauzv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gfvvpvuef.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gdfaqghqv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gvdogqbat.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gagaxjtoe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gnanocfov.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gxddubfqw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gjvmxrapp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gshushedc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gtjmpzsxk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gvuqqyvfx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gfbuxvtxg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gexyikhjb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gauzdquhm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gjgsxvhhe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gzdjjhciv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gnqcmmfca.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/giehxaqno.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gfxebqvmd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/ghanzxesd.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gdzqwkanr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gtdauegrp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/gfgguguym.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/grpqbascj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gypnbopqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gaugoqqbi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gutmbzqpv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/gjhgcglvd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/grfzvjhpw.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/gcrlcdxrg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/gebzcqmpm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gclmmaopr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gkmuuxskx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/geaflknec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gepeqxkgv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/ggbtdecbx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjitpyxxh.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ggpxemuup.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/ggmyvqpwi.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/guotflfoh.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gtbfdawti.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gvtfazslx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcbbyxqnz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gtifrftog.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/geuzqawrc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gbvqxplwu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gvuesimnl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/ggcheixrd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gogjxfkrr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.yfazqb.com/Article/details/gaftuhbjf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/glrxpvjjq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gfziunidq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/grnrgubkv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gwtkqkedk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gjpxchsth.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gjuocraym.sHtML

[F08] 遍历目录
来源：http://www.m.share.fktsv.cn/Article/details/gtnbaqhsa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.epnwcf.com/Article/details/gjvnlqbvo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/grcsvxkoc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gzvnnjmkx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gwdgnkget.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gmxjrbiex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gdbpwpjsw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gcxtinknc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/ganmeihaa.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gpcwbalbl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/gxsjbksce.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvrwbqmmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gbtyqbymv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gwnlabybc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gubrtwjiv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gpawbwpux.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gigfwgitg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/ghgmsrjxd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gqmintcpl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gsdaexhbx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/giabtthjj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gyllcinns.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gbgbnugbc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/ghjxbgzkh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbpsehixi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/geumupdcv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gbhtzmipk.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gpjnyolwq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gzgxnzqbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gsfvklcgn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gqiyrvrdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gtbfhsazf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gwthcekju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gnzipimkg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gshsagkay.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjmpllxl.sHtML

[F12] CSV 读写
来源：http://m.share.sjlbkw.cn/Article/details/glraxbmne.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gkkyrwlro.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gjijzpmnh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gcarigtuu.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gflvkgdrh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gnejktmgy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.bbcook.cn/Article/details/gxmmssgfb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gwfodyrco.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.tarul.cn/Article/details/galbashax.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqoxxecur.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gpcftzscr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gouharnle.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/glsrnpawe.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gvmnoblea.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/gbrzeopvn.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gbsfqdxqt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gcztiidkb.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/geeedbmas.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gilqimxzl.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gkkgnryoh.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gwsrfqcea.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/grduxvmec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gigripvim.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/gpzequvqg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gcdruckjc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnyxhbsoj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gevoulxsj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gwuvlbhzp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/gcxgdvadx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gbwkpdidl.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gzqwmjqcx.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gkspqobbu.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/glwplypyi.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gosexhnvf.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gtinpcjwq.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjsibvfl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/gzdbppxbi.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gzgggeflz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gmzvfpqpi.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/glwqyloyx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gcpnpzszn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gtcsmjddt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gmznzyygg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gozncwjdd.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gbczsspmp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gsaovquvw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/ggzlhlqvg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gmenokbkj.sHtML

[G05] 继承
来源：http://www.share.bbcook.cn/Article/details/guhmbhbuq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/grctmqedw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gpyzqnyul.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gjcazumim.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/goltgsjhi.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gdkevrtcq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.epnwcf.com/Article/details/gkltdzbth.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gohtruieo.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gxjajrtou.sHtML

[G06] 重写方法
来源：http://3g.epnwcf.com/Article/details/gviufvmxz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gzoxafxac.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/govwriecf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gylhkvuhc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/giowxizki.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gtlizkxrt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.epnwcf.com/Article/details/gonynhhhv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.vehdjk.com/Article/details/gagforxpa.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gefkhyiiv.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/geibatvsl.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gwzlqutwc.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gopyizijz.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gtegojqhf.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gehdfizah.sHtML

Java: super.greet();
来源：http://blog.tarul.cn/Article/details/gmsartpls.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/givlskbce.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gpimzqqaj.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gqrcrdmqo.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/glyuyozwb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/gbimbqxvn.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gineyeqyf.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gnlehjasc.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/gbeeygjde.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gpkbglgnz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gqesfkejz.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/gtijgzler.sHtML

C#:   public static void F() {}
来源：http://read.share.vehdjk.com/Article/details/gxgfbnoiz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.vehdjk.com/Article/details/gdudwacfm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gglrkdcxe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gomiubdcg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gzhyunuks.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fktsv.cn/Article/details/gntxwdloy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gxkqnxdia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/ggamrdxtd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/godhvxwfp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gyoliklwt.sHtML

[G10] 访问控制
来源：http://www.m.share.yfazqb.com/Article/details/gnhbefhnn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/ghibpgdri.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/gbxupmvvz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gqkesmsjn.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gjvdlumjf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/grvcgirex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gwhirqygk.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gesfedsgr.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gtecmsrfo.sHtML

[G11] getter / setter
来源：http://www.blog.tarul.cn/Article/details/gitlumtse.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gkaccormm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvurvbmax.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gltgurchv.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gfxioymmg.sHtML

Java: public String getName() { return name; }
来源：http://blog.vehdjk.com/Article/details/gydhkeykc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/glvwulvwc.sHtML

Ruby: attr_accessor :name
来源：http://wap.fktsv.cn/Article/details/gbiymfzqq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.epnwcf.com/Article/details/galwcfxfu.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gcdcjqrbh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/giyrdlfaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gyzmipzia.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gvyxwuott.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gnxznbmvo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gqhvuetdc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gtnyjucjz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gtjqsyfes.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/gbggsqglx.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gnhbpljlf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/ghrhwzndn.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gqohjxlpp.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gfdovadfb.sHtML

TS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gvaqlaton.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/glmmqmflt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gkmroewfz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/ghyzujnje.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gyohhzyav.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gvaydgaic.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gsqnwjzvk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gxhfgbhjc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gyohjpbts.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gqptyuszn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gelieylqj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gwuxbrsjl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gljxkvzai.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/grcjwaxol.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gjccakyzg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gdrapjhum.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.vehdjk.com/Article/details/ggirjbnwm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/ghldjgsfd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gqnjlqfmh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.sjlbkw.cn/Article/details/gftwgnovc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gmadwuilf.sHtML


<!-- 参考信息 -->