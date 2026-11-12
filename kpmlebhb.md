代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://acu.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://qgv.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kfl.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cou.smart0.xyz

[E22] 字节长度与字符长度
来源：http://rli.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pto.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pmk.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghv.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qln.yj20258888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mnl.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pub.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://uvw.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://exu.yuanzhike.top

================================================================================
来源：http://ufm.iojbl.cn

F. 文件与目录
来源：http://mto.feifeiyinyue.top

================================================================================
来源：http://hth.tian-w.cn

[F01] 读取整个文件
来源：http://llt.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://exk.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://rjg.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dqt.uphjek.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fzc.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://czc.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hls.jianghu66.top

Ruby: File.read("a.txt")
来源：http://ray.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://wjt.xziqi.cn

[F02] 逐行读取文件
来源：http://xqr.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kch.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://itk.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kfr.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gzn.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jsf.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://doc.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://amp.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gby.cdnleiting.top

[F03] 写入文件（覆盖）
来源：http://cvk.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://web.sxryk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vga.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rat.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vom.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zgm.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mfh.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://jiv.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aez.bjfxy.top

[F04] 追加写入文件
来源：http://pil.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qbo.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fae.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqk.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ytx.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://axr.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jjw.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jwi.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rca.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://kit.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://chb.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://rok.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://rxv.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://xiz.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://emp.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kkj.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://klb.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://kfo.fengsongda.top

[F06] 删除文件
来源：http://crs.yj20258.top

Py:   os.remove("a.txt")
来源：http://awy.andypj.xyz

PHP:  unlink("a.txt");
来源：http://mso.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://luy.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://bdb.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://buv.yonumen.top

Go:   os.Remove("a.txt")
来源：http://ihc.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://gkq.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://jgo.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://nym.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nug.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uob.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zbc.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jrf.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dhj.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cpz.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tny.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ocb.tanke756.top

[F08] 遍历目录
来源：http://ucd.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ddu.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kwy.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://jxb.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://hay.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://quz.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://sjs.yj202588.top

Ruby: Dir.children("dir")
来源：http://ieg.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://jfj.redwolf501.top

[F09] 获取文件大小
来源：http://qzb.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://hxa.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://qma.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://daj.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://vcv.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wmu.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kkx.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://eak.pycfn.com

C#:   new FileInfo("a.txt").Length
来源：http://wbg.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://cmm.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bkf.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kgo.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pjo.sxryk.cn

TS:   path.extname("a.txt")
来源：http://rpz.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jxv.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xte.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ihf.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ogo.sweek.top

[F11] 复制与移动文件
来源：http://gxx.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ttm.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://suf.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xoj.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tof.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lbi.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hqy.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hlv.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qtw.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://yzj.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jvh.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rfx.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://equ.jianghu66.top

TS:   // 同上
来源：http://eme.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zuw.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zuy.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://awq.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://log.yonumen.top

================================================================================
来源：http://wyh.yuxming.cn

G. 面向对象
来源：http://vsh.snrcjt.cn

================================================================================
来源：http://waa.snrcjt.cn

[G01] 定义类
来源：http://seq.jiagoushi.top

Py:   class User: pass
来源：http://wbe.daria6918.cn

PHP:  class User {}
来源：http://fkr.0kj1m.cn

JS:   class User {}
来源：http://rkh.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://exz.gotoacloud.top

Java: class User {}
来源：http://mab.bbcook.cn

Go:   type User struct { Name string }
来源：http://mir.fanxiaobao.xyz

Ruby: class User; end
来源：http://tgm.vqdsnc.cn

C#:   class User {}
来源：http://pud.wangdashe.top

[G02] 构造函数
来源：http://rif.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://ggp.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ljm.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://lzb.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://vdq.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://upa.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tir.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://hok.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://nou.bjfxy.top

[G03] 实例属性
来源：http://bbu.cheryme.top

Py:   self.name = "x"
来源：http://ukb.tarul.cn

PHP:  public string $name = "x";
来源：http://ltf.zycfv.cn

JS:   this.name = "x";
来源：http://btv.havefunace.top

TS:   name: string = "x";
来源：http://qbt.xingfuxueyuan.xyz

Java: private String name;
来源：http://akx.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pnt.316326.xyz

Ruby: @name = "x"
来源：http://itu.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://otu.ywan-chungtsiang.top

[G04] 定义方法
来源：http://kpi.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://qwb.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uju.316326.xyz

JS:   greet() { return this.name; }
来源：http://pka.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://ezc.gaohongyu789.top

Java: String greet() { return name; }
来源：http://nai.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kdu.dashuyun.cn

Ruby: def greet; @name; end
来源：http://vqx.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://osl.yongpay.top

[G05] 继承
来源：http://ucl.gotoacloud.top

Py:   class Admin(User): pass
来源：http://ovj.ivvv.top

PHP:  class Admin extends User {}
来源：http://vol.ydzc1.top

JS:   class Admin extends User {}
来源：http://fts.guannengcc.top

