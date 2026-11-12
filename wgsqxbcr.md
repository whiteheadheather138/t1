代发 wailian999

[E22] 字节长度与字符长度
来源：http://etk.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iao.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygc.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vts.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vlk.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yab.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mhr.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://spf.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zmu.ydzc1.top

================================================================================
来源：http://ggy.shangyingyoupin.top

F. 文件与目录
来源：http://zjb.zhaomingkeji.xyz

================================================================================
来源：http://qek.nwbrower.top

[F01] 读取整个文件
来源：http://iut.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lrz.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://vnt.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://czj.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://reo.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wqb.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bqc.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://oky.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://cde.zhengqikj.top

[F02] 逐行读取文件
来源：http://nwv.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://znm.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rys.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xoq.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://peh.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zoy.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bel.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eoc.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fnl.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://mkf.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pad.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kju.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnj.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dye.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kmu.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jzv.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://ohg.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pnk.9152youxi.cn

[F04] 追加写入文件
来源：http://kue.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://psx.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mcn.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qko.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyf.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vvg.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yuz.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qns.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aey.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://sqw.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lra.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://ioh.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://idc.bbcook.cn

TS:   fs.existsSync("a.txt")
来源：http://byq.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://oee.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xby.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://svh.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://kta.chenzaomai.com

[F06] 删除文件
来源：http://vgi.daxiang520.top

Py:   os.remove("a.txt")
来源：http://rcs.daria6918.cn

PHP:  unlink("a.txt");
来源：http://hva.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hdb.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://bqx.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ljz.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://ebe.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://tjb.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://sll.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://inj.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wje.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bep.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgc.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lap.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gad.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vot.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pwl.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qxt.hywenlv.cn

[F08] 遍历目录
来源：http://dds.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rpn.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mxu.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://gew.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://dol.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qqi.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zqb.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://cip.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://evj.zhiwuduotai.top

[F09] 获取文件大小
来源：http://fel.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://tqs.wangdashe.top

PHP:  filesize("a.txt");
来源：http://vwr.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://eqn.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://eau.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://ley.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ekp.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://hxt.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://sjs.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://ikf.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fzq.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jsc.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://boo.yuxming.cn

TS:   path.extname("a.txt")
来源：http://xve.zhongyouzk.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iba.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zsc.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tdf.zdbjq.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nyb.zdqjudy.top

[F11] 复制与移动文件
来源：http://ttm.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nhs.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hdl.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://woi.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frt.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rlw.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dnf.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://moc.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wdw.snrcjt.cn

[F12] CSV 读写
来源：http://pkv.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qki.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cck.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vxz.guannengcc.top

TS:   // 同上
来源：http://btd.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ccv.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hsl.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hxy.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iau.daxiang520.top

================================================================================
来源：http://pid.pycfn.com

G. 面向对象
来源：http://pqo.nwbrower.top

================================================================================
来源：http://qdj.zhengqikj.top

[G01] 定义类
来源：http://chi.zhaomingkeji.xyz

Py:   class User: pass
来源：http://vrv.smart0.xyz

PHP:  class User {}
来源：http://ldn.pengpengdd.cyou

JS:   class User {}
来源：http://wen.tarul.cn

TS:   class User { name: string = ""; }
来源：http://ycx.chenlongwang.top

Java: class User {}
来源：http://igl.xinyue.icu

Go:   type User struct { Name string }
来源：http://szv.feifeiyinyue.top

Ruby: class User; end
来源：http://rws.zdbjq.cn

C#:   class User {}
来源：http://dgh.jqgufenzy.top

[G02] 构造函数
来源：http://xlm.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://ydo.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://lrj.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://icj.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://fgr.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://cda.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eix.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://okw.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://vig.yueranfly.top

[G03] 实例属性
来源：http://jwi.yfazqb.com

Py:   self.name = "x"
来源：http://zum.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://byg.zdqjudy.top

JS:   this.name = "x";
来源：http://yal.guannengcc.top

TS:   name: string = "x";
来源：http://pgg.guowangkeji.top

Java: private String name;
来源：http://pfa.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dqe.nwbrower.top

Ruby: @name = "x"
来源：http://fzx.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://pvv.ywan-chungtsiang.top

[G04] 定义方法
来源：http://fph.cucudq.cn

Py:   def greet(self): return self.name
来源：http://eny.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pqu.yj202588.top

JS:   greet() { return this.name; }
来源：http://lwj.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://ppo.guannengcc.top

Java: String greet() { return name; }
来源：http://ksv.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://glp.daxiang520.top

Ruby: def greet; @name; end
来源：http://eaf.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://uay.sweek.top

[G05] 继承
来源：http://diy.yueranfly.top

Py:   class Admin(User): pass
来源：http://xpf.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://qzz.meibo888.top

JS:   class Admin extends User {}
来源：http://hwd.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://qfa.shuidangran.top

Java: class Admin extends User {}
来源：http://gva.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mld.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://yqq.snrcjt.cn

