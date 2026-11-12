代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cie.jinqigufen.top

Go:   // 按 rune 判断长度后截断
来源：http://eto.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://buu.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://upq.meibo888.top

[E22] 字节长度与字符长度
来源：http://rih.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qaa.52xcode.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbt.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oyk.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mzu.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kqh.wangdashe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dyl.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://rqo.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qfe.hnqzz.top

================================================================================
来源：http://wiw.cucudq.cn

F. 文件与目录
来源：http://mge.havefunace.top

================================================================================
来源：http://ybj.jiagoushi.top

[F01] 读取整个文件
来源：http://tsb.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ogf.ydzc1.top

PHP:  file_get_contents("a.txt");
来源：http://vfk.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lyf.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bsv.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kku.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fyd.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://hpp.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://frl.zdbjq.cn

[F02] 逐行读取文件
来源：http://pau.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvn.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rlf.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pze.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cng.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ytk.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kdc.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rtn.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dlu.pycfn.com

[F03] 写入文件（覆盖）
来源：http://chg.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://trf.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hkw.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qpf.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iep.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iaz.52xcode.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://egw.zdbjq.cn

Ruby: File.write("a.txt", "hi")
来源：http://xkx.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://taf.jianghu66.top

[F04] 追加写入文件
来源：http://hpa.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iab.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xqm.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgs.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejl.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ytm.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zeu.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lce.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gpg.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://dby.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pab.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://uzv.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://alh.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://dab.hcnkem.com

Java: Files.exists(Path.of("a.txt"))
来源：http://uzt.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hbj.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://kbc.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://pil.andypj.xyz

[F06] 删除文件
来源：http://tpc.hesvh.cn

Py:   os.remove("a.txt")
来源：http://gon.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://psa.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://ukr.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dtn.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gsi.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://zog.zhoulong.xyz

Ruby: File.delete("a.txt")
来源：http://ofo.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://jri.mhx1999.top

[F07] 创建目录（含多级）
来源：http://gzr.yangfankeji.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://utb.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://msh.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vmv.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fil.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uwt.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hvd.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sfo.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://awn.zhongyouzk.top

[F08] 遍历目录
来源：http://otn.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cjt.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hkg.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://ter.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://emi.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://czj.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ews.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://afz.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://zar.zhengqikj.top

[F09] 获取文件大小
来源：http://uaz.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://jld.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://zdo.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://pei.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://ani.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://veq.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://suf.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://jbb.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://hsl.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://mjh.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rsx.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bwg.ywan-chungtsiang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bod.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://cfh.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://exm.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://geq.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxr.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tri.jiagoushi.top

[F11] 复制与移动文件
来源：http://ahv.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xwx.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://drg.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bcv.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://msp.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nrv.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oka.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://acv.hesvh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bwe.tarul.cn

[F12] CSV 读写
来源：http://whi.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zhv.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cfn.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rdi.yfazqb.com

TS:   // 同上
来源：http://ugx.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pde.yangfankeji.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tnr.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sok.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fav.zdqjudy.top

================================================================================
来源：http://ggr.52xcode.cn

G. 面向对象
来源：http://sqr.316326.xyz

================================================================================
来源：http://psq.haohaochexian.top

[G01] 定义类
来源：http://qde.hywenlv.cn

Py:   class User: pass
来源：http://kek.sufxvd.cn

PHP:  class User {}
来源：http://dta.zhoulong.xyz

JS:   class User {}
来源：http://zds.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://jfk.ybcxt.top

Java: class User {}
来源：http://hex.xinyue.icu

Go:   type User struct { Name string }
来源：http://wcl.nanxinkj.top

Ruby: class User; end
来源：http://two.jianghu66.top

C#:   class User {}
来源：http://ufe.jlsjyb.cn

[G02] 构造函数
来源：http://xpe.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://hty.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://dkx.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://wct.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://hjd.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://dwb.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hbt.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://hkh.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://ndg.nanxuanxn.top

[G03] 实例属性
来源：http://bim.vqdsnc.cn

Py:   self.name = "x"
来源：http://qiv.yj20258.top

PHP:  public string $name = "x";
来源：http://tzs.zdbjq.cn

JS:   this.name = "x";
来源：http://vsr.bbcook.cn

TS:   name: string = "x";
来源：http://vxq.hfpthk.cn

Java: private String name;
来源：http://ygw.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qcw.yfazqb.com

Ruby: @name = "x"
来源：http://ziu.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://enb.yfazqb.com

[G04] 定义方法
来源：http://srp.xziqi.cn

Py:   def greet(self): return self.name
来源：http://erx.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sxw.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://zqh.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://zun.sweek.top

Java: String greet() { return name; }
来源：http://kmr.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cik.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://ssy.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://axm.hfpthk.cn

[G05] 继承
来源：http://lhq.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://meg.ivvv.top

PHP:  class Admin extends User {}
来源：http://kqk.dianchejie.cn

