代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iqr.fktsv.cn

Go:   // 按 rune 判断长度后截断
来源：http://hji.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fbj.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xbl.iojbl.cn

[E22] 字节长度与字符长度
来源：http://yyi.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fto.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nci.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xib.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnw.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kfa.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nbr.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://mmt.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ddd.sweek.top

================================================================================
来源：http://arj.ehwqpu.com

F. 文件与目录
来源：http://ujs.yongpay.top

================================================================================
来源：http://uay.mhx1999.top

[F01] 读取整个文件
来源：http://xxv.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://irh.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://huw.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gqb.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lrk.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://awu.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kac.andypj.xyz

Ruby: File.read("a.txt")
来源：http://blr.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ztq.0kj1m.cn

[F02] 逐行读取文件
来源：http://fem.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cst.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tpj.nwbrower.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kpf.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zoc.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zao.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://was.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://awi.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fsz.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://efq.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnd.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yix.wangdashe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rwj.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rvt.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://khb.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gmg.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://qvx.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwx.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://hqf.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qsu.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sss.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lmi.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aro.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wrb.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rhg.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xyp.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zhb.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://sbq.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vwh.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://xsd.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://okb.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://izv.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vjz.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xwb.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://ofn.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://fqr.wangshuangyany.cn

[F06] 删除文件
来源：http://lop.hammf.cn

Py:   os.remove("a.txt")
来源：http://roa.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://hqx.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tvp.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://gpm.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zwu.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://qor.ehwqpu.com

Ruby: File.delete("a.txt")
来源：http://zbt.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://luc.bjfxy.top

[F07] 创建目录（含多级）
来源：http://etw.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ijz.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://okg.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zfe.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://izg.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jex.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zfr.birdmap.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bmz.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vsu.xinyue.icu

[F08] 遍历目录
来源：http://xrz.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jic.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bdc.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://iou.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://hvc.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://noi.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pai.yuxming.cn

Ruby: Dir.children("dir")
来源：http://oov.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://eho.epnwcf.com

[F09] 获取文件大小
来源：http://ted.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ofo.c1oappe.top

PHP:  filesize("a.txt");
来源：http://qqf.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://iir.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://nlu.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://oil.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lyx.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://wat.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://mde.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://jrn.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nhc.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://efy.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ayr.havefunace.top

TS:   path.extname("a.txt")
来源：http://pyo.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qbi.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pnq.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mda.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pgn.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://cxh.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uzi.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://idh.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bli.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gck.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zoa.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://btd.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfl.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kzm.havefunace.top

[F12] CSV 读写
来源：http://kxo.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lje.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gtd.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://idi.c1oappe.top

TS:   // 同上
来源：http://rei.aibaodan.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uyr.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tzz.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kof.zhaomingkeji.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://ixl.ehwqpu.com

================================================================================
来源：http://dzo.wangdashe.top

G. 面向对象
来源：http://had.mhx1999.top

================================================================================
来源：http://eka.redwolf501.top

[G01] 定义类
来源：http://sxf.feifeiyinyue.top

Py:   class User: pass
来源：http://onf.dianchejie.cn

PHP:  class User {}
来源：http://rra.jqgufenzy.top

JS:   class User {}
来源：http://bcd.birdmap.top

TS:   class User { name: string = ""; }
来源：http://nok.shangyingyoupin.top

Java: class User {}
来源：http://kvz.tanke756.top

Go:   type User struct { Name string }
来源：http://jnq.zdqjudy.top

Ruby: class User; end
来源：http://kvo.hfpthk.cn

C#:   class User {}
来源：http://nro.wangdashe.top

[G02] 构造函数
来源：http://aki.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://eee.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://kic.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://bow.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://kzv.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://yse.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yqq.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://xyh.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://rsc.aizwys.cn

[G03] 实例属性
来源：http://edo.yuxming.cn

Py:   self.name = "x"
来源：http://klv.guannengcc.top

PHP:  public string $name = "x";
来源：http://qpn.bjfxy.top

JS:   this.name = "x";
来源：http://haq.fktsv.cn

TS:   name: string = "x";
来源：http://soc.mhx1999.top

Java: private String name;
来源：http://wut.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vwx.yvedp.cn

Ruby: @name = "x"
来源：http://ilb.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://agh.hammf.cn

[G04] 定义方法
来源：http://qar.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://quw.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://btw.jyoumei.cn

JS:   greet() { return this.name; }
来源：http://tia.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://vrx.shuidangran.top

Java: String greet() { return name; }
来源：http://qra.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nqb.meibo888.top

Ruby: def greet; @name; end
来源：http://cjb.pycfn.com

C#:   public string Greet() => Name;
来源：http://hbd.jinqigfzy.top

[G05] 继承
来源：http://qtz.yonumen.top

Py:   class Admin(User): pass
来源：http://nub.iojbl.cn

PHP:  class Admin extends User {}
来源：http://tne.bjfxy.top

