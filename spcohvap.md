代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yha.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blg.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://swt.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qru.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qki.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://ugw.yangfankeji.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://teg.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qzh.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://sit.sufxvd.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gfx.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yyy.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mdb.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nax.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xrj.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dmd.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://ebp.chenzaomai.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jue.yueranfly.top

================================================================================
来源：http://sau.aibaodan.cn

F. 文件与目录
来源：http://mqk.52xcode.cn

================================================================================
来源：http://djf.fehbvm.com

[F01] 读取整个文件
来源：http://xgo.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rrl.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://vcy.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dqu.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://haw.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rqg.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pkm.52xcode.cn

Ruby: File.read("a.txt")
来源：http://vfj.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://qmm.sjlbkw.cn

[F02] 逐行读取文件
来源：http://qep.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mkv.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iza.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://awp.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pqb.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zgu.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pid.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xpc.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cgx.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://qmk.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uic.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://lew.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyw.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wmg.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ese.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxj.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://hsm.kuanghao11.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://khn.yvedp.cn

[F04] 追加写入文件
来源：http://aig.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ztq.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cxp.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjj.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ite.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uyu.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zgm.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ndm.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wps.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://sck.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pgn.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://mvw.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://zvs.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://vdz.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://axm.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xdl.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://jni.zycfv.cn

C#:   File.Exists("a.txt")
来源：http://pna.yangfankeji.com

[F06] 删除文件
来源：http://jbc.gzhubu.top

Py:   os.remove("a.txt")
来源：http://zlv.sxryk.cn

PHP:  unlink("a.txt");
来源：http://vsr.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hsf.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://kna.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://otv.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://pvx.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://enx.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://vlb.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://hth.tianlin.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://asa.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bvw.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mor.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yba.shuidangran.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uiz.fengsongda.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hqq.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xly.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ory.guannengcc.top

[F08] 遍历目录
来源：http://gtu.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wzh.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kiu.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://bzr.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://lde.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://auy.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yhy.tian-w.cn

Ruby: Dir.children("dir")
来源：http://rls.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://ycb.wangdashe.top

[F09] 获取文件大小
来源：http://shs.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://jrf.cucudq.cn

PHP:  filesize("a.txt");
来源：http://zhf.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://vcw.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://otb.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://sfk.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://snp.aizwys.cn

Ruby: File.size("a.txt")
来源：http://crz.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://spj.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://xlj.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wxa.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dwi.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pij.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://sln.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eza.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xjb.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ggw.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jaq.redwolf501.top

[F11] 复制与移动文件
来源：http://fxe.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mph.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zik.316326.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://irq.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kxh.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cpw.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gej.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kco.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cbq.daria6918.cn

[F12] CSV 读写
来源：http://cmi.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zsq.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vmu.snrcjt.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://php.yuanzhike.top

TS:   // 同上
来源：http://ymr.fktsv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zwo.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qgg.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://udu.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xvo.ybcxt.top

================================================================================
来源：http://zcr.svipenyu.cn

G. 面向对象
来源：http://bpy.jyoumei.cn

================================================================================
来源：http://kuh.iojbl.cn

[G01] 定义类
来源：http://ypn.ydzc1.top

Py:   class User: pass
来源：http://tgf.aibaodan.cn

PHP:  class User {}
来源：http://qld.sjlbkw.cn

JS:   class User {}
来源：http://obc.cashguo.top

TS:   class User { name: string = ""; }
来源：http://juz.guannengcc.top

Java: class User {}
来源：http://tyz.xinyue.icu

Go:   type User struct { Name string }
来源：http://xyn.shuidangran.top

Ruby: class User; end
来源：http://lii.ivvv.top

C#:   class User {}
来源：http://wkd.ydjk.org.cn

[G02] 构造函数
来源：http://eof.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://npa.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://yhy.gzhubu.top

JS:   constructor(name) { this.name = name; }
来源：http://nsn.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://gcl.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://szk.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://moz.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://ydq.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://sud.haohaochexian.top

[G03] 实例属性
来源：http://nnu.iojbl.cn

Py:   self.name = "x"
来源：http://ega.yfazqb.com

PHP:  public string $name = "x";
来源：http://ltb.tianlin.xyz

JS:   this.name = "x";
来源：http://icw.gaohongyu789.top

TS:   name: string = "x";
来源：http://mfv.fengsongda.top

Java: private String name;
来源：http://cje.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ikc.bjfxy.top

Ruby: @name = "x"
来源：http://hrl.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://mjj.iojbl.cn

[G04] 定义方法
来源：http://xgr.yvedp.cn

Py:   def greet(self): return self.name
来源：http://ziy.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bep.redwolf501.top

JS:   greet() { return this.name; }
来源：http://bur.chenjidiqi.icu

TS:   greet(): string { return this.name; }
来源：http://abv.jiagoushi.top

Java: String greet() { return name; }
来源：http://yiv.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eiy.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://smz.tanke756.top

C#:   public string Greet() => Name;
来源：http://pmm.yueranfly.top

[G05] 继承
来源：http://ncd.nanxinkj.top

Py:   class Admin(User): pass
来源：http://xro.hnqzz.top

