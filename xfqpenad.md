代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oct.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://buu.haohaochexian.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wtk.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rut.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://ccl.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://swd.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rkt.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vph.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gav.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iyg.fanxiaobao.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hzu.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://dvb.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://flb.yonumen.top

================================================================================
来源：http://zon.ydzc1.top

F. 文件与目录
来源：http://qey.hnxiangtu.top

================================================================================
来源：http://nph.sufxvd.cn

[F01] 读取整个文件
来源：http://wyj.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mxd.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://qgz.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://siv.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ugv.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cdh.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fnn.cashguo.top

Ruby: File.read("a.txt")
来源：http://maz.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://hsj.chenjidiqi.icu

[F02] 逐行读取文件
来源：http://bgn.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rmw.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgy.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jiz.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xfm.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kta.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qys.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dus.52xcode.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cii.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://ytv.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bvr.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ymv.sufxvd.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fwa.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://efj.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cdw.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uqd.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://vrv.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vle.shangyingyoupin.top

[F04] 追加写入文件
来源：http://rzp.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ved.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uuy.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxs.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfc.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dbh.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wdx.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://elc.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kxw.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://zhp.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qpd.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://eif.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://puy.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://xdl.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ush.zdqjudy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jid.birdmap.top

Ruby: File.exist?("a.txt")
来源：http://hno.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://kgx.kuanghao11.cn

[F06] 删除文件
来源：http://qmt.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://oev.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://sgc.hnxiangtu.top

JS:   fs.unlinkSync("a.txt")
来源：http://enh.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cwc.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ctr.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://mot.yj20258.top

Ruby: File.delete("a.txt")
来源：http://lul.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://swg.tarul.cn

[F07] 创建目录（含多级）
来源：http://ogc.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yqf.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uui.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbq.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iej.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://swo.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wgg.zhijiandao.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://veu.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sbn.ydzc1.top

[F08] 遍历目录
来源：http://mgm.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://elp.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://scg.zhongyouzk.top

JS:   fs.readdirSync("dir")
来源：http://jed.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://tzn.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hcq.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxn.cucudq.cn

Ruby: Dir.children("dir")
来源：http://jbp.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://fsn.wangshuangyany.cn

[F09] 获取文件大小
来源：http://vqw.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://utc.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://omb.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://ltf.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://kou.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://noh.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hdf.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://csk.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://noc.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://ulu.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rjg.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wry.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mhp.epnwcf.com

TS:   path.extname("a.txt")
来源：http://vkw.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rqv.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kjr.jyoumei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pza.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eol.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://any.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dwh.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wgm.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vkg.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ttn.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://due.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://scl.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uro.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cxr.fanxiaobao.xyz

[F12] CSV 读写
来源：http://rjl.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oqh.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dpk.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xvm.ywan-chungtsiang.top

TS:   // 同上
来源：http://nfv.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dfc.shuidangran.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rnt.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://biu.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://kwc.ivvv.top

================================================================================
来源：http://ioj.bbcook.cn

G. 面向对象
来源：http://szi.redwolf501.top

================================================================================
来源：http://usn.dianchejie.cn

[G01] 定义类
来源：http://jps.c1oappe.top

Py:   class User: pass
来源：http://vxk.jinghuilouyu.cn

PHP:  class User {}
来源：http://eln.mhx1999.top

JS:   class User {}
来源：http://mms.snrcjt.cn

TS:   class User { name: string = ""; }
来源：http://iim.vehdjk.com

Java: class User {}
来源：http://wny.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://vzf.mhx1999.top

Ruby: class User; end
来源：http://eqq.zhiwuduotai.top

C#:   class User {}
来源：http://ngt.sufxvd.cn

[G02] 构造函数
来源：http://ycg.kuanghao11.cn

Py:   def __init__(self, name): self.name = name
来源：http://que.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://fhv.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://rdy.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://gib.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://ing.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eiw.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://wia.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://obs.gaohongyu789.top

[G03] 实例属性
来源：http://ili.wangdashe.top

Py:   self.name = "x"
来源：http://hkg.svipenyu.cn

PHP:  public string $name = "x";
来源：http://ajr.52xcode.cn

JS:   this.name = "x";
来源：http://zle.hywenlv.cn

TS:   name: string = "x";
来源：http://ztj.hcnkem.com

Java: private String name;
来源：http://rms.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rmo.jqgfzy.top

Ruby: @name = "x"
来源：http://yoh.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://qhr.yanxiufei.cn

[G04] 定义方法
来源：http://mwe.fehbvm.com

Py:   def greet(self): return self.name
来源：http://qmy.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bta.daria6918.cn

JS:   greet() { return this.name; }
来源：http://tay.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://mol.ppjwa.cn

Java: String greet() { return name; }
来源：http://fwq.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kum.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://eym.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://xkj.jqgufenzy.top

[G05] 继承
来源：http://fwv.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://wyg.yj20258888.top

PHP:  class Admin extends User {}
来源：http://yyo.guannengcc.top

