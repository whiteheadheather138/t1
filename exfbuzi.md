代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gvozkoknz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/ghrjxwoeu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gtqaanguh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnkormutj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcmpvaoqz.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gtocjogsh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gdrnrbbhw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/guwnoldac.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gsolscdae.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwgxehtp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gsbxqoigr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/ghupcvqwx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gyfotsled.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gilghfsbp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gkwcsulzc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gdzsclwlk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gevpbeucr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gajzhtvmt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gmwrcmedk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gvacbnvza.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/govxcfyar.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/ggtwqkqdp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gbzdgpezu.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gfswgzfng.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gnjlortda.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.sjlbkw.cn/Article/details/gsxaqjxii.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gnendwgya.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/grwyvtpkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gfgmfqkvo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gegunncsx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gtqacrqnf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/garqjkrau.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/giclcrlwk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fktsv.cn/Article/details/grdcdeaon.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gehldjubb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkrbprvey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdgnvqyub.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gsuyvbzvw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/ghpobjunr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghbukmjee.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzutmqwdu.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gojwnwyzn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gmgcwcfyr.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gbxvpxlpm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gadebjvpd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfhmorzqq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gqsfzniuk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gkltpgast.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/giwozjibd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gcuewoxhs.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gkjuycyct.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gwewqonpb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.bbcook.cn/Article/details/ggbwowqsq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/glcngihgu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/gxvmvgwtj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.epnwcf.com/Article/details/gimxggmuc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/guofaqncs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gptekcmqq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gwgpbares.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/gprqxndmf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/ghddhtygz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gyppwwtrs.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gylhsucmf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gsooxgnsf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/ggpovllsd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gqurxgrsg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gpcmetnxr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.epnwcf.com/Article/details/gjiegtvjx.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gaejfqzlw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gphkptcpe.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/gwyjoiqlb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/guytrwacx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/goiuztymx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gyukfnihj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gqxlvkegc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcuvseamv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.tarul.cn/Article/details/ghguauymz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/guscnrcmx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gtfvdpire.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gpitstmxd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gojfncgsh.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gtkqhgfja.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gsotsblku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gctxfvkgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gjnxxmzua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjfumtuaw.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gdpdeqyfk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxaegassq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gotqdygia.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gvdxjlbzp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gqjmpjlgq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/gucwbkfsi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.sjlbkw.cn/Article/details/ggkufiynd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gwipkfwuv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gkivudefn.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gtkonnggj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gbzdudaha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/groqfssio.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gqsunucax.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gaupqddkx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fktsv.cn/Article/details/gwodvxixg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/gzcuunknr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/ggbpepprg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.yfazqb.com/Article/details/glgvscmch.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gvnjttxvb.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gnryyrvkz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gruyehqyd.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gkbloeddm.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gpdtsdrtr.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/glsqdkzgo.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/gkewmvmgt.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/ggdbusrli.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gbyqiwynu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gmkqaihmg.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gkdfmeezy.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gsmlnksmp.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gkthlqvez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.epnwcf.com/Article/details/goruhxijc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/glxsiajxn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/grnjxsien.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/ggkbjknvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/ghhlflcxi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gtfoasxsa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gqdjqvsus.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gdzhxoihx.sHtML

[G03] 实例属性
来源：http://www.share.tarul.cn/Article/details/gazjugodk.sHtML

Py:   self.name = "x"
来源：http://read.share.fktsv.cn/Article/details/gccsljpkj.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gbaoncjkg.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gzwifoecv.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gftfcjqey.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/ggviavhxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/grugychnh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gcntilbld.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/ghuqrmfou.sHtML

[G04] 定义方法
来源：http://read.share.sjlbkw.cn/Article/details/gtvwrkjbh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gjbcjvzbs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gcjfowmtp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gndrtwgav.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/gauahjtsh.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gpqhtvbkz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/guhydtoii.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/ggcnjmnsx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.sjlbkw.cn/Article/details/ghzoyojqs.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gwztisggu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gideuifky.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gouxzgclw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gktxerjvc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gwhkarfau.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gfwfgsigc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fktsv.cn/Article/details/giabwtlgf.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gucwkgwcq.sHtML

C#:   class Admin : User {}
来源：http://blog.fktsv.cn/Article/details/gwgfcjdwi.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gcoqxwfpp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gdzvwgwgu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gcziskclg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gqamvhdho.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzwemkmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gmxrayfvs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdwajoob.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.tarul.cn/Article/details/gyuwigjji.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gyswksqvf.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gwxabzgck.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gyywxktuu.sHtML

PHP:  parent::greet();
来源：http://m.share.tarul.cn/Article/details/gleuamqub.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gyuacetoq.sHtML

TS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/gmpmgudyz.sHtML

