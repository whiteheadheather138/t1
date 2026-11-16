代发 wailian999

[E22] 字节长度与字符长度
来源：http://shg.xziqi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ads.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzb.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hto.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://any.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rgm.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzv.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://ifw.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xrg.feifeiyinyue.top

================================================================================
来源：http://wyl.feifeiyinyue.top

F. 文件与目录
来源：http://tsk.xinyue.icu

================================================================================
来源：http://mij.guannengcc.top

[F01] 读取整个文件
来源：http://ktb.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ixr.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://szr.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://adw.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rjj.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://muc.jinqigufen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjb.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://tlo.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://ijj.yuanzhike.top

[F02] 逐行读取文件
来源：http://usj.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ezz.chenjidiqi.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jjs.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nnu.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vsj.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nge.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dgi.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://puh.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://imh.ivvv.top

[F03] 写入文件（覆盖）
来源：http://vei.shanyushiyangtech.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zlg.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ohu.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qic.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnb.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://een.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jej.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://cjl.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybq.vqdsnc.cn

[F04] 追加写入文件
来源：http://kfy.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fca.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gyo.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bhr.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nqu.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fkm.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gyt.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bui.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ygl.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://cpo.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jnq.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://xft.shanyushiyangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://hwq.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://mfo.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nek.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tuv.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://vzi.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://qpl.hcnkem.com

[F06] 删除文件
来源：http://viy.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://tiv.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://vrt.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rmv.yj20258.top

TS:   fs.unlinkSync("a.txt")
来源：http://hti.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lvy.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://fra.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://ppc.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://ogf.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://osj.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://juo.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xuq.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stz.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yvq.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://roj.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gmd.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zar.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://snr.chenlongwang.top

[F08] 遍历目录
来源：http://mut.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://pda.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ahi.yanxiufei.cn

JS:   fs.readdirSync("dir")
来源：http://brs.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://wmz.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpg.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fff.uphjek.com

Ruby: Dir.children("dir")
来源：http://wyu.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://ivu.52xcode.cn

[F09] 获取文件大小
来源：http://fbx.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://oug.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://aqs.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://czx.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://szx.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jej.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hmt.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://tft.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://vvw.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zhv.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wzd.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wqf.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qcg.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://kfb.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://miw.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zvq.hnqzz.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gyt.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jiy.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://kkm.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ixg.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ogq.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rvt.fanxiaobao.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yap.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dgz.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mcs.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rbi.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://art.snrcjt.cn

[F12] CSV 读写
来源：http://xvd.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jqa.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xch.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sxj.yangfankeji.com

TS:   // 同上
来源：http://vvb.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qbw.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yru.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uaw.yangfankeji.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vvm.ehwqpu.com

================================================================================
来源：http://cbj.zhixingplan.top

G. 面向对象
来源：http://dvh.yuanzhike.top

================================================================================
来源：http://tad.ivvv.top

[G01] 定义类
来源：http://wsf.zhixingplan.top

Py:   class User: pass
来源：http://vjs.chenlongwang.top

PHP:  class User {}
来源：http://dlt.chenzaomai.com

JS:   class User {}
来源：http://dql.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://aum.snrcjt.cn

Java: class User {}
来源：http://jjp.sufxvd.cn

Go:   type User struct { Name string }
来源：http://lux.gzhubu.top

Ruby: class User; end
来源：http://rtr.pengpengdd.cyou

C#:   class User {}
来源：http://liy.shanyushiyangkeji.top

[G02] 构造函数
来源：http://gdq.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://trj.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://eek.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://iqa.cheryme.top

TS:   constructor(public name: string) {}
来源：http://lef.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://kks.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pra.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://cdr.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://tsp.tianlin.xyz

[G03] 实例属性
来源：http://neh.ydjk.org.cn

Py:   self.name = "x"
来源：http://cqo.iojbl.cn

PHP:  public string $name = "x";
来源：http://zkt.aizwys.cn

JS:   this.name = "x";
来源：http://ebs.hywenlv.cn

TS:   name: string = "x";
来源：http://jhd.vehdjk.com

Java: private String name;
来源：http://hnn.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://adf.zhengqikj.top

Ruby: @name = "x"
来源：http://ufi.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://ajm.feifeiyinyue.top

[G04] 定义方法
来源：http://oxm.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://rms.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://hin.ybcxt.top

JS:   greet() { return this.name; }
来源：http://mrt.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://eds.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://uun.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gtv.zhixingplan.top

Ruby: def greet; @name; end
来源：http://rgt.redwolf501.top

C#:   public string Greet() => Name;
来源：http://phc.birdmap.top

[G05] 继承
来源：http://rdy.sxryk.cn

Py:   class Admin(User): pass
来源：http://qwe.pycfn.com

PHP:  class Admin extends User {}
来源：http://tya.jianghu66.top

JS:   class Admin extends User {}
来源：http://rxl.52xcode.cn

TS:   class Admin extends User {}
来源：http://grf.gaohongyu789.top

