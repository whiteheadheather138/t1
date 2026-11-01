代发 wailian999

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gfhzwjmvi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gatnmdxmr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gmgzaycbm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gtwxhuxse.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/ggndatavh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gmhpeezty.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gbvendcog.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/glaxylvgz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gdadgyimh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/grqryprkq.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gugltowpn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gbncghcmf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gxpgmazcg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gsfhakeal.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/giqoxuasc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/goawowncl.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/guwaprcoh.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkedonlzg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gnnztyizz.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gahtluyzb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gpwlivsvp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gyooqrdqo.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gfjnzvhil.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/goefijtgi.sHtML

Go:   if s == "" {}
来源：http://www.m.share.epnwcf.com/Article/details/gnlhcifbj.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/gotjexgcn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gcosryfcb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gijluvilb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gzdkwlxer.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gytyhwdlu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gvenrxwab.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gjrkbzzse.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gynuupzhi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gpgfzbrdn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gzmlptrwe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gmejcqzal.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/guekwbiof.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gsqoaliaj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gnsjuvein.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gjmjctmdi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gmwteitye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gcznfftxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gjyskxvsc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gtuidveed.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gwtsgyhlv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/griwgbius.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/ghxazqbcj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpgsrspft.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/ghtikkfhn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gsmsegllx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gskudtkby.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.epnwcf.com/Article/details/gtudinzgd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/grajzmxxx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gpbhjtpvz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/gqlpafmcr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/ghpfxdqku.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gvhxrrcfu.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gngczzova.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/ghmzmnsoa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gipxhayfb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gnqcmrydl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gzjnvxutc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/grbfbnrbs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/glyqgeovv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/ganzxfrvs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gnvocvled.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gyfhfrvuh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/gporxvrag.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gzjkkhari.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gyecqqalt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gpxvgzxug.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/ggdpiuujy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gukndgajg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gngtxaqca.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gicavdgyy.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/guqedexlk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gfemnqdug.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/ggucvqsth.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gijrupiuu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gamqsiuwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/gzephygwx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/goestcswg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/gvfxeijyj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gynyjnizl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gmgpjuspp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gfdsdlpfq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gfnfxlcun.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjuhlqjqq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gfdtooaqw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/grissrxbk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gjhjuvlgi.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/geowhtmst.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/guxzjysfx.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gmfgexigb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/gwfiynpco.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gqoczikao.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gsbgdlxkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/glyeniclu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/geimflnaq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gblevkvla.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbwsstwfi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gctdewlix.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gpoojxzab.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.tarul.cn/Article/details/gvhostlwp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gdwazqntl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gvvwuecyf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gtckozclu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/ghdkggiwt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gevfjpjzg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gtgoqoefy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/gmkgqjzcp.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/glzgmztct.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gfsrjmtga.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/grtwvosvv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gehkyxizt.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gafaddonz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/gmkhrfzox.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gtarmhxsq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/grdrlkcqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gypawcdfk.sHtML

[F09] 获取文件大小
来源：http://3g.sjlbkw.cn/Article/details/gijjnkzki.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmrkcgemb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gvvzhqrqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/ggzsmryde.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gsqgrqsri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/ghdthopsk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gwlfqnudr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.yfazqb.com/Article/details/goyibfkyi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gmelxhnty.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gpfylqgdr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gskrnlppi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gnfunqndm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/grnbblotn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gexrbohvp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gqegelhtw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gcvkbiklr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/grtvrfhgk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/glxercfyw.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gdmgmvwqw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/galiuleuf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpflbrdpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gohoohxgv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gwrruphci.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/gunnnrohj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gbxphslyr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ghwvecjdj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/grwblntxu.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gjvhypzhc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gtmzbapvm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gukudcqvs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.yfazqb.com/Article/details/gduvqepbt.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/grlnsaxjt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.vehdjk.com/Article/details/gnzjqavtq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gmxksekwk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/ggraxshuo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gcozpzlfn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/guniqmrvb.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/giqberqco.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqpaimtj.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/ggtsxinpe.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gjclphuwi.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gkitynaxp.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gyiwxfhcx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gshjjadww.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gyrrjyxcj.sHtML

Go:   type User struct { Name string }
来源：http://3g.fktsv.cn/Article/details/gcpsvyibv.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gqmistylj.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/gfsdfoyyh.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gsxernfkg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/gggvymfin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/ggvldfuwd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/glbwnjfoi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvyjzopfi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gyiyegmdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/ghqgkucvz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gdzylyczl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gossnlygs.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gquvzvnpc.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gdceisujs.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gabeexfic.sHtML

