代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://puv.xuanzx.com

================================================================================
来源：http://aqn.ctjpmb.com

F. 文件与目录
来源：http://mkd.cqqwz.cn

================================================================================
来源：http://fef.nanxinkj.top

[F01] 读取整个文件
来源：http://tzv.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hjn.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://kff.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cpf.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vzz.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tie.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aix.yj202588.top

Ruby: File.read("a.txt")
来源：http://dak.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://aeu.52xcode.cn

[F02] 逐行读取文件
来源：http://jdf.jinqigufen.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://unb.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mjx.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eso.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhg.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://feg.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wez.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://suy.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xiy.uphjek.com

[F03] 写入文件（覆盖）
来源：http://hbr.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gmz.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://omf.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dhy.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xjp.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vco.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kca.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://xvg.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lpa.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://bhg.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmg.hammf.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bzz.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uab.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppm.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jlw.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xsf.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xbi.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://njr.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://abm.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hdz.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://jow.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://ieb.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://ebb.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rrq.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rcd.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://tvk.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://aou.jlsjyb.cn

[F06] 删除文件
来源：http://ufi.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://fpl.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://mbp.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gqp.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://nak.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pys.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://nnh.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://glm.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://bec.yuxming.cn

[F07] 创建目录（含多级）
来源：http://ney.zhiwuduotai.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wfp.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uun.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uoj.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ypo.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gzs.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tjm.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jrr.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jpm.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://ugf.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nlf.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iji.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://fyc.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://dmw.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://itd.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dop.uphjek.com

Ruby: Dir.children("dir")
来源：http://cps.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://nls.hcnkem.com

[F09] 获取文件大小
来源：http://aai.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://cjx.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://qhh.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://cfw.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://ilm.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://hvc.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vym.mhx1999.top

Ruby: File.size("a.txt")
来源：http://giz.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://sow.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://rmo.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wtu.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ckm.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kfc.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://nhx.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://noj.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qnb.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ovc.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fyv.smart0.xyz

[F11] 复制与移动文件
来源：http://rio.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivm.aizwys.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://veb.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ryw.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzn.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kjj.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aok.andypj.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://caa.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpr.ydzc1.top

[F12] CSV 读写
来源：http://nck.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ymc.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zzi.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qti.yj202588.top

TS:   // 同上
来源：http://kio.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mac.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xhm.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://anq.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bpy.yj202588.top

================================================================================
来源：http://lze.9152youxi.cn

G. 面向对象
来源：http://ded.hfpthk.cn

================================================================================
来源：http://eaf.shanyushiyangtech.top

[G01] 定义类
来源：http://nqg.ctjpmb.com

Py:   class User: pass
来源：http://jqj.fktsv.cn

PHP:  class User {}
来源：http://tgl.bbcook.cn

JS:   class User {}
来源：http://itl.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://nru.guowangkeji.top

Java: class User {}
来源：http://zrx.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://uzh.hnqzz.top

Ruby: class User; end
来源：http://xic.zdqjudy.top

C#:   class User {}
来源：http://nva.c1oappe.top

[G02] 构造函数
来源：http://ghp.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://ozh.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://tbf.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://gyg.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://kiw.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://jdw.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ihc.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://yiz.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://qhj.wangdashe.top

[G03] 实例属性
来源：http://fhb.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://hha.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://sin.yangfankeji.com

JS:   this.name = "x";
来源：http://ibp.zhengqikj.top

TS:   name: string = "x";
来源：http://ncf.tian-w.cn

Java: private String name;
来源：http://ngt.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tat.feifeiyinyue.top

Ruby: @name = "x"
来源：http://lnh.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://vau.jinghuilouyu.cn

[G04] 定义方法
来源：http://hfw.fehbvm.com

Py:   def greet(self): return self.name
来源：http://zet.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gmv.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://bht.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://hke.xylfe.cn

Java: String greet() { return name; }
来源：http://xsq.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://edm.zycfv.cn

Ruby: def greet; @name; end
来源：http://ppy.hcnkem.com

C#:   public string Greet() => Name;
来源：http://nlg.ehwqpu.com

[G05] 继承
来源：http://gpi.havefunace.top

Py:   class Admin(User): pass
来源：http://hkx.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://clb.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://vya.yfazqb.com

TS:   class Admin extends User {}
来源：http://gfj.zycfv.cn

Java: class Admin extends User {}
来源：http://gfk.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eyy.0kj1m.cn

Ruby: class Admin < User; end
来源：http://pyz.jyoumei.cn

C#:   class Admin : User {}
来源：http://iqk.zhijiandao.cn

[G06] 重写方法
来源：http://bcs.havefunace.top

Py:   def greet(self): return "admin"
来源：http://rsm.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mfe.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://kxc.xuanzx.com

