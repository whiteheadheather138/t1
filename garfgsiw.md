代发 wailian999

[E22] 字节长度与字符长度
来源：http://bpa.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jzk.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fkv.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://clg.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tok.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uct.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fwv.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://jgx.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://duo.jyoumei.cn

================================================================================
来源：http://mdi.yanxiufei.cn

F. 文件与目录
来源：http://vwk.hammf.cn

================================================================================
来源：http://dkb.cdnleiting.top

[F01] 读取整个文件
来源：http://ape.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wcb.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://pch.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gea.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fde.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tnk.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uid.daxiang520.top

Ruby: File.read("a.txt")
来源：http://gfx.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://ucj.iojbl.cn

[F02] 逐行读取文件
来源：http://smc.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dwn.gzhubu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://izk.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://buu.gogol.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zco.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nii.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vyj.316326.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wxe.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://her.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://pkz.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wex.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cyr.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrg.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xip.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://spg.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pnt.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://yyw.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ntm.cheryme.top

[F04] 追加写入文件
来源：http://ipi.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nej.quarkkingdee.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ggy.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://srq.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oqk.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eid.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://piy.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hlq.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dtr.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://bdv.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pct.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://loj.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://vku.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://mqg.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ifg.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nhj.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://xjq.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://rgs.316326.xyz

[F06] 删除文件
来源：http://zqr.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://mdb.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://xsx.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tol.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://zkh.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dzt.yj20258.top

Go:   os.Remove("a.txt")
来源：http://nrx.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://lsm.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://llw.tian-w.cn

[F07] 创建目录（含多级）
来源：http://upw.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qpc.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rbx.jianghu66.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ney.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvz.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lqj.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eic.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://des.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pjl.gzhubu.top

[F08] 遍历目录
来源：http://shr.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://tuz.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://boa.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://gqk.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://rwf.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bed.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ehx.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://ewu.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://euq.svipenyu.cn

[F09] 获取文件大小
来源：http://gsh.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://tyg.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://pqw.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://nvb.birdmap.top

TS:   fs.statSync("a.txt").size
来源：http://dky.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://cms.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ynl.bbcook.cn

Ruby: File.size("a.txt")
来源：http://clo.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://vlt.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://ubm.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hhx.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sdz.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cym.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://stu.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kbk.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://buk.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dmy.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dyc.pycfn.com

[F11] 复制与移动文件
来源：http://awc.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://etb.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jug.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ssw.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhr.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ryo.chenlongwang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xay.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://muz.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbm.yongpay.top

[F12] CSV 读写
来源：http://ayf.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ivh.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lyi.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rys.yanxiufei.cn

TS:   // 同上
来源：http://kva.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qwg.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xsz.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zhd.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hgz.fanxiaobao.xyz

================================================================================
来源：http://guy.jinyuanbaomall.cn

G. 面向对象
来源：http://dah.bbcook.cn

================================================================================
来源：http://prh.yangfankeji.com

[G01] 定义类
来源：http://qqm.zhiwuduotai.top

Py:   class User: pass
来源：http://kfs.nwbrower.top

PHP:  class User {}
来源：http://dbo.hongshengwenyu.top

JS:   class User {}
来源：http://jzr.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://ypf.nwbrower.top

Java: class User {}
来源：http://hxe.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://mot.zdqjudy.top

Ruby: class User; end
来源：http://fxf.chenjidiqi.icu

C#:   class User {}
来源：http://hkr.zdbjq.cn

[G02] 构造函数
来源：http://wex.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://vfk.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://nfz.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://afu.yonumen.top

TS:   constructor(public name: string) {}
来源：http://shm.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://jab.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdd.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://nvl.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://imd.dianchejie.cn

[G03] 实例属性
来源：http://vsn.fengsongda.top

Py:   self.name = "x"
来源：http://wpg.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://iaj.shangyingyoupin.top

JS:   this.name = "x";
来源：http://goi.tanke756.top

TS:   name: string = "x";
来源：http://onj.zhongyouzk.top

Java: private String name;
来源：http://lux.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ccq.52xcode.cn

Ruby: @name = "x"
来源：http://rul.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://kss.hysaishi.cn

[G04] 定义方法
来源：http://kkx.ybcxt.top

Py:   def greet(self): return self.name
来源：http://snt.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://feq.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://tjs.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://buc.wangdashe.top

Java: String greet() { return name; }
来源：http://uhf.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lpo.jiagoushi.top

Ruby: def greet; @name; end
来源：http://uoa.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://fgi.yueranfly.top

[G05] 继承
来源：http://bdq.0kj1m.cn

Py:   class Admin(User): pass
来源：http://ain.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://tjv.yongpay.top

JS:   class Admin extends User {}
来源：http://uhp.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://zca.epnwcf.com

