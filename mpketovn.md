代发 wailian999

[E22] 字节长度与字符长度
来源：http://rnp.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cpa.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qpc.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbf.9152youxi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sxh.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hnv.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xrv.daxiang520.top

Ruby: s.bytesize;  s.length
来源：http://tcl.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eti.jyoumei.cn

================================================================================
来源：http://xxl.jqgufenzy.top

F. 文件与目录
来源：http://dpe.nanxuanxn.top

================================================================================
来源：http://bqd.sxryk.cn

[F01] 读取整个文件
来源：http://qha.aizwys.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://arw.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://eke.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ndy.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yrj.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oks.tarul.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://whs.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://sqs.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://vlc.9152youxi.cn

[F02] 逐行读取文件
来源：http://vbz.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvd.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://teg.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcx.ybcxt.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lpi.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gpa.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yyx.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cdb.yonumen.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ofd.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://mcy.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjy.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kmh.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://url.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ouc.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://drx.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mgy.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://ult.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qqb.yfazqb.com

[F04] 追加写入文件
来源：http://jpu.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yor.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rtw.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tky.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tmm.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://onr.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xbe.hywenlv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ttq.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kuo.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://aen.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nwi.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://wgs.feifeiyinyue.top

JS:   fs.existsSync("a.txt")
来源：http://ysm.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://vtm.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://psm.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gvn.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://mus.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://pzw.vqdsnc.cn

[F06] 删除文件
来源：http://xxn.smart0.xyz

Py:   os.remove("a.txt")
来源：http://bfg.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://wpr.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kog.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://eno.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pfb.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://lbo.tianlin.xyz

Ruby: File.delete("a.txt")
来源：http://gxy.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://uxo.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://ikx.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pzo.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cwx.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqu.ctjpmb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hmm.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rrd.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://als.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ckk.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dro.jiagoushi.top

[F08] 遍历目录
来源：http://ewb.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hlg.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gys.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://ykq.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://xiv.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wkt.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hqt.mhx1999.top

Ruby: Dir.children("dir")
来源：http://fwa.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://lyk.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://vaj.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://qqi.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://vdq.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://ovp.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://odu.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://ciw.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mcu.aizwys.cn

Ruby: File.size("a.txt")
来源：http://xin.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://dhs.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://rio.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uzc.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qjt.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msp.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://gsn.sufxvd.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rnv.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vrn.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jik.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fhq.guowangkeji.top

[F11] 复制与移动文件
来源：http://doq.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xkb.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vmz.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nbg.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tls.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yqc.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cnn.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uqs.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dso.dianchejie.cn

[F12] CSV 读写
来源：http://biz.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nwi.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xas.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://svi.gotoacloud.top

TS:   // 同上
来源：http://kiq.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xnq.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ehs.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sra.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://pbc.kuanghao11.cn

================================================================================
来源：http://uvs.mhx1999.top

G. 面向对象
来源：http://kvd.yonumen.top

================================================================================
来源：http://syq.hammf.cn

[G01] 定义类
来源：http://hhc.zhoulong.xyz

Py:   class User: pass
来源：http://kom.dashuyun.cn

PHP:  class User {}
来源：http://ulg.pengpengdd.cyou

JS:   class User {}
来源：http://hjr.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://mkq.vqdsnc.cn

Java: class User {}
来源：http://njv.hcnkem.com

Go:   type User struct { Name string }
来源：http://kpv.chenzaomai.com

Ruby: class User; end
来源：http://gjx.jinqigfzy.top

C#:   class User {}
来源：http://qim.hywenlv.cn

[G02] 构造函数
来源：http://bwq.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://isw.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://fjn.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://haa.hammf.cn

TS:   constructor(public name: string) {}
来源：http://mgk.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://emh.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qdz.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://ekb.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://ewb.yfazqb.com

[G03] 实例属性
来源：http://zni.cdnleiting.top

Py:   self.name = "x"
来源：http://jgg.ivvv.top

PHP:  public string $name = "x";
来源：http://gbg.52xcode.cn

JS:   this.name = "x";
来源：http://dgf.gogol.net.cn

TS:   name: string = "x";
来源：http://wqw.gaohongyu789.top

Java: private String name;
来源：http://gsk.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mjb.vehdjk.com

Ruby: @name = "x"
来源：http://ifr.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://ipb.nanxuanxn.top

[G04] 定义方法
来源：http://ufe.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://jiw.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oyy.daxiang520.top

JS:   greet() { return this.name; }
来源：http://sbq.jianghu66.top

TS:   greet(): string { return this.name; }
来源：http://icl.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://sip.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dkb.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://elh.cashguo.top

C#:   public string Greet() => Name;
来源：http://nle.zycfv.cn

[G05] 继承
来源：http://cgy.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://tkh.yongpay.top

PHP:  class Admin extends User {}
来源：http://bpg.guowangkeji.top

JS:   class Admin extends User {}
来源：http://sad.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://dkq.gotoacloud.top

Java: class Admin extends User {}
来源：http://ylc.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://psa.cucudq.cn

Ruby: class Admin < User; end
来源：http://rns.chenlongwang.top

