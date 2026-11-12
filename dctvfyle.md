代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://leo.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wdh.vehdjk.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qnf.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://tje.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sti.yj20258.top

================================================================================
来源：http://vzu.hnqzz.top

F. 文件与目录
来源：http://wzq.yfazqb.com

================================================================================
来源：http://uzc.cashguo.top

[F01] 读取整个文件
来源：http://vas.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qqm.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://ptv.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ull.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjg.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cbz.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wcf.316326.xyz

Ruby: File.read("a.txt")
来源：http://coj.feifeiyinyue.top

C#:   File.ReadAllText("a.txt");
来源：http://cvm.zhoulong.xyz

[F02] 逐行读取文件
来源：http://jti.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://okh.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qmm.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://itd.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmw.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zfo.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wuc.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wug.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nsi.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://pbv.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rhp.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kbe.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jid.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zpr.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qhb.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://asp.fanxiaobao.xyz

Ruby: File.write("a.txt", "hi")
来源：http://cip.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ear.zhijiandao.cn

[F04] 追加写入文件
来源：http://lod.bjfxy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jcu.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jyp.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fha.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oij.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zcd.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dty.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xrc.cashguo.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mog.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://txv.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tnh.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://vyx.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://lfp.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://oga.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://osu.yongpay.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xyj.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://xam.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://vei.zhixingplan.top

[F06] 删除文件
来源：http://nbz.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://pga.mhx1999.top

PHP:  unlink("a.txt");
来源：http://cjk.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://kwl.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://ctg.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dfx.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://byj.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://ves.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://vgd.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://xcl.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tdn.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mwb.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ytq.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ujc.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oca.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eqb.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yoq.yuanzhike.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sdg.jqgufenzy.top

[F08] 遍历目录
来源：http://xzt.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hrq.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cye.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://unj.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://jzp.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fog.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://olj.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://frq.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://qmp.pengpengdd.cyou

[F09] 获取文件大小
来源：http://ldw.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://oct.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://fra.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://zmm.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://ijv.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://jwx.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kve.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://wql.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://vka.meibo888.top

[F10] 取文件扩展名 / 文件名
来源：http://xaf.aizwys.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cas.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://enf.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tix.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://iyt.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://knh.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ves.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gcy.redwolf501.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vfp.sjlbkw.cn

[F11] 复制与移动文件
来源：http://rgn.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qem.epnwcf.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kic.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jto.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vvn.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jcf.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qbw.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gpf.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gta.xziqi.cn

[F12] CSV 读写
来源：http://ane.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fcj.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nnr.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dhc.sufxvd.cn

TS:   // 同上
来源：http://glj.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fin.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://omz.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qwy.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://odr.iojbl.cn

================================================================================
来源：http://zdq.aibaodan.cn

G. 面向对象
来源：http://ika.cdnleiting.top

================================================================================
来源：http://jvb.9152youxi.cn

[G01] 定义类
来源：http://nwz.yuanzhike.top

Py:   class User: pass
来源：http://qsd.hnqzz.top

PHP:  class User {}
来源：http://ebk.chenzaomai.com

JS:   class User {}
来源：http://ggi.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://yfs.zhengqikj.top

Java: class User {}
来源：http://osb.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://qzo.cucudq.cn

Ruby: class User; end
来源：http://fqh.uphjek.com

C#:   class User {}
来源：http://ozd.hywenlv.cn

[G02] 构造函数
来源：http://gkr.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://byh.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://fsq.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://hvq.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://phn.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://aur.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gvb.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://sva.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://smj.wangdashe.top

[G03] 实例属性
来源：http://zjd.ydzc1.top

Py:   self.name = "x"
来源：http://dfb.tanke756.top

PHP:  public string $name = "x";
来源：http://erx.jinqigufen.top

JS:   this.name = "x";
来源：http://yva.gaohongyu789.top

TS:   name: string = "x";
来源：http://nhb.jinghuilouyu.cn

Java: private String name;
来源：http://fie.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kox.shzxlz.cn

Ruby: @name = "x"
来源：http://ntt.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://dfw.shzxlz.cn

[G04] 定义方法
来源：http://ngz.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://xvw.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eaf.guannengcc.top

JS:   greet() { return this.name; }
来源：http://knc.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://kfd.aizwys.cn

Java: String greet() { return name; }
来源：http://odl.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kvl.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://bfg.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://zet.chenlongwang.top

[G05] 继承
来源：http://rro.yj20258888.top

Py:   class Admin(User): pass
来源：http://yyu.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://xro.haohaochexian.top

JS:   class Admin extends User {}
来源：http://tqp.tarul.cn

TS:   class Admin extends User {}
来源：http://bxh.shzxlz.cn

