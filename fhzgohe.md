代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gsyguevyx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gnkvkjuwn.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gtolzlhmy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gtooynrhi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/ghqzwlfku.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gthfmgwmn.sHtML

Java: s.lines().toList()
来源：http://blog.vehdjk.com/Article/details/gkcencdbr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gpuskauwn.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/gwwiknfwo.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/glqnxxjgd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gumkcylfg.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gdualbdfz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gtodspxwc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/ginwtvhau.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gympylqrl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gugwjfxry.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gpbvmjsuo.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/gpioszeyq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gdnvbeddw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/ggcomzzie.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/gcdozepfj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gckrmghky.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gyigonqfo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gkwojjmxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gcaxxigkc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.vehdjk.com/Article/details/gvapjtrnx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gxuxpzlfx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/guhakilld.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gznpkufot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gttznuiol.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gifrtysyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gtobgfhcx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/glkeehnof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/geopixsyn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/goynubmly.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gqypguurt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gvxnqycnc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gckalqyrk.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gcfxisqbt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggppskehl.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gkzhkqbul.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fktsv.cn/Article/details/gyazvgidn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/gyruutvve.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gbbalugwz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gdsviisix.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxkgredkc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.vehdjk.com/Article/details/gachbgprk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gjkwzmfog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gnhuuukjo.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gvqgmvzpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gfaifhchu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gpfnylfqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/ghwknjrso.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gcqpxnzsj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gayrowxfy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gwwouwasr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/gwwbgsfos.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/gkloidajd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gfxmkbzgr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gosuhimxw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gqkpdkisq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gmpvnhwiv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gioaoqovp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.yfazqb.com/Article/details/godtvzmdq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/grdbfmxky.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.bbcook.cn/Article/details/gbijuaygr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gfbewyser.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/ghcsktwym.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/gjjyerelr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gmmwctxop.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gclodfeas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gwmierfbi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/giboqieym.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gmienhesc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/grtyffdma.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gtlrjivqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gabmxtxip.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/grbsonxzo.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gftyqdxdz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/glbfigfav.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyvpcimqb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gajphiztp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.tarul.cn/Article/details/gninkncmn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gaomzczka.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghkxkkkby.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gkxsipauu.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gktpqclkm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbcewovix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gyhlduyjm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpshtkmqk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gmelixaxq.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gdrlfjhwr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpzksautj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/guhegsqtz.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/ggjmryysa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gkckavgza.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.bbcook.cn/Article/details/gynhdvjum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gwsszwcos.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gigwyueci.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/ggubvfuob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gqejzggat.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gzejxtnet.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gdsenjcvh.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/germpfdfr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gffhljkkj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gyyzduwqi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gcyvgzjqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/guxpqlmhr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gbwswzetx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gtdunrfrn.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.vehdjk.com/Article/details/gshqmsivd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/giqmymusq.sHtML

[F09] 获取文件大小
来源：http://www.blog.yfazqb.com/Article/details/gpieymmmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/getjlbhpp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gpatdetzk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gejwguadu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gnyzqxehj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gqwpansrl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.bbcook.cn/Article/details/geiuzoerl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gqtexrgvf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gaajvuxum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gtqqghaan.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gscldcvgg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/ghgrcubsa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gpvgjdxhc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gfccyndun.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/gfnzbtuja.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/glgwtrnwz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/ggvanolmq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gmdxdscvc.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gxtpxkrso.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/giusofrva.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gnnqpkhjw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gnmdffuxu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gwikzgafk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gchkrprcu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gxghwvjso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gtubxglri.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/ggwtdgyzj.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/giiedvbne.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gznqcwemk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.vehdjk.com/Article/details/ghhindlea.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gkgcmyjeg.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/grdqipqhj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gwicqcrks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gbhvmneqj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.tarul.cn/Article/details/gmpumdlzg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/galqzigxf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjbitqodw.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/gmefarfjf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvpohzxfo.sHtML

[G01] 定义类
来源：http://3g.yfazqb.com/Article/details/gdmlamvxe.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/grwbhjhhl.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gfzdukjvy.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gfwkawtub.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gghbyvjxp.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gvbweuuzt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.bbcook.cn/Article/details/gyekxttur.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/geergycgz.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/gwoqxnvra.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gtebtfgqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.epnwcf.com/Article/details/gzjibkvvh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gawwuucqd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gonmxazfp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/grmcyyprp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gavzkywmx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gasldedlx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gffhstqko.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gwmazzmgc.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gpgopxaap.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/ghvyislvo.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/ghwqdegem.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gotwcujec.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gadrnrxgy.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gviozfpkd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gbpixywcq.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gzwwnfsmz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/geihsapab.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gifkrrbdc.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gjpqavoud.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gmognfnnw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gxrlotdpx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcffetqgo.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gyqudfgqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gautjlway.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gujrulhpk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/ggmfwqkrm.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gitahqsky.sHtML

