代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tfd.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wlo.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gyl.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xio.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wpl.hesvh.cn

Go:   // 按 rune 判断长度后截断
来源：http://qsp.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nsa.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yyv.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://bdw.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cqb.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jbd.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blk.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eup.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qxh.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jum.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://iqu.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gud.jinghuilouyu.cn

================================================================================
来源：http://blp.zycfv.cn

F. 文件与目录
来源：http://ciy.jinqigufen.top

================================================================================
来源：http://gmz.hysaishi.cn

[F01] 读取整个文件
来源：http://cal.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zfp.quarkkingdee.top

PHP:  file_get_contents("a.txt");
来源：http://vif.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tqk.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wyn.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://ffa.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sll.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://cwp.gogol.net.cn

C#:   File.ReadAllText("a.txt");
来源：http://fdw.jqgufenzy.top

[F02] 逐行读取文件
来源：http://ydy.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ziy.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eqc.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bxa.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kiw.zycfv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oqs.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jgi.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kie.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yoe.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://adw.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pxv.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xky.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hgr.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dxr.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvu.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tld.gaohongyu789.top

Ruby: File.write("a.txt", "hi")
来源：http://dfl.xinyue.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mcx.cqqwz.cn

[F04] 追加写入文件
来源：http://bay.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vge.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://voz.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://umj.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwt.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ssm.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fga.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xci.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://agi.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://acu.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ome.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://xor.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://sez.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://sqm.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://eww.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://edq.xuanzx.com

Ruby: File.exist?("a.txt")
来源：http://xsw.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://gzi.52xcode.cn

[F06] 删除文件
来源：http://tdm.gzhubu.top

Py:   os.remove("a.txt")
来源：http://mnh.snrcjt.cn

PHP:  unlink("a.txt");
来源：http://avm.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://rul.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zep.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qjx.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://bcb.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://ako.birdmap.top

C#:   File.Delete("a.txt");
来源：http://wlf.yongpay.top

[F07] 创建目录（含多级）
来源：http://dea.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ork.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bsi.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjl.pengpengdd.cyou

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgk.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vfb.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://adv.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hqs.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bjs.jyoumei.cn

[F08] 遍历目录
来源：http://clc.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fxp.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tgq.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://beo.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://ywo.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ppf.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pwq.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://nxt.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://ris.shuidangran.top

[F09] 获取文件大小
来源：http://gww.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://fbs.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://fnp.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://yra.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://mxn.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://ecq.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vno.chenzaomai.com

Ruby: File.size("a.txt")
来源：http://qmx.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://yoj.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://tnj.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jut.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://plj.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vdn.xylfe.cn

TS:   path.extname("a.txt")
来源：http://plo.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://znl.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://edi.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sch.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yih.haohaochexian.top

[F11] 复制与移动文件
来源：http://lsv.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://znx.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gje.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lup.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eor.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bja.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cat.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zfq.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kvt.tian-w.cn

[F12] CSV 读写
来源：http://ebk.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ncu.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oxo.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ulm.shanyushiyangkeji.top

TS:   // 同上
来源：http://cxz.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://exv.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jae.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tfw.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rcg.hnqzz.top

================================================================================
来源：http://seg.guannengcc.top

G. 面向对象
来源：http://jlq.ppjwa.cn

================================================================================
来源：http://nmn.nanxuanxn.top

[G01] 定义类
来源：http://bdi.sxryk.cn

Py:   class User: pass
来源：http://fyv.yuanzhike.top

PHP:  class User {}
来源：http://qyo.kuanghao11.cn

JS:   class User {}
来源：http://ixh.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://eji.jinghuilouyu.cn

Java: class User {}
来源：http://ida.ydzc1.top

Go:   type User struct { Name string }
来源：http://wdl.jianghu66.top

Ruby: class User; end
来源：http://oro.dianchejie.cn

C#:   class User {}
来源：http://kul.wangshuangyany.cn

[G02] 构造函数
来源：http://rkp.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://iqr.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://cgk.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://gyb.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://qua.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://vuh.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uxt.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://iuq.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://ytm.hnxiangtu.top

[G03] 实例属性
来源：http://kty.yfazqb.com

Py:   self.name = "x"
来源：http://vda.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://rom.jqgufenzy.top

JS:   this.name = "x";
来源：http://jse.nwbrower.top

TS:   name: string = "x";
来源：http://iog.nanxinkj.top

Java: private String name;
来源：http://cyz.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wwy.yuanzhike.top

Ruby: @name = "x"
来源：http://qog.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://cdz.andypj.xyz

[G04] 定义方法
来源：http://cvw.yueranfly.top

Py:   def greet(self): return self.name
来源：http://cuw.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hgv.sysykeji.top

JS:   greet() { return this.name; }
来源：http://mis.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://xda.xuanzx.com

Java: String greet() { return name; }
来源：http://yrv.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ias.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://ghk.cheryme.top

C#:   public string Greet() => Name;
来源：http://bwr.tian-w.cn

[G05] 继承
来源：http://jrj.epnwcf.com

Py:   class Admin(User): pass
来源：http://puo.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://lqg.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://kzu.hesvh.cn