TS:   class Admin extends User {}
来源：http://ohh.xuanzx.com

Java: class Admin extends User {}
来源：http://ikh.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gde.redwolf501.top

Ruby: class Admin < User; end
来源：http://jjf.gaohongyu789.top

C#:   class Admin : User {}
来源：http://env.iojbl.cn

[G06] 重写方法
来源：http://ybv.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://lug.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tey.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://xvf.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://exn.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://hzo.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crg.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://arg.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://rmq.ivvv.top

[G07] 调用父类方法
来源：http://rtc.aibaodan.cn

Py:   super().greet()
来源：http://nuh.gzhubu.top

PHP:  parent::greet();
来源：http://coj.aizwys.cn

JS:   super.greet();
来源：http://ayp.jiagoushi.top

TS:   super.greet();
来源：http://ely.sxryk.cn

Java: super.greet();
来源：http://hus.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zrf.daxiang520.top

Ruby: super
来源：http://lzj.jlsjyb.cn

C#:   base.Greet();
来源：http://usu.redwolf501.top

[G08] 静态方法与属性
来源：http://lqu.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://poc.cdnleiting.top

PHP:  public static function f() {}
来源：http://pbl.snrcjt.cn

JS:   static f() {}
来源：http://gcv.cucudq.cn

TS:   static f(): void {}
来源：http://cxi.meibo888.top

Java: static void f() {}
来源：http://ioj.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xfz.ydjk.org.cn

Ruby: def self.f; end
来源：http://sju.pycfn.com

C#:   public static void F() {}
来源：http://lvr.sxryk.cn

[G09] 接口 / 抽象类
来源：http://lor.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://wyi.sjlbkw.cn

PHP:  interface Shape { public function area(): float; }
来源：http://aga.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ryp.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://sru.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://mot.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://sep.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yaz.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://nah.9152youxi.cn

[G10] 访问控制
来源：http://shf.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://uot.epnwcf.com

PHP:  public / protected / private
来源：http://wys.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://hug.ydjk.org.cn

TS:   public / protected / private
来源：http://ntl.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://ftd.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pum.vehdjk.com

Ruby: public / protected / private
来源：http://bnh.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://wsd.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://vne.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://huc.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sln.zycfv.cn

JS:   get name() { return this._name; }
来源：http://lvr.0kj1m.cn

TS:   get name(): string { return this._name; }
来源：http://waa.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://flz.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://tvo.0kj1m.cn

Ruby: attr_accessor :name
来源：http://mwj.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://mzt.gotoacloud.top

[G12] 对象转字符串
来源：http://lqb.tanke756.top

Py:   def __str__(self): return self.name
来源：http://flb.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zky.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://apl.tanke756.top

TS:   toString(): string { return this.name; }
来源：http://vyp.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://lzt.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://rpf.andypj.xyz

Ruby: def to_s; @name; end
来源：http://pkc.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://urv.haohaochexian.top

[G13] 判断对象类型
来源：http://nzl.snrcjt.cn

Py:   isinstance(u, User)
来源：http://ibu.andypj.xyz

PHP:  $u instanceof User
来源：http://agg.iojbl.cn

JS:   u instanceof User
来源：http://rvj.hongshengwenyu.top

TS:   u instanceof User
来源：http://ska.yonumen.top

Java: u instanceof User
来源：http://zwr.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nko.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://jtx.shanyushiyangkeji.top

C#:   u is User
来源：http://yzh.cheryme.top

[G14] 数据类 / record
来源：http://jrm.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mvx.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://yly.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xsj.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://bky.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://fjg.yvedp.cn

Go:   type User struct { Name string; Age int }
来源：http://cwe.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zfd.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://hpv.bbcook.cn

[G15] 枚举
来源：http://jlh.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oic.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpl.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nle.jyoumei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hvk.uphjek.com

Java: enum Color { RED, GREEN }
来源：http://dke.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dek.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://rwp.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ncs.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://mjl.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yqv.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://hws.birdmap.top

JS:   Object.entries(obj)
来源：http://bos.hnqzz.top

TS:   Object.entries(obj)
来源：http://cqj.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aak.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://neh.hysaishi.cn

Ruby: obj.instance_variables
来源：http://vyo.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://wqp.zhixingplan.top

================================================================================
来源：http://iaa.hfpthk.cn

H. 异常与错误处理
来源：http://ycj.yanxiufei.cn

================================================================================
来源：http://wkj.svipenyu.cn

[H01] try / catch 基础
来源：http://sbj.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://weu.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjb.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bwf.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yoe.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ztm.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pvv.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kkv.bbcook.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xyg.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://lsg.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://utv.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nku.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xho.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dcw.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hgq.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vme.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://udr.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bjr.hcnkem.com

[H03] 主动抛出异常
来源：http://njx.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://dkq.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rco.cheryme.top

JS:   throw new Error("错误信息");
来源：http://wep.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://cpq.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pjk.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qbx.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://eal.shangyingyoupin.top


<!-- 参考信息 -->