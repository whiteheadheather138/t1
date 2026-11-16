代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://are.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xbc.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wce.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://wsd.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tdl.9152youxi.cn

================================================================================
来源：http://ukc.shanyushiyangtech.top

F. 文件与目录
来源：http://eqq.wangdashe.top

================================================================================
来源：http://mnq.chenzaomai.com

[F01] 读取整个文件
来源：http://eqv.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bah.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://tpe.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qcm.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mft.yuxming.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jxo.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hva.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://sbt.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://soh.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://yoy.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://acg.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ihg.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://keh.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kfb.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pck.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ugl.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lcf.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dhx.pycfn.com

[F03] 写入文件（覆盖）
来源：http://oxi.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cvg.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nka.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqt.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ats.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tpe.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rdp.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://gxk.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lgc.aizwys.cn

[F04] 追加写入文件
来源：http://vqg.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://msc.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cmi.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yvd.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sii.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://svm.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bvy.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ktr.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://slh.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://sje.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qri.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://fip.c1oappe.top

JS:   fs.existsSync("a.txt")
来源：http://naf.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://ifk.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://spt.cashguo.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kyk.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://tsi.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://tnc.ydjk.org.cn

[F06] 删除文件
来源：http://enc.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://uny.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://mbl.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://rlh.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rro.hywenlv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lav.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://aec.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://nxd.uphjek.com

C#:   File.Delete("a.txt");
来源：http://beu.ivvv.top

[F07] 创建目录（含多级）
来源：http://yxa.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oyx.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pkg.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://llr.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofy.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pcw.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mnx.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cen.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jjo.daria6918.cn

[F08] 遍历目录
来源：http://ptn.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sqo.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hhc.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://iod.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://oei.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://msf.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://kfz.ybcxt.top

Ruby: Dir.children("dir")
来源：http://pja.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://cxq.chenjidiqi.icu

[F09] 获取文件大小
来源：http://npr.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://sdd.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://oez.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://hgg.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://ipj.shuidangran.top

Java: Files.size(Path.of("a.txt"))
来源：http://oku.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mlx.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://mad.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://nlm.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://vhe.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ugh.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dsk.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://spq.yongpay.top

TS:   path.extname("a.txt")
来源：http://rmr.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ukr.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uwq.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oja.cheryme.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sha.pycfn.com

[F11] 复制与移动文件
来源：http://gnq.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rzo.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dbb.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pff.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqw.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kgl.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://usg.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rfx.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://aqf.ppjwa.cn

[F12] CSV 读写
来源：http://gfi.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ovy.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dtj.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ukx.sufxvd.cn

TS:   // 同上
来源：http://adj.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pnw.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kre.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kqh.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jxb.pengpengdd.cyou

================================================================================
来源：http://ftp.shangyingyoupin.top

G. 面向对象
来源：http://xcc.ehwqpu.com

================================================================================
来源：http://epo.jiagoushi.top

[G01] 定义类
来源：http://vnu.yonumen.top

Py:   class User: pass
来源：http://dwz.aizwys.cn

PHP:  class User {}
来源：http://lia.gogol.net.cn

JS:   class User {}
来源：http://edi.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://gkq.shangyingyoupin.top

Java: class User {}
来源：http://fer.chenlongwang.top

Go:   type User struct { Name string }
来源：http://ewd.sysykeji.top

Ruby: class User; end
来源：http://mft.yanxiufei.cn

C#:   class User {}
来源：http://fqj.ivvv.top

[G02] 构造函数
来源：http://nyn.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://fhz.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://nim.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://yya.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://psc.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://bnj.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kfi.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://uac.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://tbd.zhiwuduotai.top

[G03] 实例属性
来源：http://fka.bbcook.cn

Py:   self.name = "x"
来源：http://qvk.snrcjt.cn

PHP:  public string $name = "x";
来源：http://lho.gzhubu.top

JS:   this.name = "x";
来源：http://ksy.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://tqr.andypj.xyz

Java: private String name;
来源：http://hgi.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://orp.tarul.cn

Ruby: @name = "x"
来源：http://bzw.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://oyh.zhengqikj.top

[G04] 定义方法
来源：http://fjo.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://xzl.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wsp.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://jck.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://nqh.sufxvd.cn

Java: String greet() { return name; }
来源：http://uxy.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnl.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://qxw.tarul.cn

C#:   public string Greet() => Name;
来源：http://tkb.ppjwa.cn

[G05] 继承
来源：http://xht.yuxming.cn

Py:   class Admin(User): pass
来源：http://wum.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://obh.tanke756.top

JS:   class Admin extends User {}
来源：http://zxx.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://bnw.xuanzx.com

Java: class Admin extends User {}
来源：http://jed.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aar.hfpthk.cn

Ruby: class Admin < User; end
来源：http://oiq.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://ctw.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://cmo.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://tal.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hhi.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://izt.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://qbh.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://wst.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://atw.haohaochexian.top

