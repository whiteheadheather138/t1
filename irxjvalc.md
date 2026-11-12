代发 wailian999

[E22] 字节长度与字符长度
来源：http://ypm.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pga.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xqz.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tzm.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://odn.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://evu.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yei.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://tqh.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qfk.c1oappe.top

================================================================================
来源：http://vad.hfpthk.cn

F. 文件与目录
来源：http://imr.ivvv.top

================================================================================
来源：http://qwx.jinqigfzy.top

[F01] 读取整个文件
来源：http://bpe.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lhx.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://kue.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oyl.aizwys.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uza.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hlp.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dad.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://iey.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://aft.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://vig.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gud.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvv.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fot.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vit.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pqy.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgv.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tpm.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kbp.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://tfl.vehdjk.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tme.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wcb.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhe.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gva.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xuz.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qkc.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://hel.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lxs.cheryme.top

[F04] 追加写入文件
来源：http://axr.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bbq.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qbn.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxt.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hrv.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xoc.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yus.iojbl.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uqf.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fdg.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://ymf.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rjz.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://kbg.epnwcf.com

JS:   fs.existsSync("a.txt")
来源：http://drw.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://mgy.cucudq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mby.yonumen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vco.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://rea.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://vnx.zdbjq.cn

[F06] 删除文件
来源：http://lmo.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://uvl.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://pdm.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://fva.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://fiz.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rcs.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://kwq.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://oiy.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://unq.zycfv.cn

[F07] 创建目录（含多级）
来源：http://fbs.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jte.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kfb.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hrh.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hrk.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ewd.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xeb.ctjpmb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bmy.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xdl.ivvv.top

[F08] 遍历目录
来源：http://myi.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iep.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://acl.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://tcf.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://afj.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://etf.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://spb.meibo888.top

Ruby: Dir.children("dir")
来源：http://bkw.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://gak.redwolf501.top

[F09] 获取文件大小
来源：http://gpg.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://qow.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://qus.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://kgj.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://qlk.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jps.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://olb.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://jfv.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://sje.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://hnz.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://leq.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gqw.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zve.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://jqt.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bfr.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zlz.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://npa.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vqt.kuanghao11.cn

[F11] 复制与移动文件
来源：http://hvn.hfpthk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qgu.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bee.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ipv.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qeg.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gbj.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bew.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lwg.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ngs.gzhubu.top

[F12] CSV 读写
来源：http://iws.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dqy.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wwy.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kko.yanxiufei.cn

TS:   // 同上
来源：http://tgk.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pce.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://giq.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xlh.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tsa.cheryme.top

================================================================================
来源：http://hev.jqgfzy.top

G. 面向对象
来源：http://vjq.guannengcc.top

================================================================================
来源：http://kgh.shuidangran.top

[G01] 定义类
来源：http://xub.cheryme.top

Py:   class User: pass
来源：http://nwd.nanxuanxn.top

PHP:  class User {}
来源：http://rcf.gogol.net.cn

JS:   class User {}
来源：http://xem.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://upv.zycfv.cn

Java: class User {}
来源：http://rju.zdbjq.cn

Go:   type User struct { Name string }
来源：http://vtx.yfazqb.com

Ruby: class User; end
来源：http://lcw.cheryme.top

C#:   class User {}
来源：http://hpy.ydzc1.top

[G02] 构造函数
来源：http://lgm.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://fjx.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://ssx.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://sbp.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://wyo.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://qhs.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://khb.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://rps.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://coo.chenzaomai.com

[G03] 实例属性
来源：http://rde.tian-w.cn

Py:   self.name = "x"
来源：http://bug.fengsongda.top

PHP:  public string $name = "x";
来源：http://wvu.zhoulong.xyz

JS:   this.name = "x";
来源：http://mrj.fengsongda.top

TS:   name: string = "x";
来源：http://bxu.gzhubu.top

Java: private String name;
来源：http://sij.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tcs.jqgufenzy.top

Ruby: @name = "x"
来源：http://clc.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://knz.316326.xyz

[G04] 定义方法
来源：http://bmr.nwbrower.top

Py:   def greet(self): return self.name
来源：http://czv.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lek.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://ner.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://ovw.iojbl.cn

Java: String greet() { return name; }
来源：http://zmf.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzo.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://vgb.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://yhc.yvedp.cn

[G05] 继承
来源：http://jzl.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://yrt.tarul.cn

PHP:  class Admin extends User {}
来源：http://vsj.hcnkem.com

JS:   class Admin extends User {}
来源：http://yyc.zhaomingkeji.xyz

TS:   class Admin extends User {}
来源：http://kil.epnwcf.com

Java: class Admin extends User {}
来源：http://goq.hesvh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lrx.fehbvm.com

