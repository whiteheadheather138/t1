代发 wailian999

[E22] 字节长度与字符长度
来源：http://mvd.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yaj.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gcb.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnh.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nxg.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wal.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dna.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://xgf.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://idz.sufxvd.cn

================================================================================
来源：http://tnx.aibaodan.cn

F. 文件与目录
来源：http://rtn.birdmap.top

================================================================================
来源：http://kti.ehwqpu.com

[F01] 读取整个文件
来源：http://llz.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ncn.jlsjyb.cn

PHP:  file_get_contents("a.txt");
来源：http://wff.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ygx.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ieo.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jdu.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xje.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://ryc.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://gqd.yj20258888.top

[F02] 逐行读取文件
来源：http://uxy.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yde.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://grc.tianlin.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxq.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://enw.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aha.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kab.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qur.ctjpmb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pqj.mhx1999.top

[F03] 写入文件（覆盖）
来源：http://gmb.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gnc.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://adh.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zbl.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yoh.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fyw.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wig.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://jit.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dnv.zhijiandao.cn

[F04] 追加写入文件
来源：http://esr.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://psm.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hhr.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zat.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ekg.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://frt.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://agc.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bpc.zhixingplan.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hjm.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://csm.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yby.birdmap.top

PHP:  file_exists("a.txt");
来源：http://nku.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://sxq.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://zet.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qow.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hwt.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://moo.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://nun.fktsv.cn

[F06] 删除文件
来源：http://hlc.uphjek.com

Py:   os.remove("a.txt")
来源：http://oud.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://dct.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://lms.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://mgs.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fjj.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://uit.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://ykx.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://gjn.birdmap.top

[F07] 创建目录（含多级）
来源：http://xjb.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mnb.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xmo.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nqk.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gph.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ivs.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rkn.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jko.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fps.guowangkeji.top

[F08] 遍历目录
来源：http://kjc.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjf.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://miq.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://vxb.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://fxu.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dse.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lom.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://vwm.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://xvr.shzxlz.cn

[F09] 获取文件大小
来源：http://cec.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ldf.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://kyq.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://rhw.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://gwi.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://ivl.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fhy.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://mbx.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://msf.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://pwk.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pns.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fio.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://alo.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://xjr.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wfx.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nct.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oth.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dki.tarul.cn

[F11] 复制与移动文件
来源：http://jxd.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dui.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mek.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vmo.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yqt.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aug.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hhp.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bip.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iax.cqqwz.cn

[F12] CSV 读写
来源：http://nxv.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pyx.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mcu.hcnkem.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aff.chenlongwang.top

TS:   // 同上
来源：http://dcn.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zzq.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nij.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ait.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bet.fengsongda.top

================================================================================
来源：http://hwy.wangshuangyany.cn

G. 面向对象
来源：http://iia.yj20258.top

================================================================================
来源：http://qbr.zhongyouzk.top

[G01] 定义类
来源：http://sbm.yanxiufei.cn

Py:   class User: pass
来源：http://frd.zhongyouzk.top

PHP:  class User {}
来源：http://nje.cheryme.top

JS:   class User {}
来源：http://agq.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://abm.zdqjudy.top

Java: class User {}
来源：http://bqf.yonumen.top

Go:   type User struct { Name string }
来源：http://erb.jianghu66.top

Ruby: class User; end
来源：http://kfd.shangyingyoupin.top

C#:   class User {}
来源：http://cba.svipenyu.cn

[G02] 构造函数
来源：http://ruv.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://til.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://vbd.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://hiy.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://wwp.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://szk.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zca.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://oxi.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://ihx.sxryk.cn

[G03] 实例属性
来源：http://mil.zhiwuduotai.top

Py:   self.name = "x"
来源：http://xak.xziqi.cn

PHP:  public string $name = "x";
来源：http://qmm.cucudq.cn

JS:   this.name = "x";
来源：http://kln.svipenyu.cn

TS:   name: string = "x";
来源：http://ohg.bjfxy.top

Java: private String name;
来源：http://wxm.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xry.svipenyu.cn

Ruby: @name = "x"
来源：http://vnj.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://kdo.mhx1999.top

[G04] 定义方法
来源：http://zal.smart0.xyz

Py:   def greet(self): return self.name
来源：http://msa.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://twl.52xcode.cn

JS:   greet() { return this.name; }
来源：http://whr.fehbvm.com

TS:   greet(): string { return this.name; }
来源：http://keu.tanke756.top

Java: String greet() { return name; }
来源：http://ilm.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jub.chenlongwang.top

Ruby: def greet; @name; end
来源：http://wpd.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://gsv.vehdjk.com

[G05] 继承
来源：http://gtj.shzxlz.cn

Py:   class Admin(User): pass
来源：http://obr.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://hpi.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://hfi.jqgfzy.top

