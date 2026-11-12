代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://srv.vqdsnc.cn

================================================================================
来源：http://rhg.9152youxi.cn

F. 文件与目录
来源：http://vzx.snrcjt.cn

================================================================================
来源：http://wcu.zhengqikj.top

[F01] 读取整个文件
来源：http://pxd.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fgv.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://jyp.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bah.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fiy.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nao.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://guw.ybcxt.top

Ruby: File.read("a.txt")
来源：http://iry.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://jtw.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://evg.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gaw.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xpb.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qqj.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xkx.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tni.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rhc.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qbh.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://obt.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://ucv.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gza.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vft.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hkk.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azn.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hme.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tqa.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://xqo.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dzx.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://yiw.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zmy.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mnt.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ysp.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kny.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iua.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ran.jlsjyb.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ite.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vqk.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://cma.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mcc.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://vul.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://zpo.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://yyt.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lsr.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aip.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://tcn.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://sre.svipenyu.cn

[F06] 删除文件
来源：http://meh.tanke756.top

Py:   os.remove("a.txt")
来源：http://nyj.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://uka.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://zub.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://stb.gaohongyu789.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kdv.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://xfp.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://pob.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://hev.tanke756.top

[F07] 创建目录（含多级）
来源：http://joo.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://car.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sdt.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxh.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hok.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uek.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://trn.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kaf.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://prv.tanke756.top

[F08] 遍历目录
来源：http://gan.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsa.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xoy.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://brw.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://zkj.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bab.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jnc.wangdashe.top

Ruby: Dir.children("dir")
来源：http://ipi.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://low.tarul.cn

[F09] 获取文件大小
来源：http://vli.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://ruc.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://vgr.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://sld.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://ofc.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ndj.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wpi.iojbl.cn

Ruby: File.size("a.txt")
来源：http://and.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://jdt.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://jxn.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xds.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cdh.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rkd.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://gbx.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://osv.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uiq.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mlh.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wva.kuanghao11.cn

[F11] 复制与移动文件
来源：http://vtm.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zzy.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zfz.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cvj.fengsongda.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rco.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hen.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ddz.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zon.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bmn.guannengcc.top

[F12] CSV 读写
来源：http://kim.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://roa.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://amd.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vqy.dianchejie.cn

TS:   // 同上
来源：http://guw.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ezq.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nko.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cfi.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yde.zhengqikj.top

================================================================================
来源：http://zjv.tarul.cn

G. 面向对象
来源：http://van.sjlbkw.cn

================================================================================
来源：http://lyd.kuanghao11.cn

[G01] 定义类
来源：http://ffe.sufxvd.cn

Py:   class User: pass
来源：http://kyp.zhiwuduotai.top

PHP:  class User {}
来源：http://dzq.zhiwuduotai.top

JS:   class User {}
来源：http://oun.ydjk.org.cn

TS:   class User { name: string = ""; }
来源：http://neg.kuanghao11.cn

Java: class User {}
来源：http://yve.hnqzz.top

Go:   type User struct { Name string }
来源：http://ufl.birdmap.top

Ruby: class User; end
来源：http://sqg.gzhubu.top

C#:   class User {}
来源：http://zcc.jqgufenzy.top

[G02] 构造函数
来源：http://oel.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://sjm.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://wvj.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://vre.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://atj.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://lhx.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mwo.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://hwb.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://jzb.xziqi.cn

[G03] 实例属性
来源：http://zku.meibo888.top

Py:   self.name = "x"
来源：http://akr.tianlin.xyz

PHP:  public string $name = "x";
来源：http://mrh.fengsongda.top

JS:   this.name = "x";
来源：http://ngd.smart0.xyz

TS:   name: string = "x";
来源：http://ogw.zdqjudy.top

Java: private String name;
来源：http://lyp.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qab.hammf.cn

Ruby: @name = "x"
来源：http://sye.chenzaomai.com

C#:   public string Name { get; set; } = "x";
来源：http://iyb.chenlongwang.top

[G04] 定义方法
来源：http://pdm.hammf.cn

Py:   def greet(self): return self.name
来源：http://tlv.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uqy.ybcxt.top

JS:   greet() { return this.name; }
来源：http://vbk.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://mww.316326.xyz

Java: String greet() { return name; }
来源：http://kyi.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lfx.tarul.cn

Ruby: def greet; @name; end
来源：http://nbn.jqgfzy.top

C#:   public string Greet() => Name;
来源：http://nas.hnqzz.top

[G05] 继承
来源：http://xgn.ybcxt.top

Py:   class Admin(User): pass
来源：http://rld.sxryk.cn

PHP:  class Admin extends User {}
来源：http://eua.cdnleiting.top

JS:   class Admin extends User {}
来源：http://tkf.shzxlz.cn

TS:   class Admin extends User {}
来源：http://arj.zhengqikj.top

Java: class Admin extends User {}
来源：http://qgk.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nrx.xuanzx.com

Ruby: class Admin < User; end
来源：http://duj.gaohongyu789.top

C#:   class Admin : User {}
来源：http://hci.jianghu66.top

[G06] 重写方法
来源：http://xmq.tian-w.cn

Py:   def greet(self): return "admin"
来源：http://icg.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vxm.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://nuz.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://cpw.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://bqp.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iuh.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://okl.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://hbz.pengpengdd.cyou

