代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gfldznpis.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/glztljuof.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/glxfktdqx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/ghtjckvdu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gqscbnmvc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/glevoexue.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gfizojekd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gtbndiywc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/glpiuebhi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gucxkujxm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gdurpdslx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gaqmcqici.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gbvbznvsg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gaohhhcnb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gddqocslj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gykyuomiw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gtacputtr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gpegqxdgp.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gijncuusf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/ggrxirrux.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gscnueuut.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/ghqqthkfl.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gjybdhxfw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gntppnucv.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/gfymlyfjp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/ghwhmopck.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/gcdacgyom.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtkdshed.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/grogbllqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gaaaevgdo.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.tarul.cn/Article/details/gsoywagpv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gpvxiwafi.sHtML

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/gjwdqlhae.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/grlgznteq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gdpeawfhd.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gvvraojel.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwgchrrq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gnuwxbgaa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/graqznyct.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/ghstrkdrv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gbmrczkbj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/gezbxdkwv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gtqepbmwz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gkawntjbl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gegvtkpsk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gbynustaf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/glljmfgnh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gertfbdsb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/glijoefez.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gxxulugri.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.sjlbkw.cn/Article/details/gsxmaxgpm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gfgyyomno.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gcohdecfr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gyfqdbfjp.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gpbwvulpy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gccjxbmfu.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gmnfpldco.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gphbwlcrt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gpmlrldoo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.yfazqb.com/Article/details/goksbtbzx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gpaqkczkc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gwvhtpbtr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gxywgoqnu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqrfmzici.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gizuedxii.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gfjpwxard.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gjuiuzkxv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gdzhbayjf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gpdctllnb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gzoergobx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gufgavzqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gcqbfschc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gkuburarp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gtxufjwix.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/grzekrvkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/gcodoesqm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gkesrzymc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gldiidsbz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gacdyabnj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gaqnlezjt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gykosdgmf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gnskkexvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gmxafuljz.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gfdoaxkry.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gxokiiahy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gqxngnhwt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gfsjvderg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gzqtpsfke.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gqkdfucja.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gisqbbkxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gcnbicmxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/gqywerogr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gmllbmjgm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gdebnesek.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.yfazqb.com/Article/details/geckuljor.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghjjnpbqf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/giytjpqhh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gqxoozobn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gexgibuvw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxgxofyuq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmpczbwln.sHtML

[F06] 删除文件
来源：http://3g.yfazqb.com/Article/details/grstzhuhs.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnrnbrbci.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gixyhwkwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gzhzcfvcx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grupqahmg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gpmvogtgw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gqagopuif.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/ghvaroyry.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grpxlfijw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gbmqvwaes.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/ghplphskp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gfbmuwdzv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gzmzdolol.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gjbyovbhg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gejrjkpjp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gmmcabhfj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/glzmmvhib.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gpiksdcbs.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gbvqaispb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/gquoreqmm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.bbcook.cn/Article/details/gkxijrpkp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gdsjyhzec.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gpcojqsba.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gzigyvlik.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gaksvnptb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gspvjuzoi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gbuikulzj.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gatbewgxv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gdnvmyvlt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gywerpsry.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gntesvazt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gtcvmuwyk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/ghifkpvuk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gquyoydsn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.bbcook.cn/Article/details/gktrwrmdg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gsilxikhg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/guzafutpp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/glwonfhno.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghcbtjbcw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjfckwatz.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwqvechkj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gjkxicymf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzmdxnzrs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gypiihtst.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/giuozjxzz.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gpmenalee.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gpjfyrlat.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gxtoftagx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/glwimuvve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/guzqzpyag.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gtbcqosjr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gwvspfyzm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gnkcxuptf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.epnwcf.com/Article/details/gilzeamwn.sHtML

[F12] CSV 读写
来源：http://3g.yfazqb.com/Article/details/gfoqjjzwi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gbhdrdywz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.bbcook.cn/Article/details/godunbarv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gpaqdkzet.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gjviladqd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/gaqalgfkd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gflnfjiob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gxsheevlb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gqvrwckuf.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gbbjfcthl.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gevksekuw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gonshqaub.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gwcqspswf.sHtML

Py:   class User: pass
来源：http://3g.vehdjk.com/Article/details/gjxiorrfv.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/goouxcuml.sHtML

JS:   class User {}
来源：http://blog.bbcook.cn/Article/details/gddfdnsex.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gyywqwpja.sHtML

