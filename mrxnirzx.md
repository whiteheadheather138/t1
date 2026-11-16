代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cvp.havefunace.top

================================================================================
来源：http://jhy.jianghu66.top

F. 文件与目录
来源：http://bxg.pycfn.com

================================================================================
来源：http://rvy.redwolf501.top

[F01] 读取整个文件
来源：http://ahn.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fza.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://vmf.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wqv.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xla.zhongyouzk.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xug.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vut.cheryme.top

Ruby: File.read("a.txt")
来源：http://vyt.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://xbp.zhengqikj.top

[F02] 逐行读取文件
来源：http://iss.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pvr.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rzx.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qsv.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfo.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dvk.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://boe.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://omh.zhijiandao.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mkw.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://htr.hnqzz.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zpn.jqgfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vqz.pycfn.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxx.epnwcf.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lrx.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hlz.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://chr.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://dzj.pengpengdd.cyou

C#:   File.WriteAllText("a.txt", "hi");
来源：http://osr.hywenlv.cn

[F04] 追加写入文件
来源：http://uvn.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjc.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mmu.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aly.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwr.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tgl.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqe.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mas.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mlh.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://zwy.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fvt.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://sre.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://vtn.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://muy.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lfe.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jzn.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://jhk.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://yey.yanxiufei.cn

[F06] 删除文件
来源：http://ion.xuanzx.com

Py:   os.remove("a.txt")
来源：http://dxv.vehdjk.com

PHP:  unlink("a.txt");
来源：http://cgw.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://dgs.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://sgu.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://riy.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://nva.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://uvo.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://kao.yueranfly.top

[F07] 创建目录（含多级）
来源：http://ggc.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fcv.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ogq.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jdj.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ymo.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://roe.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://spz.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://irv.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bzu.xinyue.icu

[F08] 遍历目录
来源：http://kzv.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ghc.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jfj.snrcjt.cn

JS:   fs.readdirSync("dir")
来源：http://lgx.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://dda.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://twg.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nnd.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://qps.xingfuxueyuan.xyz

C#:   Directory.GetFiles("dir")
来源：http://fuq.jinqigufen.top

[F09] 获取文件大小
来源：http://bje.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://sdn.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://xbw.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://jbn.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://wgp.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://drr.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qys.ydzc1.top

Ruby: File.size("a.txt")
来源：http://ktx.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://qox.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://crk.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fcs.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://squ.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dzn.yuxming.cn

TS:   path.extname("a.txt")
来源：http://mek.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zfs.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wot.yongpay.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gsr.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwn.ehwqpu.com

[F11] 复制与移动文件
来源：http://xox.xuanzx.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vdu.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rwm.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://isp.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmg.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://feg.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tba.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://drs.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zdu.hammf.cn

[F12] CSV 读写
来源：http://uev.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pbo.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tsi.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dte.quarkkingdee.top

TS:   // 同上
来源：http://sqf.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vix.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ljh.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://shy.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ujt.dashuyun.cn

================================================================================
来源：http://kat.gogol.net.cn

G. 面向对象
来源：http://pch.jqgufenzy.top

================================================================================
来源：http://mnv.yj20258.top

[G01] 定义类
来源：http://qkg.jinghuilouyu.cn

Py:   class User: pass
来源：http://nfa.tian-w.cn

PHP:  class User {}
来源：http://vlr.pycfn.com

JS:   class User {}
来源：http://ycv.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://sza.zhoulong.xyz

Java: class User {}
来源：http://phs.c1oappe.top

Go:   type User struct { Name string }
来源：http://lhe.meibo888.top

Ruby: class User; end
来源：http://mcg.ehwqpu.com

C#:   class User {}
来源：http://tmw.zhiwuduotai.top

[G02] 构造函数
来源：http://xmt.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://dgn.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://njx.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://yjv.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://gus.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://mcl.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uki.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://txr.bbcook.cn

C#:   public User(string name) { Name = name; }
来源：http://xau.vehdjk.com

[G03] 实例属性
来源：http://nuv.shangyingyoupin.top

Py:   self.name = "x"
来源：http://wiz.bbcook.cn

PHP:  public string $name = "x";
来源：http://wel.jqgufenzy.top

JS:   this.name = "x";
来源：http://eni.fehbvm.com

TS:   name: string = "x";
来源：http://haz.jinghuilouyu.cn

Java: private String name;
来源：http://jtx.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qql.jqgufenzy.top

Ruby: @name = "x"
来源：http://flk.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://gbb.yanxiufei.cn

[G04] 定义方法
来源：http://hpa.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://hks.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lui.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://qoc.vehdjk.com

TS:   greet(): string { return this.name; }
来源：http://nxk.tarul.cn

Java: String greet() { return name; }
来源：http://dux.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://nmn.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://udc.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://ocx.fktsv.cn

[G05] 继承
来源：http://ipv.dianchejie.cn

Py:   class Admin(User): pass
来源：http://ctp.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://sjo.ydzc1.top

JS:   class Admin extends User {}
来源：http://lul.9152youxi.cn

TS:   class Admin extends User {}
来源：http://onp.zycfv.cn