PHP:  class Admin extends User {}
来源：http://eoi.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://ogu.shzxlz.cn

TS:   class Admin extends User {}
来源：http://vdt.fehbvm.com

Java: class Admin extends User {}
来源：http://gzw.zhengqikj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bku.dashuyun.cn

Ruby: class Admin < User; end
来源：http://kdt.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://jrx.shuidangran.top

[G06] 重写方法
来源：http://wsr.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://vag.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yhe.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://zsx.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://uxl.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://xsc.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vud.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://nta.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://vae.sxryk.cn

[G07] 调用父类方法
来源：http://xqh.zhixingplan.top

Py:   super().greet()
来源：http://tzh.yfazqb.com

PHP:  parent::greet();
来源：http://ots.haohaochexian.top

JS:   super.greet();
来源：http://vjk.ybcxt.top

TS:   super.greet();
来源：http://eed.birdmap.top

Java: super.greet();
来源：http://icx.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zkv.zdbjq.cn

Ruby: super
来源：http://gaf.chenzaomai.com

C#:   base.Greet();
来源：http://jhk.jinqigfzy.top

[G08] 静态方法与属性
来源：http://rkq.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eep.hammf.cn

PHP:  public static function f() {}
来源：http://gso.shanyushiyangtech.top

JS:   static f() {}
来源：http://zjm.wangdashe.top

TS:   static f(): void {}
来源：http://pao.yj20258.top

Java: static void f() {}
来源：http://jrl.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://laz.dashuyun.cn

Ruby: def self.f; end
来源：http://jek.cucudq.cn

C#:   public static void F() {}
来源：http://hnp.ivvv.top

[G09] 接口 / 抽象类
来源：http://wfx.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://vri.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://nwl.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rln.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://jag.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://xwi.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://wra.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://csa.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://jdm.hnqzz.top

[G10] 访问控制
来源：http://vug.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://cro.ivvv.top

PHP:  public / protected / private
来源：http://xky.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://fyb.xinyue.icu

TS:   public / protected / private
来源：http://avu.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://muy.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qlq.cdnleiting.top

Ruby: public / protected / private
来源：http://nkh.jianghu66.top

C#:   public / protected / private / internal
来源：http://ydv.c1oappe.top

[G11] getter / setter
来源：http://jij.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://wrv.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bbs.shuidangran.top

JS:   get name() { return this._name; }
来源：http://ola.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://pzn.iojbl.cn

Java: public String getName() { return name; }
来源：http://yty.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kxv.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://hur.epnwcf.com

C#:   public string Name { get; set; }
来源：http://iep.pengpengdd.cyou

[G12] 对象转字符串
来源：http://aei.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://bey.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mos.tarul.cn

JS:   toString() { return this.name; }
来源：http://nnf.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://wdp.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://ccn.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://sli.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://tde.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://oqv.chenjidiqi.icu

[G13] 判断对象类型
来源：http://gaz.haohaochexian.top

Py:   isinstance(u, User)
来源：http://dcu.316326.xyz

PHP:  $u instanceof User
来源：http://scq.iojbl.cn

JS:   u instanceof User
来源：http://fwm.fengsongda.top

TS:   u instanceof User
来源：http://whe.ehwqpu.com

Java: u instanceof User
来源：http://jyi.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jal.zhiwuduotai.top

Ruby: u.is_a?(User)
来源：http://qud.dianchejie.cn

C#:   u is User
来源：http://myj.jiagoushi.top

[G14] 数据类 / record
来源：http://fwm.jinghuilouyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lzu.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://jhm.yueranfly.top

JS:   // 无内置：普通类或对象字面量
来源：http://kpw.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://xtu.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://cmb.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://wpt.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jwn.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://hkh.dianchejie.cn

[G15] 枚举
来源：http://hyx.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cip.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vik.iojbl.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ivv.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jdv.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://cng.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bdd.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://bsz.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nmq.pengpengdd.cyou

[G16] 对象转数组 / 字典
来源：http://rsk.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ouc.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://igd.nwbrower.top

JS:   Object.entries(obj)
来源：http://coh.pycfn.com

TS:   Object.entries(obj)
来源：http://cjr.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cuh.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tno.yuanzhike.top

Ruby: obj.instance_variables
来源：http://ybl.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://uvu.jqgufenzy.top

================================================================================
来源：http://blp.haohaochexian.top

H. 异常与错误处理
来源：http://huv.daria6918.cn

================================================================================
来源：http://ehu.dianchejie.cn

[H01] try / catch 基础
来源：http://ofr.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hdo.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://key.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozy.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wuc.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://knb.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ohv.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wqu.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jet.iojbl.cn

[H02] finally / ensure 收尾
来源：http://gfl.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://see.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xci.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zxf.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lzw.jianghu66.top

Java: try { f(); } finally { cleanup(); }
来源：http://lcd.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dzl.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nxt.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tax.zhongyouzk.top

[H03] 主动抛出异常
来源：http://dib.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://pqv.chenzaomai.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://plx.meibo888.top

JS:   throw new Error("错误信息");
来源：http://zjw.chenzaomai.com


<!-- 参考信息 -->