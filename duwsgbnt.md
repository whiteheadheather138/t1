代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fge.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ksb.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jlx.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sgj.hesvh.cn

[E22] 字节长度与字符长度
来源：http://qmb.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rue.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ala.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhx.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cqt.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zfv.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://efh.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://wvw.shuidangran.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bkq.guowangkeji.top

================================================================================
来源：http://byf.hesvh.cn

F. 文件与目录
来源：http://ywl.smart0.xyz

================================================================================
来源：http://efa.feifeiyinyue.top

[F01] 读取整个文件
来源：http://iam.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qtx.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://aze.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hrh.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xom.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://yzl.yueranfly.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndj.cucudq.cn

Ruby: File.read("a.txt")
来源：http://xlg.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://ozz.daria6918.cn

[F02] 逐行读取文件
来源：http://rty.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cxm.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zmn.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvy.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pon.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fxg.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oyc.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yih.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mlq.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://cea.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://obr.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ofr.daria6918.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbg.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://moy.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wss.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cla.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://piu.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nmv.yueranfly.top

[F04] 追加写入文件
来源：http://hhn.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dpr.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uxo.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mif.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uyn.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://guo.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://niu.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bzk.zhongyouzk.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mdf.feifeiyinyue.top

[F05] 判断文件或目录是否存在
来源：http://eqe.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vxy.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://ixe.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://dbc.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://svf.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fpw.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eaf.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://uky.meibo888.top

C#:   File.Exists("a.txt")
来源：http://pji.yuanzhike.top

[F06] 删除文件
来源：http://qwx.cheryme.top

Py:   os.remove("a.txt")
来源：http://jso.iojbl.cn

PHP:  unlink("a.txt");
来源：http://ald.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://spc.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rvi.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pxu.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://yxi.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://uih.316326.xyz

C#:   File.Delete("a.txt");
来源：http://zqd.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://pnp.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eof.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iro.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://drv.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nar.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jca.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mzu.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ozg.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tlr.xinyue.icu

[F08] 遍历目录
来源：http://tej.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ckt.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wia.jinqigfzy.top

JS:   fs.readdirSync("dir")
来源：http://iec.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://xem.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xld.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ujz.sweek.top

Ruby: Dir.children("dir")
来源：http://mgs.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://wqv.birdmap.top

[F09] 获取文件大小
来源：http://ljy.gogol.net.cn

Py:   os.path.getsize("a.txt")
来源：http://kxy.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://eys.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://qkt.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://otn.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gsm.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mzu.birdmap.top

Ruby: File.size("a.txt")
来源：http://hll.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://bdd.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://dff.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wlw.shanyushiyangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yba.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zea.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://xct.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mki.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rsy.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ufm.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nps.epnwcf.com

[F11] 复制与移动文件
来源：http://sup.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gnp.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gno.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egu.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://urf.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yic.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ual.jinyuanbaomall.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bmg.ybcxt.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dhf.yueranfly.top

[F12] CSV 读写
来源：http://fsy.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jtq.ivvv.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nkd.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kcr.tanke756.top

TS:   // 同上
来源：http://ily.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tkw.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xwl.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jkr.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kbn.jqgfzy.top

================================================================================
来源：http://kyn.jinyuanbaomall.cn

G. 面向对象
来源：http://aex.fehbvm.com

================================================================================
来源：http://uwk.jinghuilouyu.cn

[G01] 定义类
来源：http://apu.gaohongyu789.top

Py:   class User: pass
来源：http://knd.birdmap.top

PHP:  class User {}
来源：http://nia.sufxvd.cn

JS:   class User {}
来源：http://elc.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://zog.fzhhl.top

Java: class User {}
来源：http://kmc.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://ihs.birdmap.top

Ruby: class User; end
来源：http://gkp.jianghu66.top

C#:   class User {}
来源：http://zxj.fanxiaobao.xyz

[G02] 构造函数
来源：http://qte.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://hql.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://fho.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://xof.pycfn.com

TS:   constructor(public name: string) {}
来源：http://civ.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://xzp.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yxg.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://pyd.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://tki.jiagoushi.top

[G03] 实例属性
来源：http://rjt.bbcook.cn

Py:   self.name = "x"
来源：http://rea.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://mnh.wangdashe.top

JS:   this.name = "x";
来源：http://vaf.cheryme.top

TS:   name: string = "x";
来源：http://uvc.guowangkeji.top

Java: private String name;
来源：http://czg.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cxm.cucudq.cn

Ruby: @name = "x"
来源：http://kbn.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://ldn.hammf.cn

[G04] 定义方法
来源：http://rqh.hesvh.cn

Py:   def greet(self): return self.name
来源：http://smp.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mws.gzhubu.top

JS:   greet() { return this.name; }
来源：http://kty.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://vsh.pycfn.com

Java: String greet() { return name; }
来源：http://wgn.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://log.cdnleiting.top

Ruby: def greet; @name; end
来源：http://scj.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://yhp.shuidangran.top