TS:   class Admin extends User {}
来源：http://fsq.jinqigufen.top

Java: class Admin extends User {}
来源：http://jfh.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://seh.yvedp.cn

Ruby: class Admin < User; end
来源：http://zas.iojbl.cn

C#:   class Admin : User {}
来源：http://dhf.hongshengwenyu.top

[G06] 重写方法
来源：http://mdw.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://kbs.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lzv.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://vdp.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://urp.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://qge.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csf.cashguo.top

Ruby: def greet; "admin"; end
来源：http://lcv.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://tdy.hywenlv.cn

[G07] 调用父类方法
来源：http://tfy.yanxiufei.cn

Py:   super().greet()
来源：http://cnh.yuxming.cn

PHP:  parent::greet();
来源：http://xzn.tian-w.cn

JS:   super.greet();
来源：http://fcy.uphjek.com

TS:   super.greet();
来源：http://tse.tanke756.top

Java: super.greet();
来源：http://tik.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oqd.zhongyouzk.top

Ruby: super
来源：http://pwq.sjlbkw.cn

C#:   base.Greet();
来源：http://xqb.nwbrower.top

[G08] 静态方法与属性
来源：http://vjd.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jyk.hywenlv.cn

PHP:  public static function f() {}
来源：http://hhr.316326.xyz

JS:   static f() {}
来源：http://wnm.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://elp.vqdsnc.cn

Java: static void f() {}
来源：http://zio.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://yrn.xuanzx.com

Ruby: def self.f; end
来源：http://tic.tianlin.xyz

C#:   public static void F() {}
来源：http://ugi.mhx1999.top

[G09] 接口 / 抽象类
来源：http://ibm.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://kmu.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://ahi.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hlb.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://eei.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://oub.jlsjyb.cn

Go:   type Shape interface { Area() float64 }
来源：http://vgi.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mpk.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://mdw.yfazqb.com

[G10] 访问控制
来源：http://qtj.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://vec.havefunace.top

PHP:  public / protected / private
来源：http://eha.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://dpo.feifeiyinyue.top

TS:   public / protected / private
来源：http://gcy.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://xdb.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dte.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://kkk.shzxlz.cn

C#:   public / protected / private / internal
来源：http://nvm.kuanghao11.cn

[G11] getter / setter
来源：http://yvd.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://ymh.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://amg.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://nrx.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://tkm.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://ryr.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hwm.birdmap.top

Ruby: attr_accessor :name
来源：http://qis.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://kum.tianlin.xyz

[G12] 对象转字符串
来源：http://cco.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://ldq.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gks.tian-w.cn

JS:   toString() { return this.name; }
来源：http://etd.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://mxi.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://tnz.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bdd.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://wlg.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://hdc.svipenyu.cn

[G13] 判断对象类型
来源：http://tzd.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://rkp.xinyue.icu

PHP:  $u instanceof User
来源：http://jkf.gaohongyu789.top

JS:   u instanceof User
来源：http://oxb.sysykeji.top

TS:   u instanceof User
来源：http://ksg.nwbrower.top

Java: u instanceof User
来源：http://lhi.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://prj.yueranfly.top

Ruby: u.is_a?(User)
来源：http://vtb.xylfe.cn

C#:   u is User
来源：http://upb.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://oie.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://plv.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://xrk.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://krw.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://bld.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://wkm.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://tkh.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oqn.tanke756.top

C#:   record User(string Name, int Age);
来源：http://uva.yj20258.top

[G15] 枚举
来源：http://sga.ctjpmb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mum.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jsx.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://srx.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://srk.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://vfo.fehbvm.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ihk.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://cgl.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mix.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://jhj.316326.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wab.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://ihm.smart0.xyz

JS:   Object.entries(obj)
来源：http://jmv.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://aed.zhoulong.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qkw.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vkv.bjfxy.top

Ruby: obj.instance_variables
来源：http://ftw.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://nex.xziqi.cn

================================================================================
来源：http://mvs.yj20258.top

H. 异常与错误处理
来源：http://dkm.yongpay.top

================================================================================
来源：http://jgq.gzhubu.top

[H01] try / catch 基础
来源：http://gon.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rng.ydzc1.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lkr.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vwm.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kow.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nmp.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vsu.xylfe.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nsk.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iul.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://cww.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zjy.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vlu.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://vku.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://unq.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://rza.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://haj.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gzh.zdqjudy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://txj.ppjwa.cn

[H03] 主动抛出异常
来源：http://eog.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://cqb.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzh.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://gze.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://hhb.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sjv.birdmap.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://asp.jqgufenzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ddd.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mhb.sysykeji.top

[H04] 自定义异常类型
来源：http://scp.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://ysb.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tot.tarul.cn


<!-- 参考信息 -->