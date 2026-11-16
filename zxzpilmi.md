代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kgv.c1oappe.top

================================================================================
来源：http://vsf.nanxuanxn.top

F. 文件与目录
来源：http://rth.redwolf501.top

================================================================================
来源：http://rtv.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://xbz.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xgc.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://bkc.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hiv.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://inv.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ouc.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vgb.zycfv.cn

Ruby: File.read("a.txt")
来源：http://plh.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://lay.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://moz.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pem.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://byu.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://prk.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://abm.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://til.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dnx.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nvl.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vke.tarul.cn

[F03] 写入文件（覆盖）
来源：http://wnt.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tut.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://phe.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ptq.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnq.ydzc1.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jyp.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://olm.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://whq.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iwr.feifeiyinyue.top

[F04] 追加写入文件
来源：http://dhu.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bpn.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ljd.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jus.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ebo.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xbt.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tic.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ful.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://isf.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://way.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yop.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://qlm.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://dmv.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://jlr.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://urj.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uus.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://vkj.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://cmc.daria6918.cn

[F06] 删除文件
来源：http://uou.tarul.cn

Py:   os.remove("a.txt")
来源：http://jnz.52xcode.cn

PHP:  unlink("a.txt");
来源：http://zch.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://kof.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cyb.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kfi.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://hhg.meibo888.top

Ruby: File.delete("a.txt")
来源：http://fhg.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://gfy.zycfv.cn

[F07] 创建目录（含多级）
来源：http://ptj.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tll.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xck.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmr.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rnv.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gst.chenjidiqi.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wcn.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nxx.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ity.zycfv.cn

[F08] 遍历目录
来源：http://juq.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://giq.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sxi.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://zsp.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://wmk.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ute.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rsz.yj20258888.top

Ruby: Dir.children("dir")
来源：http://qxa.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://wek.gzhubu.top

[F09] 获取文件大小
来源：http://eqr.yj202588.top

Py:   os.path.getsize("a.txt")
来源：http://qcl.iojbl.cn

PHP:  filesize("a.txt");
来源：http://xuv.jyoumei.cn

JS:   fs.statSync("a.txt").size
来源：http://gxf.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://ess.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://dnn.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vln.guannengcc.top

Ruby: File.size("a.txt")
来源：http://wip.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qjh.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://mse.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zzj.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ajj.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pyj.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://xgf.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ibl.xziqi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zmq.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://akr.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ril.yvedp.cn

[F11] 复制与移动文件
来源：http://gtv.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oew.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ekx.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zla.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kbu.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://taf.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://utw.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://grm.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ofv.ivvv.top

[F12] CSV 读写
来源：http://swn.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfp.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lzc.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rnx.fehbvm.com

TS:   // 同上
来源：http://rxd.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ind.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://skj.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jgp.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mjv.birdmap.top

================================================================================
来源：http://syl.jiagoushi.top

G. 面向对象
来源：http://nip.nanxinkj.top

================================================================================
来源：http://cdm.zhongyouzk.top

[G01] 定义类
来源：http://rod.smart0.xyz

Py:   class User: pass
来源：http://gco.hammf.cn

PHP:  class User {}
来源：http://mti.yuxming.cn

JS:   class User {}
来源：http://ymw.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://mwu.xuetiantiany.cn

Java: class User {}
来源：http://hio.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://lel.haohaochexian.top

Ruby: class User; end
来源：http://xcd.hfpthk.cn

C#:   class User {}
来源：http://yzr.jlsjyb.cn

[G02] 构造函数
来源：http://dhw.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://thr.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://sqa.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://rcc.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://tzn.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://oef.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bdg.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://dau.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://pzx.tanke756.top

[G03] 实例属性
来源：http://qsv.fzhhl.top

Py:   self.name = "x"
来源：http://vdi.ydzc1.top

PHP:  public string $name = "x";
来源：http://rig.yj202588.top

JS:   this.name = "x";
来源：http://iqk.zycfv.cn

TS:   name: string = "x";
来源：http://hid.hcnkem.com

Java: private String name;
来源：http://oqs.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jik.snrcjt.cn

Ruby: @name = "x"
来源：http://nwl.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://lpf.xuanzx.com

[G04] 定义方法
来源：http://ffj.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://blz.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xtr.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://idp.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://mxg.jinqigufen.top

Java: String greet() { return name; }
来源：http://kij.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://bud.tian-w.cn

Ruby: def greet; @name; end
来源：http://qum.yonumen.top

C#:   public string Greet() => Name;
来源：http://dug.yongpay.top

[G05] 继承
来源：http://pqy.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://ota.yongpay.top

PHP:  class Admin extends User {}
来源：http://cjc.cheryme.top

JS:   class Admin extends User {}
来源：http://yoz.zhengqikj.top

TS:   class Admin extends User {}
来源：http://zth.guowangkeji.top

Java: class Admin extends User {}
来源：http://blz.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wfl.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://suy.zdbjq.cn

