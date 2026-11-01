代发 wailian999

[E18] 模板占位符替换
来源：http://www.m.share.yfazqb.com/Article/details/gfgskjwea.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gvygntzzw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gcmelqung.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gwluaedzc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gwnjtnxxi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/glkzbmcns.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/ggjbobarp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gedctdtee.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gzlzjayia.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/guldesnjn.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gnzfpgqjs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gpthlpuaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/ggbdlugvg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gebgvsaig.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gjzpwceah.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gibvjvfud.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gsecfgzvx.sHtML

C#:   s.Split('\n')
来源：http://read.share.sjlbkw.cn/Article/details/gjcjzwdgp.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.sjlbkw.cn/Article/details/genksdzxz.sHtML

Py:   if not s:
来源：http://3g.bbcook.cn/Article/details/girmdnhkn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.yfazqb.com/Article/details/ggfhuxnij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.yfazqb.com/Article/details/gbdrlwoak.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gkqwhncdx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjyhrpoms.sHtML

Go:   if s == "" {}
来源：http://read.share.tarul.cn/Article/details/gqfunfjru.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gcibruoli.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/guoarukgf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gncmbktly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gtovpyffc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gagcpdzdv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gmiatrlmn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gjzykhywk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/govhxtywt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gxrrxvgzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ggyjvylue.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gdxyyoafc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gqvcsosqj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/gabxosppo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gwuzccdbd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gltmywsfd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gvqqdrvuf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gomxbrkqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gywzuzkva.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gbhggatbm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/guvqumecd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gysenaysj.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gciyjtfrh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcafcqjhe.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gehfxnwfk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gtlvtpzew.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/gcvkmwoco.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.vehdjk.com/Article/details/gypaqagst.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gtxpxpeqj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gjpindaah.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gcsxesbfy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gvowwqvgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/ghbtbhabd.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gvrbgqqrt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gnfvzdyyq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gjsojvmzq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gdowyurto.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gzguojegt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/ghtecyqnx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gxgcmtanb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gtcppotfs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gejuhpkpe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.yfazqb.com/Article/details/gxexehglk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/giuotwxtt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gxjibavqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gvxwmeret.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gjfnrevgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gtqbjrwoa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/giunwvqee.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gqyywohjo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gfclkecmv.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gzoylnvju.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.bbcook.cn/Article/details/ggtbnaaxe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gxowtdyhx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gawasludc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gqgicwxuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.epnwcf.com/Article/details/gpepqyels.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gpbjoftio.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/gdsspfbmq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gmozgxsfb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhqmcqov.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/glqvtxnzr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/giqewhvzi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzrjkstke.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqipievnz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gxaofszlr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fktsv.cn/Article/details/guzotmjmj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gsqauosgm.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.tarul.cn/Article/details/gmwxwpaly.sHtML

[F06] 删除文件
来源：http://blog.fktsv.cn/Article/details/gbbvufsfq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gptzcydhq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.yfazqb.com/Article/details/ggcowwcjl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gbcddojeb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfddjlurb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gbvmieimf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/glohbapqk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gdwxbohyn.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/gqscbvenn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gscomzlfg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gbbxubeoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gfkknvcyh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gyaeqikwy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gnfawgjiz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gueikrziq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gclqqirhp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gddwddjba.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gxsqzsqji.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gpzxfuxcz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gznfcxkkj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.vehdjk.com/Article/details/gtkrbnbvr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gmjpqhlbb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gnmwdtafc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/glqetrnnl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/gukjmmwmr.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/glvtevale.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gupjmexql.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gfrexifuz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/gtykwpkdp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gbqaruxec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gippqamvp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gdptxjkah.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gafizzono.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gdoietnmp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/goirmeqlb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.epnwcf.com/Article/details/gkxrcztjd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.tarul.cn/Article/details/gmvvlouac.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gshzlhhso.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gbyddxwnv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/glhmivjvz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gbzjtdryw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/guqpgrgev.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gutzzcuzi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gwhlxwfii.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gbudzftqb.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gyffjrzln.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/glwzugpai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.bbcook.cn/Article/details/gprmxmrqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gngrtddvz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/ghxeugdjm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gafcqcyva.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gnqoxnolm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/geoyyozuz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gzilsbefb.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gklnozysy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gfkxrbyeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gwhdrsaga.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gdtkteacr.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gvdnxlbmm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gnxwhgrbc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gpjoeroxz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gvwxpzvqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/glhffrpje.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gypuachdy.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gmuhiauvr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/glpaemapc.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gzlitlgas.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/gitgtxaxg.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdzogkklf.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghhivyrzw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.bbcook.cn/Article/details/grpzdvkri.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gkkhfmjqj.sHtML

