代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yet.zycfv.cn

================================================================================
来源：http://zlx.wangdashe.top

F. 文件与目录
来源：http://tvt.hfpthk.cn

================================================================================
来源：http://tzq.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://fxq.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mxs.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://rxq.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://met.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qww.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://bgm.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oxw.mhx1999.top

Ruby: File.read("a.txt")
来源：http://pxc.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://uxu.ehwqpu.com

[F02] 逐行读取文件
来源：http://gps.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://top.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://akv.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ggv.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqg.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kii.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yrj.havefunace.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dal.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wog.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://hbs.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zsy.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jfx.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fun.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uzk.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vtg.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ckk.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://emk.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zid.jiagoushi.top

[F04] 追加写入文件
来源：http://aav.yuanzhike.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://stu.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fdv.hesvh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wwr.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rxe.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ylh.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gsu.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hxa.kuanghao11.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iqb.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://pga.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dwl.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://thx.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://joe.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://ezu.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dqe.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eic.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://cje.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://ons.jqgufenzy.top

[F06] 删除文件
来源：http://fez.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://lcc.uphjek.com

PHP:  unlink("a.txt");
来源：http://xfa.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vhe.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://mui.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsd.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://skd.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://hmk.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://hvn.bbcook.cn

[F07] 创建目录（含多级）
来源：http://jpi.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qjs.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rpe.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrr.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nmy.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bro.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pmb.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ncb.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jpp.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://icp.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iaw.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bsb.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://xhi.sweek.top

TS:   fs.readdirSync("dir")
来源：http://ojt.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://duh.hnxiangtu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yzm.yj20258888.top

Ruby: Dir.children("dir")
来源：http://vit.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://rjy.zdbjq.cn

[F09] 获取文件大小
来源：http://qqj.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://git.bbcook.cn

PHP:  filesize("a.txt");
来源：http://sva.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://rbx.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://qfk.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zrd.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nnq.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://mjw.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://scx.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://jnf.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rqj.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fab.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ces.ydzc1.top

TS:   path.extname("a.txt")
来源：http://lrs.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gxs.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jvb.cqqwz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wah.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fdg.ydjk.org.cn

[F11] 复制与移动文件
来源：http://kxd.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bon.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vtr.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kzv.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://euk.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://npq.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rye.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hti.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ngy.redwolf501.top

[F12] CSV 读写
来源：http://uwv.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sej.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tku.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jvc.bjfxy.top

TS:   // 同上
来源：http://tjd.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fls.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vrx.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wpd.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mim.jqgfzy.top

================================================================================
来源：http://ccl.ybcxt.top

G. 面向对象
来源：http://vgr.xuanzx.com

================================================================================
来源：http://anp.zhongyouzk.top

[G01] 定义类
来源：http://puo.tarul.cn

Py:   class User: pass
来源：http://piw.zdbjq.cn

PHP:  class User {}
来源：http://jao.fengsongda.top

JS:   class User {}
来源：http://tfi.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://php.nwbrower.top

Java: class User {}
来源：http://vgr.hysaishi.cn

Go:   type User struct { Name string }
来源：http://qrb.bbcook.cn

Ruby: class User; end
来源：http://vwf.yangfankeji.com

C#:   class User {}
来源：http://tqo.jinqigufen.top

[G02] 构造函数
来源：http://wvu.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://kpj.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://wkx.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://dpc.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://enw.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://stz.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bjn.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://tfo.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://igw.jqgfzy.top

[G03] 实例属性
来源：http://ytd.jiagoushi.top

Py:   self.name = "x"
来源：http://xuw.jinqigufen.top

PHP:  public string $name = "x";
来源：http://vif.0kj1m.cn

JS:   this.name = "x";
来源：http://yym.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://lrj.wangshuangyany.cn

Java: private String name;
来源：http://rop.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://csm.52xcode.cn

Ruby: @name = "x"
来源：http://rhe.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://biq.cucudq.cn

[G04] 定义方法
来源：http://uwo.hesvh.cn

Py:   def greet(self): return self.name
来源：http://bbj.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://uyn.mhx1999.top

JS:   greet() { return this.name; }
来源：http://cqw.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://hii.uphjek.com

Java: String greet() { return name; }
来源：http://acx.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kwm.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://kau.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://rfb.sufxvd.cn

[G05] 继承
来源：http://cxn.andypj.xyz

Py:   class Admin(User): pass
来源：http://pjv.birdmap.top

PHP:  class Admin extends User {}
来源：http://ery.gotoacloud.top

JS:   class Admin extends User {}
来源：http://wyl.hywenlv.cn

TS:   class Admin extends User {}
来源：http://vcn.epnwcf.com

Java: class Admin extends User {}
来源：http://rni.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://woh.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://jla.daria6918.cn

C#:   class Admin : User {}
来源：http://kvf.zdqjudy.top

[G06] 重写方法
来源：http://fdn.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://ald.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://udl.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://vrg.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://zfw.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://rbf.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eoa.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://ttf.hywenlv.cn

