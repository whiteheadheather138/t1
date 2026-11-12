代发 wailian999

[E22] 字节长度与字符长度
来源：http://xuq.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://arn.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lyv.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rgo.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnq.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cuk.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://raz.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://syk.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bbx.xinyue.icu

================================================================================
来源：http://hbo.bbcook.cn

F. 文件与目录
来源：http://vyu.yuxming.cn

================================================================================
来源：http://lzb.smart0.xyz

[F01] 读取整个文件
来源：http://fkt.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://czo.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://gtk.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qdh.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mcs.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wee.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aqj.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://dwq.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://njo.dianchejie.cn

[F02] 逐行读取文件
来源：http://ynk.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dgc.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dra.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://llg.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dzf.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zao.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dvz.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fge.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nit.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://tja.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qpc.fzhhl.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jbv.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gub.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xsa.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kvh.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mur.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://bbd.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kjb.fzhhl.top

[F04] 追加写入文件
来源：http://ztv.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lts.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ipa.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iup.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zzk.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nvm.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ywk.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ebj.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npc.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://tqt.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bza.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://ryw.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://pkp.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://vez.fktsv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iib.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tfq.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://oab.tanke756.top

C#:   File.Exists("a.txt")
来源：http://yki.pengpengdd.cyou

[F06] 删除文件
来源：http://zcz.yueranfly.top

Py:   os.remove("a.txt")
来源：http://hry.sxryk.cn

PHP:  unlink("a.txt");
来源：http://ukd.yanxiufei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://suf.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://axn.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hgx.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://ulp.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://xjp.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://xlr.meibo888.top

[F07] 创建目录（含多级）
来源：http://cig.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://myd.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pso.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aho.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rev.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://puu.xuanzx.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vbh.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ojk.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xkf.yuanzhike.top

[F08] 遍历目录
来源：http://laz.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpg.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ydy.sweek.top

JS:   fs.readdirSync("dir")
来源：http://zox.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://hep.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://svx.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nqr.fzhhl.top

Ruby: Dir.children("dir")
来源：http://suv.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://atd.jqgfzy.top

[F09] 获取文件大小
来源：http://zhl.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://fxf.52xcode.cn

PHP:  filesize("a.txt");
来源：http://lhy.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://hba.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://qgk.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://dzg.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://moq.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://tlj.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://uvd.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://kwy.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xzy.aibaodan.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esk.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uio.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://ghe.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kct.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dvo.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oqr.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lku.zhixingplan.top

[F11] 复制与移动文件
来源：http://lpb.guannengcc.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pwx.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sad.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://chb.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dra.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kjf.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ppm.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hgg.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kco.sjlbkw.cn

[F12] CSV 读写
来源：http://for.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://adw.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tnr.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jxu.jqgufenzy.top

TS:   // 同上
来源：http://vhy.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tmo.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sfp.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hpk.wangshuangyany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://che.hnxiangtu.top

================================================================================
来源：http://pcu.c1oappe.top

G. 面向对象
来源：http://mau.vehdjk.com

================================================================================
来源：http://nux.zhengqikj.top

[G01] 定义类
来源：http://rtj.daxiang520.top

Py:   class User: pass
来源：http://atz.gaohongyu789.top

PHP:  class User {}
来源：http://ldd.yuxming.cn

JS:   class User {}
来源：http://ect.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://ifw.hongshengwenyu.top

Java: class User {}
来源：http://frv.xylfe.cn

Go:   type User struct { Name string }
来源：http://vyt.zhaomingkeji.xyz

Ruby: class User; end
来源：http://hes.cucudq.cn

C#:   class User {}
来源：http://sdz.ydjk.org.cn

[G02] 构造函数
来源：http://pwg.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://hut.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://yqi.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://xsv.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://tod.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://nlj.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jfb.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://lks.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://xef.dashuyun.cn

[G03] 实例属性
来源：http://hez.hywenlv.cn

Py:   self.name = "x"
来源：http://uvp.dianchejie.cn

PHP:  public string $name = "x";
来源：http://bzm.hfpthk.cn

JS:   this.name = "x";
来源：http://iij.yueranfly.top

TS:   name: string = "x";
来源：http://xpm.jlsjyb.cn

Java: private String name;
来源：http://bsc.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wbq.yj20258888.top

Ruby: @name = "x"
来源：http://orc.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://ebk.zhiwuduotai.top

[G04] 定义方法
来源：http://cme.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://dey.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fmr.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ked.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://wgd.zycfv.cn

Java: String greet() { return name; }
来源：http://znq.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nwb.jqgfzy.top

Ruby: def greet; @name; end
来源：http://lpw.fzhhl.top

C#:   public string Greet() => Name;
来源：http://gou.ywan-chungtsiang.top

[G05] 继承
来源：http://gaj.chenzaomai.com

Py:   class Admin(User): pass
来源：http://xma.ivvv.top

PHP:  class Admin extends User {}
来源：http://yeg.hesvh.cn

JS:   class Admin extends User {}
来源：http://ofa.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://ekq.aizwys.cn

