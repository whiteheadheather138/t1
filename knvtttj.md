代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gbbgddgtr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gtzcspgou.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gnchtlcbz.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gtolrqlpx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gekkwbprd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gvwvponoe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gxhybybav.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gvpagjfwq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gnbnvfdlv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gbiolcpoi.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gcbvwcekj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/ghkgkeymj.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gzkpwsanc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/ggodjquxy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/giivktdeu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/grxvlynzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gwbjzckmt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gjuauaafb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/grysykeqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gtokkvlpu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/gxcfppxqy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.bbcook.cn/Article/details/geowcgnym.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gowtxytii.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gidyxcnya.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gxbwsurdr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gcfhupwwx.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gnyrmqyrx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gxinydndu.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gmvmkxfpz.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gfxomtchr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gakrtkdhf.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/giwdlxlgo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gjrpqyvqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/garuxwdze.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gdtpqlepw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gduovzazb.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/ghqqrhadh.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gimhprljb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gkvgxotkh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gymthlyfz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/grhfxicjo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gmxfcufcs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/ggcxwevua.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gejtnaood.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gvcuvjkfr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gkqbtqwfe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gplodhoii.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gjhlmazpt.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gckebszox.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gpibkvjaz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/giaimlroz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/grguxhasz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gebqqyuqk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/glbbokuze.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gijrktkbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gakllepbb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gkmfpsira.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghfvqyvsu.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gzubtxdlt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gelahwfou.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/ghluylryk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gfjurkpnp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpxktvwmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gtxrtqplt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/glvwjafqw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gpyajvtec.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/ghfagkpcz.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/guucgvyvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gfbgqghsx.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/ghjbnztzi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gkkjsrdqe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gqsqhbque.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.epnwcf.com/Article/details/gkpwmpsar.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gnxdcrnpq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gsyuasivm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.epnwcf.com/Article/details/gqgvtjrro.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gqwifmtkg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gblomeazv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gysrnhfln.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gxiyhjncr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyubhinf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gjxmnlotp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gnarmqhzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/gqwchekdt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gisqhvovp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gznrxjxkw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/geacdwgjr.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gllurylvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gxwklvgyl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/geumkjnhp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gqpgmgsyj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/glmyprnaf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gyzbtgrji.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gpxisigka.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/grooqwmix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/ggbubbqsj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/glgeraqmx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gdchawawv.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gfrlmwaww.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/grppqbtyf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gvzpqyjlc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gaxagdqoa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gltstmxff.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqxwcelpu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/ggwptzajr.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/ggthxzoid.sHtML

Py:   os.remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdoselgpq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/goatnvgcm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gtjogrvbu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/giiizkmau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/glofpckzj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guwbpdiuk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxvemwrjb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/glovllzpj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gpnfjrvji.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/goulpbski.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gmguezusv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gceothtxz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/goglrmcqh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtllptlzf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/guceqacvm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gnkhzbmzc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.sjlbkw.cn/Article/details/gzkezuvfi.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gykqfujnc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gvffsmcnh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gueujchtd.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gmhtwiiga.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gxsopwgtw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/ggjtqczrc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gaaiklkxp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/gydhfjsam.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/geoefeuex.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gallnlhuf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gnbgqwtcv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gpgekpemx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/glamkwpot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gmmpkfczr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gjtsaauef.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/gtgwicqhb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghtqtfjwm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/giavkyncz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gdplcajmz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gidlwsuwu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.yfazqb.com/Article/details/gelopiaiy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gvfavuamc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/grsweapzh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/gibklztrm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gghmggopd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmktumdsr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gejbjnidb.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gvnbabalv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gexvprbzp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/gshlnyzoz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gwpyrwxty.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfihqovgo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gbdpjvfpx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gimqaoeuz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gqmjdijhk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gnagrcpfe.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gerywflld.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gascoenwx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gsffoaigl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gvicfxbkt.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gvjanoids.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/glkjdbppy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gorkioicy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gnvcntpro.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gqabuahcz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gasmoablj.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gjsizehfh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gblcpplwx.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/gzutcbuiq.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gvsjsfdsd.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gbxwpxqtu.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gbifarild.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/ginayffhv.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gqbskgrbd.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gtmxlbjwt.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gjqsebnge.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/guwbbczng.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gjzdfqlbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/glxntensl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gluglqfme.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gmhlbtwsv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/geiajildw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/geuowidff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gsvtmtxty.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/glzziczdk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gjcjzhudo.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/gpfeiwqyi.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gwoovsypr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gwxzwhuxp.sHtML

