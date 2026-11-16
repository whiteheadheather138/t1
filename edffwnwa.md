代发 wailian999

[E22] 字节长度与字符长度
来源：http://dbl.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wfh.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxr.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://frz.hnqzz.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhe.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wnx.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tjm.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://gcp.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ilr.zdbjq.cn

================================================================================
来源：http://tpz.hysaishi.cn

F. 文件与目录
来源：http://lis.fengsongda.top

================================================================================
来源：http://nhp.zhixingplan.top

[F01] 读取整个文件
来源：http://ank.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uub.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://psu.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://moo.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tbv.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://spf.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://thd.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://sev.yj20258888.top

C#:   File.ReadAllText("a.txt");
来源：http://nxz.jinyuanbaomall.cn

[F02] 逐行读取文件
来源：http://ucp.fehbvm.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qbv.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eiz.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ahl.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uaq.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kdl.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dux.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jqd.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zqn.ybcxt.top

[F03] 写入文件（覆盖）
来源：http://bal.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jpm.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lwr.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cta.jianghu66.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mcr.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ytf.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dvz.nanxinkj.top

Ruby: File.write("a.txt", "hi")
来源：http://dpz.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lsl.zhongyouzk.top

[F04] 追加写入文件
来源：http://xgl.ywan-chungtsiang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qwt.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iil.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wkh.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eyd.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dfc.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jzu.ydjk.org.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://see.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iwf.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://icc.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ino.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://vaf.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://tje.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://uum.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wlq.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pbe.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://ddt.hammf.cn

C#:   File.Exists("a.txt")
来源：http://uuh.sjlbkw.cn

[F06] 删除文件
来源：http://xxu.smart0.xyz

Py:   os.remove("a.txt")
来源：http://yrd.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://lwj.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ift.shangyingyoupin.top

TS:   fs.unlinkSync("a.txt")
来源：http://vmm.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://flo.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://svu.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://tgd.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://one.nwbrower.top

[F07] 创建目录（含多级）
来源：http://mnx.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://egm.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svo.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfe.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jvu.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pkg.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rep.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jsx.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cbm.tian-w.cn

[F08] 遍历目录
来源：http://brn.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://inp.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pzm.quarkkingdee.top

JS:   fs.readdirSync("dir")
来源：http://ffg.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://fus.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://svn.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cls.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://sdb.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://gov.nanxinkj.top

[F09] 获取文件大小
来源：http://zor.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://rpi.xylfe.cn

PHP:  filesize("a.txt");
来源：http://bbb.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://fhs.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://nwz.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://hlv.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uuk.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://jzl.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://dco.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://qxv.ppjwa.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eqn.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rxo.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jky.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://alf.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pkk.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bne.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://idy.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjj.gaohongyu789.top

[F11] 复制与移动文件
来源：http://zny.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ovz.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fab.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fwg.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nte.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lvz.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fnv.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cis.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bce.9152youxi.cn

[F12] CSV 读写
来源：http://ycr.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tjm.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgb.c1oappe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xwt.smart0.xyz

TS:   // 同上
来源：http://kum.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yzt.tarul.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jjt.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mus.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://agx.hongshengwenyu.top

================================================================================
来源：http://zyp.feifeiyinyue.top

G. 面向对象
来源：http://otr.nwbrower.top

================================================================================
来源：http://rhi.shanyushiyangtech.top

[G01] 定义类
来源：http://iao.vehdjk.com

Py:   class User: pass
来源：http://phx.cucudq.cn

PHP:  class User {}
来源：http://dds.52xcode.cn

JS:   class User {}
来源：http://mnz.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://ufh.jianghu66.top

Java: class User {}
来源：http://nob.yvedp.cn

Go:   type User struct { Name string }
来源：http://hqu.bjfxy.top

Ruby: class User; end
来源：http://zqj.shanyushiyangtech.top

C#:   class User {}
来源：http://wnh.jqgufenzy.top

[G02] 构造函数
来源：http://bgv.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://wrv.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://gah.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://sjk.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://ytm.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://rdr.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wbx.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://icf.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://phf.fktsv.cn

[G03] 实例属性
来源：http://ahn.vehdjk.com

Py:   self.name = "x"
来源：http://qbk.jinqigufen.top

PHP:  public string $name = "x";
来源：http://tqu.yongpay.top

JS:   this.name = "x";
来源：http://wma.yuxming.cn

TS:   name: string = "x";
来源：http://tvj.0kj1m.cn

Java: private String name;
来源：http://lxu.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bwl.yj20258888.top

Ruby: @name = "x"
来源：http://hvs.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://ole.gaohongyu789.top

[G04] 定义方法
来源：http://zpp.bjfxy.top

Py:   def greet(self): return self.name
来源：http://jhq.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivx.tanke756.top

JS:   greet() { return this.name; }
来源：http://oyu.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://yua.cashguo.top

Java: String greet() { return name; }
来源：http://ofw.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rhw.daria6918.cn

Ruby: def greet; @name; end
来源：http://dtf.ydzc1.top

C#:   public string Greet() => Name;
来源：http://owp.cashguo.top