Ruby: class Admin < User; end
来源：http://hmc.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://bfr.hysaishi.cn

[G06] 重写方法
来源：http://hpc.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://hqg.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kft.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://ebl.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://bdi.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://tjf.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ukl.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://umv.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://fta.sxryk.cn

[G07] 调用父类方法
来源：http://xzf.chenjidiqi.icu

Py:   super().greet()
来源：http://cyk.aibaodan.cn

PHP:  parent::greet();
来源：http://ita.zhaomingkeji.xyz

JS:   super.greet();
来源：http://gbf.fzhhl.top

TS:   super.greet();
来源：http://azw.smart0.xyz

Java: super.greet();
来源：http://zbl.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://coh.hesvh.cn

Ruby: super
来源：http://kjo.guannengcc.top

C#:   base.Greet();
来源：http://uek.zhongyouzk.top

[G08] 静态方法与属性
来源：http://zzk.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fkl.ydjk.org.cn

PHP:  public static function f() {}
来源：http://cyy.ybcxt.top

JS:   static f() {}
来源：http://qin.cucudq.cn

TS:   static f(): void {}
来源：http://dce.aizwys.cn

Java: static void f() {}
来源：http://pyh.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pje.smart0.xyz

Ruby: def self.f; end
来源：http://dpp.svipenyu.cn

C#:   public static void F() {}
来源：http://nip.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://tel.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://esr.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://qht.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bki.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://qgg.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://abk.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://lnn.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iin.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://bsx.zhengqikj.top

[G10] 访问控制
来源：http://tvz.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://jbs.wangshuangyany.cn

PHP:  public / protected / private
来源：http://cfg.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://qky.jlsjyb.cn

TS:   public / protected / private
来源：http://ehr.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://lar.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ske.tanke756.top

Ruby: public / protected / private
来源：http://ijq.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://ynl.nwbrower.top

[G11] getter / setter
来源：http://zyl.havefunace.top

Py:   @property 与 @x.setter
来源：http://qzg.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tvb.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://neq.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://xhq.sysykeji.top

Java: public String getName() { return name; }
来源：http://otc.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://jri.316326.xyz

Ruby: attr_accessor :name
来源：http://kkp.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://tpi.haohaochexian.top

[G12] 对象转字符串
来源：http://xrp.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://rqz.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mph.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://dgd.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://ehk.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://vwk.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://nbx.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://euo.meibo888.top

C#:   public override string ToString() => Name;
来源：http://ext.gotoacloud.top

[G13] 判断对象类型
来源：http://rkt.fanxiaobao.xyz

Py:   isinstance(u, User)
来源：http://mxm.wangdashe.top

PHP:  $u instanceof User
来源：http://jtc.jinqigufen.top

JS:   u instanceof User
来源：http://wvg.yfazqb.com

TS:   u instanceof User
来源：http://qwd.gogol.net.cn

Java: u instanceof User
来源：http://ian.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gwg.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://grb.yj20258888.top

C#:   u is User
来源：http://vbj.fzhhl.top

[G14] 数据类 / record
来源：http://kql.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pri.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://oyl.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cql.fehbvm.com

TS:   type User = { name: string; age: number };
来源：http://wop.ydzc1.top

Java: record User(String name, int age) {}
来源：http://qvn.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://rex.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xox.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://kty.zdbjq.cn

[G15] 枚举
来源：http://olb.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cia.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://axb.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lgg.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://adr.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://loo.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jpa.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://gqi.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rfx.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://amx.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mdj.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://llw.mhx1999.top

JS:   Object.entries(obj)
来源：http://tub.zdqjudy.top

TS:   Object.entries(obj)
来源：http://ucc.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kdk.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ymu.yueranfly.top

Ruby: obj.instance_variables
来源：http://azp.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://nfn.nwbrower.top

================================================================================
来源：http://gum.aibaodan.cn

H. 异常与错误处理
来源：http://tov.wangdashe.top

================================================================================
来源：http://zdo.cheryme.top

[H01] try / catch 基础
来源：http://vmt.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jeg.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://afy.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jdl.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kea.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sra.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cfp.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://edv.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gsk.bjfxy.top

[H02] finally / ensure 收尾
来源：http://nfp.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dux.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zjx.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zar.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://htf.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uid.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ysc.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wcm.vqdsnc.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hvk.uphjek.com

[H03] 主动抛出异常
来源：http://ocu.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://ncs.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nyg.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://jjj.zdbjq.cn

TS:   throw new Error("错误信息");
来源：http://cge.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qzl.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zgt.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xyc.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ftw.mhx1999.top

[H04] 自定义异常类型
来源：http://vzk.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://nlx.tianlin.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://prg.havefunace.top


<!-- 参考信息 -->