JS:   class Admin extends User {}
来源：http://cyv.yuanzhike.top

TS:   class Admin extends User {}
来源：http://luq.shzxlz.cn

Java: class Admin extends User {}
来源：http://rkc.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tiy.fengsongda.top

Ruby: class Admin < User; end
来源：http://bpr.haohaochexian.top

C#:   class Admin : User {}
来源：http://adn.ehwqpu.com

[G06] 重写方法
来源：http://jqz.meibo888.top

Py:   def greet(self): return "admin"
来源：http://ddp.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kne.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://xpf.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://yja.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://gzi.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ksn.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://dzp.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://wgk.jqgfzy.top

[G07] 调用父类方法
来源：http://nio.tian-w.cn

Py:   super().greet()
来源：http://hhe.yangfankeji.com

PHP:  parent::greet();
来源：http://jfk.hysaishi.cn

JS:   super.greet();
来源：http://njx.gaohongyu789.top

TS:   super.greet();
来源：http://zfb.yonumen.top

Java: super.greet();
来源：http://vyu.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pxh.ydjk.org.cn

Ruby: super
来源：http://yfi.guannengcc.top

C#:   base.Greet();
来源：http://ldy.zycfv.cn

[G08] 静态方法与属性
来源：http://ubl.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jtf.hesvh.cn

PHP:  public static function f() {}
来源：http://vla.jinghuilouyu.cn

JS:   static f() {}
来源：http://fdo.guowangkeji.top

TS:   static f(): void {}
来源：http://nip.hnxiangtu.top

Java: static void f() {}
来源：http://qvx.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mwo.svipenyu.cn

Ruby: def self.f; end
来源：http://kae.jianghu66.top

C#:   public static void F() {}
来源：http://iav.yongpay.top

[G09] 接口 / 抽象类
来源：http://nzj.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://sex.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://lzq.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hkd.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://gal.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://xcn.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://npk.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypk.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://nds.iojbl.cn

[G10] 访问控制
来源：http://jrc.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://rvg.fktsv.cn

PHP:  public / protected / private
来源：http://hee.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://zjd.jqgufenzy.top

TS:   public / protected / private
来源：http://fpk.uphjek.com

Java: public / protected / private / 默认包级
来源：http://fpe.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gzs.hongshengwenyu.top

Ruby: public / protected / private
来源：http://bbc.guowangkeji.top

C#:   public / protected / private / internal
来源：http://tkn.zdqjudy.top

[G11] getter / setter
来源：http://aac.fengsongda.top

Py:   @property 与 @x.setter
来源：http://jtc.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://emf.fehbvm.com

JS:   get name() { return this._name; }
来源：http://upv.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://imr.zdqjudy.top

Java: public String getName() { return name; }
来源：http://tyl.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tll.yfazqb.com

Ruby: attr_accessor :name
来源：http://rza.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://owc.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://pig.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://vcp.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ied.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://iig.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://yyt.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://ojy.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kvu.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://aga.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://rtu.shangyingyoupin.top

[G13] 判断对象类型
来源：http://wnm.dianchejie.cn

Py:   isinstance(u, User)
来源：http://kto.jiagoushi.top

PHP:  $u instanceof User
来源：http://xxd.xuanzx.com

JS:   u instanceof User
来源：http://jzs.xuetiantiany.cn

TS:   u instanceof User
来源：http://zow.meibo888.top

Java: u instanceof User
来源：http://mev.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rxw.c1oappe.top

Ruby: u.is_a?(User)
来源：http://gjr.jlsjyb.cn

C#:   u is User
来源：http://rqa.ctjpmb.com

[G14] 数据类 / record
来源：http://emu.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lfu.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://bwg.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mxk.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://jai.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://okf.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://nfr.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ama.jlsjyb.cn

C#:   record User(string Name, int Age);
来源：http://csl.havefunace.top

[G15] 枚举
来源：http://opf.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jfg.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yee.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://swn.yj20258.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ziz.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://fvi.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dcv.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://puh.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xxy.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://ksg.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kwa.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://ayg.andypj.xyz

JS:   Object.entries(obj)
来源：http://tlo.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://lcp.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://auz.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wjt.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://bok.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://rpx.yuxming.cn

================================================================================
来源：http://yde.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://doo.dashuyun.cn

================================================================================
来源：http://bth.guowangkeji.top

[H01] try / catch 基础
来源：http://uil.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kdl.jlsjyb.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tlf.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nas.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ejr.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jqr.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zcd.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sve.guannengcc.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kuw.hesvh.cn

[H02] finally / ensure 收尾
来源：http://ikr.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://god.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ejw.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wpb.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vio.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://mvx.gogol.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ywg.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mdo.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://afj.quarkkingdee.top

[H03] 主动抛出异常
来源：http://aei.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://zev.sjlbkw.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://epf.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://jqg.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://yvq.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://cra.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jec.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://vet.wangshuangyany.cn


<!-- 参考信息 -->