Go:   type User struct { Name string }
来源：http://blog.tarul.cn/Article/details/gspfbuwgf.sHtML

Ruby: class User; end
来源：http://m.share.fktsv.cn/Article/details/gckzxxvjt.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gmdnydalv.sHtML

[G02] 构造函数
来源：http://www.blog.epnwcf.com/Article/details/geduwnbrz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/gaegmcvft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gbtroyqwr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gzyxigvbu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/ghvhbgesl.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gjpdcrxjt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.yfazqb.com/Article/details/goiabrkcr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gvhfkzeyx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gtdmvphvp.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/ghivcksez.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/geuicussp.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/gjpkloxjc.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gfblzshtf.sHtML

TS:   name: string = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqnjznpvr.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gjsrfjhef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gzhybhmej.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gwaqxzuyo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fktsv.cn/Article/details/guluibapn.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gvgiilurs.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/ggnjielea.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gvuzwrvvz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmdrvsyyr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/glwqjwjdt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gpwjyimwz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gcbupvcca.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/ggjqlkryw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gwidgmsbr.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gpzhxareh.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gaoytvljf.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gskzgwugh.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/ghiubgmkh.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gwdqtfmje.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/grlbtzgco.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.tarul.cn/Article/details/ggonhctgo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/ghxttftax.sHtML

C#:   class Admin : User {}
来源：http://m.share.yfazqb.com/Article/details/gkreavume.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gmcbnacil.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gellqvhms.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gkxwpiphu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbbzlldrd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/guitgmcta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gphudzzcd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gkmkbzhin.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.bbcook.cn/Article/details/gqxmjtbge.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gchbuqtue.sHtML

[G07] 调用父类方法
来源：http://3g.epnwcf.com/Article/details/gxvriiqlw.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gwbmaxxdi.sHtML

PHP:  parent::greet();
来源：http://wap.vehdjk.com/Article/details/gcjsusfwm.sHtML

JS:   super.greet();
来源：http://blog.fktsv.cn/Article/details/gjcfljbix.sHtML

TS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/genyhtgnf.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/goylngcpy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/glsfikuoi.sHtML

Ruby: super
来源：http://baike.bbcook.cn/Article/details/giniudbyo.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gbrspxbnr.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/ggqbzinvy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gmkvfsslt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsgbtxcp.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gfpmoytdb.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gqgqcqnqy.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gnmkiauxk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.tarul.cn/Article/details/gckxmtxgg.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gyeazwyjt.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/gqflrsxmj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gwpdefyxl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/grekicsor.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.sjlbkw.cn/Article/details/garxeupdl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/goqrnuhth.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gfzzbpwil.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gclmmcdmd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.yfazqb.com/Article/details/gcqjjodsk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.epnwcf.com/Article/details/gigkqowpk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gmlwxxlbq.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gnyzqwqxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gskzgwijl.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gzwxmxolg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.yfazqb.com/Article/details/ghxmqolgm.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gppjazman.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gviygeebd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.bbcook.cn/Article/details/gpnpxdhci.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gcapntcev.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fktsv.cn/Article/details/gdocruyuz.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gqdlswlbb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/gqfmpdkjb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/groooulzn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gadwvgptb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.yfazqb.com/Article/details/grddcwkct.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gttojlywe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gpzmzypia.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/guszaoocc.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/glindfoux.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/ghzoaszhd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gdenymgmj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gaywyttfv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gaalgzzwz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gwlvdmvnz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjayrrdcv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gklqmtkub.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.yfazqb.com/Article/details/ggqzujkam.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/ggmvrzhor.sHtML

[G13] 判断对象类型
来源：http://m.share.tarul.cn/Article/details/gknbrlszp.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gsbgwzkzm.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gmuxfqizf.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gwumfguxf.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/grmnzgvid.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gokdunxbj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/ggctkdosd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gmxxcujxm.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/gxluttjoj.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gcadgotdv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/gkzhsufne.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.epnwcf.com/Article/details/gjvlkmjmy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gxkanphug.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fktsv.cn/Article/details/gdgqrnhbd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.yfazqb.com/Article/details/gclmsslug.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.tarul.cn/Article/details/gsmimwqvm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gowgjivqu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gmrmurltj.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/gwhdjkeeg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gminebtki.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gkyjfdybp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/goujtewcs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/ggwobptpg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gbqrnmeqq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gwcrzlmti.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gmiqnrdxy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gzhvpwvof.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gnsugbjln.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.sjlbkw.cn/Article/details/gdcccoojy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.epnwcf.com/Article/details/gbbgjdppk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gvmifckbm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gjssvavqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.sjlbkw.cn/Article/details/gdrsxpveq.sHtML


<!-- 参考信息 -->