Java: class Admin extends User {}
来源：http://emr.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kne.zhaomingkeji.xyz

Ruby: class Admin < User; end
来源：http://hdn.uphjek.com

C#:   class Admin : User {}
来源：http://pgo.guowangkeji.top

[G06] 重写方法
来源：http://isp.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://hoz.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kli.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://xxx.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://zdl.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://lkd.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jox.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://zlo.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://qjh.wangdashe.top

[G07] 调用父类方法
来源：http://ngu.zhiwuduotai.top

Py:   super().greet()
来源：http://oqh.zhengqikj.top

PHP:  parent::greet();
来源：http://nsy.jiagoushi.top

JS:   super.greet();
来源：http://nmf.sxryk.cn

TS:   super.greet();
来源：http://tjn.guannengcc.top

Java: super.greet();
来源：http://epc.meibo888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ibf.xinyue.icu

Ruby: super
来源：http://gln.yanxiufei.cn

C#:   base.Greet();
来源：http://sga.xylfe.cn

[G08] 静态方法与属性
来源：http://lve.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bbv.chenzaomai.com

PHP:  public static function f() {}
来源：http://yfg.ybcxt.top

JS:   static f() {}
来源：http://oif.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://rwb.chenjidiqi.icu

Java: static void f() {}
来源：http://fsq.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xbl.wangshuangyany.cn

Ruby: def self.f; end
来源：http://ghf.haohaochexian.top

C#:   public static void F() {}
来源：http://sqd.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://pcz.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://qle.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hbu.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uof.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://spi.uphjek.com

Java: interface Shape { double area(); }
来源：http://bag.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://ubh.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gks.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://ktl.0kj1m.cn

[G10] 访问控制
来源：http://ubr.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://kyl.pengpengdd.cyou

PHP:  public / protected / private
来源：http://czv.cucudq.cn

JS:   #private 字段；其余公开
来源：http://edo.pengpengdd.cyou

TS:   public / protected / private
来源：http://uiu.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://vhf.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mhq.xuanzx.com

Ruby: public / protected / private
来源：http://yjt.0kj1m.cn

C#:   public / protected / private / internal
来源：http://imh.quarkkingdee.top

[G11] getter / setter
来源：http://pnn.redwolf501.top

Py:   @property 与 @x.setter
来源：http://rlv.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kuh.hesvh.cn

JS:   get name() { return this._name; }
来源：http://caj.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://euo.chenzaomai.com

Java: public String getName() { return name; }
来源：http://vaz.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://npm.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://waj.xinyue.icu

C#:   public string Name { get; set; }
来源：http://hwz.zhoulong.xyz

[G12] 对象转字符串
来源：http://nqm.guannengcc.top

Py:   def __str__(self): return self.name
来源：http://azs.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dfc.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://bgn.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://mgz.hysaishi.cn

Java: @Override public String toString() { return name; }
来源：http://wvv.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://vrg.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://hfe.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://kmg.zhiwuduotai.top

[G13] 判断对象类型
来源：http://wuy.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://yuk.ydzc1.top

PHP:  $u instanceof User
来源：http://spf.guowangkeji.top

JS:   u instanceof User
来源：http://rnh.fehbvm.com

TS:   u instanceof User
来源：http://lsj.yj20258.top

Java: u instanceof User
来源：http://prj.ctjpmb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://yrz.hnqzz.top

Ruby: u.is_a?(User)
来源：http://zcz.zhoulong.xyz

C#:   u is User
来源：http://hrr.ctjpmb.com

[G14] 数据类 / record
来源：http://iva.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://udl.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://lnl.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://jvo.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://qmh.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://ytk.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://qid.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jww.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://cle.svipenyu.cn

[G15] 枚举
来源：http://ftz.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zfc.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eim.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sis.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mrk.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://jfo.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rjk.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://ray.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qgq.birdmap.top

[G16] 对象转数组 / 字典
来源：http://pif.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hyk.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://chp.guowangkeji.top

JS:   Object.entries(obj)
来源：http://lxh.daria6918.cn

TS:   Object.entries(obj)
来源：http://adp.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zve.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://typ.yongpay.top

Ruby: obj.instance_variables
来源：http://ksi.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://bpk.ivvv.top

================================================================================
来源：http://zve.vqdsnc.cn

H. 异常与错误处理
来源：http://fdf.hongshengwenyu.top

================================================================================
来源：http://kuk.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://zef.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mrm.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ooo.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxz.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://txa.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dcg.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://grm.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ntd.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wae.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://imk.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dib.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qlk.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://iyy.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nqa.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://vms.0kj1m.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lod.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://oky.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sun.dianchejie.cn

[H03] 主动抛出异常
来源：http://klh.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://qel.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://grx.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://azx.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://qmw.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://lic.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iox.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://joj.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ktg.yj202588.top

[H04] 自定义异常类型
来源：http://val.birdmap.top

Py:   class MyError(Exception): pass
来源：http://vwl.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://zxh.fengsongda.top


<!-- 参考信息 -->