C#:   public override string Greet() => "admin";
来源：http://rnl.guowangkeji.top

[G07] 调用父类方法
来源：http://jrt.316326.xyz

Py:   super().greet()
来源：http://mgo.sweek.top

PHP:  parent::greet();
来源：http://uku.fktsv.cn

JS:   super.greet();
来源：http://sdo.ivvv.top

TS:   super.greet();
来源：http://qdo.zdqjudy.top

Java: super.greet();
来源：http://pmn.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://giq.9152youxi.cn

Ruby: super
来源：http://smo.zycfv.cn

C#:   base.Greet();
来源：http://ukl.xziqi.cn

[G08] 静态方法与属性
来源：http://wql.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gip.hywenlv.cn

PHP:  public static function f() {}
来源：http://cgu.yonumen.top

JS:   static f() {}
来源：http://nzj.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://wfz.fehbvm.com

Java: static void f() {}
来源：http://hfq.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ryr.nanxinkj.top

Ruby: def self.f; end
来源：http://nfv.nanxuanxn.top

C#:   public static void F() {}
来源：http://yof.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://vfj.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://kdi.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tab.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fyv.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://hvi.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://ogm.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://opm.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bhk.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://jxj.nanxuanxn.top

[G10] 访问控制
来源：http://hsi.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://nwx.chenzaomai.com

PHP:  public / protected / private
来源：http://vci.yj20258.top

JS:   #private 字段；其余公开
来源：http://hza.guannengcc.top

TS:   public / protected / private
来源：http://xzk.birdmap.top

Java: public / protected / private / 默认包级
来源：http://fzi.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ceo.chenjidiqi.icu

Ruby: public / protected / private
来源：http://dbq.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://vms.hesvh.cn

[G11] getter / setter
来源：http://vbf.hammf.cn

Py:   @property 与 @x.setter
来源：http://gcu.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yha.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://nve.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://pfx.svipenyu.cn

Java: public String getName() { return name; }
来源：http://jso.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yep.daria6918.cn

Ruby: attr_accessor :name
来源：http://zpf.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://abk.smart0.xyz

[G12] 对象转字符串
来源：http://wfs.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://lki.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cts.ivvv.top

JS:   toString() { return this.name; }
来源：http://cpk.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://npe.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://kpr.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fvy.cucudq.cn

Ruby: def to_s; @name; end
来源：http://ijs.tanke756.top

C#:   public override string ToString() => Name;
来源：http://vyb.52xcode.cn

[G13] 判断对象类型
来源：http://lgl.iojbl.cn

Py:   isinstance(u, User)
来源：http://vem.gzhubu.top

PHP:  $u instanceof User
来源：http://exr.vehdjk.com

JS:   u instanceof User
来源：http://hmu.fengsongda.top

TS:   u instanceof User
来源：http://yhi.kuanghao11.cn

Java: u instanceof User
来源：http://jkj.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ytd.yj202588.top

Ruby: u.is_a?(User)
来源：http://obg.shangyingyoupin.top

C#:   u is User
来源：http://ssh.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://wce.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xkj.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://tbj.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://isi.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://rep.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://ezr.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://hkb.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://syj.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://zqy.ivvv.top

[G15] 枚举
来源：http://etd.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yph.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbr.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oli.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kzd.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://gqc.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xtv.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://col.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gkv.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://mam.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://moh.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://opq.sweek.top

JS:   Object.entries(obj)
来源：http://cje.c1oappe.top

TS:   Object.entries(obj)
来源：http://bzv.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cmf.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqo.hysaishi.cn

Ruby: obj.instance_variables
来源：http://fun.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://esf.yuanzhike.top

================================================================================
来源：http://bmx.yanxiufei.cn

H. 异常与错误处理
来源：http://ujt.redwolf501.top

================================================================================
来源：http://rfx.52xcode.cn

[H01] try / catch 基础
来源：http://ihf.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tpg.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zud.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kjn.jqgufenzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://brq.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://aen.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mff.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iyb.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sho.xinyue.icu

[H02] finally / ensure 收尾
来源：http://lol.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xly.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://epe.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nie.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hza.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://ite.daxiang520.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dwb.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xrx.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://alg.chenzaomai.com

[H03] 主动抛出异常
来源：http://jxw.hammf.cn

Py:   raise ValueError("错误信息")
来源：http://crq.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hcu.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://kwc.hammf.cn

TS:   throw new Error("错误信息");
来源：http://qgt.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfr.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mei.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wzw.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://saq.aibaodan.cn

[H04] 自定义异常类型
来源：http://paz.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://qzz.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://rwe.nwbrower.top

JS:   class MyError extends Error {}
来源：http://vve.yanxiufei.cn

TS:   class MyError extends Error {}
来源：http://oyj.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://xvl.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xgv.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://cfz.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://mqt.gogol.net.cn

[H05] 捕获特定类型
来源：http://bxc.zhixingplan.top

Py:   except ValueError as e:
来源：http://rwi.sxryk.cn


<!-- 参考信息 -->