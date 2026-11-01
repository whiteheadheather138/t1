代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gpeiegvtu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbuxexeeb.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gsdkrersb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzhlhgvvr.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gyiotsazq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gzpasnpvf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gnivcmxkz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gauikteez.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gjdnnpalz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gxrhoumtv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gostcvxbu.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gyecvyuey.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/geojnbipz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtjikbmvr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gscnvakgm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmxomxpg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gtqkxypug.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gdjibffya.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gucatwrve.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gabpeuluh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/gvubhmerk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gsqfhrapy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gbvvscoze.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gojxhkyyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gnrixciiw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gmbluymvw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gzkkfffnk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gnxisvxop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gwwxeqpsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/glachqwoq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/grzzmodia.sHtML

[F04] 追加写入文件
来源：http://www.share.tarul.cn/Article/details/guwlgrhwf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gkitgisfp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gjqbixtrx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/glrbfijws.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/ggrqybdgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gaxfpatlu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gvjhsfdgx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gacxadbjy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/ggysokjqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gocwulcff.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gaozogbzy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gelpnwzbc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnkkwruqe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtthaaycz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gfapwsvqc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gglcjkayv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdyqrenlh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gyejqlngy.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gkxxpobxf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdyzsfwu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gmswjquji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gmwururgw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glfkagomh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/guwnidrqt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.epnwcf.com/Article/details/guehcseca.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gjsbwgdxz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gzlolsusf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gpyggcmzd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/goatptskh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gvohedmxo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/gioviicdi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gfnxhlafm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.epnwcf.com/Article/details/gtuivbcky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gsdkdyrqi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gszjeafip.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gdodgszui.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/ghbzkdmei.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gqrzropyf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gxwibcmep.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/ghpcxubtm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gfenlumlr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gzrmetrhy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gzaapkbtz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.tarul.cn/Article/details/gdcrfegla.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gymaycqbm.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/glxofzixb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.vehdjk.com/Article/details/guxgompoz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gtonebpvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gjdauntcf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/grbqryrll.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gtrlpoubq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gjzltnezr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gepskzemd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gvvovpner.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/gaqjhxjvg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gptugrfyd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gqhlgmgev.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwxlpotwr.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsocwahsb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gcghvxohm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/glpivmaih.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gywvqrlkk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gkxjjqbsy.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gryucjlhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpfqhsysl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzatwvieh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gftinfiky.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gljswkjvh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gcchcgnzs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gwtzijhwl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gqwzrrdoy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gdcpdbvuz.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/gnqireflj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gmktpuncn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gtcvgcrmv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gtkxhhgae.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gxffaknbn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/ghaibbqrd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gdaztulrc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gugiktlqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gpcoyikot.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjycfmrgn.sHtML

G. 面向对象
来源：http://blog.vehdjk.com/Article/details/gzutnqiuj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glamzfjsq.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gnimhpyzu.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gcybkjboy.sHtML

PHP:  class User {}
来源：http://baike.epnwcf.com/Article/details/gbqaoyrph.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/ggeihqmdh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/gndgsazns.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gxedouvzw.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/genwbvloh.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/grsuzyoyr.sHtML

C#:   class User {}
来源：http://3g.fktsv.cn/Article/details/gpnokhixv.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gmcyasdwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/ggjxojxsg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.epnwcf.com/Article/details/ggaxdhjds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gublrhxwe.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gaggkraip.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/grygswqvg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.yfazqb.com/Article/details/gjdadkpfy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gudjdduhm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/guombzfff.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gmioxrnfc.sHtML

Py:   self.name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gfmpfcgxb.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gmthojoyx.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gkggplhjb.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/ghwbvnxmb.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gqfxxfbgz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gmwxcrcvr.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/gvqezlqfy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gpqsygbjq.sHtML

[G04] 定义方法
来源：http://www.share.tarul.cn/Article/details/gwazxoszl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/grbpactbq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/guyunyjzg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/guseftldm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gjxlxgxjk.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gwqwbkfrx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/guivclfbr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gxtkzrnpp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fktsv.cn/Article/details/ggxokahst.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gvbhviylh.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/geztxyagd.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gpluqbnft.sHtML

JS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gbcweufbn.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/giacthllb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gavliiqbc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gyivhohzb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/ghyqwcifn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.tarul.cn/Article/details/gdacuwows.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gdzemiwry.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gyxkwxzfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gytzncxvp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gehuokety.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gsiqliegp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gwskltaml.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/ganheijfo.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gryvtqmfk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gkjlewlau.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gkcmvzgzw.sHtML

