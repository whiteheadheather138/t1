代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pkd.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://syj.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qwe.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://did.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tkq.aibaodan.cn

================================================================================
来源：http://knl.dianchejie.cn

F. 文件与目录
来源：http://mhy.jyoumei.cn

================================================================================
来源：http://sfp.zhengqikj.top

[F01] 读取整个文件
来源：http://ivo.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jow.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://rxa.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rwo.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://euk.yonumen.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yvs.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gqj.sysykeji.top

Ruby: File.read("a.txt")
来源：http://fpr.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://hif.pengpengdd.cyou

[F02] 逐行读取文件
来源：http://qqh.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qel.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gth.pycfn.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hmn.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tja.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://shh.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sam.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ieq.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rwx.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://gjh.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nlu.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hwh.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuo.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://idn.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gdi.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycb.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://bch.guannengcc.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zjq.ivvv.top

[F04] 追加写入文件
来源：http://sth.hesvh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ckr.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bed.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eko.tianlin.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgz.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hta.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mca.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rjc.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sqb.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://sny.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cuf.sweek.top

PHP:  file_exists("a.txt");
来源：http://rdn.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://qgo.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://lhx.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yxa.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xqw.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://chy.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://ogm.cheryme.top

[F06] 删除文件
来源：http://dsx.yfazqb.com

Py:   os.remove("a.txt")
来源：http://axp.yfazqb.com

PHP:  unlink("a.txt");
来源：http://ark.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://juf.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://ulx.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jfp.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://mbd.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://arb.yj20258.top

C#:   File.Delete("a.txt");
来源：http://gvw.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://odr.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jed.bjfxy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yye.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bhg.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ykc.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://itx.jlsjyb.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eof.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://glb.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ghn.gaohongyu789.top

[F08] 遍历目录
来源：http://gom.yanxiufei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tgl.xziqi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eeg.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://tdn.tarul.cn

TS:   fs.readdirSync("dir")
来源：http://jja.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mru.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://zhu.pengpengdd.cyou

Ruby: Dir.children("dir")
来源：http://ppn.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://ukb.yvedp.cn

[F09] 获取文件大小
来源：http://sqa.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://olw.xingfuxueyuan.xyz

PHP:  filesize("a.txt");
来源：http://esp.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://gkh.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://esu.hammf.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mzx.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://weu.sxryk.cn

Ruby: File.size("a.txt")
来源：http://hgn.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://nfv.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://rss.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xcu.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qfs.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://asn.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://qgr.haohaochexian.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hro.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nnu.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jfr.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://prq.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://gyh.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uiy.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dha.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vci.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vtl.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdz.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zhy.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ilq.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmy.tanke756.top

[F12] CSV 读写
来源：http://ivs.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zgc.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqm.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://npw.hfpthk.cn

TS:   // 同上
来源：http://wmb.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pnd.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qen.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://obn.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wvt.zhiwuduotai.top

================================================================================
来源：http://xav.yueranfly.top

G. 面向对象
来源：http://zwk.zhijiandao.cn

================================================================================
来源：http://oky.ybcxt.top

[G01] 定义类
来源：http://dsk.guannengcc.top

Py:   class User: pass
来源：http://qjd.havefunace.top

PHP:  class User {}
来源：http://dvl.sjlbkw.cn

JS:   class User {}
来源：http://yop.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://mei.sweek.top

Java: class User {}
来源：http://byq.sweek.top

Go:   type User struct { Name string }
来源：http://iig.fanxiaobao.xyz

Ruby: class User; end
来源：http://zlc.yonumen.top

C#:   class User {}
来源：http://vvf.fanxiaobao.xyz

[G02] 构造函数
来源：http://qtj.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://wae.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://pth.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wjp.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://diq.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://fur.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gpi.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://wqc.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://kyi.fehbvm.com

[G03] 实例属性
来源：http://zyo.ehwqpu.com

Py:   self.name = "x"
来源：http://vru.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://fvz.chenlongwang.top

JS:   this.name = "x";
来源：http://rbm.guowangkeji.top

TS:   name: string = "x";
来源：http://ykx.xziqi.cn

Java: private String name;
来源：http://oyx.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yfe.hnqzz.top

Ruby: @name = "x"
来源：http://det.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://gse.zhijiandao.cn

[G04] 定义方法
来源：http://pfo.hammf.cn

Py:   def greet(self): return self.name
来源：http://olm.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mta.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://qfr.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://fvw.tarul.cn

Java: String greet() { return name; }
来源：http://zri.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://isa.fengsongda.top

Ruby: def greet; @name; end
来源：http://uaj.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://uir.fktsv.cn

[G05] 继承
来源：http://nen.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://eav.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://rrz.sweek.top

JS:   class Admin extends User {}
来源：http://evo.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://fgh.c1oappe.top

Java: class Admin extends User {}
来源：http://nxd.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vos.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://gdi.yj20258888.top

C#:   class Admin : User {}
来源：http://udj.snrcjt.cn

[G06] 重写方法
来源：http://ncb.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://thu.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kqz.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://bsk.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://qsm.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://tsp.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://avp.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://hda.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://exd.sxryk.cn

