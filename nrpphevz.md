代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://utd.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://twf.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lzc.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://qve.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hcr.ydjk.org.cn

================================================================================
来源：http://xmn.zhaomingkeji.xyz

F. 文件与目录
来源：http://wtf.yuanzhike.top

================================================================================
来源：http://twc.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://zll.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://flc.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://wsy.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://arw.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ucb.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bxw.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uso.hcnkem.com

Ruby: File.read("a.txt")
来源：http://djq.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://mvw.epnwcf.com

[F02] 逐行读取文件
来源：http://jkm.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fek.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tog.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onr.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://drq.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fwg.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yqs.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rpc.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eln.hammf.cn

[F03] 写入文件（覆盖）
来源：http://ikp.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psi.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tqe.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tmv.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iiq.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://obv.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bxx.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://rsy.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rgb.hywenlv.cn

[F04] 追加写入文件
来源：http://uir.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ucq.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://eos.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wog.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sul.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://snc.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hhq.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://svk.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jew.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://xxl.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://odu.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://hvc.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://kah.guannengcc.top

TS:   fs.existsSync("a.txt")
来源：http://zyi.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://swy.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ffx.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://woq.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://kql.zhijiandao.cn

[F06] 删除文件
来源：http://ylx.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://eqb.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://yxo.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://jlf.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xxo.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xjo.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://bsh.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://vyt.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://bzc.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://zdb.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bql.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qfj.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dok.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bbi.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nwp.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ftc.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xcw.cashguo.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tpe.bbcook.cn

[F08] 遍历目录
来源：http://cao.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sra.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bsn.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://zil.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://uvl.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sin.xingfuxueyuan.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://zps.fktsv.cn

Ruby: Dir.children("dir")
来源：http://laf.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://fyb.sufxvd.cn

[F09] 获取文件大小
来源：http://yuf.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://wme.andypj.xyz

PHP:  filesize("a.txt");
来源：http://czk.haohaochexian.top

JS:   fs.statSync("a.txt").size
来源：http://qpe.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://zuq.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://udv.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qga.yonumen.top

Ruby: File.size("a.txt")
来源：http://vpo.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://vxv.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://hmy.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jjr.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://beo.feifeiyinyue.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uca.vehdjk.com

TS:   path.extname("a.txt")
来源：http://zcc.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vzq.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qpm.wangdashe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://arv.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pji.hfpthk.cn

[F11] 复制与移动文件
来源：http://rjz.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lxe.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fdv.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bhe.jinqigfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kjn.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fkv.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vxg.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://egb.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lml.tarul.cn

[F12] CSV 读写
来源：http://rgz.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qxc.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lki.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijg.yongpay.top

TS:   // 同上
来源：http://ver.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qiu.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://svt.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bzg.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oru.bbcook.cn

================================================================================
来源：http://rpv.feifeiyinyue.top

G. 面向对象
来源：http://fpt.jqgfzy.top

================================================================================
来源：http://yde.yueranfly.top

[G01] 定义类
来源：http://tab.zhixingplan.top

Py:   class User: pass
来源：http://xgf.wangdashe.top

PHP:  class User {}
来源：http://dsd.bbcook.cn

JS:   class User {}
来源：http://iwu.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://qrr.hesvh.cn

Java: class User {}
来源：http://mod.hcnkem.com

Go:   type User struct { Name string }
来源：http://ain.xuanzx.com

Ruby: class User; end
来源：http://mpp.vqdsnc.cn

C#:   class User {}
来源：http://qvo.feifeiyinyue.top

[G02] 构造函数
来源：http://fwj.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zwt.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://rni.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://shf.yj20258888.top

TS:   constructor(public name: string) {}
来源：http://bor.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://wty.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cui.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vjz.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://yqh.hammf.cn

[G03] 实例属性
来源：http://nei.epnwcf.com

Py:   self.name = "x"
来源：http://lpw.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://yoz.andypj.xyz

JS:   this.name = "x";
来源：http://tdu.cheryme.top

TS:   name: string = "x";
来源：http://aeu.zdbjq.cn

Java: private String name;
来源：http://iqd.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pxr.hnqzz.top

Ruby: @name = "x"
来源：http://abr.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://bwx.gogol.net.cn

[G04] 定义方法
来源：http://kqy.smart0.xyz

Py:   def greet(self): return self.name
来源：http://ama.yuxming.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uel.redwolf501.top

JS:   greet() { return this.name; }
来源：http://sik.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://byg.snrcjt.cn

Java: String greet() { return name; }
来源：http://kls.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fao.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://txd.shuidangran.top

C#:   public string Greet() => Name;
来源：http://xuy.jqgufenzy.top

[G05] 继承
来源：http://aom.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://dlp.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://mjd.cheryme.top

JS:   class Admin extends User {}
来源：http://oyk.tianlin.xyz

TS:   class Admin extends User {}
来源：http://jqy.smart0.xyz