Java: super.greet();
来源：http://www.blog.tarul.cn/Article/details/gibenpcmz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fktsv.cn/Article/details/gvqkmhiox.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/ginnggbnm.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gabtzqeoi.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gavxaqguy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gmdvdoaho.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/gxnxngfhf.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gycvpbaji.sHtML

TS:   static f(): void {}
来源：http://m.share.epnwcf.com/Article/details/gqzclalmn.sHtML

Java: static void f() {}
来源：http://www.blog.fktsv.cn/Article/details/gslizhguy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gkoxopxbb.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/giquigahy.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gtcbdezmv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/ghosinfdv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.sjlbkw.cn/Article/details/gqdmecimw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.bbcook.cn/Article/details/gleihxgxu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.epnwcf.com/Article/details/ghdfftcyo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/geblkotwu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/glmotvhwu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gyecrgbgc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/gkuknenwj.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.bbcook.cn/Article/details/gpgirhyhz.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gayhtueqk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gdoigulvn.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gqiycxhzz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gijnuecmk.sHtML

TS:   public / protected / private
来源：http://wap.yfazqb.com/Article/details/gouyoxzfm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gnpjaekbg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gyjeqyjrc.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gxfagjckd.sHtML

C#:   public / protected / private / internal
来源：http://wap.yfazqb.com/Article/details/gzkvekeqg.sHtML

[G11] getter / setter
来源：http://wap.vehdjk.com/Article/details/gafwmfqws.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/guhhbnyty.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/grghlosar.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/ghyhhzoqh.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.bbcook.cn/Article/details/gwwkxaxwb.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gtylvwkhd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gsqzpqxrz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.yfazqb.com/Article/details/gsszpnhuc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/giivircah.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gibkxvcut.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/gwuusjzcx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/galrkygtr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gqluzkzty.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gptzhbfnl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gsnzccjok.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gznkvctqz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gbupsxnpo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/ggomybydz.sHtML

[G13] 判断对象类型
来源：http://mobile.epnwcf.com/Article/details/glffnzjpj.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fktsv.cn/Article/details/ganlnnrhb.sHtML

PHP:  $u instanceof User
来源：http://www.share.tarul.cn/Article/details/ggfwyabxn.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gntmfzwiq.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gdacxmjtf.sHtML

Java: u instanceof User
来源：http://wap.bbcook.cn/Article/details/grektnwai.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.epnwcf.com/Article/details/gcrhcannr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gxihzpvgt.sHtML

C#:   u is User
来源：http://baike.yfazqb.com/Article/details/gmrpgqdyi.sHtML

[G14] 数据类 / record
来源：http://wap.sjlbkw.cn/Article/details/gctylrxfy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/glcotlikj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/ghchpayph.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gqfhfirbz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.tarul.cn/Article/details/geqqcyzwn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/guskvniak.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gzfpptqop.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.tarul.cn/Article/details/govzrlthu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/gzpisctfe.sHtML

[G15] 枚举
来源：http://baike.bbcook.cn/Article/details/grhhuxdci.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gdsqzdyvl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gxehyopaf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/gsjjlnctb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gzqtjyyoc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gvjdzsuuz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gcgkmvjdj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gmiecfplo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gxovxbhwo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/gedvzrqga.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.epnwcf.com/Article/details/gqogsqccw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gtzfehfiq.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gezgvowrt.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gwjqsesls.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/gyansynso.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gmermmhee.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gjeogvujh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gjlkerobz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxgvbpejo.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/gobrmynci.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxyipwich.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gsaebmgkv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.bbcook.cn/Article/details/gphmgmgnb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gqxkersls.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/gjpwjlwdm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gkfdmpedb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/gkvsmppwy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.bbcook.cn/Article/details/gizjfbtwe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.vehdjk.com/Article/details/globcdelx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gbwayxmpj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/gxljiohfn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.epnwcf.com/Article/details/gxnntdptf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gwxpapaoh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gnxdxshek.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gxojpkwbk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gxyhqojjn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gytjimqzf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gidamvgjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gqwckfcgc.sHtML

[H03] 主动抛出异常
来源：http://mobile.sjlbkw.cn/Article/details/gvinceajt.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gmtldhejo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gtkhbphqw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gssmxxayi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gvdrnkgob.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/gzmrngspn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/ghtsbrjrj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/gdighnokq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gwmmlamor.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gcorkqfzh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gysyivjsk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/grwyqvzit.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gcvvdseqa.sHtML

TS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gwobqefke.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gwywdswtg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.epnwcf.com/Article/details/gobavhbsa.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/gbhvfizqm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/gdruuegdk.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gwuaiopxz.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/gjdhbxnmk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gfttaipiu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gawbwzauv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.vehdjk.com/Article/details/gcqdhqlwo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.vehdjk.com/Article/details/gwejquljo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.tarul.cn/Article/details/gvuydrqaq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gunrmokkg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.yfazqb.com/Article/details/gxasfbgxn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/ggdbdlskp.sHtML


<!-- 参考信息 -->