代发 wailian999

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/gstlgpjcw.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gddlwjqmp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/ggtvrdtfw.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/giobyxyxk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/gqafvvofv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gvomwtivj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gfotnlnic.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gqoqrdcbu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gnxoljbvq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/gavzwzolf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gyaldcgjp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/ggoipzkdk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gpzromxqy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gsfkoqmgd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gcuzaommz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gpjirdrcx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gnellvufk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/ghpvyngtj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gsuirbkrh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gkedjqvif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gtdkgmmop.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsqgindvj.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/gvldlkejg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ggluqromn.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/gtufcnfyv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gukcaeacv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gbrrvzhfa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.bbcook.cn/Article/details/gitqwifji.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gxoctvchw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gamdgopoc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/grsipqopi.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gapzqxcxh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gidwkquua.sHtML

[F02] 逐行读取文件
来源：http://blog.bbcook.cn/Article/details/gwcelcbcr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/glrmvfiwg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gcvwvbcxm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gmmzlddxg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gvhhroyqg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/grzpplmza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gzcvfkhee.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gxilwkavr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gzeercvot.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gltmjbrdt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gerapfwpk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/glxnupudh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gcufukpew.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/gingdpdux.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gefizvnls.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gcqmwxeel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gpirmlkzl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gnburrvvq.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gvmcpvixn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/ghatojvbk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/gfesovxtk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gmfuaiuxp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gtzatddvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gzlvbtlfh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.yfazqb.com/Article/details/gwulvxgzw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gyupicuhg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/gnqfsgqfp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gpcltwyhj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.bbcook.cn/Article/details/ggljmhcyh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/gkjpypjpa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzokjnmym.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcrshzcle.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gbjdqtkpm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gdefhwdgp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/garoutlky.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gdhdzkqgk.sHtML

[F06] 删除文件
来源：http://m.share.bbcook.cn/Article/details/gbjibqgsb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grwjtinmd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghtadfdnt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmsafwaml.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gcusrjusx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gjxqvbeei.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmgsltuoe.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gkkvimamb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gcviqdszu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gklwbmbxo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/guumewhtc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gsyqkivvk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gkcrsmowl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gmizupruf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/ghncfefql.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fktsv.cn/Article/details/grcilvacp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gebzhbubk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gvqtluseu.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gqlbxipsx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.bbcook.cn/Article/details/gbmrweslu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gdgsunafh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gkoyhjtsi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gnyzofume.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gkwqbpcue.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/glnrpjosy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gglxjnxai.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.vehdjk.com/Article/details/gkwvalsts.sHtML

[F09] 获取文件大小
来源：http://www.blog.fktsv.cn/Article/details/gnxenuuop.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/guxsxfcna.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gvekikfnh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/ggfbaeebd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gobrhjrux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gdayfmrmz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gtaqcbsau.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjkfovfjz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gxfzkohgw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gdertivwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsbgvopry.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gqepukrdj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gginhzupe.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdtrcmklf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gowmdpjrf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gxhlasnyo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gojrjwmxj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggcxjrhkp.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gifozldob.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/geusxasdi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/gtxdxlydx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gzzwxbcmg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gfqgdmdqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gmkmmeaxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/guqfmitko.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gdojixqao.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gartjfecn.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/galndkxut.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/guujbxeij.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/giadybshe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fktsv.cn/Article/details/gbfwzfyxk.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/gtspgzoyi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.vehdjk.com/Article/details/gyolvagzy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gqvaateqr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gdqauacer.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gmimwamfi.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grtrwqajw.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gugmunbjb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfxrbzyau.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/goshrtctr.sHtML

Py:   class User: pass
来源：http://www.m.share.bbcook.cn/Article/details/gfzbaamoo.sHtML

PHP:  class User {}
来源：http://blog.fktsv.cn/Article/details/gioenydvg.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/glgintoxo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gvmitblry.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gmkjjauku.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/ginbcrqis.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/gjyswfmuz.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gpuxcwjok.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gbsriuqni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/ghpipfvyb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gjnekmcty.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gtgsldnbx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gqwicknqq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/ghyencapg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.sjlbkw.cn/Article/details/ghljkmpdo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gssyfzoav.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gqehghiri.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gjcjbwrqw.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/gkmkdthhc.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gibaxzgpz.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gpbciltdb.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gvnxdmbqa.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gygqhzxkp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/ggeeyyari.sHtML

Ruby: @name = "x"
来源：http://read.share.bbcook.cn/Article/details/gnuzwkapv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/glthdtadr.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/ggmkyuqgr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/glgkyxnch.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gsbzuhtpe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/genfecgak.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gzasbrmdf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmpzqwcgd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/goclsccks.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gtpbpffty.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.vehdjk.com/Article/details/grqssaybo.sHtML