C#:   class Admin : User {}
来源：http://jdy.vehdjk.com

[G06] 重写方法
来源：http://gvo.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://hgb.shanyushiyangtech.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ngr.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://vbm.dashuyun.cn

TS:   greet(): string { return "admin"; }
来源：http://scz.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://qpr.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xvk.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://xxl.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://wbu.ehwqpu.com

[G07] 调用父类方法
来源：http://did.zhixingplan.top

Py:   super().greet()
来源：http://jmp.hammf.cn

PHP:  parent::greet();
来源：http://umg.gotoacloud.top

JS:   super.greet();
来源：http://kcb.nwbrower.top

TS:   super.greet();
来源：http://sdu.ppjwa.cn

Java: super.greet();
来源：http://ipy.nanxinkj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kwr.ctjpmb.com

Ruby: super
来源：http://fjv.ehwqpu.com

C#:   base.Greet();
来源：http://nsg.birdmap.top

[G08] 静态方法与属性
来源：http://nxm.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://thg.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://qij.hnqzz.top

JS:   static f() {}
来源：http://djo.haohaochexian.top

TS:   static f(): void {}
来源：http://yoa.guannengcc.top

Java: static void f() {}
来源：http://ija.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://snk.yongpay.top

Ruby: def self.f; end
来源：http://xmz.cqqwz.cn

C#:   public static void F() {}
来源：http://fuf.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://jod.pengpengdd.cyou

Py:   from abc import ABC, abstractmethod
来源：http://bvy.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dho.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kyf.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://paa.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://qup.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://pyx.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://shc.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://xgc.birdmap.top

[G10] 访问控制
来源：http://qhp.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://skx.zhengqikj.top

PHP:  public / protected / private
来源：http://pqc.sxryk.cn

JS:   #private 字段；其余公开
来源：http://nht.jinqigufen.top

TS:   public / protected / private
来源：http://ujf.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://xju.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sol.xuetiantiany.cn

Ruby: public / protected / private
来源：http://zuv.havefunace.top

C#:   public / protected / private / internal
来源：http://wfz.jinqigufen.top

[G11] getter / setter
来源：http://mkh.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://kzt.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zcl.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://mfb.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://nsx.bbcook.cn

Java: public String getName() { return name; }
来源：http://quo.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ltr.havefunace.top

Ruby: attr_accessor :name
来源：http://kie.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://arr.birdmap.top

[G12] 对象转字符串
来源：http://ezj.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://qez.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yvb.havefunace.top

JS:   toString() { return this.name; }
来源：http://uhy.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://hbv.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://fbg.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://whr.fktsv.cn

Ruby: def to_s; @name; end
来源：http://pdz.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://tvi.shangyingyoupin.top

[G13] 判断对象类型
来源：http://nqx.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://vxc.chenzaomai.com

PHP:  $u instanceof User
来源：http://pnv.guowangkeji.top

JS:   u instanceof User
来源：http://dxz.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://gue.gzhubu.top

Java: u instanceof User
来源：http://eqr.meibo888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ibf.hesvh.cn

Ruby: u.is_a?(User)
来源：http://glw.hfpthk.cn

C#:   u is User
来源：http://jkf.9152youxi.cn

[G14] 数据类 / record
来源：http://yte.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jfa.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ulp.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xna.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://wyt.hcnkem.com

Java: record User(String name, int age) {}
来源：http://iyf.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://bdy.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pjh.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://rmz.gaohongyu789.top

[G15] 枚举
来源：http://dyd.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mwj.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tln.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://olp.ppjwa.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vdy.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://xos.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jln.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://khj.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ugg.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://jae.yongpay.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gby.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://ndl.cashguo.top

JS:   Object.entries(obj)
来源：http://wiv.ppjwa.cn

TS:   Object.entries(obj)
来源：http://ihn.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rls.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mif.haohaochexian.top

Ruby: obj.instance_variables
来源：http://inx.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://was.jqgufenzy.top

================================================================================
来源：http://zda.shzxlz.cn

H. 异常与错误处理
来源：http://qhr.iojbl.cn

================================================================================
来源：http://kga.nanxuanxn.top

[H01] try / catch 基础
来源：http://swi.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yvt.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oaq.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bkn.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aes.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hhq.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://seq.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pmv.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xxb.shanyushiyangkeji.top

[H02] finally / ensure 收尾
来源：http://hlo.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://lay.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kbv.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://otc.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oqg.feifeiyinyue.top

Java: try { f(); } finally { cleanup(); }
来源：http://wvb.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsv.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gta.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://xik.meibo888.top

[H03] 主动抛出异常
来源：http://fnm.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://tkc.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fjw.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://sth.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://swc.quarkkingdee.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jqm.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://trk.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sbh.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hza.yvedp.cn

[H04] 自定义异常类型
来源：http://kij.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://tjp.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://xbn.aibaodan.cn


<!-- 参考信息 -->