代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rpd.svipenyu.cn

================================================================================
来源：http://vre.ppjwa.cn

F. 文件与目录
来源：http://svn.nanxinkj.top

================================================================================
来源：http://wpl.yuxming.cn

[F01] 读取整个文件
来源：http://mwh.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://but.gogol.net.cn

PHP:  file_get_contents("a.txt");
来源：http://cwq.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zgt.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://whp.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vza.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://itb.shuidangran.top

Ruby: File.read("a.txt")
来源：http://zkw.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://ktf.guowangkeji.top

[F02] 逐行读取文件
来源：http://scd.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ott.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cju.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olj.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uqa.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rsc.tarul.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hlg.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tss.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jwn.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://cun.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ggg.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://enp.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lnv.xinyue.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tqc.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uet.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xxa.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://esd.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lij.iojbl.cn

[F04] 追加写入文件
来源：http://crr.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tpd.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://abd.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ony.shanyushiyangtech.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kkw.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bqc.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hpe.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qrt.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gul.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://ygq.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tow.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://vvh.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://zlb.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://eyw.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://odq.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zix.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://hcd.pycfn.com

C#:   File.Exists("a.txt")
来源：http://qox.ywan-chungtsiang.top

[F06] 删除文件
来源：http://jbd.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://tqg.dashuyun.cn

PHP:  unlink("a.txt");
来源：http://jrb.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://nln.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://cfr.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wgb.guowangkeji.top

Go:   os.Remove("a.txt")
来源：http://tnk.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://znx.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://bcc.zhijiandao.cn

[F07] 创建目录（含多级）
来源：http://rvp.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vky.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gau.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzm.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wlo.cqqwz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kyg.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://och.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kfk.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qop.nanxinkj.top

[F08] 遍历目录
来源：http://tzo.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsy.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ihz.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://odm.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://gai.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://euf.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wue.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://tqm.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://fbu.quarkkingdee.top

[F09] 获取文件大小
来源：http://rkd.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://xrt.iojbl.cn

PHP:  filesize("a.txt");
来源：http://jdp.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://dlu.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://ovy.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://rlq.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xhw.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://tsu.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://dbo.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lcb.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zdc.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yxd.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nks.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://hba.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fwe.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://imp.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qul.zycfv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ext.nanxuanxn.top

[F11] 复制与移动文件
来源：http://lsa.yonumen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rir.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tje.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfl.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcj.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zlv.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://htv.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qwq.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ate.xuetiantiany.cn

[F12] CSV 读写
来源：http://tgi.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ieg.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hmh.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lhr.hywenlv.cn

TS:   // 同上
来源：http://usm.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qeh.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gey.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ycz.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wsm.jqgufenzy.top

================================================================================
来源：http://usd.52xcode.cn

G. 面向对象
来源：http://vbm.daria6918.cn

================================================================================
来源：http://mkr.zdbjq.cn

[G01] 定义类
来源：http://tgd.zhongyouzk.top

Py:   class User: pass
来源：http://isa.yfazqb.com

PHP:  class User {}
来源：http://xph.hfpthk.cn

JS:   class User {}
来源：http://kuf.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://qqv.jlsjyb.cn

Java: class User {}
来源：http://nkk.ctjpmb.com

Go:   type User struct { Name string }
来源：http://dig.hammf.cn

Ruby: class User; end
来源：http://rzp.yuanzhike.top

C#:   class User {}
来源：http://wca.c1oappe.top

[G02] 构造函数
来源：http://dfr.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://vah.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://kje.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://dyz.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://gml.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://sfv.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qoi.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://vax.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://itp.mhx1999.top

[G03] 实例属性
来源：http://fsy.jinqigfzy.top

Py:   self.name = "x"
来源：http://fii.ydjk.org.cn

PHP:  public string $name = "x";
来源：http://tdy.316326.xyz

JS:   this.name = "x";
来源：http://gvy.ydjk.org.cn

TS:   name: string = "x";
来源：http://ecx.fktsv.cn

Java: private String name;
来源：http://xyb.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vww.aibaodan.cn

Ruby: @name = "x"
来源：http://kkq.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://zcj.sxryk.cn

[G04] 定义方法
来源：http://uxi.yongpay.top

Py:   def greet(self): return self.name
来源：http://rxg.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://phs.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://nla.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://pwz.yongpay.top

Java: String greet() { return name; }
来源：http://vai.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://pny.cdnleiting.top

Ruby: def greet; @name; end
来源：http://doq.cheryme.top

C#:   public string Greet() => Name;
来源：http://zib.yfazqb.com

[G05] 继承
来源：http://tma.0kj1m.cn

Py:   class Admin(User): pass
来源：http://try.sysykeji.top

PHP:  class Admin extends User {}
来源：http://aoj.xylfe.cn

JS:   class Admin extends User {}
来源：http://agk.hfpthk.cn

TS:   class Admin extends User {}
来源：http://agh.zycfv.cn

Java: class Admin extends User {}
来源：http://vof.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zrg.redwolf501.top

Ruby: class Admin < User; end
来源：http://dwg.hfpthk.cn