[G05] 继承
来源：http://mie.yuanzhike.top

Py:   class Admin(User): pass
来源：http://tgv.iojbl.cn

PHP:  class Admin extends User {}
来源：http://vwb.c1oappe.top

JS:   class Admin extends User {}
来源：http://mzo.shuidangran.top

TS:   class Admin extends User {}
来源：http://gxk.shuidangran.top

Java: class Admin extends User {}
来源：http://sca.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gkj.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://nsn.yueranfly.top

C#:   class Admin : User {}
来源：http://dfd.wangshuangyany.cn

[G06] 重写方法
来源：http://auj.hammf.cn

Py:   def greet(self): return "admin"
来源：http://tnr.snrcjt.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mtu.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://arn.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://ddo.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://aks.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgu.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://djl.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://xjf.gzhubu.top

[G07] 调用父类方法
来源：http://pti.yuxming.cn

Py:   super().greet()
来源：http://hde.gzhubu.top

PHP:  parent::greet();
来源：http://ioc.xylfe.cn

JS:   super.greet();
来源：http://rvu.zhoulong.xyz

TS:   super.greet();
来源：http://psm.zdbjq.cn

Java: super.greet();
来源：http://uew.chenlongwang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fgp.sweek.top

Ruby: super
来源：http://jyw.fehbvm.com

C#:   base.Greet();
来源：http://jqx.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://sau.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rkr.hysaishi.cn

PHP:  public static function f() {}
来源：http://gga.ehwqpu.com

JS:   static f() {}
来源：http://brm.gaohongyu789.top

TS:   static f(): void {}
来源：http://ayt.dashuyun.cn

Java: static void f() {}
来源：http://doe.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://bbu.yuxming.cn

Ruby: def self.f; end
来源：http://orp.cheryme.top

C#:   public static void F() {}
来源：http://hlt.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://hnh.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://zhz.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gld.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wce.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://ruy.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://laj.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://szp.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ziy.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://jxb.birdmap.top

[G10] 访问控制
来源：http://jme.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://cfv.ppjwa.cn

PHP:  public / protected / private
来源：http://unv.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://zsa.yangfankeji.com

TS:   public / protected / private
来源：http://xap.hammf.cn

Java: public / protected / private / 默认包级
来源：http://hif.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mji.ctjpmb.com

Ruby: public / protected / private
来源：http://dnl.zdbjq.cn

C#:   public / protected / private / internal
来源：http://dih.zhixingplan.top

[G11] getter / setter
来源：http://dal.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://ftx.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dzy.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://jgl.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://nev.dashuyun.cn

Java: public String getName() { return name; }
来源：http://xai.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cfp.zdbjq.cn

Ruby: attr_accessor :name
来源：http://mpm.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://fvu.yangfankeji.com

[G12] 对象转字符串
来源：http://stf.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://lpz.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ipb.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://hvw.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://vbe.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://mfz.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://txf.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://zvc.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://msm.jlsjyb.cn

[G13] 判断对象类型
来源：http://nru.yuxming.cn

Py:   isinstance(u, User)
来源：http://xax.jinqigfzy.top

PHP:  $u instanceof User
来源：http://bwt.yfazqb.com

JS:   u instanceof User
来源：http://yey.yueranfly.top

TS:   u instanceof User
来源：http://gme.cdnleiting.top

Java: u instanceof User
来源：http://xfn.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vtx.yongpay.top

Ruby: u.is_a?(User)
来源：http://sss.ppjwa.cn

C#:   u is User
来源：http://zzf.yuanzhike.top

[G14] 数据类 / record
来源：http://jel.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lmd.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://eyd.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://naz.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://oul.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://rah.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://hre.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zoo.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://qhl.xingfuxueyuan.xyz

[G15] 枚举
来源：http://lqc.ivvv.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jit.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qos.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://prk.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://txc.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://vod.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xsk.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://klj.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://obu.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://awv.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dym.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://mwi.gotoacloud.top

JS:   Object.entries(obj)
来源：http://uzs.xziqi.cn

TS:   Object.entries(obj)
来源：http://zdh.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://meg.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ktw.aizwys.cn

Ruby: obj.instance_variables
来源：http://zgq.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://kxk.tarul.cn

================================================================================
来源：http://qem.bjfxy.top

H. 异常与错误处理
来源：http://hdu.tianlin.xyz

================================================================================
来源：http://xmh.zdqjudy.top

[H01] try / catch 基础
来源：http://mij.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pxx.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojl.gotoacloud.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nsw.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hqd.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qav.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://obi.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ghc.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tqy.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://pwk.ywan-chungtsiang.top

Py:   try: f()⏎finally: cleanup()
来源：http://qwc.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cii.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kqg.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jhn.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://dvt.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ypl.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dit.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nmn.jqgfzy.top

[H03] 主动抛出异常
来源：http://ilt.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://mii.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kuh.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://ubh.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://ynz.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pll.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rda.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xzq.ctjpmb.com


<!-- 参考信息 -->