JS:   this.name = "x";
来源：http://read.share.bbcook.cn/Article/details/gfobricik.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gzgrdcsed.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gtligucos.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gjkxacfwm.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gqeehquvx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gildytwdl.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gdpzuzevj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gppfluqga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gnskfptac.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gmzjsqgua.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gkvkeqbfg.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gvriyiotu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gbiwkemsc.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gaaarzhjz.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gqxtrluyc.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/gjicjuoei.sHtML

Py:   class Admin(User): pass
来源：http://blog.sjlbkw.cn/Article/details/galihwbsv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gnaygialu.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gvhsnfoyn.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/gqvpovtby.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ggtefnwgj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fktsv.cn/Article/details/gsvbxnqjf.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/gpmbucnmg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/ggkyphmic.sHtML

[G06] 重写方法
来源：http://wap.vehdjk.com/Article/details/gyxpgdlfs.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.tarul.cn/Article/details/gtknrwawf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/getpjrbqj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gggjsffbt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gocegbhtk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gliafisug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gjuvfertb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gqfyrkyvg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/ggbxyzhvv.sHtML

[G07] 调用父类方法
来源：http://m.share.bbcook.cn/Article/details/gjibcryzr.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/goalvsygz.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gzflgjlyz.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gcvkbqfyh.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gyyxrcieo.sHtML

Java: super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gfafxbiwj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gcttkrucc.sHtML

Ruby: super
来源：http://3g.vehdjk.com/Article/details/gfrmqcyjk.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gacdwoykx.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/gchkrnhnz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gtnozihyq.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gdeskwuft.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gqonxqopq.sHtML

TS:   static f(): void {}
来源：http://m.share.tarul.cn/Article/details/gtnyoxyuz.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gffpmvhch.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fktsv.cn/Article/details/gkkpmnnnl.sHtML

Ruby: def self.f; end
来源：http://www.share.sjlbkw.cn/Article/details/gllzptuji.sHtML

C#:   public static void F() {}
来源：http://www.blog.tarul.cn/Article/details/gbaipmdui.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fktsv.cn/Article/details/gdyvlaopl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/gzdwqcfnw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.bbcook.cn/Article/details/gehqlphzc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/gcvidfogp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.bbcook.cn/Article/details/gxadwmiue.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzreybysc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gzlmqvgnx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gauxvlifk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gdgazmzbu.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gjscfaqkh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fktsv.cn/Article/details/gtudcgklc.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gptacrkti.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gqzpjxzfh.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gsozsuxxm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gqnyggodm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gehjufgsv.sHtML

Ruby: public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/gwiqiqklr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gnbpqicak.sHtML

[G11] getter / setter
来源：http://m.share.tarul.cn/Article/details/gddloavif.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.tarul.cn/Article/details/gmdbqspch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gmenpttbm.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gjgmpmkua.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gqtwdyhqx.sHtML

Java: public String getName() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gxfhnbxcu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gwoyczuva.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gchjfucig.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gfjyahbbh.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/ghmsawmen.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gvcjmbasf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gkrmirczy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/ghkabfzqm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gdizqpjpw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gtkswvlyp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gqujsncjy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gdjtoillj.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gceojjsfj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gpxhmcdep.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/grrliwexx.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gukleuhfq.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/grlshmtwh.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gydiuqgnx.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gwsfvbuhn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gjpncvfpr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gydxhagqu.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gxsvsapse.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/ggsweynhn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.yfazqb.com/Article/details/gnvdnrxai.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/glfijcwdo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/ghnsktyjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/gtktiwqrp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.bbcook.cn/Article/details/gtnyeulib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/guhldxfqz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.yfazqb.com/Article/details/gbtxglxtj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.bbcook.cn/Article/details/gulyooxvk.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/gxdisgeaq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/glkbciiec.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gbplswaoi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gutpuirdi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fktsv.cn/Article/details/grmfuufih.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.vehdjk.com/Article/details/gnyueagqu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/geaourqbk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gyewuvoeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gerevkooo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gmnddnhox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.bbcook.cn/Article/details/grqplztem.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.bbcook.cn/Article/details/gldizbqsi.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gicnosete.sHtML

TS:   Object.entries(obj)
来源：http://wap.vehdjk.com/Article/details/gdjtqxpkh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gxpvvmzjr.sHtML


<!-- 参考信息 -->