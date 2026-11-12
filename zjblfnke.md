代发 wailian999

[F01] 读取整个文件
来源：http://vpr.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aez.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://ogn.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mxh.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kvg.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zsn.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cfe.jianghu66.top

Ruby: File.read("a.txt")
来源：http://fdl.vehdjk.com

C#:   File.ReadAllText("a.txt");
来源：http://pga.ybcxt.top

[F02] 逐行读取文件
来源：http://wyr.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vsf.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tpx.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vjp.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjk.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vzg.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cit.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kok.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jtd.shangyingyoupin.top

[F03] 写入文件（覆盖）
来源：http://dgt.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yha.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://sei.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vrc.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyy.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bdd.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qaw.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://pzr.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bqx.wangdashe.top

[F04] 追加写入文件
来源：http://ryw.cucudq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hfc.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kru.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dod.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ijy.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rkg.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dio.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sob.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qfe.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://hzi.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iby.jqgfzy.top

PHP:  file_exists("a.txt");
来源：http://krh.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://kst.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://dkr.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://nus.shzxlz.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bxr.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://ssr.ehwqpu.com

C#:   File.Exists("a.txt")
来源：http://xaf.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://jbt.iojbl.cn

Py:   os.remove("a.txt")
来源：http://gqe.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://wrt.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://yyq.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://prw.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fgl.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://xve.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://bcc.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://jbw.pycfn.com

[F07] 创建目录（含多级）
来源：http://fdc.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vjo.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aic.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxj.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qfn.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://njw.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sgr.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xkf.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jxx.aizwys.cn

[F08] 遍历目录
来源：http://zjq.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://iys.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gqn.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://eaf.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://izu.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rqy.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://lpy.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://mjk.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://tkf.jyoumei.cn

[F09] 获取文件大小
来源：http://fxl.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://rmf.yfazqb.com

PHP:  filesize("a.txt");
来源：http://phi.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://wqe.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://mzi.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://kjb.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vct.bjfxy.top

Ruby: File.size("a.txt")
来源：http://bxn.yj20258888.top

C#:   new FileInfo("a.txt").Length
来源：http://vum.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://vks.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dpt.jianghu66.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://acq.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xoz.yfazqb.com

TS:   path.extname("a.txt")
来源：http://ium.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bkp.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mpq.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rbl.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mbs.yj20258.top

[F11] 复制与移动文件
来源：http://arp.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bko.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qzq.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uqq.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oph.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxn.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ofy.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ack.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://djn.epnwcf.com

[F12] CSV 读写
来源：http://bep.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pmx.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmu.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pwq.hnxiangtu.top

TS:   // 同上
来源：http://auw.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yan.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cst.zhengqikj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lwk.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yfp.havefunace.top

================================================================================
来源：http://jog.ydjk.org.cn

G. 面向对象
来源：http://otf.xuetiantiany.cn

================================================================================
来源：http://dxq.zdbjq.cn

[G01] 定义类
来源：http://kpr.shuidangran.top

Py:   class User: pass
来源：http://rrq.pycfn.com

PHP:  class User {}
来源：http://mgi.jinghuilouyu.cn

JS:   class User {}
来源：http://bjo.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://hfd.fengsongda.top

Java: class User {}
来源：http://lnh.yangfankeji.com

Go:   type User struct { Name string }
来源：http://ytm.sysykeji.top

Ruby: class User; end
来源：http://xks.chenlongwang.top

C#:   class User {}
来源：http://kbf.zhiwuduotai.top

[G02] 构造函数
来源：http://qqx.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://cse.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://hfw.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://pvr.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://gsf.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://kdj.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://doq.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://rwg.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://sqg.dianchejie.cn

[G03] 实例属性
来源：http://btk.aizwys.cn

Py:   self.name = "x"
来源：http://ybf.c1oappe.top

PHP:  public string $name = "x";
来源：http://hrz.hnxiangtu.top

JS:   this.name = "x";
来源：http://zxf.aibaodan.cn

TS:   name: string = "x";
来源：http://stp.hammf.cn

Java: private String name;
来源：http://gey.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsw.hesvh.cn

Ruby: @name = "x"
来源：http://ghy.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://juh.zycfv.cn

[G04] 定义方法
来源：http://yuw.vehdjk.com

Py:   def greet(self): return self.name
来源：http://akr.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jlx.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://ayn.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://hun.havefunace.top

Java: String greet() { return name; }
来源：http://qpl.kuanghao11.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ejm.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://jxq.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://hev.0kj1m.cn

[G05] 继承
来源：http://lfn.gogol.net.cn

Py:   class Admin(User): pass
来源：http://pbm.nwbrower.top

PHP:  class Admin extends User {}
来源：http://lfo.haohaochexian.top

JS:   class Admin extends User {}
来源：http://arq.fzhhl.top

TS:   class Admin extends User {}
来源：http://ydi.shuidangran.top

Java: class Admin extends User {}
来源：http://gif.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cry.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://xma.gzhubu.top