Java: class Admin extends User {}
来源：http://hks.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://urp.svipenyu.cn

Ruby: class Admin < User; end
来源：http://kyh.yfazqb.com

C#:   class Admin : User {}
来源：http://njd.hysaishi.cn

[G06] 重写方法
来源：http://lcy.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://iew.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://feu.pycfn.com

JS:   greet() { return "admin"; }
来源：http://qve.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://omi.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://uik.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xzm.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://uxl.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://jib.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://wfd.sufxvd.cn

Py:   super().greet()
来源：http://yys.hysaishi.cn

PHP:  parent::greet();
来源：http://aex.ppjwa.cn

JS:   super.greet();
来源：http://qtq.guowangkeji.top

TS:   super.greet();
来源：http://rcb.jianghu66.top

Java: super.greet();
来源：http://fhl.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sma.zhixingplan.top

Ruby: super
来源：http://uvw.yonumen.top

C#:   base.Greet();
来源：http://ktc.hnxiangtu.top

[G08] 静态方法与属性
来源：http://vwk.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ltg.tianlin.xyz

PHP:  public static function f() {}
来源：http://huk.smart0.xyz

JS:   static f() {}
来源：http://hxe.wangdashe.top

TS:   static f(): void {}
来源：http://eau.bjfxy.top

Java: static void f() {}
来源：http://vwf.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ssj.hysaishi.cn

Ruby: def self.f; end
来源：http://wsq.havefunace.top

C#:   public static void F() {}
来源：http://ypj.mhx1999.top

[G09] 接口 / 抽象类
来源：http://cxg.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://qbu.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://fbs.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wxv.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://xxz.ydzc1.top

Java: interface Shape { double area(); }
来源：http://xpy.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://ynh.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bgb.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://zpr.daxiang520.top

[G10] 访问控制
来源：http://fqr.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://dus.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://pun.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://zml.iojbl.cn

TS:   public / protected / private
来源：http://qgg.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://bvi.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://nfr.zhiwuduotai.top

Ruby: public / protected / private
来源：http://ijs.zhixingplan.top

C#:   public / protected / private / internal
来源：http://hoy.guannengcc.top

[G11] getter / setter
来源：http://kxv.tarul.cn

Py:   @property 与 @x.setter
来源：http://lod.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gpr.epnwcf.com

JS:   get name() { return this._name; }
来源：http://ktj.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://lkm.xuetiantiany.cn

Java: public String getName() { return name; }
来源：http://wcz.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aln.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://gxe.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://gkq.uphjek.com

[G12] 对象转字符串
来源：http://peb.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://mtu.hywenlv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mhs.yvedp.cn

JS:   toString() { return this.name; }
来源：http://qzu.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://olp.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://uzm.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://jzw.andypj.xyz

Ruby: def to_s; @name; end
来源：http://zve.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://vbg.nwbrower.top

[G13] 判断对象类型
来源：http://owj.redwolf501.top

Py:   isinstance(u, User)
来源：http://jbl.haohaochexian.top

PHP:  $u instanceof User
来源：http://ihx.sweek.top

JS:   u instanceof User
来源：http://qbj.shanyushiyangtech.top

TS:   u instanceof User
来源：http://ijs.pycfn.com

Java: u instanceof User
来源：http://evm.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://psq.zhaomingkeji.xyz

Ruby: u.is_a?(User)
来源：http://qot.feifeiyinyue.top

C#:   u is User
来源：http://smo.cqqwz.cn

[G14] 数据类 / record
来源：http://iel.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lyd.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://cvh.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://vlq.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://tqu.fengsongda.top

Java: record User(String name, int age) {}
来源：http://xrt.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://jwu.xingfuxueyuan.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qfy.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://vwf.wangdashe.top

[G15] 枚举
来源：http://tfh.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://scp.yonumen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vez.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wdm.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://axy.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://igo.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zhq.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://uzh.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://grs.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://vtn.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gxl.yj20258.top

PHP:  get_object_vars($obj);
来源：http://qdd.daria6918.cn

JS:   Object.entries(obj)
来源：http://vkp.zhixingplan.top

TS:   Object.entries(obj)
来源：http://emk.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fmd.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ssu.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://ypb.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ekg.daria6918.cn

================================================================================
来源：http://ssd.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://xyz.tanke756.top

================================================================================
来源：http://tmg.hfpthk.cn

[H01] try / catch 基础
来源：http://oqr.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://chw.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uhh.xingfuxueyuan.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iih.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cpo.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://muz.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iid.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oni.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zaf.sweek.top

[H02] finally / ensure 收尾
来源：http://yth.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vck.guowangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xnt.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://taa.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://clt.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ykx.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://fme.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://svv.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nrm.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://xnc.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://mpk.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zbo.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://zek.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://sex.jqgfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cjn.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gru.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zbf.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://sik.sufxvd.cn

[H04] 自定义异常类型
来源：http://ulv.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://rvs.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://oia.jiagoushi.top


<!-- 参考信息 -->