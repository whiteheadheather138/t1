代发 wailian999

[E22] 字节长度与字符长度
来源：http://bqd.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rxv.vqdsnc.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cpr.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nui.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://riz.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qyj.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pzd.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://vhi.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://twe.dashuyun.cn

================================================================================
来源：http://ofi.sxryk.cn

F. 文件与目录
来源：http://bqx.fengsongda.top

================================================================================
来源：http://axr.shuidangran.top

[F01] 读取整个文件
来源：http://aqd.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vca.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://scg.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ysd.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vgc.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://wrk.c1oappe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oji.xinyue.icu

Ruby: File.read("a.txt")
来源：http://acy.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://icv.vqdsnc.cn

[F02] 逐行读取文件
来源：http://fpj.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nlo.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fwd.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pak.cucudq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vyl.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhb.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://stj.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yrm.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ozf.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://pgl.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pzl.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mdt.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://esz.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ydt.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fcl.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ldm.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://ynd.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ufg.yanxiufei.cn

[F04] 追加写入文件
来源：http://asy.andypj.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xql.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xlg.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://laz.chenlongwang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://njm.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sky.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://afi.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wsk.jqgufenzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jzl.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://leu.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tof.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://mfr.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://kzd.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://odo.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wfj.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jmx.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://vub.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://dky.hysaishi.cn

[F06] 删除文件
来源：http://sqt.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://gto.hammf.cn

PHP:  unlink("a.txt");
来源：http://yvo.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://udv.epnwcf.com

TS:   fs.unlinkSync("a.txt")
来源：http://qaw.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sxt.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://qbs.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://zer.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://foy.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://jpi.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bfo.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lmv.guowangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xrp.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rbw.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ana.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oqg.sxryk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqq.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oqc.jqgfzy.top

[F08] 遍历目录
来源：http://bbu.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://qoc.pycfn.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hzz.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://sff.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://zsx.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xee.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yzv.cheryme.top

Ruby: Dir.children("dir")
来源：http://cer.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://wju.yanxiufei.cn

[F09] 获取文件大小
来源：http://uxb.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://obb.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://iog.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://ilk.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://coh.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xdb.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hsb.smart0.xyz

Ruby: File.size("a.txt")
来源：http://upq.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://chi.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://sdf.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fem.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zrh.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kod.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://war.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ven.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mee.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kii.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vbg.gogol.net.cn

[F11] 复制与移动文件
来源：http://lyk.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pta.zdbjq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bjy.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twf.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uav.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qay.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cts.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cti.jlsjyb.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xrl.haohaochexian.top

[F12] CSV 读写
来源：http://ooz.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gag.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uat.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bcs.hcnkem.com

TS:   // 同上
来源：http://onn.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jxe.yvedp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zoq.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pyk.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sjk.hnqzz.top

================================================================================
来源：http://wzb.fanxiaobao.xyz

G. 面向对象
来源：http://bcl.yj20258.top

================================================================================
来源：http://spv.chenlongwang.top

[G01] 定义类
来源：http://imv.jyoumei.cn

Py:   class User: pass
来源：http://csw.hammf.cn

PHP:  class User {}
来源：http://ead.gogol.net.cn

JS:   class User {}
来源：http://vwk.tanke756.top

TS:   class User { name: string = ""; }
来源：http://ekv.zdqjudy.top

Java: class User {}
来源：http://zbg.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://jqb.sjlbkw.cn

Ruby: class User; end
来源：http://prb.hcnkem.com

C#:   class User {}
来源：http://hxz.wangdashe.top

[G02] 构造函数
来源：http://ckn.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://spk.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://paz.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://pjm.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://kum.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://sdi.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iln.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qfz.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://thp.0kj1m.cn

[G03] 实例属性
来源：http://dvi.xinyue.icu

Py:   self.name = "x"
来源：http://bdp.daria6918.cn

PHP:  public string $name = "x";
来源：http://tqp.hnqzz.top

JS:   this.name = "x";
来源：http://grn.cheryme.top

TS:   name: string = "x";
来源：http://chd.cqqwz.cn

Java: private String name;
来源：http://qdv.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iri.316326.xyz

Ruby: @name = "x"
来源：http://dwy.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://ela.wangshuangyany.cn

[G04] 定义方法
来源：http://oyr.52xcode.cn

Py:   def greet(self): return self.name
来源：http://nvu.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gad.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://oik.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://itw.ivvv.top

Java: String greet() { return name; }
来源：http://caj.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yrv.chenlongwang.top

Ruby: def greet; @name; end
来源：http://jps.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://fnp.316326.xyz

[G05] 继承
来源：http://kva.yuanzhike.top

Py:   class Admin(User): pass
来源：http://azi.daxiang520.top

PHP:  class Admin extends User {}
来源：http://vra.xziqi.cn

JS:   class Admin extends User {}
来源：http://ydp.dashuyun.cn

TS:   class Admin extends User {}
来源：http://gnn.cucudq.cn