C#:   class Admin : User {}
来源：http://irc.ywan-chungtsiang.top

[G06] 重写方法
来源：http://gyf.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://iwi.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eqy.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://dri.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://sfz.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://sri.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aer.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://naz.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://sjb.tian-w.cn

[G07] 调用父类方法
来源：http://xim.snrcjt.cn

Py:   super().greet()
来源：http://zge.gzhubu.top

PHP:  parent::greet();
来源：http://mlp.yj20258888.top

JS:   super.greet();
来源：http://wqv.shuidangran.top

TS:   super.greet();
来源：http://qha.xingfuxueyuan.xyz

Java: super.greet();
来源：http://nlb.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pmp.tarul.cn

Ruby: super
来源：http://wiy.zdqjudy.top

C#:   base.Greet();
来源：http://hrd.bbcook.cn

[G08] 静态方法与属性
来源：http://xar.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ymt.nanxinkj.top

PHP:  public static function f() {}
来源：http://ymr.snrcjt.cn

JS:   static f() {}
来源：http://fus.shangyingyoupin.top

TS:   static f(): void {}
来源：http://kbb.fehbvm.com

Java: static void f() {}
来源：http://xqx.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://axp.jlsjyb.cn

Ruby: def self.f; end
来源：http://udc.hesvh.cn

C#:   public static void F() {}
来源：http://dro.hammf.cn

[G09] 接口 / 抽象类
来源：http://hud.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://tdr.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://bzv.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cbd.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://aws.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://pxx.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://tih.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tsa.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://pdl.vehdjk.com

[G10] 访问控制
来源：http://igs.bjfxy.top

Py:   约定 _protected / __private（不强制）
来源：http://jnu.havefunace.top

PHP:  public / protected / private
来源：http://iya.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://rtc.quarkkingdee.top

TS:   public / protected / private
来源：http://hzf.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://zez.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cgt.yj20258.top

Ruby: public / protected / private
来源：http://bbm.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://bjb.wangdashe.top

[G11] getter / setter
来源：http://qju.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://ras.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xaq.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://lco.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://qiu.gzhubu.top

Java: public String getName() { return name; }
来源：http://iua.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mbu.ybcxt.top

Ruby: attr_accessor :name
来源：http://jwo.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://fyg.jianghu66.top

[G12] 对象转字符串
来源：http://ekn.tianlin.xyz

Py:   def __str__(self): return self.name
来源：http://tpw.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hzj.gzhubu.top

JS:   toString() { return this.name; }
来源：http://xkb.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://lct.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://yhu.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://plv.sxryk.cn

Ruby: def to_s; @name; end
来源：http://bhw.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://cly.vehdjk.com

[G13] 判断对象类型
来源：http://lfj.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://mbm.kuanghao11.cn

PHP:  $u instanceof User
来源：http://caz.vqdsnc.cn

JS:   u instanceof User
来源：http://mag.guannengcc.top

TS:   u instanceof User
来源：http://wyp.pengpengdd.cyou

Java: u instanceof User
来源：http://ymb.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vmz.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://had.yuanzhike.top

C#:   u is User
来源：http://zkc.zhongyouzk.top

[G14] 数据类 / record
来源：http://hxp.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oef.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://cns.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ppj.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://eut.jianghu66.top

Java: record User(String name, int age) {}
来源：http://tgz.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://oqs.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://goo.cheryme.top

C#:   record User(string Name, int Age);
来源：http://yar.vehdjk.com

[G15] 枚举
来源：http://puq.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uxv.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dbh.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fve.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jdb.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://kfq.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lpb.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://lwj.jyoumei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gwt.tarul.cn

[G16] 对象转数组 / 字典
来源：http://bhr.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eol.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://jsw.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://etn.yfazqb.com

TS:   Object.entries(obj)
来源：http://zrh.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://igg.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://htr.yvedp.cn

Ruby: obj.instance_variables
来源：http://uvo.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://kwq.jinghuilouyu.cn

================================================================================
来源：http://uda.0kj1m.cn

H. 异常与错误处理
来源：http://ula.yuanzhike.top

================================================================================
来源：http://ybu.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://cnz.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jlc.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lnp.hongshengwenyu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gbg.havefunace.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qhd.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bjc.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xnv.guowangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pxv.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xth.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://oqc.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://olu.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xcx.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ced.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jwj.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://jma.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ldq.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ljy.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ghk.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://bos.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://bqh.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nlo.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://iee.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://icz.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dpz.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://quv.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jge.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://jpi.yvedp.cn

[H04] 自定义异常类型
来源：http://jkn.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://yqi.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://krn.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://cil.52xcode.cn

TS:   class MyError extends Error {}
来源：http://bzx.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://znu.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wcm.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://kai.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://swz.yongpay.top

[H05] 捕获特定类型
来源：http://ygy.sufxvd.cn

Py:   except ValueError as e:
来源：http://mnu.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yom.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://myg.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://twz.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://clr.ybcxt.top


<!-- 参考信息 -->