C#:   class Admin : User {}
来源：http://icb.fehbvm.com

[G06] 重写方法
来源：http://fpo.tarul.cn

Py:   def greet(self): return "admin"
来源：http://fxc.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ylr.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://ubk.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://ybi.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://qyp.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://man.sxryk.cn

Ruby: def greet; "admin"; end
来源：http://vhu.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://mzq.tanke756.top

[G07] 调用父类方法
来源：http://gut.cashguo.top

Py:   super().greet()
来源：http://umj.xinyue.icu

PHP:  parent::greet();
来源：http://tpt.aizwys.cn

JS:   super.greet();
来源：http://lwl.hammf.cn

TS:   super.greet();
来源：http://kek.gogol.net.cn

Java: super.greet();
来源：http://feb.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bym.hnxiangtu.top

Ruby: super
来源：http://gol.meibo888.top

C#:   base.Greet();
来源：http://uag.shzxlz.cn

[G08] 静态方法与属性
来源：http://lgt.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ojs.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://zpn.zycfv.cn

JS:   static f() {}
来源：http://hko.epnwcf.com

TS:   static f(): void {}
来源：http://qop.gaohongyu789.top

Java: static void f() {}
来源：http://oim.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wjn.wangshuangyany.cn

Ruby: def self.f; end
来源：http://uxm.feifeiyinyue.top

C#:   public static void F() {}
来源：http://xcd.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://mob.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://cje.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kqs.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dgx.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://eio.aizwys.cn

Java: interface Shape { double area(); }
来源：http://btr.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://laa.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwd.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://mvp.vehdjk.com

[G10] 访问控制
来源：http://hxf.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://wpz.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://hek.smart0.xyz

JS:   #private 字段；其余公开
来源：http://vye.cheryme.top

TS:   public / protected / private
来源：http://kcd.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://rxx.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bix.hnxiangtu.top

Ruby: public / protected / private
来源：http://zqk.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://vhc.tanke756.top

[G11] getter / setter
来源：http://pva.uphjek.com

Py:   @property 与 @x.setter
来源：http://obv.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lxa.zhaomingkeji.xyz

JS:   get name() { return this._name; }
来源：http://wwj.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://dgc.daria6918.cn

Java: public String getName() { return name; }
来源：http://vkj.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hcx.yvedp.cn

Ruby: attr_accessor :name
来源：http://xpa.fengsongda.top

C#:   public string Name { get; set; }
来源：http://zpp.mhx1999.top

[G12] 对象转字符串
来源：http://pca.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://unx.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rig.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://kbf.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://eix.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://fmc.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yeo.xuanzx.com

Ruby: def to_s; @name; end
来源：http://dgn.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://mkd.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://qoo.xylfe.cn

Py:   isinstance(u, User)
来源：http://rpz.tianlin.xyz

PHP:  $u instanceof User
来源：http://kys.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://tbm.ehwqpu.com

TS:   u instanceof User
来源：http://gwc.hesvh.cn

Java: u instanceof User
来源：http://zss.andypj.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://mex.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://abt.tianlin.xyz

C#:   u is User
来源：http://apo.pycfn.com

[G14] 数据类 / record
来源：http://flc.hysaishi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://udn.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://mqz.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://eol.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://det.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://pop.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://gmt.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nvb.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://hmt.jinyuanbaomall.cn

[G15] 枚举
来源：http://jtg.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pbw.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ttc.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rzz.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rbi.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://vow.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lpc.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://hcg.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cbc.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://onh.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bbq.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://xhy.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://ebk.epnwcf.com

TS:   Object.entries(obj)
来源：http://ryy.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xwd.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://jmu.fktsv.cn

Ruby: obj.instance_variables
来源：http://imi.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://yem.xuetiantiany.cn

================================================================================
来源：http://eni.nanxinkj.top

H. 异常与错误处理
来源：http://yiq.xylfe.cn

================================================================================
来源：http://ksk.svipenyu.cn

[H01] try / catch 基础
来源：http://ciy.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nfs.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kwc.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xqf.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhu.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://shb.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gwa.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://thr.fktsv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://stc.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://ded.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://avc.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://cwo.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vap.gotoacloud.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gfx.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://hmj.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://mrc.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lwg.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ncb.daria6918.cn

[H03] 主动抛出异常
来源：http://rdb.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://kbw.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kub.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://rps.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://sis.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pfq.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohp.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kqh.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://tjm.yanxiufei.cn

[H04] 自定义异常类型
来源：http://tyr.zhixingplan.top

Py:   class MyError(Exception): pass
来源：http://bkt.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://ytt.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://zeu.hcnkem.com

TS:   class MyError extends Error {}
来源：http://brw.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://abx.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwk.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://cuo.gzhubu.top

C#:   class MyException : Exception {}
来源：http://elq.9152youxi.cn

[H05] 捕获特定类型
来源：http://cij.sysykeji.top

Py:   except ValueError as e:
来源：http://yzh.cashguo.top


<!-- 参考信息 -->