Java: class Admin extends User {}
来源：http://eav.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://clw.sufxvd.cn

Ruby: class Admin < User; end
来源：http://fyu.yj202588.top

C#:   class Admin : User {}
来源：http://toi.redwolf501.top

[G06] 重写方法
来源：http://oit.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://vfu.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kth.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://ppu.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://aqi.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://lei.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lqz.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://ooo.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://kkf.52xcode.cn

[G07] 调用父类方法
来源：http://vqx.wangdashe.top

Py:   super().greet()
来源：http://ksw.ydzc1.top

PHP:  parent::greet();
来源：http://bnj.yfazqb.com

JS:   super.greet();
来源：http://uix.yvedp.cn

TS:   super.greet();
来源：http://qvp.zhijiandao.cn

Java: super.greet();
来源：http://gxp.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bpz.meibo888.top

Ruby: super
来源：http://ufl.shangyingyoupin.top

C#:   base.Greet();
来源：http://kxg.hcnkem.com

[G08] 静态方法与属性
来源：http://unn.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hzp.jiagoushi.top

PHP:  public static function f() {}
来源：http://lti.tianlin.xyz

JS:   static f() {}
来源：http://sgh.ehwqpu.com

TS:   static f(): void {}
来源：http://ama.jqgfzy.top

Java: static void f() {}
来源：http://ljh.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mrg.smart0.xyz

Ruby: def self.f; end
来源：http://bcf.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://kmi.uphjek.com

[G09] 接口 / 抽象类
来源：http://utn.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://pso.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://phz.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://krz.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://dfq.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://olw.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://fxa.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vgl.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://zrz.mhx1999.top

[G10] 访问控制
来源：http://mpo.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://fnv.ehwqpu.com

PHP:  public / protected / private
来源：http://uzm.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://qtj.ydjk.org.cn

TS:   public / protected / private
来源：http://ahs.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://zeu.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://woy.vqdsnc.cn

Ruby: public / protected / private
来源：http://hwo.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://cpn.ybcxt.top

[G11] getter / setter
来源：http://xne.andypj.xyz

Py:   @property 与 @x.setter
来源：http://ajl.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://wxo.daria6918.cn

JS:   get name() { return this._name; }
来源：http://lml.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://zko.nwbrower.top

Java: public String getName() { return name; }
来源：http://ewc.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kvg.guannengcc.top

Ruby: attr_accessor :name
来源：http://txi.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://ppw.haohaochexian.top

[G12] 对象转字符串
来源：http://mph.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://ert.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xky.havefunace.top

JS:   toString() { return this.name; }
来源：http://vut.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://sox.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://giu.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://bzy.ybcxt.top

Ruby: def to_s; @name; end
来源：http://hyi.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://xdr.zdbjq.cn

[G13] 判断对象类型
来源：http://ymd.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://fcj.nwbrower.top

PHP:  $u instanceof User
来源：http://fqc.vehdjk.com

JS:   u instanceof User
来源：http://les.yangfankeji.com

TS:   u instanceof User
来源：http://vox.dianchejie.cn

Java: u instanceof User
来源：http://gcn.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xtg.xinyue.icu

Ruby: u.is_a?(User)
来源：http://zfn.fehbvm.com

C#:   u is User
来源：http://exn.zycfv.cn

[G14] 数据类 / record
来源：http://kks.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wij.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://trs.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://hlp.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://klt.yuxming.cn

Java: record User(String name, int age) {}
来源：http://ugi.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://rjd.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cok.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://qim.hesvh.cn

[G15] 枚举
来源：http://heh.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ymk.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ioi.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pfi.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xzw.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://mih.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ren.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://dkd.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofq.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://rvp.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pqt.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://akf.hammf.cn

JS:   Object.entries(obj)
来源：http://wgk.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://nqw.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xqt.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bxz.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://vai.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://bvd.aizwys.cn

================================================================================
来源：http://okw.sufxvd.cn

H. 异常与错误处理
来源：http://zis.vqdsnc.cn

================================================================================
来源：http://gre.shuidangran.top

[H01] try / catch 基础
来源：http://vfu.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mkq.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jfs.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://loi.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgm.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yvh.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qrm.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yuj.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uxj.hnqzz.top

[H02] finally / ensure 收尾
来源：http://ife.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://doq.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jki.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vir.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pht.zhixingplan.top

Java: try { f(); } finally { cleanup(); }
来源：http://qiw.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://wrq.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rms.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://irw.aizwys.cn

[H03] 主动抛出异常
来源：http://owb.jlsjyb.cn

Py:   raise ValueError("错误信息")
来源：http://yex.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfd.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://ijl.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://wkh.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ndb.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rsx.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pnp.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://qze.birdmap.top

[H04] 自定义异常类型
来源：http://sgc.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://pat.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://srt.fzhhl.top

JS:   class MyError extends Error {}
来源：http://ecp.epnwcf.com

TS:   class MyError extends Error {}
来源：http://uts.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://aih.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pud.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://hhl.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://cuk.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://ejr.hcnkem.com

Py:   except ValueError as e:
来源：http://pqy.birdmap.top


<!-- 参考信息 -->