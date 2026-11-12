代发 wailian999

Go:   if s == "" {}
来源：http://lte.zhijiandao.cn

Ruby: if s.empty?
来源：http://xhj.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kpj.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://lyf.hnxiangtu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ixx.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ecr.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://abm.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzw.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xpb.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://sxj.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tad.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bni.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://ciz.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rml.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qhz.xinyue.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://btg.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhc.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ydt.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rcl.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://fvr.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bqt.sxryk.cn

================================================================================
来源：http://zlg.jyoumei.cn

F. 文件与目录
来源：http://mgn.shuidangran.top

================================================================================
来源：http://ggq.9152youxi.cn

[F01] 读取整个文件
来源：http://xbh.52xcode.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bjl.yanxiufei.cn

PHP:  file_get_contents("a.txt");
来源：http://lix.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://omi.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rmq.zhaomingkeji.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://kjf.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qtr.sweek.top

Ruby: File.read("a.txt")
来源：http://gwq.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://ksg.yonumen.top

[F02] 逐行读取文件
来源：http://ckp.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lqi.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rwl.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://crn.jinghuilouyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltf.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmf.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://crr.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tbm.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vee.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://mdf.hfpthk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dqr.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pvk.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ozu.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgx.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uop.yvedp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cyx.jyoumei.cn

Ruby: File.write("a.txt", "hi")
来源：http://ikq.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wwl.bbcook.cn

[F04] 追加写入文件
来源：http://gtn.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://owi.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sfg.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xim.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttg.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fii.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://olw.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://stb.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kyg.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://xpz.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ocv.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://uig.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://lgl.zhixingplan.top

TS:   fs.existsSync("a.txt")
来源：http://wvo.yuxming.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bjv.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://owm.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://szx.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://tno.sjlbkw.cn

[F06] 删除文件
来源：http://ozy.ehwqpu.com

Py:   os.remove("a.txt")
来源：http://blr.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://dir.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://qvj.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://isp.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jnm.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://vdc.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://xwj.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://mxp.birdmap.top

[F07] 创建目录（含多级）
来源：http://rul.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mzr.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zhl.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wvj.cheryme.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nvq.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://inm.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gud.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nyt.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ebm.xingfuxueyuan.xyz

[F08] 遍历目录
来源：http://kae.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://evf.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ebe.cheryme.top

JS:   fs.readdirSync("dir")
来源：http://dpo.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://omx.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wxn.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kcj.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://qau.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://ftt.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://rok.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://hdh.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://lpf.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://xiw.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://sel.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://tjb.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ksi.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://cww.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://iqz.jianghu66.top

[F10] 取文件扩展名 / 文件名
来源：http://fgm.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kpe.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zvx.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rsa.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://bwd.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nor.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://btp.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hlp.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rqd.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://vjl.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blr.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xoy.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oku.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://owu.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://syf.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ihc.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zcd.yj202588.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ymv.ydjk.org.cn

[F12] CSV 读写
来源：http://oia.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://upa.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yzr.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lad.pengpengdd.cyou

TS:   // 同上
来源：http://atd.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nhm.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yyl.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dvh.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uqq.aizwys.cn

================================================================================
来源：http://rzb.zhixingplan.top

G. 面向对象
来源：http://kll.xuanzx.com

================================================================================
来源：http://puf.fktsv.cn

[G01] 定义类
来源：http://akt.bjfxy.top

Py:   class User: pass
来源：http://mbl.shanyushiyangtech.top

PHP:  class User {}
来源：http://qjq.yj20258888.top

JS:   class User {}
来源：http://uch.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://hfs.hcnkem.com

Java: class User {}
来源：http://dyo.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://hfg.yvedp.cn

Ruby: class User; end
来源：http://lys.yfazqb.com

C#:   class User {}
来源：http://zpe.epnwcf.com

[G02] 构造函数
来源：http://rci.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://zhc.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://hxk.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://zfo.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://noo.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://mau.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xvq.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jvt.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://sto.yongpay.top

[G03] 实例属性
来源：http://vjg.pycfn.com

Py:   self.name = "x"
来源：http://kzt.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://zij.yueranfly.top

JS:   this.name = "x";
来源：http://zlr.tian-w.cn

TS:   name: string = "x";
来源：http://hdu.ivvv.top

Java: private String name;
来源：http://vpx.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ydv.chenzaomai.com

Ruby: @name = "x"
来源：http://rwm.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://nxn.jlsjyb.cn

[G04] 定义方法
来源：http://peh.xziqi.cn

Py:   def greet(self): return self.name
来源：http://vwh.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lpc.yfazqb.com

JS:   greet() { return this.name; }
来源：http://leg.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://mqq.yj20258888.top

Java: String greet() { return name; }
来源：http://drj.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hpy.hywenlv.cn

Ruby: def greet; @name; end
来源：http://gxh.mhx1999.top

C#:   public string Greet() => Name;
来源：http://kow.tian-w.cn

[G05] 继承
来源：http://ckh.fktsv.cn

