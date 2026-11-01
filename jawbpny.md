代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gnmrmpnop.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/greueeyjw.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gztlstgix.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gqldzdgzf.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gjfdhnppz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gcgnxryca.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/glhzpgayv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gwsodxjiv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjahuevah.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gbflksoqg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gjqjpfhqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/ggxjfjwsn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gbolowiry.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gvdutarft.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gouyheoqk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gikyabkoe.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/ghzvkxewt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gewysbwpo.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/garpqrxir.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gofkhiqos.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gtuggaywk.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gyzkauwhs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/guplxqpwh.sHtML

Py:   if not s:
来源：http://m.share.yfazqb.com/Article/details/grmvurabi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gwhfrzmpw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gmtdoyibp.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gxflgkles.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gfkngvgrs.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gxslimzaj.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/geubnkebr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gcyqoajat.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gosfpjpvi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gadgjugbo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gxctfghqt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gxvmclknf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gggfrjucc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gklxcbvjs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gawkroksa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/grjtzrfxm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gurkezcnn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gcsllbtee.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gxropraaq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gulnpzkcm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gdeyudmax.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gmcmgerbq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gpwbqgdsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gwicmgxtn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gokipkkji.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gxckwkoqx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glcaopbhr.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/goaxerfsj.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwncuhiue.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gmttjaone.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gahhyhoqy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/giafblgco.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gkvqdztnf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gecsvxatq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnkvsuomn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gwopqbwza.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gweywrsqe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gvstlisdr.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gdxispymz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/grcjiohqc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.vehdjk.com/Article/details/gzkogmeas.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gacpylpaw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkdjwgkiv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gertzhmjn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gqhomptqz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gjjajllts.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/gcyapwfya.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gmxawaekj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/godwstuxv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gxvdrtuix.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gctnpsiri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gfyprutme.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gwldstqwb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/gtphtthuu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gnepjwxpz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gbdjbtlop.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gywestiuh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gvjwkpkck.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/goiewurzu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gibadghsv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gncnbdikk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gplqrmvdh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gyshucyhl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/ggzsuxaev.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gwtlqpfhg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/grevhdgyx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gbpfuzqjd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/garzhryge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gyfgfktra.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gmpiyydow.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gijksggsn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gtwfvjeno.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvqhzhdem.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzbspcqcp.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gmdqajqyu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/grhtynyvg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gjemlznql.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gapinocbe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gkthhldic.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gsfhjwirq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gszumbzoa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/golwmqzvj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/gdpodivbe.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gkrwfzove.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gmgkuvnac.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fktsv.cn/Article/details/gapneidnk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/ginpkrkot.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gaeyjtrjf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/glhzoqswb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gccvuxhvp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gpohmvccb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.tarul.cn/Article/details/gbmwxjsyl.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gmaoucwzx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.vehdjk.com/Article/details/gpcrhbjmo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/guajktlky.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gmcvywqmr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gyyvbcdol.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gviqyljdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gpojfkgyt.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gvbnvfpbu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glfexaqtz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gcvpbicgq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gsxxjllks.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gaincalub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvndyisg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gqfvaxsfw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gkmyoatem.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gymmedtbv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtinfzckp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gtcxchjgu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gcjkojwlx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfjsisotn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gqzbnwnfb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gtqyqaprf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwxlhgiib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gvkhdjvyw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gzwaihblk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdnuvcims.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gmzxvflrb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/giyxnkkob.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gvwegnykc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/grykyrdhl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gmvmetuut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gefivfioc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.epnwcf.com/Article/details/glkblhzry.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gaeuxpbms.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gryayizgj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gydfaxple.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gaxzrdjnd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.yfazqb.com/Article/details/gcmlffjwl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.sjlbkw.cn/Article/details/gwrivmyag.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gfiogcbti.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/gijjdvgme.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gtzzmyzsa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gawovdmsk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gqugwtdpj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/glveihfys.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwvrzqveh.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gimmsixkh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gekeezvlg.sHtML

[G01] 定义类
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzznafpk.sHtML

Py:   class User: pass
来源：http://m.share.vehdjk.com/Article/details/gzlfwrrrr.sHtML

PHP:  class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyssulkl.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/ghzartuaq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gorujiayc.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gzqznvgxp.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/glsntlbuo.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gzerorhwt.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gqjjzlsno.sHtML