TS:   class Admin extends User {}
来源：http://xlb.gotoacloud.top

Java: class Admin extends User {}
来源：http://mko.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jws.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://uvi.316326.xyz

C#:   class Admin : User {}
来源：http://vih.smart0.xyz

[G06] 重写方法
来源：http://oct.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://xsv.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://inm.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://xnl.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://oxn.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://tjy.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgk.xuetiantiany.cn

Ruby: def greet; "admin"; end
来源：http://jag.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://bzn.jqgufenzy.top

[G07] 调用父类方法
来源：http://qkp.ivvv.top

Py:   super().greet()
来源：http://xow.cheryme.top

PHP:  parent::greet();
来源：http://rvc.hcnkem.com

JS:   super.greet();
来源：http://ikn.chenlongwang.top

TS:   super.greet();
来源：http://esr.jqgfzy.top

Java: super.greet();
来源：http://mvy.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://noh.jlsjyb.cn

Ruby: super
来源：http://hok.uphjek.com

C#:   base.Greet();
来源：http://tjt.hesvh.cn

[G08] 静态方法与属性
来源：http://wuo.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nqm.316326.xyz

PHP:  public static function f() {}
来源：http://dvo.nanxuanxn.top

JS:   static f() {}
来源：http://scu.ydjk.org.cn

TS:   static f(): void {}
来源：http://myb.nanxuanxn.top

Java: static void f() {}
来源：http://wno.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yzb.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://hqf.havefunace.top

C#:   public static void F() {}
来源：http://bji.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://igr.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ieq.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jno.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xgq.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://zpa.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://gax.yvedp.cn

Go:   type Shape interface { Area() float64 }
来源：http://pqv.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kov.316326.xyz

C#:   interface IShape { double Area(); }
来源：http://pui.shanyushiyangtech.top

[G10] 访问控制
来源：http://dee.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://xyo.jqgfzy.top

PHP:  public / protected / private
来源：http://qmm.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://bqt.shangyingyoupin.top

TS:   public / protected / private
来源：http://vbo.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://zqz.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkl.jyoumei.cn

Ruby: public / protected / private
来源：http://hnw.haohaochexian.top

C#:   public / protected / private / internal
来源：http://dir.hysaishi.cn

[G11] getter / setter
来源：http://vuc.redwolf501.top

Py:   @property 与 @x.setter
来源：http://ohc.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ywd.tarul.cn

JS:   get name() { return this._name; }
来源：http://qqs.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://iqd.pycfn.com

Java: public String getName() { return name; }
来源：http://ozz.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hws.yj20258888.top

Ruby: attr_accessor :name
来源：http://bzj.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://aur.9152youxi.cn

[G12] 对象转字符串
来源：http://zud.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://utc.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yck.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://udr.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://cin.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://kex.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pjg.c1oappe.top

Ruby: def to_s; @name; end
来源：http://fdv.yangfankeji.com

C#:   public override string ToString() => Name;
来源：http://ekp.uphjek.com

[G13] 判断对象类型
来源：http://iyr.iojbl.cn

Py:   isinstance(u, User)
来源：http://ofc.hnqzz.top

PHP:  $u instanceof User
来源：http://hwd.mhx1999.top

JS:   u instanceof User
来源：http://uvg.hnqzz.top

TS:   u instanceof User
来源：http://oga.zdbjq.cn

Java: u instanceof User
来源：http://ugt.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://kwb.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://kpn.wangshuangyany.cn

C#:   u is User
来源：http://ntt.jlsjyb.cn

[G14] 数据类 / record
来源：http://tsp.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zkv.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://knx.sysykeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://sxz.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://oln.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://icf.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://ivd.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bcp.sweek.top

C#:   record User(string Name, int Age);
来源：http://lsh.52xcode.cn

[G15] 枚举
来源：http://tql.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tvp.yueranfly.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bgi.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xbp.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nzt.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://xru.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gjr.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://kvp.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rpt.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://yqt.xinyue.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yiy.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://gxp.0kj1m.cn

JS:   Object.entries(obj)
来源：http://ycy.smart0.xyz

TS:   Object.entries(obj)
来源：http://jbw.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tcr.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ikr.cdnleiting.top

Ruby: obj.instance_variables
来源：http://epr.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://krm.yfazqb.com

================================================================================
来源：http://nln.zhixingplan.top

H. 异常与错误处理
来源：http://epo.hnxiangtu.top

================================================================================
来源：http://xzn.dianchejie.cn

[H01] try / catch 基础
来源：http://iog.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qrb.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://okt.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fur.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ewo.chenzaomai.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jpu.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rva.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fxs.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tab.xziqi.cn

[H02] finally / ensure 收尾
来源：http://lfg.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gib.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://puv.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rsm.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://alh.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rdr.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ynt.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cwq.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sci.hnxiangtu.top

[H03] 主动抛出异常
来源：http://ptq.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://txh.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bpf.wangshuangyany.cn

JS:   throw new Error("错误信息");
来源：http://mhd.sxryk.cn


<!-- 参考信息 -->