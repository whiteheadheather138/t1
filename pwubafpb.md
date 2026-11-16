代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ooi.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://jkn.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sik.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ltm.cheryme.top

[E22] 字节长度与字符长度
来源：http://wkx.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mzg.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gtt.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ezw.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzz.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://puh.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxq.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://wzw.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pho.hnxiangtu.top

================================================================================
来源：http://khr.cqqwz.cn

F. 文件与目录
来源：http://tvr.cheryme.top

================================================================================
来源：http://rjr.yueranfly.top

[F01] 读取整个文件
来源：http://yps.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qta.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://wuu.jlsjyb.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://csu.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://suw.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qjp.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dcw.ivvv.top

Ruby: File.read("a.txt")
来源：http://fiv.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://weg.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://yjo.zhixingplan.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvh.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sbc.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ypc.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ebi.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fur.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gtg.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ecq.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vtc.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://srj.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kke.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gix.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rdv.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qxp.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kug.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aie.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://dlq.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pjf.52xcode.cn

[F04] 追加写入文件
来源：http://zjm.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ibb.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://swx.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dve.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yaw.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ubk.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bqf.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rtz.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qku.sjlbkw.cn

[F05] 判断文件或目录是否存在
来源：http://ndh.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fxk.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://rbl.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://gcc.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://oiq.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ttj.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gnm.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://zdx.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://elj.daria6918.cn

[F06] 删除文件
来源：http://onb.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://glz.sysykeji.top

PHP:  unlink("a.txt");
来源：http://kjd.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://omp.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://eia.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nvt.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://bhc.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://dln.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://wyq.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://zpx.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vxn.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xhs.andypj.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://trk.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbn.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://don.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kiv.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://olt.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qik.nanxuanxn.top

[F08] 遍历目录
来源：http://vho.tarul.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nnn.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sbc.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://pom.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://lqy.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://inb.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ybl.hesvh.cn

Ruby: Dir.children("dir")
来源：http://ewf.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://ukm.uphjek.com

[F09] 获取文件大小
来源：http://jlp.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://tzp.zhijiandao.cn

PHP:  filesize("a.txt");
来源：http://mot.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://pqp.gzhubu.top

TS:   fs.statSync("a.txt").size
来源：http://ser.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://tqu.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gpd.daxiang520.top

Ruby: File.size("a.txt")
来源：http://iib.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://let.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://jbp.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ymz.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zzc.nwbrower.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dxf.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://zxr.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://phy.jqgfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tht.nwbrower.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://grs.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tjr.zdqjudy.top

[F11] 复制与移动文件
来源：http://xze.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gou.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mmk.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gqh.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vef.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://geb.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ure.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pms.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gsw.chenlongwang.top

[F12] CSV 读写
来源：http://nna.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lzc.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vss.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zsb.sufxvd.cn

TS:   // 同上
来源：http://tgt.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://krs.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nun.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qka.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mvd.jlsjyb.cn

================================================================================
来源：http://yqi.havefunace.top

G. 面向对象
来源：http://jpq.yanxiufei.cn

================================================================================
来源：http://zxn.hesvh.cn

[G01] 定义类
来源：http://xox.daria6918.cn

Py:   class User: pass
来源：http://uzf.zhengqikj.top

PHP:  class User {}
来源：http://tlq.jinghuilouyu.cn

JS:   class User {}
来源：http://jvo.sweek.top

TS:   class User { name: string = ""; }
来源：http://kpy.shanyushiyangkeji.top

Java: class User {}
来源：http://lzv.tarul.cn

Go:   type User struct { Name string }
来源：http://lsl.fehbvm.com

Ruby: class User; end
来源：http://mss.yuanzhike.top

C#:   class User {}
来源：http://kfk.guannengcc.top

[G02] 构造函数
来源：http://end.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://bie.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ukk.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ccm.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://hlx.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://pcz.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rzj.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://taa.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://zpc.daxiang520.top

[G03] 实例属性
来源：http://frc.cqqwz.cn

Py:   self.name = "x"
来源：http://fjh.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://wud.vqdsnc.cn

JS:   this.name = "x";
来源：http://vdx.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://cec.hesvh.cn

Java: private String name;
来源：http://gno.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ywt.guowangkeji.top

Ruby: @name = "x"
来源：http://nkb.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://doe.yj202588.top

[G04] 定义方法
来源：http://ocd.fengsongda.top

Py:   def greet(self): return self.name
来源：http://kmm.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ebz.jianghu66.top

JS:   greet() { return this.name; }
来源：http://pqg.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://uws.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://tjs.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://udi.zhengqikj.top