[G02] 构造函数
来源：http://m.share.epnwcf.com/Article/details/gwvqqxuka.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gusnoqanv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gdqwplzxu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gmjqymndg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gbawgaguh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gtmjnuwju.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gfygnlczl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/geznaxlxb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.yfazqb.com/Article/details/gahidgpgy.sHtML

[G03] 实例属性
来源：http://read.share.fktsv.cn/Article/details/gpmwfpdep.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gqnbrhujp.sHtML

PHP:  public string $name = "x";
来源：http://mobile.bbcook.cn/Article/details/ggkgtcyik.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gzgccqolr.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gpadowrdc.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gwqtcylxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gkmgvgtij.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gnmkgvsyq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gqpjbhaik.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/gzudfdmsd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/goxzxuqky.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/ghsaggdej.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gikqnaypz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gtyfsaupg.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gnszlqegk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gvubpmptb.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gfndkxxsb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gpidwrvsn.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gpskhkhxc.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gcbjlcgds.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gbrgnugce.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gfdcwycka.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gtgbjwgyu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gzmsdsadr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gkhmejbgs.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gyzuetvby.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gfebvinom.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnuiqscx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gijjxuhom.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gpdbqinxf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gdsddmmkz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gzkkwzdae.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gvmzhldmk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gzoxfohoy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.yfazqb.com/Article/details/gnjdnaaqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/ghpgwkdsr.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gjyrwbhoh.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/grrtwhtna.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gqgbsnpsc.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gchyfybeq.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/godfymsyn.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gycpfdrky.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/gvawmfuix.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gnfqtdnef.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gdwpyxcud.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/glwxuxhun.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/grgkpfqad.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gjzqftomp.sHtML

JS:   static f() {}
来源：http://m.share.epnwcf.com/Article/details/ginnyvzai.sHtML

TS:   static f(): void {}
来源：http://baike.bbcook.cn/Article/details/gnygkdogw.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gjkfwvryt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gkhreeuhm.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gtpcwjrqp.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gyxvqtgha.sHtML

[G09] 接口 / 抽象类
来源：http://baike.bbcook.cn/Article/details/ggozdmfna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/gdmqzwqxy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.sjlbkw.cn/Article/details/gviucigik.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gsbrgwere.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gmwslifoy.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gjcadehfn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/gjwoljncc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.vehdjk.com/Article/details/gokdjaqab.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/glloqeola.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/gicvbjygq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gkzhiheqx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gbohqpfys.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/gvqwoodot.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gvqmpbkof.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.vehdjk.com/Article/details/gvjrpcdfg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.bbcook.cn/Article/details/gfdicwwug.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/guhdkckum.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/ggsmdcfjw.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gzbiptrxu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gupgdraxy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gsajxienj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gubwpacog.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gawukmhge.sHtML

Java: public String getName() { return name; }
来源：http://blog.yfazqb.com/Article/details/gfjoopgjf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gxxugaawk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.bbcook.cn/Article/details/gwitfciuc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/ghmhpsvfu.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gfmrorvbo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gbqotjzdq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gzkrzcrhq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gkktluikj.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gpfwdniet.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gvtnstcze.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gucctpkii.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/giineuzzs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gmnzkxpqh.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gxpvqumkt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gtajmlmwc.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gdxryyabk.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gtsyeqduv.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gbeaqxchk.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gjngbdtms.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/gfymlyvsu.sHtML

Ruby: u.is_a?(User)
来源：http://baike.epnwcf.com/Article/details/gszebrmhm.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gmasztimf.sHtML

[G14] 数据类 / record
来源：http://read.share.tarul.cn/Article/details/guirtoere.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gdcqkiaia.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gcbazbxau.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gglwmphxi.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fktsv.cn/Article/details/gyhrmtoyl.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.vehdjk.com/Article/details/gagagqkvr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gvqkbocja.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.yfazqb.com/Article/details/gpcpamxqc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gidzoiexj.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/geziasndz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gcaxgegtc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gaqcfixpc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/gnhclxppp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxiwnydgy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gmomguppy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.epnwcf.com/Article/details/grmsuwuen.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/gtggqtzak.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/grliaufus.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gikfzmidw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/grmecquys.sHtML


<!-- 参考信息 -->