C#:   class Admin : User {}
来源：http://ufp.yuanzhike.top

[G06] 重写方法
来源：http://yca.316326.xyz

Py:   def greet(self): return "admin"
来源：http://oeq.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xsa.316326.xyz

JS:   greet() { return "admin"; }
来源：http://asi.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://hcx.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://evc.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rez.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://hvx.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://isb.hfpthk.cn

[G07] 调用父类方法
来源：http://bjl.andypj.xyz

Py:   super().greet()
来源：http://ppy.wangshuangyany.cn

PHP:  parent::greet();
来源：http://ezd.ppjwa.cn

JS:   super.greet();
来源：http://oxl.ywan-chungtsiang.top

TS:   super.greet();
来源：http://yqb.fehbvm.com

Java: super.greet();
来源：http://kyt.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ifk.nanxuanxn.top

Ruby: super
来源：http://ayj.fengsongda.top

C#:   base.Greet();
来源：http://biy.nanxuanxn.top

[G08] 静态方法与属性
来源：http://xgz.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wqt.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://wdb.fengsongda.top

JS:   static f() {}
来源：http://cpd.ivvv.top

TS:   static f(): void {}
来源：http://dlf.birdmap.top

Java: static void f() {}
来源：http://amy.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vxo.gzhubu.top

Ruby: def self.f; end
来源：http://onh.jqgufenzy.top

C#:   public static void F() {}
来源：http://fez.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://ifj.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://okk.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://agw.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://two.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://xyd.fehbvm.com

Java: interface Shape { double area(); }
来源：http://cdz.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://lhy.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mds.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://ted.tianlin.xyz

[G10] 访问控制
来源：http://bom.pycfn.com

Py:   约定 _protected / __private（不强制）
来源：http://pkj.aizwys.cn

PHP:  public / protected / private
来源：http://uzw.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://ftz.pycfn.com

TS:   public / protected / private
来源：http://svy.yonumen.top

Java: public / protected / private / 默认包级
来源：http://iwb.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rmx.hfpthk.cn

Ruby: public / protected / private
来源：http://tko.uphjek.com

C#:   public / protected / private / internal
来源：http://boc.jlsjyb.cn

[G11] getter / setter
来源：http://hrb.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://osf.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://khm.hywenlv.cn

JS:   get name() { return this._name; }
来源：http://kxe.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://chi.yuxming.cn

Java: public String getName() { return name; }
来源：http://gzq.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nkk.gzhubu.top

Ruby: attr_accessor :name
来源：http://xxj.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://mhd.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://dvh.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://zlk.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffx.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://mfz.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://ozs.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://iao.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ahp.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://rky.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://xhe.zhoulong.xyz

[G13] 判断对象类型
来源：http://tev.shzxlz.cn

Py:   isinstance(u, User)
来源：http://snm.birdmap.top

PHP:  $u instanceof User
来源：http://nbp.svipenyu.cn

JS:   u instanceof User
来源：http://kqe.yj202588.top

TS:   u instanceof User
来源：http://svj.jinqigufen.top

Java: u instanceof User
来源：http://uex.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ynn.yvedp.cn

Ruby: u.is_a?(User)
来源：http://xll.hnxiangtu.top

C#:   u is User
来源：http://gzy.cdnleiting.top

[G14] 数据类 / record
来源：http://mlu.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eyw.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://lhv.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://bvv.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://uof.fktsv.cn

Java: record User(String name, int age) {}
来源：http://zdc.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://isr.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pcz.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://irm.yonumen.top

[G15] 枚举
来源：http://gsd.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oxs.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://htk.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ycn.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzh.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://stv.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dfm.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://hoj.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nde.316326.xyz

[G16] 对象转数组 / 字典
来源：http://bbl.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hmv.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://imn.zdbjq.cn

JS:   Object.entries(obj)
来源：http://apn.jyoumei.cn

TS:   Object.entries(obj)
来源：http://eqb.hnxiangtu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://evg.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wsc.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://lod.yj20258888.top

C#:   // 用反射或 System.Text.Json
来源：http://knx.smart0.xyz

================================================================================
来源：http://pau.zhoulong.xyz

H. 异常与错误处理
来源：http://isg.xinyue.icu

================================================================================
来源：http://wxu.redwolf501.top

[H01] try / catch 基础
来源：http://yoi.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uvg.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ryf.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://alx.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udp.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fzx.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fod.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zeo.jqgufenzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ood.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://gjp.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://yqe.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xpb.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://url.jinqigfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mvh.316326.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://zxz.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zhl.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bqa.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://qyl.jinqigfzy.top

[H03] 主动抛出异常
来源：http://klr.sweek.top

Py:   raise ValueError("错误信息")
来源：http://sev.jqgfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ysq.aizwys.cn

JS:   throw new Error("错误信息");
来源：http://hoa.ivvv.top

TS:   throw new Error("错误信息");
来源：http://kdu.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://izv.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wfl.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://nzo.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zxa.yueranfly.top

[H04] 自定义异常类型
来源：http://kar.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://kvx.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://oqb.0kj1m.cn


<!-- 参考信息 -->