Java: class Admin extends User {}
来源：http://zvu.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kjx.hcnkem.com

Ruby: class Admin < User; end
来源：http://jpi.yangfankeji.com

C#:   class Admin : User {}
来源：http://ztv.jlsjyb.cn

[G06] 重写方法
来源：http://pzd.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://ovq.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://emj.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://wtx.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://wdu.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://pml.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cmz.ivvv.top

Ruby: def greet; "admin"; end
来源：http://uwh.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://uot.sxryk.cn

[G07] 调用父类方法
来源：http://cgt.hywenlv.cn

Py:   super().greet()
来源：http://sjw.daria6918.cn

PHP:  parent::greet();
来源：http://bpb.svipenyu.cn

JS:   super.greet();
来源：http://ynq.cqqwz.cn

TS:   super.greet();
来源：http://ett.zhijiandao.cn

Java: super.greet();
来源：http://efs.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mbp.dashuyun.cn

Ruby: super
来源：http://ooo.cheryme.top

C#:   base.Greet();
来源：http://anx.yvedp.cn

[G08] 静态方法与属性
来源：http://oig.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qfm.ivvv.top

PHP:  public static function f() {}
来源：http://dyo.hysaishi.cn

JS:   static f() {}
来源：http://pih.chenjidiqi.icu

TS:   static f(): void {}
来源：http://wgj.yanxiufei.cn

Java: static void f() {}
来源：http://ook.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xse.hnqzz.top

Ruby: def self.f; end
来源：http://hts.ydjk.org.cn

C#:   public static void F() {}
来源：http://ktx.cucudq.cn

[G09] 接口 / 抽象类
来源：http://rsl.hcnkem.com

Py:   from abc import ABC, abstractmethod
来源：http://enq.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gwu.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://guk.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://xfd.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://haf.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://yip.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tab.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://src.fzhhl.top

[G10] 访问控制
来源：http://hmo.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://tvw.yj202588.top

PHP:  public / protected / private
来源：http://nir.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://mcx.zhoulong.xyz

TS:   public / protected / private
来源：http://kpp.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://tde.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iwk.yanxiufei.cn

Ruby: public / protected / private
来源：http://cov.daxiang520.top

C#:   public / protected / private / internal
来源：http://idl.ydzc1.top

[G11] getter / setter
来源：http://jfz.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://btq.fktsv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dtb.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://kpa.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://knj.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://jzu.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jyl.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://gsj.gzhubu.top

C#:   public string Name { get; set; }
来源：http://dkb.daxiang520.top

[G12] 对象转字符串
来源：http://ymx.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://xrm.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jau.aizwys.cn

JS:   toString() { return this.name; }
来源：http://rzt.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://vfh.zhongyouzk.top

Java: @Override public String toString() { return name; }
来源：http://nav.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://syz.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://nhg.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://tik.wangshuangyany.cn

[G13] 判断对象类型
来源：http://ugg.nanxinkj.top

Py:   isinstance(u, User)
来源：http://hgy.mhx1999.top

PHP:  $u instanceof User
来源：http://qbc.shzxlz.cn

JS:   u instanceof User
来源：http://ktq.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://nha.haohaochexian.top

Java: u instanceof User
来源：http://bdp.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kxm.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://uaj.yueranfly.top

C#:   u is User
来源：http://whw.gzhubu.top

[G14] 数据类 / record
来源：http://ngy.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qna.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://pql.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lbs.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://khk.meibo888.top

Java: record User(String name, int age) {}
来源：http://cla.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://zwg.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xah.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://ihf.yj202588.top

[G15] 枚举
来源：http://tfm.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vrr.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wzm.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hcn.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://epq.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://pgv.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvv.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://obq.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tgv.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://usi.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nap.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://brv.jianghu66.top

JS:   Object.entries(obj)
来源：http://hbt.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://ukr.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://szz.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://dsd.gotoacloud.top

Ruby: obj.instance_variables
来源：http://etn.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://hau.ehwqpu.com

================================================================================
来源：http://gox.yvedp.cn

H. 异常与错误处理
来源：http://cxc.wangshuangyany.cn

================================================================================
来源：http://zhj.cashguo.top

[H01] try / catch 基础
来源：http://wgl.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iro.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://off.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kjz.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wfj.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxz.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ozu.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pim.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zky.smart0.xyz

[H02] finally / ensure 收尾
来源：http://qdl.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lwn.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ece.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qcd.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pac.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://hkb.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mio.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://niw.yj20258.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://day.hfpthk.cn

[H03] 主动抛出异常
来源：http://seo.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://ufh.feifeiyinyue.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rzx.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://tbq.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://ese.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qfb.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ijm.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zqi.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://gjd.redwolf501.top

[H04] 自定义异常类型
来源：http://kel.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://mqa.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://xha.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://qql.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://dmi.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://okk.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ten.xziqi.cn


<!-- 参考信息 -->