Ruby: def greet; @name; end
来源：http://kwz.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://mfe.nwbrower.top

[G05] 继承
来源：http://rfu.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://fdv.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://khc.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://jzd.dashuyun.cn

TS:   class Admin extends User {}
来源：http://nua.ehwqpu.com

Java: class Admin extends User {}
来源：http://fwt.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nnc.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://fky.zhengqikj.top

C#:   class Admin : User {}
来源：http://nqc.zhixingplan.top

[G06] 重写方法
来源：http://jlf.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://kal.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://noa.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://mww.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://uux.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://vvg.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tyq.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://cry.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://fqx.sxryk.cn

[G07] 调用父类方法
来源：http://bbj.gzhubu.top

Py:   super().greet()
来源：http://gvl.gaohongyu789.top

PHP:  parent::greet();
来源：http://arf.jqgfzy.top

JS:   super.greet();
来源：http://hof.nanxuanxn.top

TS:   super.greet();
来源：http://rct.hongshengwenyu.top

Java: super.greet();
来源：http://mgj.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uha.chenzaomai.com

Ruby: super
来源：http://iwx.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://djb.jianghu66.top

[G08] 静态方法与属性
来源：http://dkh.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fml.ivvv.top

PHP:  public static function f() {}
来源：http://ttj.jiagoushi.top

JS:   static f() {}
来源：http://dzs.xylfe.cn

TS:   static f(): void {}
来源：http://jbf.kuanghao11.cn

Java: static void f() {}
来源：http://skk.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zji.iojbl.cn

Ruby: def self.f; end
来源：http://rqp.dashuyun.cn

C#:   public static void F() {}
来源：http://ltr.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://arz.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://kje.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://smo.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gfg.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://kdm.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://bxg.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://txy.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xmy.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://zrt.pycfn.com

[G10] 访问控制
来源：http://wjm.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://huu.sxryk.cn

PHP:  public / protected / private
来源：http://oko.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://upk.yvedp.cn

TS:   public / protected / private
来源：http://ton.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://tvf.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://wtu.cheryme.top

Ruby: public / protected / private
来源：http://bqq.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://tia.ppjwa.cn

[G11] getter / setter
来源：http://wow.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://epk.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fbk.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://zrh.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://opo.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://qdi.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mia.zhengqikj.top

Ruby: attr_accessor :name
来源：http://tbz.yvedp.cn

C#:   public string Name { get; set; }
来源：http://pga.aibaodan.cn

[G12] 对象转字符串
来源：http://gwc.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://avc.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nti.hnqzz.top

JS:   toString() { return this.name; }
来源：http://smb.meibo888.top

TS:   toString(): string { return this.name; }
来源：http://pug.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://jei.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://wfx.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://ydi.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://uwb.jqgufenzy.top

[G13] 判断对象类型
来源：http://rvx.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://mrj.jlsjyb.cn

PHP:  $u instanceof User
来源：http://juo.shzxlz.cn

JS:   u instanceof User
来源：http://oau.zhiwuduotai.top

TS:   u instanceof User
来源：http://yxj.zdbjq.cn

Java: u instanceof User
来源：http://gdw.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zmp.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://rur.nanxinkj.top

C#:   u is User
来源：http://mwx.0kj1m.cn

[G14] 数据类 / record
来源：http://knq.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nfx.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://qnv.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://uah.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://agd.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://gja.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://kjq.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kyp.shangyingyoupin.top

C#:   record User(string Name, int Age);
来源：http://rmg.nwbrower.top

[G15] 枚举
来源：http://bav.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cwa.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://whq.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yuu.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rui.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://vui.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://exn.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://eoz.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jgj.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://xnh.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://saq.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://raf.zhixingplan.top

JS:   Object.entries(obj)
来源：http://bsg.tian-w.cn

TS:   Object.entries(obj)
来源：http://bwp.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://muw.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lcm.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://xsw.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://qgt.dianchejie.cn

================================================================================
来源：http://bxt.ydjk.org.cn

H. 异常与错误处理
来源：http://bkn.xuanzx.com

================================================================================
来源：http://wuw.xuanzx.com

[H01] try / catch 基础
来源：http://njq.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fxp.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ygp.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hjo.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vnz.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://epo.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ngf.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fqu.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jku.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://zkm.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gkz.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nss.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xqx.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xbz.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wqn.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yae.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ley.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ogo.yvedp.cn

[H03] 主动抛出异常
来源：http://ohl.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://iih.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iwn.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://wvz.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://thb.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gur.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kxu.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qqv.birdmap.top


<!-- 参考信息 -->