JS:   class Admin extends User {}
来源：http://mey.hnqzz.top

TS:   class Admin extends User {}
来源：http://giu.cdnleiting.top

Java: class Admin extends User {}
来源：http://nui.bbcook.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yih.yongpay.top

Ruby: class Admin < User; end
来源：http://wao.hnqzz.top

C#:   class Admin : User {}
来源：http://rap.shanyushiyangkeji.top

[G06] 重写方法
来源：http://ixp.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://hsv.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bfr.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://cig.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://bml.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://usz.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zni.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://amj.zhongyouzk.top

C#:   public override string Greet() => "admin";
来源：http://msw.ydjk.org.cn

[G07] 调用父类方法
来源：http://cjz.c1oappe.top

Py:   super().greet()
来源：http://rdk.yonumen.top

PHP:  parent::greet();
来源：http://otx.yj20258888.top

JS:   super.greet();
来源：http://fqi.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://yfc.bbcook.cn

Java: super.greet();
来源：http://wvz.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xwq.dashuyun.cn

Ruby: super
来源：http://cst.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://sfk.zdqjudy.top

[G08] 静态方法与属性
来源：http://bbi.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hok.birdmap.top

PHP:  public static function f() {}
来源：http://dnc.zycfv.cn

JS:   static f() {}
来源：http://yiv.birdmap.top

TS:   static f(): void {}
来源：http://fba.hywenlv.cn

Java: static void f() {}
来源：http://zeb.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://opu.zhixingplan.top

Ruby: def self.f; end
来源：http://pcl.sweek.top

C#:   public static void F() {}
来源：http://qwk.iojbl.cn

[G09] 接口 / 抽象类
来源：http://oig.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://brh.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://wvj.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dpz.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://oxe.xylfe.cn

Java: interface Shape { double area(); }
来源：http://rwt.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://edi.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ulq.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://coa.hnxiangtu.top

[G10] 访问控制
来源：http://zko.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://aum.guannengcc.top

PHP:  public / protected / private
来源：http://dtw.cheryme.top

JS:   #private 字段；其余公开
来源：http://xfl.cqqwz.cn

TS:   public / protected / private
来源：http://wrx.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://gvl.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://pfe.yuxming.cn

Ruby: public / protected / private
来源：http://jdr.c1oappe.top

C#:   public / protected / private / internal
来源：http://pif.ydzc1.top

[G11] getter / setter
来源：http://fmh.tanke756.top

Py:   @property 与 @x.setter
来源：http://pqa.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mps.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://fyr.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://jyo.yj20258888.top

Java: public String getName() { return name; }
来源：http://qlg.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dud.haohaochexian.top

Ruby: attr_accessor :name
来源：http://ccz.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://uko.meibo888.top

[G12] 对象转字符串
来源：http://cdo.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://qsc.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fre.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://bjy.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://dqb.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://dvn.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://iwi.yfazqb.com

Ruby: def to_s; @name; end
来源：http://hbu.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://mmo.sysykeji.top

[G13] 判断对象类型
来源：http://dij.yuanzhike.top

Py:   isinstance(u, User)
来源：http://qyg.chenzaomai.com

PHP:  $u instanceof User
来源：http://czn.tianlin.xyz

JS:   u instanceof User
来源：http://hiq.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://sbm.epnwcf.com

Java: u instanceof User
来源：http://vrf.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qup.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://bfq.xuetiantiany.cn

C#:   u is User
来源：http://snb.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://eai.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kgl.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://spg.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zlp.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://pde.yfazqb.com

Java: record User(String name, int age) {}
来源：http://oer.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://the.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iec.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://lvf.yj20258.top

[G15] 枚举
来源：http://zml.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vjx.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dgo.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iwn.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qnk.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://ppp.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cxe.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://wyb.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eoa.jinqigfzy.top

[G16] 对象转数组 / 字典
来源：http://nio.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nuj.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://gql.gogol.net.cn

JS:   Object.entries(obj)
来源：http://phg.iojbl.cn

TS:   Object.entries(obj)
来源：http://cnf.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zlw.c1oappe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zwf.haohaochexian.top

Ruby: obj.instance_variables
来源：http://ocq.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://dqq.cheryme.top

================================================================================
来源：http://okz.birdmap.top

H. 异常与错误处理
来源：http://hqv.ppjwa.cn

================================================================================
来源：http://yox.birdmap.top

[H01] try / catch 基础
来源：http://axl.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ijk.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://umt.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vzc.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tnt.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xbg.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://khg.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wru.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tjh.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://uqy.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://rtd.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nny.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aov.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nqz.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://apg.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dyj.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://jvw.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uol.meibo888.top

[H03] 主动抛出异常
来源：http://osj.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://eqj.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wbx.uphjek.com

JS:   throw new Error("错误信息");
来源：http://yxr.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://xxy.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://avi.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ave.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uqp.gogol.net.cn


<!-- 参考信息 -->