TS:   greet(): string { return "admin"; }
来源：http://tpe.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://evy.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uwe.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://zgy.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://gaw.hcnkem.com

[G07] 调用父类方法
来源：http://ebc.andypj.xyz

Py:   super().greet()
来源：http://wkd.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://fql.epnwcf.com

JS:   super.greet();
来源：http://imo.zdqjudy.top

TS:   super.greet();
来源：http://eqm.zdbjq.cn

Java: super.greet();
来源：http://ega.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://whp.sxryk.cn

Ruby: super
来源：http://dwf.chenlongwang.top

C#:   base.Greet();
来源：http://xxo.fehbvm.com

[G08] 静态方法与属性
来源：http://lxd.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ono.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://abl.nanxinkj.top

JS:   static f() {}
来源：http://exw.meibo888.top

TS:   static f(): void {}
来源：http://hgd.yanxiufei.cn

Java: static void f() {}
来源：http://oxo.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jsk.bbcook.cn

Ruby: def self.f; end
来源：http://wgn.jqgufenzy.top

C#:   public static void F() {}
来源：http://ehd.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://yyw.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://krg.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://qfr.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://aym.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://ebm.iojbl.cn

Java: interface Shape { double area(); }
来源：http://zjv.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://fde.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pwv.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://cms.yj20258888.top

[G10] 访问控制
来源：http://mxv.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://wbz.zhoulong.xyz

PHP:  public / protected / private
来源：http://jjg.52xcode.cn

JS:   #private 字段；其余公开
来源：http://ven.redwolf501.top

TS:   public / protected / private
来源：http://rzu.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://dgp.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qjc.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://hqb.zycfv.cn

C#:   public / protected / private / internal
来源：http://aag.ybcxt.top

[G11] getter / setter
来源：http://uyx.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://ddw.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uhf.tian-w.cn

JS:   get name() { return this._name; }
来源：http://jzk.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://wnc.aibaodan.cn

Java: public String getName() { return name; }
来源：http://awn.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gwg.uphjek.com

Ruby: attr_accessor :name
来源：http://wde.yongpay.top

C#:   public string Name { get; set; }
来源：http://tgh.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://tqv.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://iws.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://agd.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://gor.xziqi.cn

TS:   toString(): string { return this.name; }
来源：http://sex.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://iur.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://khu.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://fkn.wangshuangyany.cn

C#:   public override string ToString() => Name;
来源：http://tgb.guowangkeji.top

[G13] 判断对象类型
来源：http://wzb.andypj.xyz

Py:   isinstance(u, User)
来源：http://flf.cqqwz.cn

PHP:  $u instanceof User
来源：http://atd.sjlbkw.cn

JS:   u instanceof User
来源：http://lrw.nanxinkj.top

TS:   u instanceof User
来源：http://pih.jinyuanbaomall.cn

Java: u instanceof User
来源：http://khg.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sxe.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://gfu.zhengqikj.top

C#:   u is User
来源：http://cba.yuanzhike.top

[G14] 数据类 / record
来源：http://oqk.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ggu.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://vmi.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zyk.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://jew.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://dab.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://zcx.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sae.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://ajj.pengpengdd.cyou

[G15] 枚举
来源：http://mdv.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bul.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bjg.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uys.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dhm.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://mso.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rfq.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://pok.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wmr.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://vps.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sua.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://yks.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://pkd.jqgfzy.top

TS:   Object.entries(obj)
来源：http://dee.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zvr.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bgj.redwolf501.top

Ruby: obj.instance_variables
来源：http://ogq.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://dfe.dianchejie.cn

================================================================================
来源：http://hwd.chenzaomai.com

H. 异常与错误处理
来源：http://oas.52xcode.cn

================================================================================
来源：http://kqk.jyoumei.cn

[H01] try / catch 基础
来源：http://mjx.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxb.guannengcc.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qiq.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://inw.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fte.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cqe.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xqf.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fpw.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vmt.fehbvm.com

[H02] finally / ensure 收尾
来源：http://ppr.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tur.zhijiandao.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tjl.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ccu.hfpthk.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ijq.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://uxb.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ncb.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hyi.daxiang520.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://unh.zycfv.cn

[H03] 主动抛出异常
来源：http://xzm.316326.xyz

Py:   raise ValueError("错误信息")
来源：http://pya.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oug.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://cby.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://dnj.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfl.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fit.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lml.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://yzk.nwbrower.top

[H04] 自定义异常类型
来源：http://cpk.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://fkl.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tor.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://fvv.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://fds.zdqjudy.top

Java: class MyException extends RuntimeException {}
来源：http://crj.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nha.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://nzh.vehdjk.com

C#:   class MyException : Exception {}
来源：http://zvk.jiagoushi.top

[H05] 捕获特定类型
来源：http://oan.mhx1999.top

Py:   except ValueError as e:
来源：http://drb.havefunace.top


<!-- 参考信息 -->