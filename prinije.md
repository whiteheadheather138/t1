代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gcuhrknac.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/grgxwinhs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gmnsflehl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/glfiuyvly.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gvebolnfw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gcigrvqay.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gzihurhlr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.yfazqb.com/Article/details/gavkyuxaz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gnnfhizuz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqgejxdpw.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/gvkftwofj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gslxgjgeg.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gvreqxlug.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/gjnirqioc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gnfrohmhh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gyrfahsvj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/ggkttyjkx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gsmbtrano.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gqfyniijq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/glcsbtvhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gpnkvlhje.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/grkzqnmyf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gvhbvtivg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/guxawlhgf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gimehxlfh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gbfhwwdvv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gfcpvbaox.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/grcsxoyyl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gdjfhykow.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.epnwcf.com/Article/details/gawvkpzwd.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fktsv.cn/Article/details/gtbhicwwl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gmhoxmuqs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gajmxiwsl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gueqjxgkm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/ginxxwoki.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.yfazqb.com/Article/details/gzimebyaw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gnnhwswqm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gutachypi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gpwrjsufr.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/galpyoivx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gckruolae.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gvxpzomvi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gfioxnqxm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gnpqpxhgi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gxzdcmcrh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/ginewfser.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gokwijoja.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gwcuzumxj.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/guxkebbxg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gctmuoezm.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gnslagggb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gnkcnozwx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtfecmiwf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gfpnrnpll.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gqwyxzkgf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gxttatksb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnmjhcmnv.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/grceowbgm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gucuvlmmh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gxpbmkfyh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gsuleztmc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gaqbkwxzx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gnkhvrdnc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gmkthpjtq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gomeudetu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gakdibqqa.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gudduvusq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.sjlbkw.cn/Article/details/gmezitsun.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gbemuubnr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gteygnvwm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gbzbfpakf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gyonayakp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gwgbtsicr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.vehdjk.com/Article/details/gwukxknfa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gynoyenyb.sHtML

[F08] 遍历目录
来源：http://www.blog.vehdjk.com/Article/details/gjpqycujz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gxrhugbkd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gmjfxhrhm.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gbosiinwy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gorfwvbjt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gfioavtrh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fktsv.cn/Article/details/gxxrtuxhl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gsbfbxinf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/ggdusgysz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gofpxeoft.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwkdfknzy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gkevdfnhm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gnandzkhn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gqonigfao.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gqzlkzquy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gvisnbwfq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwrayurab.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gqclfravl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.yfazqb.com/Article/details/gemhwjmfu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gahvqpbvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gwpvxxgcv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gaiikbfej.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gidajtftm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gkwyxcbvk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gxfwlugrq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/glhyvruyu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gdeapxngi.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/gtibrnjzo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/giceybkll.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.vehdjk.com/Article/details/ggdimbcls.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzwzvqqv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/godovkrcb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.yfazqb.com/Article/details/gwjqhapvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gpyfqmpgn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/giplreidh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gcgqlflsf.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/gsnyharzu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gfprrinsn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gvffxnykp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.bbcook.cn/Article/details/gynzftsiz.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/gdtwfvonr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gbfzdeyzt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.bbcook.cn/Article/details/gqewvvcsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gwgfzcltf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/gxounqgxk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/godtmdrad.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gphfowjuy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbudwpnzx.sHtML

[G01] 定义类
来源：http://read.share.yfazqb.com/Article/details/gochxcnqs.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gxnnksciy.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gyhuipjrz.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gswsyhmgv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gemccepys.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gyquprzzg.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/guxdrxmgl.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/ghlxtaovs.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gkqdyherz.sHtML

[G02] 构造函数
来源：http://www.blog.yfazqb.com/Article/details/gafgodirw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/gxexbqrxy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/gapoevxka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gvdswvnms.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.bbcook.cn/Article/details/gzoocuhyq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gxgmbckkj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.sjlbkw.cn/Article/details/gtbxzjoib.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gsqubrfwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/ggozjwjkf.sHtML

[G03] 实例属性
来源：http://blog.fktsv.cn/Article/details/gqjokqvgg.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gihtdfmou.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gqrbilmew.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gwyyafkgq.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gzlscndjy.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gweowkocj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gfxweajph.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gjjpqlpmp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gqmoohile.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gdnncbeyx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gvteapwef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gfuktpuhs.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/guppafmqz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gxpwzmbqd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/ggdqwdrcb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gtbxyzocb.sHtML

Ruby: def greet; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gdekmrfay.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gausuohgd.sHtML

[G05] 继承
来源：http://wap.tarul.cn/Article/details/gpuvkacui.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/grnlpnvkx.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/ggfsubeia.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzoxbbnhp.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkwkaxxqh.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gixheqlsb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gcvyjepwa.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/ghayfbkeq.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gpbosgdrw.sHtML