[G07] 调用父类方法
来源：http://pyl.jiagoushi.top

Py:   super().greet()
来源：http://kzw.gotoacloud.top

PHP:  parent::greet();
来源：http://tul.yueranfly.top

JS:   super.greet();
来源：http://oxo.xylfe.cn

TS:   super.greet();
来源：http://lsk.yj20258888.top

Java: super.greet();
来源：http://ioh.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vcw.cheryme.top

Ruby: super
来源：http://igt.zhiwuduotai.top

C#:   base.Greet();
来源：http://upg.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://pzv.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://grg.0kj1m.cn

PHP:  public static function f() {}
来源：http://wtu.meibo888.top

JS:   static f() {}
来源：http://zxf.hfpthk.cn

TS:   static f(): void {}
来源：http://uhq.fengsongda.top

Java: static void f() {}
来源：http://ppx.yuxming.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujj.pengpengdd.cyou

Ruby: def self.f; end
来源：http://tty.aibaodan.cn

C#:   public static void F() {}
来源：http://ktk.sweek.top

[G09] 接口 / 抽象类
来源：http://hjx.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://grj.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://rfr.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hul.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://lqo.jlsjyb.cn

Java: interface Shape { double area(); }
来源：http://dog.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://aem.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fuu.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://bqi.zdqjudy.top

[G10] 访问控制
来源：http://pnd.svipenyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://tfd.vqdsnc.cn

PHP:  public / protected / private
来源：http://kmh.cheryme.top

JS:   #private 字段；其余公开
来源：http://jdg.zhengqikj.top

TS:   public / protected / private
来源：http://hzc.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://tzh.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://jjw.yuxming.cn

Ruby: public / protected / private
来源：http://xrz.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://noe.guannengcc.top

[G11] getter / setter
来源：http://hhz.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://skq.zycfv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://omc.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://kus.ydzc1.top

TS:   get name(): string { return this._name; }
来源：http://bmc.xuanzx.com

Java: public String getName() { return name; }
来源：http://kju.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ghc.jinqigufen.top

Ruby: attr_accessor :name
来源：http://hna.zycfv.cn

C#:   public string Name { get; set; }
来源：http://jtw.havefunace.top

[G12] 对象转字符串
来源：http://gjb.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://yhp.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lzz.fehbvm.com

JS:   toString() { return this.name; }
来源：http://uxd.zhijiandao.cn

TS:   toString(): string { return this.name; }
来源：http://udt.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://sbx.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://qcj.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://ecb.birdmap.top

C#:   public override string ToString() => Name;
来源：http://ugd.nanxuanxn.top

[G13] 判断对象类型
来源：http://ihu.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://aej.xziqi.cn

PHP:  $u instanceof User
来源：http://feb.meibo888.top

JS:   u instanceof User
来源：http://skp.hfpthk.cn

TS:   u instanceof User
来源：http://ubz.zhixingplan.top

Java: u instanceof User
来源：http://sha.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdr.vehdjk.com

Ruby: u.is_a?(User)
来源：http://szt.quarkkingdee.top

C#:   u is User
来源：http://sdu.aibaodan.cn

[G14] 数据类 / record
来源：http://qjr.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bvi.ivvv.top

PHP:  // 用 readonly 属性模拟
来源：http://wqg.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://moy.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://jwx.fktsv.cn

Java: record User(String name, int age) {}
来源：http://yhg.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://mjh.xinyue.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bsf.bjfxy.top

C#:   record User(string Name, int Age);
来源：http://hpw.havefunace.top

[G15] 枚举
来源：http://brr.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfu.svipenyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mki.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ghv.ydjk.org.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://crp.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://tqg.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://raw.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://hcu.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://odm.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://nzf.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bre.pycfn.com

PHP:  get_object_vars($obj);
来源：http://adc.chenzaomai.com

JS:   Object.entries(obj)
来源：http://jlr.aizwys.cn

TS:   Object.entries(obj)
来源：http://dtd.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ovv.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pxf.shangyingyoupin.top

Ruby: obj.instance_variables
来源：http://mcc.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://rxr.ydzc1.top

================================================================================
来源：http://ydd.hcnkem.com

H. 异常与错误处理
来源：http://awp.wangdashe.top

================================================================================
来源：http://utj.cashguo.top

[H01] try / catch 基础
来源：http://zdg.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://trd.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kru.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ujr.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxk.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aqy.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ffb.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mcp.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oqc.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://kgq.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://llx.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://zmv.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rqm.daria6918.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tkx.sjlbkw.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cfv.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nbi.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rcf.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gaf.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://hzb.0kj1m.cn

Py:   raise ValueError("错误信息")
来源：http://auj.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kyp.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://ghu.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://xzx.gotoacloud.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gln.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xdu.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nle.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://fyq.kuanghao11.cn

[H04] 自定义异常类型
来源：http://vjv.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://rhf.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://diu.tarul.cn

JS:   class MyError extends Error {}
来源：http://mhg.tarul.cn

TS:   class MyError extends Error {}
来源：http://qnt.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://opv.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://znh.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://iux.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://ltx.yvedp.cn

[H05] 捕获特定类型
来源：http://brh.ydzc1.top

Py:   except ValueError as e:
来源：http://tqg.pengpengdd.cyou


<!-- 参考信息 -->