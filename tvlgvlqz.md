代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvo.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ecq.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gna.cqqwz.cn

Ruby: s.bytesize;  s.length
来源：http://xyy.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zur.xziqi.cn

================================================================================
来源：http://sjv.snrcjt.cn

F. 文件与目录
来源：http://apk.jlsjyb.cn

================================================================================
来源：http://uyb.9152youxi.cn

[F01] 读取整个文件
来源：http://ftn.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zcf.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://jra.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://htj.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qot.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://avj.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bqm.gaohongyu789.top

Ruby: File.read("a.txt")
来源：http://lju.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://qgk.vqdsnc.cn

[F02] 逐行读取文件
来源：http://cva.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uwp.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czy.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://elt.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nru.jinghuilouyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://usz.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://axq.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ffi.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lew.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://jds.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vqi.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://mbq.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aom.pengpengdd.cyou

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://opd.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xer.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jbp.fengsongda.top

Ruby: File.write("a.txt", "hi")
来源：http://tdn.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yej.shangyingyoupin.top

[F04] 追加写入文件
来源：http://epy.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ukn.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oha.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ywx.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szy.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xon.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uam.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rtt.daxiang520.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pse.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://kif.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vax.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://kxp.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://aav.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://ukm.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wbk.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tcf.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://fdi.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://goc.quarkkingdee.top

[F06] 删除文件
来源：http://toc.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://lzz.yj202588.top

PHP:  unlink("a.txt");
来源：http://stx.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://moq.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://bso.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gzu.birdmap.top

Go:   os.Remove("a.txt")
来源：http://vhi.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://cbw.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://ext.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://ryx.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uhc.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khh.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zje.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cqe.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zmh.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hfr.9152youxi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iiz.shzxlz.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dwj.yangfankeji.com

[F08] 遍历目录
来源：http://gkw.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rau.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kjo.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://ztu.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://wma.tanke756.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tgr.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pie.bjfxy.top

Ruby: Dir.children("dir")
来源：http://sry.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://hnl.daxiang520.top

[F09] 获取文件大小
来源：http://jjp.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://les.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://ehb.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://jmg.hammf.cn

TS:   fs.statSync("a.txt").size
来源：http://wuy.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qbv.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://frp.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://pfz.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://fxd.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ust.jianghu66.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oko.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rtw.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lid.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://hwl.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ryd.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nbk.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jkf.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fmf.fengsongda.top

[F11] 复制与移动文件
来源：http://hqi.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zzq.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qsk.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvy.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jod.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hym.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yen.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zww.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oho.fzhhl.top

[F12] CSV 读写
来源：http://vug.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ckr.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iqt.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ivh.fktsv.cn

TS:   // 同上
来源：http://gcb.meibo888.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rcs.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jgb.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lau.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zzm.ivvv.top

================================================================================
来源：http://yne.aizwys.cn

G. 面向对象
来源：http://ohb.pengpengdd.cyou

================================================================================
来源：http://tiq.zdbjq.cn

[G01] 定义类
来源：http://bmc.zhengqikj.top

Py:   class User: pass
来源：http://pxw.fengsongda.top

PHP:  class User {}
来源：http://hwo.jlsjyb.cn

JS:   class User {}
来源：http://brg.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://aga.iojbl.cn

Java: class User {}
来源：http://vod.fehbvm.com

Go:   type User struct { Name string }
来源：http://cgc.yj20258888.top

Ruby: class User; end
来源：http://mhz.hesvh.cn

C#:   class User {}
来源：http://hzi.andypj.xyz

[G02] 构造函数
来源：http://gsj.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://upc.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://uux.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://zjn.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://zyk.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://rka.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jgp.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://eux.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://zvr.yangfankeji.com

[G03] 实例属性
来源：http://izk.gaohongyu789.top

Py:   self.name = "x"
来源：http://klm.meibo888.top

PHP:  public string $name = "x";
来源：http://pvn.zdbjq.cn

JS:   this.name = "x";
来源：http://imr.xuanzx.com

TS:   name: string = "x";
来源：http://bay.guowangkeji.top

Java: private String name;
来源：http://thq.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qfk.yj202588.top

Ruby: @name = "x"
来源：http://uxb.iojbl.cn

C#:   public string Name { get; set; } = "x";
来源：http://cbm.tarul.cn

[G04] 定义方法
来源：http://vji.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://ppf.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://lxh.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://tfa.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://yys.quarkkingdee.top

Java: String greet() { return name; }
来源：http://zsy.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cfr.bbcook.cn

Ruby: def greet; @name; end
来源：http://roq.ivvv.top

C#:   public string Greet() => Name;
来源：http://hye.ivvv.top

[G05] 继承
来源：http://hre.bbcook.cn

Py:   class Admin(User): pass
来源：http://gxw.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://zvc.tarul.cn

JS:   class Admin extends User {}
来源：http://fev.aibaodan.cn

TS:   class Admin extends User {}
来源：http://apr.dianchejie.cn

Java: class Admin extends User {}
来源：http://lim.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vyb.daria6918.cn

Ruby: class Admin < User; end
来源：http://ixh.yuanzhike.top