[G06] 重写方法
来源：http://read.share.vehdjk.com/Article/details/gbyybkqaq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.tarul.cn/Article/details/gtcazpnpg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gkizftyui.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ggzvdxqcm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gmefxofyh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gjvrsojcl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/ghvybaksc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gwgbrpowv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.epnwcf.com/Article/details/gblxuesip.sHtML

[G07] 调用父类方法
来源：http://read.share.vehdjk.com/Article/details/gndtmobxl.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gwovqqiki.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/glpoqibhz.sHtML

JS:   super.greet();
来源：http://www.share.bbcook.cn/Article/details/gdfdasysd.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gbuowiykb.sHtML

Java: super.greet();
来源：http://read.share.tarul.cn/Article/details/ggnclhxee.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fktsv.cn/Article/details/gxzrbtkxu.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gpqtfxawd.sHtML

C#:   base.Greet();
来源：http://read.share.yfazqb.com/Article/details/gookbqrcc.sHtML

[G08] 静态方法与属性
来源：http://wap.sjlbkw.cn/Article/details/gosorljwv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gcshuuthi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fktsv.cn/Article/details/ghqucgtbl.sHtML

JS:   static f() {}
来源：http://wap.yfazqb.com/Article/details/gkfwtwudd.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/ghuadbvke.sHtML

Java: static void f() {}
来源：http://blog.vehdjk.com/Article/details/gfkqkabfa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fktsv.cn/Article/details/gbjjgjorv.sHtML

Ruby: def self.f; end
来源：http://blog.bbcook.cn/Article/details/gexewcoaw.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gyuczascf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.yfazqb.com/Article/details/ghtaoizli.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/grgxvgous.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gpsjjdiwq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.sjlbkw.cn/Article/details/gxsacyqze.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/gubeqrkno.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzisvyqmu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.vehdjk.com/Article/details/gzcvqupge.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fktsv.cn/Article/details/gadbuahbq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.epnwcf.com/Article/details/gksaeqrsj.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/grbniepcz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.vehdjk.com/Article/details/godfcspfm.sHtML

PHP:  public / protected / private
来源：http://3g.fktsv.cn/Article/details/ghfjseaup.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.yfazqb.com/Article/details/glfnrvlni.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gxluzympb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gaarbrfwl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gqjdmtkur.sHtML

Ruby: public / protected / private
来源：http://baike.fktsv.cn/Article/details/gmdzugrqv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.epnwcf.com/Article/details/gmmaxsqkn.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gvhwxriwv.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.yfazqb.com/Article/details/gncogjkxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gonmvzpcl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gndnnlhzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gtkjdtlfc.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gcsebonrk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gjpvepoph.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gmxgvzmav.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/gxghwtsnd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gpvybvnnz.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/govftatvm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gdsosvyzq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gggvjizix.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gbifdbqeg.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.tarul.cn/Article/details/gfberhxsz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gunkgwrqf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.yfazqb.com/Article/details/giptthwqk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gugqyszph.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gxwwhpuoc.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/gncajrewr.sHtML

PHP:  $u instanceof User
来源：http://read.share.tarul.cn/Article/details/gsjiexbyd.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gwsubxyrn.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gwbphypnv.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gnebsafbd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gakfjrvxt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.bbcook.cn/Article/details/gslnsmwog.sHtML

C#:   u is User
来源：http://blog.bbcook.cn/Article/details/gkavjjjtn.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gefsjsszg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gmawxpenq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.sjlbkw.cn/Article/details/grgkokcep.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.vehdjk.com/Article/details/ghfykzvze.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.vehdjk.com/Article/details/ggykdabgk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gkeembrhv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gxcgoiidu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gmffoznnd.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gaobetyfu.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gxxrtxall.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gyykvjhas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gxaebtmfg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gazmhttly.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gyszfleij.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gighwddks.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gnbuibbnw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxnjadrl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gfqemvxwj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/gtwxkzuzx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gdvixqybl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gclfijfcu.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbzlohrno.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnijwqviz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gxbrlplnz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/guxiycdxg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/ggtaaifax.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgpymjmg.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggsorcmih.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gbfoprmhw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtwqggepx.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gaxrwzqfk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gqfejefqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gtnaumidf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gsygzyges.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gwxnpjtqj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gwkggwrup.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.yfazqb.com/Article/details/guzucpzkp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.epnwcf.com/Article/details/gdvvrikkm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gfltcpbpe.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/ggfmfchti.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgjcttkn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzbaemoul.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gfjridrxo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/ghdqbruyy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gdxavibvv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.vehdjk.com/Article/details/gutgehnle.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gedvgbbyz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gcbvzvguk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gofbxnmcz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/gboufevvl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/giffttboz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gdkcgcrfs.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/glqnkfeuu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gysyswsix.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gpuwjqgvs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.vehdjk.com/Article/details/gbtlfkxyk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gxobzzsua.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gscjyobju.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gvlpqikcx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gxqqbkfym.sHtML


<!-- 参考信息 -->