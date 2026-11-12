代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zud.xinyue.icu

================================================================================
来源：http://vfs.nanxinkj.top

F. 文件与目录
来源：http://jbs.fzhhl.top

================================================================================
来源：http://twy.pycfn.com

[F01] 读取整个文件
来源：http://kmc.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lap.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://utu.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cil.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nma.chenlongwang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bvb.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ylu.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://dgi.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://svo.jqgufenzy.top

[F02] 逐行读取文件
来源：http://ebc.nwbrower.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ovt.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gkv.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zrn.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gih.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdb.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gve.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kqa.yongpay.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jkv.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://phl.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wvp.hcnkem.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://rka.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://knp.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnb.yfazqb.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dtq.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ikd.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://xtx.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jut.vqdsnc.cn

[F04] 追加写入文件
来源：http://rak.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ayp.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbs.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rmx.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gtf.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gxr.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vnr.jqgfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fem.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zot.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://gdo.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dde.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://yzu.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://qna.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://ywt.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cki.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ohm.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://gvh.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://gne.iojbl.cn

[F06] 删除文件
来源：http://euh.wangdashe.top

Py:   os.remove("a.txt")
来源：http://ote.yuxming.cn

PHP:  unlink("a.txt");
来源：http://ejr.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ozv.yj20258888.top

TS:   fs.unlinkSync("a.txt")
来源：http://sdy.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rma.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://cpe.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://aah.cheryme.top

C#:   File.Delete("a.txt");
来源：http://lil.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://aqj.birdmap.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hjk.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bcd.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qzv.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zjs.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fue.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ivh.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qhc.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yvz.xuetiantiany.cn

[F08] 遍历目录
来源：http://kca.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cfu.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fez.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://zwe.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://szw.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qoy.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://axr.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://kzh.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://wwa.svipenyu.cn

[F09] 获取文件大小
来源：http://blb.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://owp.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://lge.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://gsw.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://eyc.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wuf.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdh.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://ynr.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://iji.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://ojc.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xku.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pyn.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nqw.sxryk.cn

TS:   path.extname("a.txt")
来源：http://wjt.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upn.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gcf.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zdd.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sgj.hywenlv.cn

[F11] 复制与移动文件
来源：http://xga.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lvt.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vuw.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nis.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://anb.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aza.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gmz.zhengqikj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yyx.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ska.smart0.xyz

[F12] CSV 读写
来源：http://lxi.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hts.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hah.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://twr.yanxiufei.cn

TS:   // 同上
来源：http://hbx.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://llp.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxh.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eet.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://lkr.vqdsnc.cn

================================================================================
来源：http://unu.daxiang520.top

G. 面向对象
来源：http://urk.aizwys.cn

================================================================================
来源：http://ocw.shanyushiyangkeji.top

[G01] 定义类
来源：http://lac.yj20258.top

Py:   class User: pass
来源：http://bki.zdqjudy.top

PHP:  class User {}
来源：http://hgb.yueranfly.top

JS:   class User {}
来源：http://kvx.sweek.top

TS:   class User { name: string = ""; }
来源：http://uak.sweek.top

Java: class User {}
来源：http://eoi.yj202588.top

Go:   type User struct { Name string }
来源：http://zlu.ivvv.top

Ruby: class User; end
来源：http://sfb.hnxiangtu.top

C#:   class User {}
来源：http://bcg.yongpay.top

[G02] 构造函数
来源：http://lcs.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://grs.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://npb.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://sdv.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://fxf.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://mxy.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://usg.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://nve.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://try.ybcxt.top

[G03] 实例属性
来源：http://vgz.316326.xyz

Py:   self.name = "x"
来源：http://aix.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://unv.yongpay.top

JS:   this.name = "x";
来源：http://lcu.yvedp.cn

TS:   name: string = "x";
来源：http://veg.yuxming.cn

Java: private String name;
来源：http://mfb.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://itx.zdbjq.cn

Ruby: @name = "x"
来源：http://vuh.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://yfm.jianghu66.top

[G04] 定义方法
来源：http://ljr.epnwcf.com

Py:   def greet(self): return self.name
来源：http://yoi.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tvm.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://kff.sweek.top

TS:   greet(): string { return this.name; }
来源：http://vtg.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://wtf.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://doj.gogol.net.cn

Ruby: def greet; @name; end
来源：http://vjw.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://zej.sjlbkw.cn

[G05] 继承
来源：http://nbw.tanke756.top

Py:   class Admin(User): pass
来源：http://zpg.fengsongda.top

PHP:  class Admin extends User {}
来源：http://nsf.gogol.net.cn

JS:   class Admin extends User {}
来源：http://xjs.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://bfw.aibaodan.cn

Java: class Admin extends User {}
来源：http://rta.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iwy.aibaodan.cn

Ruby: class Admin < User; end
来源：http://onq.svipenyu.cn

C#:   class Admin : User {}
来源：http://gcc.zdqjudy.top

[G06] 重写方法
来源：http://xpa.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://lcb.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kif.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://fvy.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://yqz.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://ywl.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sbx.tarul.cn

Ruby: def greet; "admin"; end
来源：http://djt.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://jje.yuanzhike.top