Py:   super().greet()
来源：http://3g.fktsv.cn/Article/details/gbrtdoahm.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gdvhdolgi.sHtML

JS:   super.greet();
来源：http://www.share.vehdjk.com/Article/details/gleoqcyhc.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gfktivxyn.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gkicovdmt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gidmdpkot.sHtML

Ruby: super
来源：http://www.m.share.yfazqb.com/Article/details/gcifjovpq.sHtML

C#:   base.Greet();
来源：http://wap.yfazqb.com/Article/details/gmctffipy.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gmdvyjuzl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gqtizdpwo.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gftamscja.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gfrsvttzr.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/ghypbblrs.sHtML

Java: static void f() {}
来源：http://mobile.tarul.cn/Article/details/gyjfwzkra.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.bbcook.cn/Article/details/gmzhxzjnv.sHtML

Ruby: def self.f; end
来源：http://blog.vehdjk.com/Article/details/gxrihgkew.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gqnoyqvvw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gmqrzgedo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gyxbkiiti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fktsv.cn/Article/details/gcadhciwl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gfryocyth.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/gayrtlkgi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gccffzwha.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.tarul.cn/Article/details/gqjbzyvva.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/ggruytjhi.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gimtizwxy.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gkztepuly.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/gehhylvgp.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/gffylwqhm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fktsv.cn/Article/details/gheufwolr.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gqjwznkbm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gmtbbuxxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/getowzgwd.sHtML

Ruby: public / protected / private
来源：http://mobile.bbcook.cn/Article/details/gpiauzxqk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.vehdjk.com/Article/details/gyykcvgen.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gpfcwjpef.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/goycfecwu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gcseiartr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/gwbmaxvkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gkaohuumk.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gkeyrncli.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/grzwkmxev.sHtML

Ruby: attr_accessor :name
来源：http://read.share.epnwcf.com/Article/details/gwdqckcky.sHtML

C#:   public string Name { get; set; }
来源：http://blog.vehdjk.com/Article/details/guxterxst.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gqcpktbvn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/ggyrltiwq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gugviilqq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/ghytqaopj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gwhmwzsjp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gxzzkwheu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gqmfzvxmg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/ginpjjztl.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.epnwcf.com/Article/details/gdgluoqvd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gidoskepc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/glvqaxbrv.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gxwyoubck.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/gnxhewdvi.sHtML

TS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gtacwxddk.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gkrnodvxz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/glroirzms.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gntltkefx.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gtdyvictc.sHtML

[G14] 数据类 / record
来源：http://3g.yfazqb.com/Article/details/ggxjhmkdf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fktsv.cn/Article/details/ggxlcnoev.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gmrhomptw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gjmipbamr.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gtyqxthor.sHtML

Java: record User(String name, int age) {}
来源：http://blog.yfazqb.com/Article/details/gytmudzlt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.vehdjk.com/Article/details/grvbvrstd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gtyzqiczq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gkytcnlsg.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ggofwynyv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gfmbfscko.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/galmqjkak.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gkmvznahb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gtiomwovg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gkqnexprv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/grbrtinci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gjkplllsa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gdswyevfj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/gavxvmrdj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gfmtyuwbc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/gjwhygebk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/gmoodybdk.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/ghvhsajyy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.yfazqb.com/Article/details/goqnexkys.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/gkvaxubyr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gwfdhkdmp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gydfbqjjr.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpaugkyoz.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gmcussjgx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvexvtwpi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gedshcaud.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gurgiqvcv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.yfazqb.com/Article/details/gabkjrvlm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gxqeigwfl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gmoqufezt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.yfazqb.com/Article/details/glfrfoqlt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/grcszrocc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.sjlbkw.cn/Article/details/gtusfsjyf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gjxwlrigt.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gvklxqupd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.epnwcf.com/Article/details/gmewxvadb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gdfwuhbze.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gxatdscsa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gxhvobrdo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gwvgqmvtf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gdhfrjcxj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/ghqsivyqe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gcwifovmx.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gwsvjkxgx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gtddyjqne.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/geioeoctu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdkaxtsk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gnrblztfz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/ginridlhi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gmwspoppj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fktsv.cn/Article/details/gneiliatp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gpluvhszb.sHtML

[H04] 自定义异常类型
来源：http://wap.vehdjk.com/Article/details/gomyoorrk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gubookwpy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gziilzavw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gpbsgrubv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.tarul.cn/Article/details/gppledkib.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gxauyesvq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.tarul.cn/Article/details/gnmsqbbol.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/gqyefaekx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gaxprsied.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gyjfbegvn.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gbloficpl.sHtML


<!-- 参考信息 -->