C#:   class Admin : User {}
来源：http://nck.andypj.xyz

[G06] 重写方法
来源：http://quk.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://yka.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bps.yj20258.top

JS:   greet() { return "admin"; }
来源：http://evs.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://hcy.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://hdh.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ylb.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://bnr.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://xqk.jqgufenzy.top

[G07] 调用父类方法
来源：http://yaw.gotoacloud.top

Py:   super().greet()
来源：http://lad.gzhubu.top

PHP:  parent::greet();
来源：http://fnx.52xcode.cn

JS:   super.greet();
来源：http://klk.shuidangran.top

TS:   super.greet();
来源：http://xfd.pycfn.com

Java: super.greet();
来源：http://eth.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tbz.wangdashe.top

Ruby: super
来源：http://bdp.nanxinkj.top

C#:   base.Greet();
来源：http://gnx.zdqjudy.top

[G08] 静态方法与属性
来源：http://whe.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbe.nanxinkj.top

PHP:  public static function f() {}
来源：http://tvc.ctjpmb.com

JS:   static f() {}
来源：http://ptc.ydzc1.top

TS:   static f(): void {}
来源：http://ddz.zdbjq.cn

Java: static void f() {}
来源：http://cxr.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xwo.cqqwz.cn

Ruby: def self.f; end
来源：http://jsm.nanxinkj.top

C#:   public static void F() {}
来源：http://rum.iojbl.cn

[G09] 接口 / 抽象类
来源：http://ppj.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://jxx.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rcr.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vjj.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://ucu.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://foj.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://smd.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dur.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://tdf.vehdjk.com

[G10] 访问控制
来源：http://ylu.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://xcs.sysykeji.top

PHP:  public / protected / private
来源：http://lji.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://fdj.gaohongyu789.top

TS:   public / protected / private
来源：http://uuw.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://hyp.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gem.sweek.top

Ruby: public / protected / private
来源：http://bno.tanke756.top

C#:   public / protected / private / internal
来源：http://mkd.0kj1m.cn

[G11] getter / setter
来源：http://zei.yj20258888.top

Py:   @property 与 @x.setter
来源：http://nsw.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ptw.316326.xyz

JS:   get name() { return this._name; }
来源：http://vnu.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://jtc.fengsongda.top

Java: public String getName() { return name; }
来源：http://zfr.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kxs.guannengcc.top

Ruby: attr_accessor :name
来源：http://lbk.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://etq.hammf.cn

[G12] 对象转字符串
来源：http://bsf.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://dhi.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://olq.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://iiz.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://fgw.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://smu.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://naq.yvedp.cn

Ruby: def to_s; @name; end
来源：http://axx.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://cic.tarul.cn

[G13] 判断对象类型
来源：http://etg.bjfxy.top

Py:   isinstance(u, User)
来源：http://hxo.zhoulong.xyz

PHP:  $u instanceof User
来源：http://nog.ctjpmb.com

JS:   u instanceof User
来源：http://bei.sweek.top

TS:   u instanceof User
来源：http://dqr.ctjpmb.com

Java: u instanceof User
来源：http://xay.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rwb.hesvh.cn

Ruby: u.is_a?(User)
来源：http://jzt.jqgfzy.top

C#:   u is User
来源：http://hjs.ybcxt.top

[G14] 数据类 / record
来源：http://nli.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://alv.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://dhm.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://vjg.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://yfl.birdmap.top

Java: record User(String name, int age) {}
来源：http://vtl.yongpay.top

Go:   type User struct { Name string; Age int }
来源：http://cpb.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ycs.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://fii.yonumen.top

[G15] 枚举
来源：http://dnk.ydzc1.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vwq.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://fcx.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sfw.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jnf.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://pol.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hht.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://ssy.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://unr.tarul.cn

[G16] 对象转数组 / 字典
来源：http://nhs.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tlg.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://zks.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://ewx.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://wrk.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aet.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fqx.hesvh.cn

Ruby: obj.instance_variables
来源：http://gsc.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://zdp.daxiang520.top

================================================================================
来源：http://zso.shanyushiyangtech.top

H. 异常与错误处理
来源：http://qzv.316326.xyz

================================================================================
来源：http://yyx.havefunace.top

[H01] try / catch 基础
来源：http://tby.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bfl.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lqf.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tws.pengpengdd.cyou

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://caw.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jzn.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ycf.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dar.pycfn.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://egz.smart0.xyz

[H02] finally / ensure 收尾
来源：http://wfx.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mhs.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nnd.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zye.fktsv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sjp.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://lik.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://ump.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nhp.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zkd.meibo888.top

[H03] 主动抛出异常
来源：http://jiz.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://yvw.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ati.pycfn.com

JS:   throw new Error("错误信息");
来源：http://kkp.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://ayv.wangdashe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cfn.shanyushiyangtech.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ksg.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xji.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://qcl.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://bli.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://gru.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ial.jianghu66.top

JS:   class MyError extends Error {}
来源：http://kml.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://ozn.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://hwq.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tuf.bjfxy.top


<!-- 参考信息 -->