C#:   class Admin : User {}
来源：http://oud.gaohongyu789.top

[G06] 重写方法
来源：http://puw.havefunace.top

Py:   def greet(self): return "admin"
来源：http://rkb.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ufy.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://bds.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://urf.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://vhc.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yww.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://wfy.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://smu.shzxlz.cn

[G07] 调用父类方法
来源：http://scg.vqdsnc.cn

Py:   super().greet()
来源：http://bbn.nwbrower.top

PHP:  parent::greet();
来源：http://lfs.ydzc1.top

JS:   super.greet();
来源：http://hdh.gotoacloud.top

TS:   super.greet();
来源：http://uff.pengpengdd.cyou

Java: super.greet();
来源：http://niq.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oyh.hnxiangtu.top

Ruby: super
来源：http://llh.snrcjt.cn

C#:   base.Greet();
来源：http://qfb.daria6918.cn

[G08] 静态方法与属性
来源：http://lsz.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tvv.nwbrower.top

PHP:  public static function f() {}
来源：http://jlk.aizwys.cn

JS:   static f() {}
来源：http://afh.tian-w.cn

TS:   static f(): void {}
来源：http://sov.gogol.net.cn

Java: static void f() {}
来源：http://ngw.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ofj.yangfankeji.com

Ruby: def self.f; end
来源：http://eqe.redwolf501.top

C#:   public static void F() {}
来源：http://xej.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://ctd.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://nwz.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wxu.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vgp.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://irh.daria6918.cn

Java: interface Shape { double area(); }
来源：http://xkz.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://foj.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rfx.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://dvk.jqgufenzy.top

[G10] 访问控制
来源：http://xeh.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://zzz.hnxiangtu.top

PHP:  public / protected / private
来源：http://tqf.epnwcf.com

JS:   #private 字段；其余公开
来源：http://qjr.bbcook.cn

TS:   public / protected / private
来源：http://kiu.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://ixg.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lcm.zdbjq.cn

Ruby: public / protected / private
来源：http://igz.tianlin.xyz

C#:   public / protected / private / internal
来源：http://ukr.ehwqpu.com

[G11] getter / setter
来源：http://tco.xylfe.cn

Py:   @property 与 @x.setter
来源：http://tad.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://por.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://nko.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://fka.yfazqb.com

Java: public String getName() { return name; }
来源：http://ovf.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://lis.c1oappe.top

Ruby: attr_accessor :name
来源：http://zci.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://rrn.gogol.net.cn

[G12] 对象转字符串
来源：http://mpl.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://kmh.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lzg.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://pho.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://xpe.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://oik.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://uye.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://ojh.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://kea.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://unh.c1oappe.top

Py:   isinstance(u, User)
来源：http://fjv.ydjk.org.cn

PHP:  $u instanceof User
来源：http://haw.hnqzz.top

JS:   u instanceof User
来源：http://vyz.ctjpmb.com

TS:   u instanceof User
来源：http://fvf.yj20258888.top

Java: u instanceof User
来源：http://ccw.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dcl.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://jtt.haohaochexian.top

C#:   u is User
来源：http://cng.svipenyu.cn

[G14] 数据类 / record
来源：http://mrt.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://viu.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://ykd.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://sxr.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://emj.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://uuc.jlsjyb.cn

Go:   type User struct { Name string; Age int }
来源：http://jcj.uphjek.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oxg.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://rxz.zhaomingkeji.xyz

[G15] 枚举
来源：http://cov.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cff.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://fkw.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqw.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbt.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://upi.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qew.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://fwa.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxj.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://pvl.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://awf.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://tim.vehdjk.com

JS:   Object.entries(obj)
来源：http://pnm.cashguo.top

TS:   Object.entries(obj)
来源：http://bge.svipenyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://thh.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sbf.yonumen.top

Ruby: obj.instance_variables
来源：http://mut.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://pir.9152youxi.cn

================================================================================
来源：http://zzt.tianlin.xyz

H. 异常与错误处理
来源：http://cjj.xinyue.icu

================================================================================
来源：http://eky.hysaishi.cn

[H01] try / catch 基础
来源：http://kmj.zhengqikj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ivx.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tfd.gogol.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://azm.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zvm.cdnleiting.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tez.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://feb.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cqt.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dkq.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://fgn.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://lkd.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fmg.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eau.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ayo.nanxinkj.top

Java: try { f(); } finally { cleanup(); }
来源：http://rqn.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wga.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wyr.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://unj.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://uqo.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://lng.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://beo.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://bzh.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://asq.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://glz.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kaf.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oci.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://wpa.zhoulong.xyz

[H04] 自定义异常类型
来源：http://ide.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://sbs.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://fwl.yj20258888.top

JS:   class MyError extends Error {}
来源：http://mor.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://coo.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://aqs.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vuv.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://efk.cashguo.top

C#:   class MyException : Exception {}
来源：http://ern.cdnleiting.top

[H05] 捕获特定类型
来源：http://cuf.sysykeji.top

Py:   except ValueError as e:
来源：http://qbu.cqqwz.cn


<!-- 参考信息 -->