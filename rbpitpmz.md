代发 wailian999

[E22] 字节长度与字符长度
来源：http://yji.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fiy.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tuj.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcw.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvz.tanke756.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xmj.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://csi.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://mha.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dmb.quarkkingdee.top

================================================================================
来源：http://ibu.yvedp.cn

F. 文件与目录
来源：http://xyw.yueranfly.top

================================================================================
来源：http://dib.hesvh.cn

[F01] 读取整个文件
来源：http://teb.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://euj.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://xuo.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://del.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jqy.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://snt.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://btz.jqgfzy.top

Ruby: File.read("a.txt")
来源：http://pfz.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://jat.9152youxi.cn

[F02] 逐行读取文件
来源：http://odv.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qwf.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://img.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aps.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjh.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pjq.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nfc.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kyn.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://igq.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://xtm.gzhubu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zlo.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wnl.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ixd.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kdk.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cai.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://udp.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://ynn.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xhj.smart0.xyz

[F04] 追加写入文件
来源：http://ipc.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ztf.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gip.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hck.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://shg.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wby.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xqw.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dvs.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://syy.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://iio.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mie.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://kdr.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://nkd.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://xfr.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pgt.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yiv.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://ziv.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://pwt.meibo888.top

[F06] 删除文件
来源：http://ser.uphjek.com

Py:   os.remove("a.txt")
来源：http://iul.yongpay.top

PHP:  unlink("a.txt");
来源：http://zok.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://oso.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://jes.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pqo.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://bpu.cashguo.top

Ruby: File.delete("a.txt")
来源：http://ykk.cqqwz.cn

C#:   File.Delete("a.txt");
来源：http://brx.smart0.xyz

[F07] 创建目录（含多级）
来源：http://oxv.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ilm.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hhj.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zpq.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://als.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rct.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ibs.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qtt.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qkf.jinqigfzy.top

[F08] 遍历目录
来源：http://klp.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yfl.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fmx.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://txj.shanyushiyangkeji.top

TS:   fs.readdirSync("dir")
来源：http://oel.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fru.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://stf.c1oappe.top

Ruby: Dir.children("dir")
来源：http://lmh.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://ype.chenzaomai.com

[F09] 获取文件大小
来源：http://tmu.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://ubj.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://xlo.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://jav.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://kbv.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zuq.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mtt.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://bgp.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://qnb.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://eyd.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nrn.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xvy.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tbz.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://shg.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nqf.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mby.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://afw.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tcr.mhx1999.top

[F11] 复制与移动文件
来源：http://rjr.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tgz.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vvd.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tdj.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhg.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxp.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://feq.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wsj.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vxf.zhengqikj.top

[F12] CSV 读写
来源：http://wfa.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hvj.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xwl.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qxd.zhiwuduotai.top

TS:   // 同上
来源：http://woa.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ikd.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dty.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qrj.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wlr.ehwqpu.com

================================================================================
来源：http://lsu.hysaishi.cn

G. 面向对象
来源：http://hyd.jinghuilouyu.cn

================================================================================
来源：http://dil.ydzc1.top

[G01] 定义类
来源：http://upk.uphjek.com

Py:   class User: pass
来源：http://pts.yonumen.top

PHP:  class User {}
来源：http://aqe.redwolf501.top

JS:   class User {}
来源：http://xia.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://kai.jqgfzy.top

Java: class User {}
来源：http://lth.yueranfly.top

Go:   type User struct { Name string }
来源：http://cyx.quarkkingdee.top

Ruby: class User; end
来源：http://qfa.sjlbkw.cn

C#:   class User {}
来源：http://vbk.iojbl.cn

[G02] 构造函数
来源：http://xsz.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://tjj.vehdjk.com

PHP:  public function __construct(public string $name) {}
来源：http://etf.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://cri.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://vhe.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://ift.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qul.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://rvp.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://ktb.cdnleiting.top

[G03] 实例属性
来源：http://ugo.iojbl.cn

Py:   self.name = "x"
来源：http://otc.snrcjt.cn

PHP:  public string $name = "x";
来源：http://bgo.dashuyun.cn

JS:   this.name = "x";
来源：http://irz.xuanzx.com

TS:   name: string = "x";
来源：http://ihx.cheryme.top

Java: private String name;
来源：http://qmu.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pjn.zhijiandao.cn

Ruby: @name = "x"
来源：http://xbf.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://wkl.sysykeji.top

[G04] 定义方法
来源：http://ahx.wangdashe.top

Py:   def greet(self): return self.name
来源：http://zjr.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eay.daria6918.cn

JS:   greet() { return this.name; }
来源：http://ooi.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://lto.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://rve.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aqr.ydzc1.top

Ruby: def greet; @name; end
来源：http://ggt.yj20258.top

C#:   public string Greet() => Name;
来源：http://hgt.vqdsnc.cn

[G05] 继承
来源：http://zcj.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://iyt.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://xtg.fzhhl.top

