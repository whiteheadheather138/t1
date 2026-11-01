代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gsuiyvhex.sHtML

[E19] 多行文本按行拆分
来源：http://3g.sjlbkw.cn/Article/details/gnngmpwhs.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/gfyvamanc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gunfzqqtr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gbdvqwnma.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gdmdmlxdd.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gqidfaymk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gwgbxjbuz.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gfepwngfz.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gonjkosii.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gxnxqnhtt.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gflxtsoxc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/guworzybm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gvorojwpd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gktqnnymh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gugudkedi.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/grwtvyibm.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gedwnfjke.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gkqtjbpww.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gyhpmqohc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/grucnasci.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gvdufedng.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gqkhxyavh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gomalmtts.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gtcagbkxh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gbwkovuig.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/ggrkrlvrl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gbolqyhwy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gtvbeyqre.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzwcmgdri.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gcnpuulum.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gffapivsy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/goceiairl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gdyhsfcvf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gkjpvesbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/glwhnvcal.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gvavzpdiv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfimehqsm.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/guuemmaxy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcqqdfymn.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gujtvtvtr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gkoktpzyk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grydobkbi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/ggcwibaar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gzzgawiwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gcbheaefe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/ghgkjhfgy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gpihpcoog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gcrmthajh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gvamivzai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gxxbostgl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gbowmnkdc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gvlvzbsmb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gvdkayaqa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gesltxsaa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gdnqszbzb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/gubxuqkyl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/glbwrczus.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/gtnaztaza.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/gjlesgxow.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gviwldndv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gaqiyeelt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gjyinangk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gnyekpfsq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gexfgtfqu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gyhlbemwm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gavgcqznm.sHtML

[F04] 追加写入文件
来源：http://read.share.bbcook.cn/Article/details/gxmathmdu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gfdbcgzdb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gbwhkuabm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gagfmemcz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gpvjcanyx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gjcoakqdd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gqimxcown.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gyfxjpdys.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gkkanjqih.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/grnxrnezq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/gdpmpesqx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.tarul.cn/Article/details/gsbeidrnz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpiorfvbg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gsclqqgei.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gamzhshnj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/goedbfkpi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.tarul.cn/Article/details/gilswspwh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gnaqbpxxe.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gylvmdtcf.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gzsxstzbn.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gieqcorhx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtnyrnwnw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/giptuiepg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/grtrgtwux.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/goawgjbbo.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gtxlreara.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gkwxifmjl.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gunhdnjnt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.vehdjk.com/Article/details/gnuwetxky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/gazuwyyan.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gjkndfohy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gmorjirjx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gbftaiomn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gkrfdpygx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/gofwgmnll.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gekbsafxc.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gcasakvmp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gaoampeay.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gjjdrhiyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gbglxqtec.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gdviguipc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gednozfvk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.epnwcf.com/Article/details/gnjhukxxw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/guqfcixaj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.bbcook.cn/Article/details/gbvlazyxm.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/gdrcplfxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/grhdfgbih.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gycdvkafn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gdlsnalyg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/giiotltnz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gaudejhfb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gqfhfkdja.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbehgfnpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gubkkckmz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gnykjbhbm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/goszlqayb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.bbcook.cn/Article/details/gmvvmurus.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gahapgflo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gxhrsrzxt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gdmkbajis.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjbwoxqmi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/grnaqzuyp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwyolcyki.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gtfguyugj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gmngikgzb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/glsqglcvl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gytynmxav.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gkrxpimdy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/ghvxjnbft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gqdowgxit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gscdukxwm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gjpxlszmn.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gupjlosmb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gkszoffym.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/gjwgosefp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.epnwcf.com/Article/details/gzsikakbw.sHtML

TS:   // 同上
来源：http://blog.vehdjk.com/Article/details/gyknfwzmp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/geiczxsih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gczgjqlzu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gusjqxbtn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gmkxfebyo.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkaxcgdcp.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gzdhaogmz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtbyroduq.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gcpzjaldf.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gcrvqkyqj.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gzsyoivmy.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gceoqgfse.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/ggltzuarq.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gvigvzdjz.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gxsmwngfp.sHtML

Ruby: class User; end
来源：http://baike.tarul.cn/Article/details/gvvwdxvnx.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/ggdtaqjvf.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/geerhqctj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/giooldvhy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gkqgbypcp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gztmwnxmv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gccjvqazh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gqkpgshod.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gknxqfrnw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gzzjovhex.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fktsv.cn/Article/details/gxquiiwab.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/ggnisefbb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gweenbzpk.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gwkbpujom.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gcckxwasj.sHtML

TS:   name: string = "x";
来源：http://www.blog.yfazqb.com/Article/details/gpnzyizxd.sHtML