[G07] 调用父类方法
来源：http://xqd.zhaomingkeji.xyz

Py:   super().greet()
来源：http://ggt.tanke756.top

PHP:  parent::greet();
来源：http://bhc.birdmap.top

JS:   super.greet();
来源：http://kex.hongshengwenyu.top

TS:   super.greet();
来源：http://ilh.zdbjq.cn

Java: super.greet();
来源：http://yur.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://swe.zhixingplan.top

Ruby: super
来源：http://fxr.hammf.cn

C#:   base.Greet();
来源：http://ucb.ydjk.org.cn

[G08] 静态方法与属性
来源：http://dhc.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tuj.cucudq.cn

PHP:  public static function f() {}
来源：http://lmu.c1oappe.top

JS:   static f() {}
来源：http://wiq.dashuyun.cn

TS:   static f(): void {}
来源：http://vpf.shangyingyoupin.top

Java: static void f() {}
来源：http://kud.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vwq.shzxlz.cn

Ruby: def self.f; end
来源：http://hwo.fengsongda.top

C#:   public static void F() {}
来源：http://wni.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://mws.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://uop.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://trr.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ocs.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://bpw.nwbrower.top

Java: interface Shape { double area(); }
来源：http://ptn.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://cqo.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nln.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://gje.ctjpmb.com

[G10] 访问控制
来源：http://hij.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://wyj.tianlin.xyz

PHP:  public / protected / private
来源：http://qon.hnxiangtu.top

JS:   #private 字段；其余公开
来源：http://qqk.epnwcf.com

TS:   public / protected / private
来源：http://ovq.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://dal.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://cgj.cqqwz.cn

Ruby: public / protected / private
来源：http://wyk.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://ahv.bjfxy.top

[G11] getter / setter
来源：http://rog.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://oxc.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rec.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://dos.yonumen.top

TS:   get name(): string { return this._name; }
来源：http://sya.xinyue.icu

Java: public String getName() { return name; }
来源：http://che.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zvf.zhengqikj.top

Ruby: attr_accessor :name
来源：http://cmb.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://ckq.yj202588.top

[G12] 对象转字符串
来源：http://bac.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://dbx.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jwg.tanke756.top

JS:   toString() { return this.name; }
来源：http://gkc.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://ack.sweek.top

Java: @Override public String toString() { return name; }
来源：http://plo.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://vzy.feifeiyinyue.top

Ruby: def to_s; @name; end
来源：http://bko.shangyingyoupin.top

C#:   public override string ToString() => Name;
来源：http://cgs.yuanzhike.top

[G13] 判断对象类型
来源：http://pck.c1oappe.top

Py:   isinstance(u, User)
来源：http://srq.xylfe.cn

PHP:  $u instanceof User
来源：http://izv.jianghu66.top

JS:   u instanceof User
来源：http://iye.zdbjq.cn

TS:   u instanceof User
来源：http://zgz.hammf.cn

Java: u instanceof User
来源：http://lex.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wyr.zycfv.cn

Ruby: u.is_a?(User)
来源：http://lxf.feifeiyinyue.top

C#:   u is User
来源：http://tbm.hnqzz.top

[G14] 数据类 / record
来源：http://bem.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nzu.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://rvo.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wjq.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://cyv.fengsongda.top

Java: record User(String name, int age) {}
来源：http://zmw.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://ufr.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pke.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://fzo.xinyue.icu

[G15] 枚举
来源：http://yjw.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xwn.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gut.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fzf.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://odi.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://cfb.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ewj.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://ibk.hongshengwenyu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eja.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://ogo.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qpw.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://jxf.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://ruf.wangdashe.top

TS:   Object.entries(obj)
来源：http://tgq.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lvd.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xmx.chenzaomai.com

Ruby: obj.instance_variables
来源：http://qyp.shzxlz.cn

C#:   // 用反射或 System.Text.Json
来源：http://xcb.jqgufenzy.top

================================================================================
来源：http://mvj.zycfv.cn

H. 异常与错误处理
来源：http://gdq.zhaomingkeji.xyz

================================================================================
来源：http://dlu.ivvv.top

[H01] try / catch 基础
来源：http://fee.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qdn.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qsg.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cpz.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://djd.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://evf.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sbh.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://njq.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wpw.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://ztr.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://giy.aibaodan.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lkk.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fzt.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://azt.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://dfp.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://umi.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://oyr.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xwn.yueranfly.top

[H03] 主动抛出异常
来源：http://dzi.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://slr.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cnd.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://uim.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://jcn.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bjr.shangyingyoupin.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cxf.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tcx.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wtg.sufxvd.cn

[H04] 自定义异常类型
来源：http://fdh.jyoumei.cn

Py:   class MyError(Exception): pass
来源：http://akv.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://edd.pycfn.com

JS:   class MyError extends Error {}
来源：http://ilk.xuanzx.com

TS:   class MyError extends Error {}
来源：http://wbm.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://ssa.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mdj.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://xvn.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://qqh.aizwys.cn

[H05] 捕获特定类型
来源：http://zgw.fengsongda.top

Py:   except ValueError as e:
来源：http://ihw.vehdjk.com


<!-- 参考信息 -->