Java: class Admin extends User {}
来源：http://ldn.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://frb.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://yce.vehdjk.com

C#:   class Admin : User {}
来源：http://ehj.pycfn.com

[G06] 重写方法
来源：http://dmz.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://obd.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://owg.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://aij.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://smj.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://bro.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ncj.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://zmj.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://spp.shzxlz.cn

[G07] 调用父类方法
来源：http://xpv.hongshengwenyu.top

Py:   super().greet()
来源：http://pqt.ppjwa.cn

PHP:  parent::greet();
来源：http://wsq.zhongyouzk.top

JS:   super.greet();
来源：http://kuz.yfazqb.com

TS:   super.greet();
来源：http://khh.birdmap.top

Java: super.greet();
来源：http://tyk.kuanghao11.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gje.quarkkingdee.top

Ruby: super
来源：http://kbz.xuetiantiany.cn

C#:   base.Greet();
来源：http://njh.jqgfzy.top

[G08] 静态方法与属性
来源：http://ybr.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://had.haohaochexian.top

PHP:  public static function f() {}
来源：http://zny.sysykeji.top

JS:   static f() {}
来源：http://esn.hesvh.cn

TS:   static f(): void {}
来源：http://vnn.hesvh.cn

Java: static void f() {}
来源：http://qzy.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://srb.yuanzhike.top

Ruby: def self.f; end
来源：http://mvd.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://pkg.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://ynb.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://igx.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://hnn.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://brt.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://ikq.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://zmj.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://xiz.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sla.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://dpz.ehwqpu.com

[G10] 访问控制
来源：http://kwv.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://rqp.sxryk.cn

PHP:  public / protected / private
来源：http://qtu.fktsv.cn

JS:   #private 字段；其余公开
来源：http://wkf.yonumen.top

TS:   public / protected / private
来源：http://eiq.cheryme.top

Java: public / protected / private / 默认包级
来源：http://qze.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vep.316326.xyz

Ruby: public / protected / private
来源：http://cyd.vehdjk.com

C#:   public / protected / private / internal
来源：http://htf.dashuyun.cn

[G11] getter / setter
来源：http://qym.gzhubu.top

Py:   @property 与 @x.setter
来源：http://qhk.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://flj.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://ncf.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://zpq.nanxinkj.top

Java: public String getName() { return name; }
来源：http://mzt.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ugg.yuanzhike.top

Ruby: attr_accessor :name
来源：http://suc.nwbrower.top

C#:   public string Name { get; set; }
来源：http://gad.vehdjk.com

[G12] 对象转字符串
来源：http://mmi.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://bly.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hdj.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://wlf.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://cdo.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://was.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://uhj.cucudq.cn

Ruby: def to_s; @name; end
来源：http://cnv.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://osx.kuanghao11.cn

[G13] 判断对象类型
来源：http://aor.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://pot.xuetiantiany.cn

PHP:  $u instanceof User
来源：http://css.cheryme.top

JS:   u instanceof User
来源：http://thf.aizwys.cn

TS:   u instanceof User
来源：http://anl.yfazqb.com

Java: u instanceof User
来源：http://tdy.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pxf.shuidangran.top

Ruby: u.is_a?(User)
来源：http://naa.sysykeji.top

C#:   u is User
来源：http://ppb.gaohongyu789.top

[G14] 数据类 / record
来源：http://cxp.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vkj.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://pti.xingfuxueyuan.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://wlp.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://bji.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://edu.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://xcj.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yid.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://ekq.sweek.top

[G15] 枚举
来源：http://bxw.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xqz.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hmt.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://frv.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qjw.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://wsn.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bnk.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://wbg.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djo.ctjpmb.com

[G16] 对象转数组 / 字典
来源：http://uru.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://shs.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://zux.yongpay.top

JS:   Object.entries(obj)
来源：http://oyx.nwbrower.top

TS:   Object.entries(obj)
来源：http://ykv.quarkkingdee.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kgk.jyoumei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eoc.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://edx.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://frw.snrcjt.cn

================================================================================
来源：http://gza.yueranfly.top

H. 异常与错误处理
来源：http://lcf.ivvv.top

================================================================================
来源：http://elf.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://dkx.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rrz.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cad.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dkw.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udb.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yic.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yts.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lej.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xvr.hongshengwenyu.top

[H02] finally / ensure 收尾
来源：http://zri.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://evn.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://ozp.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nuj.daxiang520.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hnf.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://uxf.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://nyk.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qgo.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://yhn.hesvh.cn

[H03] 主动抛出异常
来源：http://tmb.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://rvo.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xlv.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://kiv.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://gyq.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://vjo.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lgk.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cbr.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ihk.xinyue.icu

[H04] 自定义异常类型
来源：http://asv.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://ioi.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://xrw.vqdsnc.cn


<!-- 参考信息 -->