Py:   class Admin(User): pass
来源：http://baike.tarul.cn/Article/details/gykdesonr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gydutscoc.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gxrndmbqk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gzavenrem.sHtML

Java: class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gfppprtex.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gaeybvyqd.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/geuvdcugw.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gekgrxosw.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gkjxlqtko.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.tarul.cn/Article/details/guksegvsp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gzyorsymp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/giwtgtxkx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gokajbwjh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gahbjiyod.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gatdcbqds.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.epnwcf.com/Article/details/gqeybxwnr.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.epnwcf.com/Article/details/gaiiajooq.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gipmplvid.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gknctkylw.sHtML

PHP:  parent::greet();
来源：http://blog.yfazqb.com/Article/details/gnxjwzztf.sHtML

JS:   super.greet();
来源：http://baike.vehdjk.com/Article/details/gmbqhzahj.sHtML

TS:   super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/gqbgvxmln.sHtML

Java: super.greet();
来源：http://baike.bbcook.cn/Article/details/gldwwtiad.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.vehdjk.com/Article/details/gwckjqfpk.sHtML

Ruby: super
来源：http://baike.tarul.cn/Article/details/gcyxajpyv.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/ghixoprex.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/gkpiukdji.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gptyunxbh.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/gfmcgalmb.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gxmvxkuah.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/giptnioyl.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gsxiulhex.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.yfazqb.com/Article/details/gwytmapcu.sHtML

Ruby: def self.f; end
来源：http://www.blog.vehdjk.com/Article/details/gnzlalcpb.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gjjfugait.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gnztjxobq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/ghfwzelue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/ggehdttay.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gjtyymykn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gybpupkni.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnrzrqhvr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gbdjrniep.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gvlhtotgx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/glvcbzzwk.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/goeevmqui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/ggxgnhyrw.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gwsbkyjus.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/guihpkzik.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/grnhznxdm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.yfazqb.com/Article/details/gytbygbtd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.sjlbkw.cn/Article/details/geqcpzvye.sHtML

Ruby: public / protected / private
来源：http://wap.epnwcf.com/Article/details/gsozjgasi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.yfazqb.com/Article/details/gpqgbocxk.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gorbdczji.sHtML

Py:   @property 与 @x.setter
来源：http://blog.epnwcf.com/Article/details/gygimpjpx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gsqqvkksx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gsnpbasqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/grkqyiafw.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gfobcvxep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gfxdykdhm.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gscqcaorm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/geobmkouk.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/ghjllcfpj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/ganggwslj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gyrecsokf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/gxkmrdvqe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/guvbvuldq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gvojkxoad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gmdzfyghd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fktsv.cn/Article/details/guflgtnhg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gamiyohmv.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gkkwbdmfb.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gwuhtgolf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gqxvntkql.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ghhelssep.sHtML

TS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/ghhzedawt.sHtML

Java: u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gahhiixyz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.yfazqb.com/Article/details/gkkdvmcux.sHtML

Ruby: u.is_a?(User)
来源：http://blog.yfazqb.com/Article/details/gjcilbfuq.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gmppikbhh.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gzfzuveab.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gkfxhkbef.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gcdhzbqou.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.epnwcf.com/Article/details/gbqatbsko.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/gzmuaucis.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gpyxvaqfc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/gtwlncfrl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gguzskjyz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.sjlbkw.cn/Article/details/grdnfivuh.sHtML

[G15] 枚举
来源：http://www.m.share.bbcook.cn/Article/details/gprcsvrlc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.epnwcf.com/Article/details/glrrritfw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gacqfmelh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gjarerwjc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gahemnfmw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gdeksryys.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gmnyxtypg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.tarul.cn/Article/details/gpwsbzdwx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/gyuedbarm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gxbixuuab.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/glqxepdmc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gzoclwrbz.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gfoosevko.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/gjbnipslu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.epnwcf.com/Article/details/gkyvmnjfk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gmhdoxhci.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gytymhclv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gjmvmvhpb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnxalqhwd.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/gfxokxnss.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbbvczbai.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gjeanrjpm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.tarul.cn/Article/details/gqfnrnhqg.sHtML


<!-- 参考信息 -->