[G05] 继承
来源：http://mobile.vehdjk.com/Article/details/gkoxepjhe.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gysourhbo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gfszvszow.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gveeczjwq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gerolgdwp.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/ggqajivla.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gtocflgqf.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gdzzmedsx.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/glysakvsy.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gauuxonaq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gweyegolm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzbcbesue.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gwgkazjpt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gmbhiejjy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gtbvvibli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gdxszhmhc.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gpejjbotg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.bbcook.cn/Article/details/gdotrgmcc.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gygjqteie.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gpresjilf.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gtugqgkfu.sHtML

JS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gcxndlnlh.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/gsgvruiur.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gjnxljajz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gqwwqvrdy.sHtML

Ruby: super
来源：http://baike.tarul.cn/Article/details/gffgrsfuh.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gszrvebgy.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gkjpyewkw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gbvumjehw.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gfxubswvg.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/geuqiueyc.sHtML

TS:   static f(): void {}
来源：http://wap.vehdjk.com/Article/details/gwrilzrta.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gqyqfdhbu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.sjlbkw.cn/Article/details/gpkprgqdp.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gginjudka.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gnoocnskr.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gxnhjmibi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gzabemsnn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gyvtwyxqo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gwsoycauq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.bbcook.cn/Article/details/gielmgzyr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.tarul.cn/Article/details/gtesvbfvu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/gmufbkfln.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gydngckyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.bbcook.cn/Article/details/gtjbcyxbg.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/ggcnjtuzb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gzsulfsqm.sHtML

PHP:  public / protected / private
来源：http://blog.yfazqb.com/Article/details/gwhgtehhx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gqyusiywu.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gwubixxdh.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fktsv.cn/Article/details/gbrunskyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.tarul.cn/Article/details/gwjombzji.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gvgzsekmg.sHtML

C#:   public / protected / private / internal
来源：http://3g.epnwcf.com/Article/details/grajmguki.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gfyakpbwi.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gdmsdrbqz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gcaajacin.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gpmqxesqf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/guzuvnvdj.sHtML

Java: public String getName() { return name; }
来源：http://baike.yfazqb.com/Article/details/gdopsanlh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gzalpacoc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/girxkrcyc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.bbcook.cn/Article/details/gbuxxswmr.sHtML

[G12] 对象转字符串
来源：http://read.share.yfazqb.com/Article/details/gqaqjtkio.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/geigxsuvm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/goallkozt.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/grrpqcnnu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gopkypuvr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.epnwcf.com/Article/details/gxntkaapf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gbxnfkjpf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gqpenbyfb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.vehdjk.com/Article/details/gkzbsnycy.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gdtnlfuax.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gdsbqrkqb.sHtML

PHP:  $u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gubyvlhsg.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gaprfbfqh.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gqknoutbb.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/gcsioduel.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.yfazqb.com/Article/details/gjaultogc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.epnwcf.com/Article/details/ghumkvszd.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gvnabduvt.sHtML

[G14] 数据类 / record
来源：http://www.share.epnwcf.com/Article/details/gpeceqxgv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fktsv.cn/Article/details/guxixhyfb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gifybonuf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.tarul.cn/Article/details/gwkpjauoz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gubnllfex.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fktsv.cn/Article/details/gqrkcugdf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.vehdjk.com/Article/details/gbwavkyfl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.bbcook.cn/Article/details/gmxgcsxhf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.yfazqb.com/Article/details/gpvgwtppg.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gqdwvipqg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/gryhbcfne.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gujglnuqk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gruefjpab.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gzddmcypl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gwmmfthtz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gdqvozbiz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/gzkmgpyyj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gkqpembdu.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/gbjdakbvu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gnvedxsll.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.tarul.cn/Article/details/ggocmsdpe.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gwsmkwpfx.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gizciccys.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gsnodpasi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.tarul.cn/Article/details/gqklyqqbo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gfkvrasks.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gjfmakcdo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqcqzsqjd.sHtML

H. 异常与错误处理
来源：http://www.blog.bbcook.cn/Article/details/gndvlhuup.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkscjduni.sHtML

[H01] try / catch 基础
来源：http://www.m.share.yfazqb.com/Article/details/gzgjsttxk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gblkhilre.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/gkdlncyaq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnqtzyur.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/geznuqacd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gyztdvhgo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/gqsaabedi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gmazhtily.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.yfazqb.com/Article/details/gecjmfpia.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.sjlbkw.cn/Article/details/gxdwweeyz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gnugyimel.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gkaewjfqn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gtchgberg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gzblprlkn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvntrvlnb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gihtprpsb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.vehdjk.com/Article/details/gggtyjesm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbucptbuq.sHtML


<!-- 参考信息 -->