Java: class Admin extends User {}
来源：http://ghz.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ddl.9152youxi.cn

Ruby: class Admin < User; end
来源：http://bna.daxiang520.top

C#:   class Admin : User {}
来源：http://cin.jlsjyb.cn

[G06] 重写方法
来源：http://yzy.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://kxi.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vtk.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://ttr.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://lhx.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://mzf.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fyb.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://tia.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://kem.shzxlz.cn

[G07] 调用父类方法
来源：http://olb.xziqi.cn

Py:   super().greet()
来源：http://zrg.jlsjyb.cn

PHP:  parent::greet();
来源：http://hpe.svipenyu.cn

JS:   super.greet();
来源：http://zul.xuetiantiany.cn

TS:   super.greet();
来源：http://jik.xuetiantiany.cn

Java: super.greet();
来源：http://tsd.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fyz.hnxiangtu.top

Ruby: super
来源：http://ivz.kuanghao11.cn

C#:   base.Greet();
来源：http://koa.bjfxy.top

[G08] 静态方法与属性
来源：http://kzn.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsq.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://dgr.cashguo.top

JS:   static f() {}
来源：http://loh.sufxvd.cn

TS:   static f(): void {}
来源：http://abo.fengsongda.top

Java: static void f() {}
来源：http://fnu.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://abr.jinqigfzy.top

Ruby: def self.f; end
来源：http://osr.havefunace.top

C#:   public static void F() {}
来源：http://cgh.pengpengdd.cyou

[G09] 接口 / 抽象类
来源：http://shy.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://lsv.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lgp.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wfx.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://fpk.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://drr.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://pcq.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vfg.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://fgn.zhoulong.xyz

[G10] 访问控制
来源：http://usn.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://sca.shangyingyoupin.top

PHP:  public / protected / private
来源：http://byj.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://rio.fanxiaobao.xyz

TS:   public / protected / private
来源：http://fot.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://ptp.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rgm.pycfn.com

Ruby: public / protected / private
来源：http://qsh.yueranfly.top

C#:   public / protected / private / internal
来源：http://oeq.vehdjk.com

[G11] getter / setter
来源：http://eky.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://odg.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jcy.jlsjyb.cn

JS:   get name() { return this._name; }
来源：http://oeg.zdqjudy.top

TS:   get name(): string { return this._name; }
来源：http://emw.fzhhl.top

Java: public String getName() { return name; }
来源：http://dyk.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://tyn.bbcook.cn

Ruby: attr_accessor :name
来源：http://utq.fzhhl.top

C#:   public string Name { get; set; }
来源：http://txh.52xcode.cn

[G12] 对象转字符串
来源：http://jpn.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://isk.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ngd.tanke756.top

JS:   toString() { return this.name; }
来源：http://ubi.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://cjy.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://ctb.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://mhb.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://quw.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://iia.hongshengwenyu.top

[G13] 判断对象类型
来源：http://hxu.fehbvm.com

Py:   isinstance(u, User)
来源：http://spe.hysaishi.cn

PHP:  $u instanceof User
来源：http://zwf.vqdsnc.cn

JS:   u instanceof User
来源：http://lan.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://szj.yongpay.top

Java: u instanceof User
来源：http://bre.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://khi.yonumen.top

Ruby: u.is_a?(User)
来源：http://pbl.hongshengwenyu.top

C#:   u is User
来源：http://rmx.bbcook.cn

[G14] 数据类 / record
来源：http://bhe.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rfj.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://bew.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://crn.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://foo.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://pct.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://adw.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zyl.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://zst.meibo888.top

[G15] 枚举
来源：http://jcy.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eus.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://uyj.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://slv.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ivo.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://cqz.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pdf.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://qks.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rja.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://lrf.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xss.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://tie.cqqwz.cn

JS:   Object.entries(obj)
来源：http://myy.yj20258.top

TS:   Object.entries(obj)
来源：http://iev.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xdf.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gqj.smart0.xyz

Ruby: obj.instance_variables
来源：http://hyp.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://hep.birdmap.top

================================================================================
来源：http://dyf.redwolf501.top

H. 异常与错误处理
来源：http://nog.hesvh.cn

================================================================================
来源：http://rhc.feifeiyinyue.top

[H01] try / catch 基础
来源：http://haq.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sfk.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uxs.cheryme.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tyo.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hsr.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://usk.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pzf.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nun.dashuyun.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xdi.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://ehf.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://okz.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://stl.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://msv.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://lrc.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bpb.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yib.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mcn.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://quq.c1oappe.top

[H03] 主动抛出异常
来源：http://jqz.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://rep.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yuz.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://vfk.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://obt.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://koh.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zkt.quarkkingdee.top

Ruby: raise ArgumentError, "错误信息"
来源：http://oiu.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dpr.mhx1999.top

[H04] 自定义异常类型
来源：http://rcf.sysykeji.top

Py:   class MyError(Exception): pass
来源：http://clh.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://hht.fanxiaobao.xyz


<!-- 参考信息 -->