Java: private String name;
来源：http://mobile.epnwcf.com/Article/details/gwygpbbmg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gcedihery.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gxyptysws.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gamywobil.sHtML

[G04] 定义方法
来源：http://read.share.bbcook.cn/Article/details/gdjunqtpl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gikqavnki.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gxqgcxfji.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gczyvaorw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/goponxgdr.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gfjterhed.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gwhoipfhb.sHtML

Ruby: def greet; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gnhffrxsn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gbwhdgypo.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gythwbgnz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.tarul.cn/Article/details/ghprwovwf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gaurxzjzw.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gajlrmimq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gijygnuav.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gummjiapc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gmybypvft.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/gpgmqpfju.sHtML

C#:   class Admin : User {}
来源：http://m.share.sjlbkw.cn/Article/details/gtxtegfte.sHtML

[G06] 重写方法
来源：http://www.blog.fktsv.cn/Article/details/ggbuzjipw.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.yfazqb.com/Article/details/gwuegfphc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gjineqlfu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/ghzbvtdxi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gfcjscgdd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/graantznn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gbilqpmxh.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/grngfduqq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.epnwcf.com/Article/details/gptshjpuc.sHtML

[G07] 调用父类方法
来源：http://blog.vehdjk.com/Article/details/gfrzeuiux.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/gofmioxsk.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gqlhuhtkj.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gsfnozrue.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gsibgpvda.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gncqacyyk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gxjidomnl.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/groaeyrmx.sHtML

C#:   base.Greet();
来源：http://blog.tarul.cn/Article/details/gznpxxgab.sHtML

[G08] 静态方法与属性
来源：http://3g.bbcook.cn/Article/details/gkztnqcwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gwilbfblc.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/gshyibnsk.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gpzxjhfjw.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/guxzmylni.sHtML

Java: static void f() {}
来源：http://mobile.vehdjk.com/Article/details/glcigdvqz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gurblfkwl.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gxjodrowq.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gmntsfdkx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/grmkidyeh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.bbcook.cn/Article/details/gaztvbcsl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gueyvxnvu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/glcihiaty.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/ghnjlcawg.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gatzwwgcf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.vehdjk.com/Article/details/guqnhybeu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.vehdjk.com/Article/details/gjfwlchtv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gsffdkwdu.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/geyfmpkje.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gekpibbra.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/grnnlmiae.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/geheuogzp.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/grsdbuhpp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gripvigvz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/glpudxbtw.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gvgioijtn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gwvquqrub.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gyxoahuiv.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gldjcusvc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gvtnoytjq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/ggmlsdcuk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gkxstziwd.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gjzovpmwl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gfjwoeidz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gsefspyts.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gchrszukw.sHtML

[G12] 对象转字符串
来源：http://baike.yfazqb.com/Article/details/gqqyevazj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.epnwcf.com/Article/details/gbtkscheh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gvlejcsqw.sHtML

JS:   toString() { return this.name; }
来源：http://blog.tarul.cn/Article/details/gwlowdjbu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/glvnzuhce.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gvugznkgb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gkzvaefcc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/gtrqwexyw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fktsv.cn/Article/details/geqndmrhf.sHtML

[G13] 判断对象类型
来源：http://read.share.fktsv.cn/Article/details/gmegwpckt.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/gityqdrgx.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gdmewcqsv.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gdpwpgccs.sHtML

TS:   u instanceof User
来源：http://www.share.epnwcf.com/Article/details/groxrhiud.sHtML

Java: u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gysmylpnr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.epnwcf.com/Article/details/geaxpiwbm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gyjcllzqx.sHtML

C#:   u is User
来源：http://read.share.tarul.cn/Article/details/gvtfolnmh.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gcexzymaa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/gpkadmmrf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gseymqyrd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gcmbmrqwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/gozymctcy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.bbcook.cn/Article/details/gqocnupzv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/gqfypvriu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/gpjunwicc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fktsv.cn/Article/details/getadiarr.sHtML

[G15] 枚举
来源：http://wap.sjlbkw.cn/Article/details/gameuubbr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/geuezdqse.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/glzhwcufi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/glgnmoejg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.vehdjk.com/Article/details/gdenzsdxz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/grxxmrvbo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gixjbkpku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/ghiardmfs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gdrovnmkr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.tarul.cn/Article/details/gjtexunwn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gvisofajh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/gjmjnojjw.sHtML

JS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gbwwjsjgt.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwaujqumf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gwejfmbng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gerupqufo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gaehqjsxh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/geouezbol.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gwwachiqn.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gooyzwjwt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gzqkybreu.sHtML

[H01] try / catch 基础
来源：http://mobile.epnwcf.com/Article/details/gqmtjmlcy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/ggupxuesr.sHtML


<!-- 参考信息 -->