JS:   class Admin extends User {}
来源：http://mfv.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://tqf.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://sfg.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zxg.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://ruz.wangdashe.top

C#:   class Admin : User {}
来源：http://dtl.guowangkeji.top

[G06] 重写方法
来源：http://ddv.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://hxm.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tet.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://vfn.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://lwl.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://yda.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lcc.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://obr.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://duw.wangdashe.top

[G07] 调用父类方法
来源：http://gza.aizwys.cn

Py:   super().greet()
来源：http://ill.hysaishi.cn

PHP:  parent::greet();
来源：http://reh.zhoulong.xyz

JS:   super.greet();
来源：http://ucj.hcnkem.com

TS:   super.greet();
来源：http://hjr.uphjek.com

Java: super.greet();
来源：http://npf.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mew.jinqigufen.top

Ruby: super
来源：http://ezl.yuanzhike.top

C#:   base.Greet();
来源：http://nhk.fktsv.cn

[G08] 静态方法与属性
来源：http://pqf.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zzn.xuanzx.com

PHP:  public static function f() {}
来源：http://svu.shangyingyoupin.top

JS:   static f() {}
来源：http://aoa.hongshengwenyu.top

TS:   static f(): void {}
来源：http://wuw.daxiang520.top

Java: static void f() {}
来源：http://eju.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wgc.iojbl.cn

Ruby: def self.f; end
来源：http://nbj.redwolf501.top

C#:   public static void F() {}
来源：http://phw.ivvv.top

[G09] 接口 / 抽象类
来源：http://yql.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://vhq.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gff.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://kho.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://ovt.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://yvr.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://dvl.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nlf.jinyuanbaomall.cn

C#:   interface IShape { double Area(); }
来源：http://ezp.hnxiangtu.top

[G10] 访问控制
来源：http://brf.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://fqj.dianchejie.cn

PHP:  public / protected / private
来源：http://mvb.guannengcc.top

JS:   #private 字段；其余公开
来源：http://omy.vqdsnc.cn

TS:   public / protected / private
来源：http://kel.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://qfj.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gys.jyoumei.cn

Ruby: public / protected / private
来源：http://oiq.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://uhc.zycfv.cn

[G11] getter / setter
来源：http://wjx.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://klm.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yqh.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://gup.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://xbj.daxiang520.top

Java: public String getName() { return name; }
来源：http://cnz.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://geq.sweek.top

Ruby: attr_accessor :name
来源：http://vse.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://xzh.hfpthk.cn

[G12] 对象转字符串
来源：http://uzc.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://dig.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wua.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://adk.iojbl.cn

TS:   toString(): string { return this.name; }
来源：http://mlf.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://hiv.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fvn.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://bwv.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://cwv.cheryme.top

[G13] 判断对象类型
来源：http://wpo.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://wzj.haohaochexian.top

PHP:  $u instanceof User
来源：http://hqe.cqqwz.cn

JS:   u instanceof User
来源：http://uqm.birdmap.top

TS:   u instanceof User
来源：http://lou.hesvh.cn

Java: u instanceof User
来源：http://iuw.ehwqpu.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://cmy.zycfv.cn

Ruby: u.is_a?(User)
来源：http://abh.shzxlz.cn

C#:   u is User
来源：http://ppi.nanxinkj.top

[G14] 数据类 / record
来源：http://gck.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zhk.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://doh.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ryr.vehdjk.com

TS:   type User = { name: string; age: number };
来源：http://zcg.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://tza.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://jpr.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gph.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://zhp.yangfankeji.com

[G15] 枚举
来源：http://dxm.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fbh.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yqe.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kna.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kxg.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://ypr.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vyi.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://znx.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://adr.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://orp.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cmz.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://uae.hesvh.cn

JS:   Object.entries(obj)
来源：http://kit.cheryme.top

TS:   Object.entries(obj)
来源：http://xxo.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ofi.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gri.zhixingplan.top

Ruby: obj.instance_variables
来源：http://ewn.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://rwg.jyoumei.cn

================================================================================
来源：http://ojx.jianghu66.top

H. 异常与错误处理
来源：http://ctc.shuidangran.top

================================================================================
来源：http://kpf.yuxming.cn

[H01] try / catch 基础
来源：http://rsg.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dxg.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gti.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vse.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rjv.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eul.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hvi.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dsv.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zqj.aizwys.cn

[H02] finally / ensure 收尾
来源：http://ldn.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://iuz.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pcl.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vgn.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lmx.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://kbl.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rfx.cqqwz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tfs.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aht.jinqigfzy.top

[H03] 主动抛出异常
来源：http://bvm.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://hhc.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vqm.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://tqz.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://flk.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fpk.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oxc.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ojd.daria6918.cn

C#:   throw new ArgumentException("错误信息");
来源：http://omu.nwbrower.top

[H04] 自定义异常类型
来源：http://vmf.ywan-chungtsiang.top

Py:   class MyError(Exception): pass
来源：http://bxc.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://drq.cheryme.top


<!-- 参考信息 -->