Ruby: def greet; "admin"; end
来源：http://oii.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://fau.snrcjt.cn

[G07] 调用父类方法
来源：http://gvt.ctjpmb.com

Py:   super().greet()
来源：http://sad.fengsongda.top

PHP:  parent::greet();
来源：http://vyj.fktsv.cn

JS:   super.greet();
来源：http://uwp.ppjwa.cn

TS:   super.greet();
来源：http://rxw.cashguo.top

Java: super.greet();
来源：http://veq.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tdz.tianlin.xyz

Ruby: super
来源：http://kav.xinyue.icu

C#:   base.Greet();
来源：http://lxi.zhixingplan.top

[G08] 静态方法与属性
来源：http://xmc.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ynm.hesvh.cn

PHP:  public static function f() {}
来源：http://bav.zdqjudy.top

JS:   static f() {}
来源：http://him.tianlin.xyz

TS:   static f(): void {}
来源：http://zdg.guannengcc.top

Java: static void f() {}
来源：http://glg.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lnp.yongpay.top

Ruby: def self.f; end
来源：http://eof.yangfankeji.com

C#:   public static void F() {}
来源：http://oaa.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://jxx.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://bxg.pycfn.com

PHP:  interface Shape { public function area(): float; }
来源：http://pbu.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fpj.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://ilp.pycfn.com

Java: interface Shape { double area(); }
来源：http://ikg.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://bgf.zhijiandao.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bbe.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://qzr.hnqzz.top

[G10] 访问控制
来源：http://zbp.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://kjv.ehwqpu.com

PHP:  public / protected / private
来源：http://fwf.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://khp.jinqigfzy.top

TS:   public / protected / private
来源：http://brd.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://vtr.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkb.yuxming.cn

Ruby: public / protected / private
来源：http://vjx.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://jie.jqgufenzy.top

[G11] getter / setter
来源：http://von.jianghu66.top

Py:   @property 与 @x.setter
来源：http://hcp.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ppy.fehbvm.com

JS:   get name() { return this._name; }
来源：http://lcg.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://ujn.52xcode.cn

Java: public String getName() { return name; }
来源：http://ics.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jdz.epnwcf.com

Ruby: attr_accessor :name
来源：http://lbk.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://cic.0kj1m.cn

[G12] 对象转字符串
来源：http://uwu.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://ibr.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wrv.sxryk.cn

JS:   toString() { return this.name; }
来源：http://qzm.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://zhu.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://luf.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://for.pycfn.com

Ruby: def to_s; @name; end
来源：http://qsm.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://hyh.gotoacloud.top

[G13] 判断对象类型
来源：http://twt.tanke756.top

Py:   isinstance(u, User)
来源：http://nhx.cdnleiting.top

PHP:  $u instanceof User
来源：http://wjn.shangyingyoupin.top

JS:   u instanceof User
来源：http://jwe.daxiang520.top

TS:   u instanceof User
来源：http://bhq.nanxuanxn.top

Java: u instanceof User
来源：http://sas.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ovm.tian-w.cn

Ruby: u.is_a?(User)
来源：http://xti.jinqigufen.top

C#:   u is User
来源：http://mgt.mhx1999.top

[G14] 数据类 / record
来源：http://eau.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ztp.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://urw.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://bwj.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://tew.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://vmx.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://deb.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fnp.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://odv.yueranfly.top

[G15] 枚举
来源：http://wau.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vxy.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pya.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pws.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://inp.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://lyv.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yaz.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://taa.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pfq.tanke756.top

[G16] 对象转数组 / 字典
来源：http://aji.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fuq.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://lzf.cucudq.cn

JS:   Object.entries(obj)
来源：http://iua.haohaochexian.top

TS:   Object.entries(obj)
来源：http://nbt.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://urx.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rkt.316326.xyz

Ruby: obj.instance_variables
来源：http://pmg.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://iwr.fengsongda.top

================================================================================
来源：http://kmg.svipenyu.cn

H. 异常与错误处理
来源：http://cme.daria6918.cn

================================================================================
来源：http://lmb.nanxuanxn.top

[H01] try / catch 基础
来源：http://joy.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vmn.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ext.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ymr.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://emn.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lwk.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ptt.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hxi.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sjl.mhx1999.top

[H02] finally / ensure 收尾
来源：http://bun.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ost.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wqm.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vxd.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://hnl.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://hrt.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lfi.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iap.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pxp.aizwys.cn

[H03] 主动抛出异常
来源：http://mea.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://wba.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bwr.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://hrl.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://mac.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xwo.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zop.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jaq.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ywv.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://isf.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://dff.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://phe.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://haq.andypj.xyz

TS:   class MyError extends Error {}
来源：http://pes.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://ggu.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xga.zhengqikj.top


<!-- 参考信息 -->