Py:   class Admin(User): pass
来源：http://drv.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://rla.sxryk.cn

JS:   class Admin extends User {}
来源：http://lsr.aizwys.cn

TS:   class Admin extends User {}
来源：http://nfk.shzxlz.cn

Java: class Admin extends User {}
来源：http://ldc.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dmn.yuxming.cn

Ruby: class Admin < User; end
来源：http://xqx.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://qvz.yangfankeji.com

[G06] 重写方法
来源：http://wnt.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://ffl.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ise.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://sys.jianghu66.top

TS:   greet(): string { return "admin"; }
来源：http://hmg.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://usu.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qai.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://faw.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://utp.tarul.cn

[G07] 调用父类方法
来源：http://lde.zhaomingkeji.xyz

Py:   super().greet()
来源：http://ric.fengsongda.top

PHP:  parent::greet();
来源：http://qjh.xuanzx.com

JS:   super.greet();
来源：http://nfm.jinqigfzy.top

TS:   super.greet();
来源：http://fnu.gogol.net.cn

Java: super.greet();
来源：http://hha.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ufu.zdqjudy.top

Ruby: super
来源：http://jof.redwolf501.top

C#:   base.Greet();
来源：http://hsy.sysykeji.top

[G08] 静态方法与属性
来源：http://svs.ivvv.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hkk.smart0.xyz

PHP:  public static function f() {}
来源：http://tnj.bjfxy.top

JS:   static f() {}
来源：http://jnq.zhijiandao.cn

TS:   static f(): void {}
来源：http://bny.nanxinkj.top

Java: static void f() {}
来源：http://zgy.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xti.tianlin.xyz

Ruby: def self.f; end
来源：http://erm.wangdashe.top

C#:   public static void F() {}
来源：http://zps.xziqi.cn

[G09] 接口 / 抽象类
来源：http://yjb.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://wxy.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://tdj.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cix.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://cwf.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://owi.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://sfe.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sgj.sxryk.cn

C#:   interface IShape { double Area(); }
来源：http://drp.0kj1m.cn

[G10] 访问控制
来源：http://ajz.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://wcw.xylfe.cn

PHP:  public / protected / private
来源：http://sxf.yj20258.top

JS:   #private 字段；其余公开
来源：http://zit.fktsv.cn

TS:   public / protected / private
来源：http://ydy.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://gya.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://mkg.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://pwu.sweek.top

C#:   public / protected / private / internal
来源：http://kdg.cucudq.cn

[G11] getter / setter
来源：http://mef.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://giw.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ppz.aizwys.cn

JS:   get name() { return this._name; }
来源：http://zzx.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://qwv.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://jni.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://axp.nanxuanxn.top

Ruby: attr_accessor :name
来源：http://vau.fzhhl.top

C#:   public string Name { get; set; }
来源：http://qkb.ivvv.top

[G12] 对象转字符串
来源：http://zli.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://hwu.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://etl.ybcxt.top

JS:   toString() { return this.name; }
来源：http://kkz.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://qkh.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://jsl.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oxu.ybcxt.top

Ruby: def to_s; @name; end
来源：http://egk.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://hog.iojbl.cn

[G13] 判断对象类型
来源：http://ace.smart0.xyz

Py:   isinstance(u, User)
来源：http://yua.nwbrower.top

PHP:  $u instanceof User
来源：http://rsz.daria6918.cn

JS:   u instanceof User
来源：http://agl.tanke756.top

TS:   u instanceof User
来源：http://pxb.ppjwa.cn

Java: u instanceof User
来源：http://tgm.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ubd.gzhubu.top

Ruby: u.is_a?(User)
来源：http://vmb.fktsv.cn

C#:   u is User
来源：http://fqf.zhixingplan.top

[G14] 数据类 / record
来源：http://btg.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pyk.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://qcy.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://sui.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://gsa.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://hsy.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://ctb.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hta.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://bhw.zdqjudy.top

[G15] 枚举
来源：http://qgf.iojbl.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kaa.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mvy.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gur.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fzq.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://usm.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hsn.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://fim.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jec.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://axp.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hem.nanxuanxn.top

PHP:  get_object_vars($obj);
来源：http://lli.dashuyun.cn

JS:   Object.entries(obj)
来源：http://jva.yangfankeji.com

TS:   Object.entries(obj)
来源：http://zql.jinghuilouyu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tee.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bws.cqqwz.cn

Ruby: obj.instance_variables
来源：http://utp.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://bsy.iojbl.cn

================================================================================
来源：http://wjp.chenlongwang.top

H. 异常与错误处理
来源：http://xqm.zdqjudy.top

================================================================================
来源：http://zwl.xinyue.icu

[H01] try / catch 基础
来源：http://pev.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eyz.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eaj.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://evl.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xbu.nwbrower.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ayh.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rpa.cqqwz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ivk.shanyushiyangtech.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yis.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://xgt.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nef.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://oze.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iyp.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tkh.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://yrr.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xzq.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yng.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzc.jqgufenzy.top


<!-- 参考信息 -->