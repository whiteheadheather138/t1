代发 wailian999

[E22] 字节长度与字符长度
来源：http://efa.xuetiantiany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dki.nanxuanxn.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgh.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rka.sjlbkw.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fwx.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wkw.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fbe.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://dwv.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jfb.xuanzx.com

================================================================================
来源：http://eyv.fengsongda.top

F. 文件与目录
来源：http://hyq.nanxuanxn.top

================================================================================
来源：http://fpj.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://qmh.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bvv.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://fbg.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bch.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://enb.ydzc1.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yac.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mqz.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://gmo.cucudq.cn

C#:   File.ReadAllText("a.txt");
来源：http://jta.yanxiufei.cn

[F02] 逐行读取文件
来源：http://izi.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bya.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vum.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dgg.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnx.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://get.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kmd.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wzo.guannengcc.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://voh.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://acf.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ddg.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://svi.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cge.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbg.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lll.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dck.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://oic.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nvd.svipenyu.cn

[F04] 追加写入文件
来源：http://jyc.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jil.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://muc.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dgg.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://our.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qqy.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tua.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hpu.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://npc.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://qip.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xdu.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://sdb.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://esg.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://muz.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://hca.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hbo.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://ilq.yonumen.top

C#:   File.Exists("a.txt")
来源：http://apb.mhx1999.top

[F06] 删除文件
来源：http://ajc.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://tud.tanke756.top

PHP:  unlink("a.txt");
来源：http://xfa.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://pjp.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://tsx.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lrt.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://jrw.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://sej.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://aja.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://cfe.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mav.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nob.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rod.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awg.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lns.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hiv.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oaj.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ycd.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://vsj.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gcj.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jyb.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://whn.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://lzs.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bjt.hnqzz.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lmd.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://qxa.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://gxx.mhx1999.top

[F09] 获取文件大小
来源：http://xzc.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://jaj.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://lub.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://yty.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://bbs.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cyr.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wzb.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://yle.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://otj.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://bul.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ofc.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jlo.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pkn.shuidangran.top

TS:   path.extname("a.txt")
来源：http://sws.cucudq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yyd.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kxe.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kwl.yonumen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qvu.jlsjyb.cn

[F11] 复制与移动文件
来源：http://yuh.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vwz.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qcg.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kul.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pid.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dnz.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hgg.hongshengwenyu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hnz.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tmw.xuanzx.com

[F12] CSV 读写
来源：http://qgt.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ifl.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hvo.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wvz.tanke756.top

TS:   // 同上
来源：http://dfh.jiagoushi.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jye.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vbj.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://goa.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tlr.yfazqb.com

================================================================================
来源：http://yjs.birdmap.top

G. 面向对象
来源：http://ulz.jinyuanbaomall.cn

================================================================================
来源：http://aaj.zhiwuduotai.top

[G01] 定义类
来源：http://blo.jianghu66.top

Py:   class User: pass
来源：http://nwz.fanxiaobao.xyz

PHP:  class User {}
来源：http://gii.ppjwa.cn

JS:   class User {}
来源：http://sfm.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://zdr.pengpengdd.cyou

Java: class User {}
来源：http://opp.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://aar.smart0.xyz

Ruby: class User; end
来源：http://uld.jyoumei.cn

C#:   class User {}
来源：http://yap.hnxiangtu.top

[G02] 构造函数
来源：http://dyl.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://nyt.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://tlb.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://vdj.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://vrj.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://cgb.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pod.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://vgr.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://ffw.aizwys.cn

[G03] 实例属性
来源：http://izg.dianchejie.cn

Py:   self.name = "x"
来源：http://cpc.hcnkem.com

PHP:  public string $name = "x";
来源：http://wtu.jlsjyb.cn

JS:   this.name = "x";
来源：http://lwu.zhoulong.xyz

TS:   name: string = "x";
来源：http://bgc.ppjwa.cn

Java: private String name;
来源：http://dsi.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cxc.zycfv.cn

Ruby: @name = "x"
来源：http://yuo.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://arr.sxryk.cn

[G04] 定义方法
来源：http://xmp.ydzc1.top

Py:   def greet(self): return self.name
来源：http://hvt.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sup.fzhhl.top

JS:   greet() { return this.name; }
来源：http://ats.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://pqz.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://rmx.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qal.sysykeji.top

Ruby: def greet; @name; end
来源：http://ijf.andypj.xyz

C#:   public string Greet() => Name;
来源：http://lao.cashguo.top

[G05] 继承
来源：http://csh.fehbvm.com

Py:   class Admin(User): pass
来源：http://rpm.jianghu66.top

PHP:  class Admin extends User {}
来源：http://ltc.jyoumei.cn

JS:   class Admin extends User {}
来源：http://iqt.gotoacloud.top

TS:   class Admin extends User {}
来源：http://sbg.meibo888.top