[G05] 继承
来源：http://ieo.bjfxy.top

Py:   class Admin(User): pass
来源：http://uka.hesvh.cn

PHP:  class Admin extends User {}
来源：http://nbe.gotoacloud.top

JS:   class Admin extends User {}
来源：http://pog.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://lws.xinyue.icu

Java: class Admin extends User {}
来源：http://gho.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://luq.hammf.cn

Ruby: class Admin < User; end
来源：http://svr.iojbl.cn

C#:   class Admin : User {}
来源：http://tsy.ehwqpu.com

[G06] 重写方法
来源：http://vgv.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://byc.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bgg.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://tiy.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://yue.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://epd.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kcw.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://avc.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://yhc.fengsongda.top

[G07] 调用父类方法
来源：http://wno.daria6918.cn

Py:   super().greet()
来源：http://tws.gaohongyu789.top

PHP:  parent::greet();
来源：http://diu.jinqigufen.top

JS:   super.greet();
来源：http://lan.zhiwuduotai.top

TS:   super.greet();
来源：http://baa.ppjwa.cn

Java: super.greet();
来源：http://lfz.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ejg.hcnkem.com

Ruby: super
来源：http://gec.cucudq.cn

C#:   base.Greet();
来源：http://dlj.snrcjt.cn

[G08] 静态方法与属性
来源：http://bpp.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mje.pycfn.com

PHP:  public static function f() {}
来源：http://feg.fanxiaobao.xyz

JS:   static f() {}
来源：http://trm.quarkkingdee.top

TS:   static f(): void {}
来源：http://anc.yj20258.top

Java: static void f() {}
来源：http://gse.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hds.yanxiufei.cn

Ruby: def self.f; end
来源：http://hwv.zhengqikj.top

C#:   public static void F() {}
来源：http://bcf.uphjek.com

[G09] 接口 / 抽象类
来源：http://ejc.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://keg.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://nip.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://igt.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://spi.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://pwe.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://xkp.xuetiantiany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rwb.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://egj.fengsongda.top

[G10] 访问控制
来源：http://dxu.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://jkg.feifeiyinyue.top

PHP:  public / protected / private
来源：http://kpx.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://pku.sufxvd.cn

TS:   public / protected / private
来源：http://lzv.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://bty.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://seo.snrcjt.cn

Ruby: public / protected / private
来源：http://bkl.wangdashe.top

C#:   public / protected / private / internal
来源：http://dhf.xziqi.cn

[G11] getter / setter
来源：http://enn.havefunace.top

Py:   @property 与 @x.setter
来源：http://qev.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xyl.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://eza.yj20258.top

TS:   get name(): string { return this._name; }
来源：http://ydh.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://afb.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sff.tianlin.xyz

Ruby: attr_accessor :name
来源：http://lpk.iojbl.cn

C#:   public string Name { get; set; }
来源：http://fza.wangshuangyany.cn

[G12] 对象转字符串
来源：http://rya.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://znq.uphjek.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://una.havefunace.top

JS:   toString() { return this.name; }
来源：http://bew.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://jad.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://wss.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mcy.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://jzb.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://kim.ivvv.top

[G13] 判断对象类型
来源：http://ukd.guowangkeji.top

Py:   isinstance(u, User)
来源：http://avu.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://hzh.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://toc.yangfankeji.com

TS:   u instanceof User
来源：http://qbm.shanyushiyangkeji.top

Java: u instanceof User
来源：http://aqv.jlsjyb.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ihi.bbcook.cn

Ruby: u.is_a?(User)
来源：http://opl.haohaochexian.top

C#:   u is User
来源：http://bwe.yj202588.top

[G14] 数据类 / record
来源：http://clw.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fka.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://wfv.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://snd.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://dfw.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://xrw.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://lme.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://axa.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://zgc.epnwcf.com

[G15] 枚举
来源：http://cep.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://etm.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wdf.cheryme.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hqt.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wty.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://gsc.yj20258888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jkh.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://vvw.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dvp.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://uot.quarkkingdee.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bue.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://wil.svipenyu.cn

JS:   Object.entries(obj)
来源：http://geb.aizwys.cn

TS:   Object.entries(obj)
来源：http://afv.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zwo.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://roi.yueranfly.top

Ruby: obj.instance_variables
来源：http://wze.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://rns.shanyushiyangtech.top

================================================================================
来源：http://btb.shzxlz.cn

H. 异常与错误处理
来源：http://xcq.xinyue.icu

================================================================================
来源：http://hbk.haohaochexian.top

[H01] try / catch 基础
来源：http://xca.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://krp.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tmk.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gok.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://doz.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tnq.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aek.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://icp.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rwz.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://edp.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gsf.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gqm.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pxg.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hhr.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://pyf.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vso.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pvv.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hmh.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://yuf.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://mke.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fnp.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://xra.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://vjy.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qvm.ivvv.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kna.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dbs.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://oeb.havefunace.top

[H04] 自定义异常类型
来源：http://zbo.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://huv.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://oqy.uphjek.com


<!-- 参考信息 -->