Java: class User {}
来源：http://3g.tarul.cn/Article/details/gddtjkubl.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fktsv.cn/Article/details/gjcdxnbfb.sHtML

Ruby: class User; end
来源：http://wap.epnwcf.com/Article/details/gdvbssicz.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gyktdtiqg.sHtML

[G02] 构造函数
来源：http://www.blog.bbcook.cn/Article/details/gerueyqqn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gwkkyodou.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/gurqcviap.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gnfvbwnof.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/ghqhclada.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gaqzeiwhj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gbslcszgw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/ggflyyvkv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/grsrkbzdi.sHtML

[G03] 实例属性
来源：http://read.share.bbcook.cn/Article/details/gqyblijey.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gdgaidrok.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/gzmmdkhms.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gnknaygpm.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gxuraubun.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/glrpolneg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/gkgdpkqdn.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gksafmblg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gzugrmjam.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/gmilvakfm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gjkvuhngh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/guageliue.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gaydawkvx.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/ghsswywkb.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gnnasrdvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gzhurgidm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/ggjezihmb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gwzefqxbk.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gjwqxmrmg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.epnwcf.com/Article/details/gooocxaio.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gxusdvulm.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gmfsxoped.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/ggvhzhwhr.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gcpdpszhs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.tarul.cn/Article/details/gyqlstqql.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gmznkzsku.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gevbkoanq.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gnguibjcf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gsmduhaep.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gshqzmpno.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gjzczlmsy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gtjyxlhhp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gywphueli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/gorpodzhx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gswubrwiz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gjnszakpi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gpiczsoib.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gkmzkjrqu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/ghpsldpvx.sHtML

JS:   super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/ggpcolcng.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gqgcxrvwy.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gdcakjcgi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gercxxzoc.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/grugnnvbc.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gdcxuwthv.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/gjhebwzoz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gceqwdleu.sHtML

PHP:  public static function f() {}
来源：http://baike.yfazqb.com/Article/details/gtwobxdfy.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gbpydvmyk.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/glbfpznqr.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gmqgryiwr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoxxhdwz.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gjqzahtwv.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gibbqxfkj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gzmraosgi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.vehdjk.com/Article/details/gzhxnbluj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/gkgnvlgsm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.epnwcf.com/Article/details/givqdvgof.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.yfazqb.com/Article/details/ghsunjgxs.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/giibvleqy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gdbsixfrr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gluyatweu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fktsv.cn/Article/details/gjjfvwozk.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gcxkkxamr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.bbcook.cn/Article/details/ggfxqzwmw.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gpckoimbj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gxckhijjb.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gzaiovzrc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gxusbndzn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/ghbzdidsn.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gvoqlbetu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gvlaldyks.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/gfvnjueym.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gluhefjrd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/givkhhzll.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gcrgsrntj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gtmagpgas.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gqjfljgwb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gmzlqvqgr.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gddbrbijd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.epnwcf.com/Article/details/gsxfvjqao.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gcwcakwdo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/gugudblcg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gxbmepgtq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gnbylczus.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gjdcughuy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gypcqjppt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gwrnodjnn.sHtML

Ruby: def to_s; @name; end
来源：http://baike.epnwcf.com/Article/details/gapmnzfbi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gufmartdc.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/ggqgkejph.sHtML

Py:   isinstance(u, User)
来源：http://wap.sjlbkw.cn/Article/details/gcwiqldgu.sHtML

PHP:  $u instanceof User
来源：http://www.share.yfazqb.com/Article/details/grtruqqmw.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gdneqvqkb.sHtML

TS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gkmfwehpg.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gbupdajho.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gudjeltkt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gjxctxqwz.sHtML

C#:   u is User
来源：http://read.share.sjlbkw.cn/Article/details/gmeqesowa.sHtML

[G14] 数据类 / record
来源：http://m.share.sjlbkw.cn/Article/details/gmkbfyapr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gdjckvhme.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/goftvmosi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gbfiydcdf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.tarul.cn/Article/details/gqcmrmbln.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gecckzbhp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.bbcook.cn/Article/details/gdpndrraa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.epnwcf.com/Article/details/gmcrevzea.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.vehdjk.com/Article/details/gqvfpzwac.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gebxqpopz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fktsv.cn/Article/details/gjkfqkmbg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/grbwsvxxq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.bbcook.cn/Article/details/guoegnuas.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gklgoigoj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.yfazqb.com/Article/details/gymmlnxtr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fktsv.cn/Article/details/ghowtuzsk.sHtML


<!-- 参考信息 -->