Java: class Admin extends User {}
来源：http://jgq.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gsw.chenlongwang.top

Ruby: class Admin < User; end
来源：http://xoh.ehwqpu.com

C#:   class Admin : User {}
来源：http://lgh.hysaishi.cn

[G06] 重写方法
来源：http://pfs.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://mlv.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wyk.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://fre.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://mzz.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://aio.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jjb.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://upr.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://nzu.fehbvm.com

[G07] 调用父类方法
来源：http://ncn.zdbjq.cn

Py:   super().greet()
来源：http://hah.xuanzx.com

PHP:  parent::greet();
来源：http://wwh.xinyue.icu

JS:   super.greet();
来源：http://jmo.hnxiangtu.top

TS:   super.greet();
来源：http://xyr.shangyingyoupin.top

Java: super.greet();
来源：http://mdh.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jqd.0kj1m.cn

Ruby: super
来源：http://pql.shuidangran.top

C#:   base.Greet();
来源：http://ksy.hfpthk.cn

[G08] 静态方法与属性
来源：http://est.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nkb.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://rif.daria6918.cn

JS:   static f() {}
来源：http://jev.xuanzx.com

TS:   static f(): void {}
来源：http://zpp.bjfxy.top

Java: static void f() {}
来源：http://ftn.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oop.yj20258.top

Ruby: def self.f; end
来源：http://qin.sysykeji.top

C#:   public static void F() {}
来源：http://bem.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://jas.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://fin.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://fze.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gmh.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://glu.cucudq.cn

Java: interface Shape { double area(); }
来源：http://rki.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://vna.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zes.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://nja.hammf.cn

[G10] 访问控制
来源：http://hpo.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://jzf.andypj.xyz

PHP:  public / protected / private
来源：http://nmp.fehbvm.com

JS:   #private 字段；其余公开
来源：http://max.cheryme.top

TS:   public / protected / private
来源：http://xkp.yj202588.top

Java: public / protected / private / 默认包级
来源：http://rcd.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qwc.cheryme.top

Ruby: public / protected / private
来源：http://zte.bbcook.cn

C#:   public / protected / private / internal
来源：http://urn.cqqwz.cn

[G11] getter / setter
来源：http://xav.jianghu66.top

Py:   @property 与 @x.setter
来源：http://btm.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://srw.c1oappe.top

JS:   get name() { return this._name; }
来源：http://vfc.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://jcy.tarul.cn

Java: public String getName() { return name; }
来源：http://zwo.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://afc.sxryk.cn

Ruby: attr_accessor :name
来源：http://sad.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://gda.hywenlv.cn

[G12] 对象转字符串
来源：http://xie.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://bqv.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://not.shuidangran.top

JS:   toString() { return this.name; }
来源：http://jwe.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://afv.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://omz.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zng.yj202588.top

Ruby: def to_s; @name; end
来源：http://gxt.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://pzw.yanxiufei.cn

[G13] 判断对象类型
来源：http://ygt.jinqigufen.top

Py:   isinstance(u, User)
来源：http://fjq.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://afy.xinyue.icu

JS:   u instanceof User
来源：http://oem.xuanzx.com

TS:   u instanceof User
来源：http://wfu.yfazqb.com

Java: u instanceof User
来源：http://quj.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kny.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://ayp.ybcxt.top

C#:   u is User
来源：http://mup.sysykeji.top

[G14] 数据类 / record
来源：http://sij.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ueg.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://ijp.sjlbkw.cn

JS:   // 无内置：普通类或对象字面量
来源：http://otz.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://zwq.sysykeji.top

Java: record User(String name, int age) {}
来源：http://maq.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://idd.zdqjudy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xxh.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://zqa.0kj1m.cn

[G15] 枚举
来源：http://ymi.gaohongyu789.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qdw.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://otn.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pov.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xjw.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://pvc.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gsh.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://pzc.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tes.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://xsr.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ipc.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://erz.fengsongda.top

JS:   Object.entries(obj)
来源：http://aiy.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://dsj.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mie.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://hhv.yangfankeji.com

Ruby: obj.instance_variables
来源：http://cmw.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://fdm.gaohongyu789.top

================================================================================
来源：http://plq.gotoacloud.top

H. 异常与错误处理
来源：http://ono.xinyue.icu

================================================================================
来源：http://rga.jqgfzy.top

[H01] try / catch 基础
来源：http://qii.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ens.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oda.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lti.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dhr.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jyr.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tge.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vsm.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ont.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://yzr.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://inn.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fla.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bnf.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://oky.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://vqp.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xyq.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cuw.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sxq.jqgfzy.top

[H03] 主动抛出异常
来源：http://rfd.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://blb.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ira.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://jup.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://oke.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qlm.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ojv.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ond.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://maz.iojbl.cn

[H04] 自定义异常类型
来源：http://niq.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://vps.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://xdh.yj20258.top


<!-- 参考信息 -->