[G07] 调用父类方法
来源：http://bib.yvedp.cn

Py:   super().greet()
来源：http://pxx.sjlbkw.cn

PHP:  parent::greet();
来源：http://zoz.ydjk.org.cn

JS:   super.greet();
来源：http://ywr.meibo888.top

TS:   super.greet();
来源：http://hoh.wangdashe.top

Java: super.greet();
来源：http://mlz.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://irh.cdnleiting.top

Ruby: super
来源：http://uwh.quarkkingdee.top

C#:   base.Greet();
来源：http://cly.fengsongda.top

[G08] 静态方法与属性
来源：http://lbi.hfpthk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mid.gotoacloud.top

PHP:  public static function f() {}
来源：http://eea.fzhhl.top

JS:   static f() {}
来源：http://qrm.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://uqp.kuanghao11.cn

Java: static void f() {}
来源：http://epr.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qet.meibo888.top

Ruby: def self.f; end
来源：http://jde.tianlin.xyz

C#:   public static void F() {}
来源：http://ped.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://vvk.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://ihd.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ybr.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://out.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://rzz.wangdashe.top

Java: interface Shape { double area(); }
来源：http://qhh.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://kah.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ekd.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://whz.jiagoushi.top

[G10] 访问控制
来源：http://vwv.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://duo.fengsongda.top

PHP:  public / protected / private
来源：http://cvg.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://uwf.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://sbn.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://mrg.ppjwa.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hql.zdbjq.cn

Ruby: public / protected / private
来源：http://nat.havefunace.top

C#:   public / protected / private / internal
来源：http://cfp.316326.xyz

[G11] getter / setter
来源：http://qqf.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://ruo.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gzi.jianghu66.top

JS:   get name() { return this._name; }
来源：http://vve.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://aaf.cashguo.top

Java: public String getName() { return name; }
来源：http://mmo.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xcp.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://mbz.havefunace.top

C#:   public string Name { get; set; }
来源：http://vsw.yuxming.cn

[G12] 对象转字符串
来源：http://hge.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://ink.jlsjyb.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wan.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://lbi.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://jtz.xinyue.icu

Java: @Override public String toString() { return name; }
来源：http://gfv.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://tvc.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://uyk.jqgufenzy.top

C#:   public override string ToString() => Name;
来源：http://tgq.cucudq.cn

[G13] 判断对象类型
来源：http://hsd.dianchejie.cn

Py:   isinstance(u, User)
来源：http://brj.yj20258888.top

PHP:  $u instanceof User
来源：http://pjb.ctjpmb.com

JS:   u instanceof User
来源：http://ikq.sufxvd.cn

TS:   u instanceof User
来源：http://uzh.gogol.net.cn

Java: u instanceof User
来源：http://oqu.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://izn.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://jkj.vqdsnc.cn

C#:   u is User
来源：http://qez.sysykeji.top

[G14] 数据类 / record
来源：http://xcy.zdbjq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ovk.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://git.birdmap.top

JS:   // 无内置：普通类或对象字面量
来源：http://shd.haohaochexian.top

TS:   type User = { name: string; age: number };
来源：http://fil.hcnkem.com

Java: record User(String name, int age) {}
来源：http://add.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://kpm.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oxo.316326.xyz

C#:   record User(string Name, int Age);
来源：http://elf.dianchejie.cn

[G15] 枚举
来源：http://oji.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qsc.wangshuangyany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://smg.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://txg.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qlj.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://cau.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cys.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://jox.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ngo.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://wvn.wangdashe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://igd.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://uek.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://rom.cqqwz.cn

TS:   Object.entries(obj)
来源：http://nwc.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xbx.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kap.316326.xyz

Ruby: obj.instance_variables
来源：http://hfk.zhiwuduotai.top

C#:   // 用反射或 System.Text.Json
来源：http://sne.andypj.xyz

================================================================================
来源：http://ddv.ehwqpu.com

H. 异常与错误处理
来源：http://uwv.zycfv.cn

================================================================================
来源：http://srr.zhijiandao.cn

[H01] try / catch 基础
来源：http://apo.pengpengdd.cyou

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ztx.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://psc.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ajx.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xiv.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ert.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ugg.shangyingyoupin.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zci.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sbt.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://jen.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://ups.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://azm.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pbo.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://shd.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://lct.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zmr.sufxvd.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kdd.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xpr.ehwqpu.com

[H03] 主动抛出异常
来源：http://pcr.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://ork.aibaodan.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xsy.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://ple.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://aer.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hdi.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kda.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bgk.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://odw.ybcxt.top

[H04] 自定义异常类型
来源：http://shz.nanxinkj.top

Py:   class MyError(Exception): pass
来源：http://cve.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://ctz.sysykeji.top

JS:   class MyError extends Error {}
来源：http://baz.hcnkem.com

TS:   class MyError extends Error {}
来源：http://tvw.jinyuanbaomall.cn

Java: class MyException extends RuntimeException {}
来源：http://mrx.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vil.ybcxt.top


<!-- 参考信息 -->