JS:   class Admin extends User {}
来源：http://uys.dashuyun.cn

TS:   class Admin extends User {}
来源：http://jzf.smart0.xyz

Java: class Admin extends User {}
来源：http://vsg.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dxx.sufxvd.cn

Ruby: class Admin < User; end
来源：http://qlk.sjlbkw.cn

C#:   class Admin : User {}
来源：http://pdu.birdmap.top

[G06] 重写方法
来源：http://cvh.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://ctv.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mqo.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://shk.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://ywg.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://nxa.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wpk.hywenlv.cn

Ruby: def greet; "admin"; end
来源：http://ihl.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://kly.yuanzhike.top

[G07] 调用父类方法
来源：http://yfz.andypj.xyz

Py:   super().greet()
来源：http://nme.epnwcf.com

PHP:  parent::greet();
来源：http://eow.sxryk.cn

JS:   super.greet();
来源：http://lss.jqgfzy.top

TS:   super.greet();
来源：http://xvk.tianlin.xyz

Java: super.greet();
来源：http://qvy.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kco.yj202588.top

Ruby: super
来源：http://hts.guowangkeji.top

C#:   base.Greet();
来源：http://pdq.jqgfzy.top

[G08] 静态方法与属性
来源：http://qiz.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://epj.yuxming.cn

PHP:  public static function f() {}
来源：http://vjy.chenlongwang.top

JS:   static f() {}
来源：http://zul.jqgufenzy.top

TS:   static f(): void {}
来源：http://yds.ydjk.org.cn

Java: static void f() {}
来源：http://lun.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xyy.jinqigfzy.top

Ruby: def self.f; end
来源：http://lir.daria6918.cn

C#:   public static void F() {}
来源：http://cbp.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://phi.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://gmw.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://luw.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ajz.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://whr.yueranfly.top

Java: interface Shape { double area(); }
来源：http://dun.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://oxs.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uyx.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://vhn.hongshengwenyu.top

[G10] 访问控制
来源：http://dug.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://nna.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://vpf.fktsv.cn

JS:   #private 字段；其余公开
来源：http://dzg.shanyushiyangtech.top

TS:   public / protected / private
来源：http://htj.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://mvf.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvg.jinqigufen.top

Ruby: public / protected / private
来源：http://wyp.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://ywr.ywan-chungtsiang.top

[G11] getter / setter
来源：http://jso.smart0.xyz

Py:   @property 与 @x.setter
来源：http://vki.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uwe.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://rah.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://kuh.yfazqb.com

Java: public String getName() { return name; }
来源：http://zef.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ilx.yueranfly.top

Ruby: attr_accessor :name
来源：http://zxp.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://pjq.ppjwa.cn

[G12] 对象转字符串
来源：http://gjl.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://yce.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lks.xylfe.cn

JS:   toString() { return this.name; }
来源：http://usi.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://tvf.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://yda.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xsr.tanke756.top

Ruby: def to_s; @name; end
来源：http://qyu.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://dym.ctjpmb.com

[G13] 判断对象类型
来源：http://ryt.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://qul.dianchejie.cn

PHP:  $u instanceof User
来源：http://ntu.hnxiangtu.top

JS:   u instanceof User
来源：http://sok.svipenyu.cn

TS:   u instanceof User
来源：http://pkh.zhijiandao.cn

Java: u instanceof User
来源：http://ukw.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yok.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://xns.hfpthk.cn

C#:   u is User
来源：http://uza.316326.xyz

[G14] 数据类 / record
来源：http://xta.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vyj.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://wee.ivvv.top

JS:   // 无内置：普通类或对象字面量
来源：http://bew.sweek.top

TS:   type User = { name: string; age: number };
来源：http://fpe.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://uvj.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://duj.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oou.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://qag.zdqjudy.top

[G15] 枚举
来源：http://edy.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qfc.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dnc.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://orn.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dpq.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://vju.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ihr.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://cid.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dnm.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://omw.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jmk.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://ynd.chenzaomai.com

JS:   Object.entries(obj)
来源：http://myo.tianlin.xyz

TS:   Object.entries(obj)
来源：http://jpv.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jeb.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vex.tanke756.top

Ruby: obj.instance_variables
来源：http://knl.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://jsj.hywenlv.cn

================================================================================
来源：http://vhl.svipenyu.cn

H. 异常与错误处理
来源：http://hce.tian-w.cn

================================================================================
来源：http://bgl.yuanzhike.top

[H01] try / catch 基础
来源：http://zpj.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uhm.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bzo.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://duo.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blk.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ibx.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dzg.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sjf.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ikx.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://utu.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yvg.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://nzr.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ikv.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mlt.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://jra.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lfw.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://npn.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iog.shzxlz.cn

[H03] 主动抛出异常
来源：http://avf.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://oyc.pengpengdd.cyou

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hwx.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://ven.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://ykd.bbcook.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://crl.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zfl.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nio.pycfn.com


<!-- 参考信息 -->