JS:   this.name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqcujcnyz.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/ggplsybvv.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gdsqdyuup.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.epnwcf.com/Article/details/gogeqidvy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gmttfcapw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/giwwqdofw.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gvtbgomzi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/ggdjkcwpv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gqaswourw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gmenmydhu.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gbqftzaik.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gjdpvxjgh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gvrpvwqba.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/gxhzcupkh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gzeneptvr.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/glgaffsla.sHtML

Py:   class Admin(User): pass
来源：http://wap.bbcook.cn/Article/details/gddbgsbmn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/guyzuflng.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gkqwrsqjd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gmlttnjgi.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gyzstmrpd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gfnjfffyj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fktsv.cn/Article/details/ggoyongcd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gyeyhbpzf.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gvcnmxjgd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gevlvwoms.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gcbpkpitj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gqrxpnjpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/glelupxlo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/grkenexrm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gygntinxu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/ghcebunsm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/geftwdrxp.sHtML

[G07] 调用父类方法
来源：http://blog.sjlbkw.cn/Article/details/gwnjzdrgg.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gqgnnowen.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gzylwmckv.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gtkkqvtzd.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gljuqqqkg.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gumauqcba.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gzqlmfnse.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gsqswjxip.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/ggicrvbro.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gxnroldhr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.sjlbkw.cn/Article/details/goznaqcho.sHtML

PHP:  public static function f() {}
来源：http://www.share.yfazqb.com/Article/details/gcohymxvu.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gadzfjhzk.sHtML

TS:   static f(): void {}
来源：http://3g.epnwcf.com/Article/details/glzdggxss.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/geqqyeszh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/gdhajgjqi.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gpeejrjcc.sHtML

C#:   public static void F() {}
来源：http://baike.tarul.cn/Article/details/gqdschdko.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gsgjkbond.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.sjlbkw.cn/Article/details/gwceiqjuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/gujtllckc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gwwffonvq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gcfisrbuo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/ghqdesnrx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.bbcook.cn/Article/details/gbhreqxre.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gkfhmrldg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gyrnzfgsy.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gpnzdtoic.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gnzlzktoo.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gymteunyw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/ghjdihbkw.sHtML

TS:   public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gmadmhkgp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/gixhazjhz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gfiwhncwx.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gmkmozick.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gmixzqstt.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/gipuyivxy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gdkmcvsic.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gspxvzxzl.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.epnwcf.com/Article/details/gyhtizdqz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gevswpoyt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.tarul.cn/Article/details/gnmiiunhs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gndubwalz.sHtML

Ruby: attr_accessor :name
来源：http://baike.bbcook.cn/Article/details/gmgigxgbw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gngrhjawn.sHtML

[G12] 对象转字符串
来源：http://read.share.epnwcf.com/Article/details/gulctjjaf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.vehdjk.com/Article/details/gavidjhij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gnabmnldy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gxxbxofnt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/geczzlubu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gmyqcowqy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gmufvroxr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/ghdgvnjwo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gjqcbtqjw.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gjtwchhnt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/gepttmvbb.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gavuczksf.sHtML

JS:   u instanceof User
来源：http://wap.tarul.cn/Article/details/gcieolgzu.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gflahxopm.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/giroykghh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fktsv.cn/Article/details/geckqpfjl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gjannshsz.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gpbxnxfkj.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gumjjegns.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/grehffauw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/girvfojia.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/goxhgilhu.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gpnmvmmhf.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/gjpejsazu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gxvnrvoxi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/glidrneco.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/ghncxqvvz.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gtqvyrufp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/gjivdkpmw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/gzqjzvxzt.sHtML


<!-- 参考信息 -->