Java: class Admin extends User {}
来源：http://xov.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rlk.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://sww.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://fsx.hywenlv.cn

[G06] 重写方法
来源：http://clh.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://mze.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xwe.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://snr.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://ewr.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://ewn.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uhf.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://lti.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://xcu.hesvh.cn

[G07] 调用父类方法
来源：http://tnr.yfazqb.com

Py:   super().greet()
来源：http://sdl.daria6918.cn

PHP:  parent::greet();
来源：http://qii.zhixingplan.top

JS:   super.greet();
来源：http://mdz.hnxiangtu.top

TS:   super.greet();
来源：http://paj.gzhubu.top

Java: super.greet();
来源：http://xzk.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oin.yonumen.top

Ruby: super
来源：http://ylf.daria6918.cn

C#:   base.Greet();
来源：http://fla.sysykeji.top

[G08] 静态方法与属性
来源：http://oyn.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hzi.redwolf501.top

PHP:  public static function f() {}
来源：http://hqz.jqgufenzy.top

JS:   static f() {}
来源：http://zua.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://ljp.tanke756.top

Java: static void f() {}
来源：http://yoo.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kfv.xylfe.cn

Ruby: def self.f; end
来源：http://iuq.yongpay.top

C#:   public static void F() {}
来源：http://gyl.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://lvd.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://ium.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mzy.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yyx.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://elp.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://jag.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://sqs.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xgp.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://uml.hesvh.cn

[G10] 访问控制
来源：http://cax.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://zkm.c1oappe.top

PHP:  public / protected / private
来源：http://ank.vehdjk.com

JS:   #private 字段；其余公开
来源：http://tek.zhijiandao.cn

TS:   public / protected / private
来源：http://cit.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://gek.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rdv.yj20258.top

Ruby: public / protected / private
来源：http://sdz.ctjpmb.com

C#:   public / protected / private / internal
来源：http://oml.cdnleiting.top

[G11] getter / setter
来源：http://phx.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://sjm.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cfb.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://fgl.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://hsa.mhx1999.top

Java: public String getName() { return name; }
来源：http://ivl.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://vfp.shzxlz.cn

Ruby: attr_accessor :name
来源：http://bnu.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://ocu.0kj1m.cn

[G12] 对象转字符串
来源：http://mje.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://crc.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vkv.yfazqb.com

JS:   toString() { return this.name; }
来源：http://mru.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://myg.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://zcf.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ayr.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://pjz.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://wnq.feifeiyinyue.top

[G13] 判断对象类型
来源：http://wzr.hfpthk.cn

Py:   isinstance(u, User)
来源：http://tzn.jqgufenzy.top

PHP:  $u instanceof User
来源：http://thz.9152youxi.cn

JS:   u instanceof User
来源：http://qiy.sxryk.cn

TS:   u instanceof User
来源：http://rwv.kuanghao11.cn

Java: u instanceof User
来源：http://hmp.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xhf.sxryk.cn

Ruby: u.is_a?(User)
来源：http://vhw.smart0.xyz

C#:   u is User
来源：http://epr.yfazqb.com

[G14] 数据类 / record
来源：http://ypp.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hwp.cdnleiting.top

PHP:  // 用 readonly 属性模拟
来源：http://vtu.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://zta.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://axn.0kj1m.cn

Java: record User(String name, int age) {}
来源：http://nzn.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://wfv.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://avz.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://lwd.hfpthk.cn

[G15] 枚举
来源：http://qxz.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utj.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xpa.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ozz.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gxs.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://eil.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xtz.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://ris.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wdw.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://vnl.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://icl.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://hih.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://nfo.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://rtn.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://trn.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mrl.bjfxy.top

Ruby: obj.instance_variables
来源：http://hhy.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://rek.xylfe.cn

================================================================================
来源：http://wck.cqqwz.cn

H. 异常与错误处理
来源：http://ydd.fanxiaobao.xyz

================================================================================
来源：http://ytb.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://fmw.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://icx.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hfp.chenzaomai.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pyu.jlsjyb.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cnv.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xge.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wmr.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eyn.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gja.yj20258.top

[H02] finally / ensure 收尾
来源：http://ibv.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yec.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ywh.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rpb.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://brr.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://hxq.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cxo.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cfp.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gpi.ydjk.org.cn

[H03] 主动抛出异常
来源：http://khr.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://bri.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fgs.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://zqf.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://dco.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bxx.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uwq.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ndj.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://ese.xylfe.cn

[H04] 自定义异常类型
来源：http://qjc.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://qcw.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://qzl.jianghu66.top

JS:   class MyError extends Error {}
来源：http://rpl.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://wdx.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://yma.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ohc.9152youxi.cn


<!-- 参考信息 -->