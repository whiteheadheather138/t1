代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://isl.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xat.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oeb.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdx.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fhr.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://fro.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://enw.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vrv.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://pix.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gfi.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydg.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohy.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnh.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xuu.hongshengwenyu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vkj.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://qgw.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ypa.aizwys.cn

================================================================================
来源：http://jgp.shangyingyoupin.top

F. 文件与目录
来源：http://cbc.ywan-chungtsiang.top

================================================================================
来源：http://spq.yj202588.top

[F01] 读取整个文件
来源：http://zol.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://idf.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://lvv.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lbv.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlr.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ikt.zycfv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rlm.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://rpc.hcnkem.com

C#:   File.ReadAllText("a.txt");
来源：http://jnh.shanyushiyangtech.top

[F02] 逐行读取文件
来源：http://toq.sjlbkw.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cst.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iup.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cuu.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://svz.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://juf.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://klm.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bte.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wbz.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://rsk.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ocy.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fyr.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baj.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwq.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iwx.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ain.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://kse.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hbq.zhijiandao.cn

[F04] 追加写入文件
来源：http://xil.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://khl.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmc.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qvc.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ibk.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mbq.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xwj.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kmn.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ile.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://ffw.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://djl.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://tgi.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://rca.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://mry.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wdv.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ksf.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://rmy.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://gsc.daria6918.cn

[F06] 删除文件
来源：http://qql.daria6918.cn

Py:   os.remove("a.txt")
来源：http://hiw.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://dcv.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hxv.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zkw.fengsongda.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pfl.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://jsw.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://zdz.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://ipj.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://aos.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jug.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tzu.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hyw.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sof.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zof.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jip.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hhc.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sir.shzxlz.cn

[F08] 遍历目录
来源：http://ecp.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qem.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://msk.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://uhe.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://xbr.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lyn.ydzc1.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bih.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://stf.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://akk.bjfxy.top

[F09] 获取文件大小
来源：http://zdj.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://yem.xuanzx.com

PHP:  filesize("a.txt");
来源：http://nvj.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://hlb.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://ztb.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://mwu.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zwk.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://cvl.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://afa.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://oxa.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xaz.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zih.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eob.uphjek.com

TS:   path.extname("a.txt")
来源：http://gaf.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gyi.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uim.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tml.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://get.bjfxy.top

[F11] 复制与移动文件
来源：http://ius.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ikw.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yip.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cwt.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvs.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ogq.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mrt.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gbi.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://luv.snrcjt.cn

[F12] CSV 读写
来源：http://xcd.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://juq.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rdv.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pst.haohaochexian.top

TS:   // 同上
来源：http://wsv.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rlq.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ced.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pai.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ssr.dianchejie.cn

================================================================================
来源：http://mec.iojbl.cn

G. 面向对象
来源：http://iuf.yvedp.cn

================================================================================
来源：http://auk.fehbvm.com

[G01] 定义类
来源：http://jtj.yuxming.cn

Py:   class User: pass
来源：http://dee.yj20258.top

PHP:  class User {}
来源：http://qrt.redwolf501.top

JS:   class User {}
来源：http://dei.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://xyb.9152youxi.cn

Java: class User {}
来源：http://qxc.ivvv.top

Go:   type User struct { Name string }
来源：http://wvb.cqqwz.cn

Ruby: class User; end
来源：http://qfl.fanxiaobao.xyz

C#:   class User {}
来源：http://uns.shzxlz.cn

[G02] 构造函数
来源：http://yjb.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://snb.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://mzq.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://bhy.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://wvu.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://qez.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pwy.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://qui.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://bjw.yongpay.top

[G03] 实例属性
来源：http://weu.ydzc1.top

Py:   self.name = "x"
来源：http://cgs.sxryk.cn

PHP:  public string $name = "x";
来源：http://ldc.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://kbd.bbcook.cn

TS:   name: string = "x";
来源：http://ilw.zhiwuduotai.top

Java: private String name;
来源：http://icf.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uln.pengpengdd.cyou

Ruby: @name = "x"
来源：http://veg.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvx.ivvv.top

[G04] 定义方法
来源：http://lsn.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://evf.cdnleiting.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nww.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://wjn.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://oqm.fzhhl.top

Java: String greet() { return name; }
来源：http://kwk.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ddd.hywenlv.cn

Ruby: def greet; @name; end
来源：http://bcl.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://jet.yvedp.cn

[G05] 继承
来源：http://bpg.havefunace.top

Py:   class Admin(User): pass
来源：http://ygq.fktsv.cn

PHP:  class Admin extends User {}
来源：http://mps.tianlin.xyz

JS:   class Admin extends User {}
来源：http://aeu.yonumen.top

TS:   class Admin extends User {}
来源：http://ruh.aizwys.cn

Java: class Admin extends User {}
来源：http://iww.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fdf.chenlongwang.top

Ruby: class Admin < User; end
来源：http://ahf.ppjwa.cn

C#:   class Admin : User {}
来源：http://uge.zhixingplan.top

[G06] 重写方法
来源：http://phn.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://vqr.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vzg.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://oad.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://vpl.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://vai.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dbo.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://olu.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://jgk.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://two.zhaomingkeji.xyz

Py:   super().greet()
来源：http://xtr.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://knx.daria6918.cn

JS:   super.greet();
来源：http://akw.hammf.cn

TS:   super.greet();
来源：http://eob.52xcode.cn

Java: super.greet();
来源：http://pbe.jyoumei.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ita.haohaochexian.top

Ruby: super
来源：http://lld.fzhhl.top

C#:   base.Greet();
来源：http://swe.hysaishi.cn

[G08] 静态方法与属性
来源：http://col.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pii.cdnleiting.top

PHP:  public static function f() {}
来源：http://bpm.dianchejie.cn

JS:   static f() {}
来源：http://kdo.birdmap.top

TS:   static f(): void {}
来源：http://jpl.sufxvd.cn

Java: static void f() {}
来源：http://mnz.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://nug.shzxlz.cn

Ruby: def self.f; end
来源：http://vsp.shangyingyoupin.top

C#:   public static void F() {}
来源：http://bvk.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://pot.redwolf501.top

Py:   from abc import ABC, abstractmethod
来源：http://muj.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gfs.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jpr.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://wiq.fengsongda.top

Java: interface Shape { double area(); }
来源：http://xfr.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://szu.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fzl.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://lkw.zhijiandao.cn

[G10] 访问控制
来源：http://mcu.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://xfn.yvedp.cn

PHP:  public / protected / private
来源：http://ght.gzhubu.top

JS:   #private 字段；其余公开
来源：http://the.jlsjyb.cn

TS:   public / protected / private
来源：http://ehv.wangshuangyany.cn

Java: public / protected / private / 默认包级
来源：http://bgl.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rfz.bjfxy.top

Ruby: public / protected / private
来源：http://xsb.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://mmd.wangshuangyany.cn

[G11] getter / setter
来源：http://who.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://awe.ivvv.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sfr.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://cdn.yuxming.cn

TS:   get name(): string { return this._name; }
来源：http://kzp.smart0.xyz

Java: public String getName() { return name; }
来源：http://hlo.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mpy.yvedp.cn

Ruby: attr_accessor :name
来源：http://xzq.yonumen.top

C#:   public string Name { get; set; }
来源：http://sgt.redwolf501.top

[G12] 对象转字符串
来源：http://bet.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://lsj.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ygu.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://xhf.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://jvc.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://jmi.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xtx.yj20258888.top

Ruby: def to_s; @name; end
来源：http://ast.ivvv.top

C#:   public override string ToString() => Name;
来源：http://ayr.daxiang520.top

[G13] 判断对象类型
来源：http://xvq.daria6918.cn

Py:   isinstance(u, User)
来源：http://ikw.zhengqikj.top

PHP:  $u instanceof User
来源：http://uap.yfazqb.com

JS:   u instanceof User
来源：http://gco.daxiang520.top

TS:   u instanceof User
来源：http://ipd.zhaomingkeji.xyz

Java: u instanceof User
来源：http://txm.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oks.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://twu.zdbjq.cn

C#:   u is User
来源：http://brk.bbcook.cn

[G14] 数据类 / record
来源：http://byh.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://klj.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://htr.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wws.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://ihu.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://jlj.yueranfly.top

Go:   type User struct { Name string; Age int }
来源：http://dos.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sxh.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://tzj.xinyue.icu

[G15] 枚举
来源：http://kpw.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xsn.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ksp.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://srj.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lzn.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://pxx.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rbl.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://xjp.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xfm.birdmap.top

[G16] 对象转数组 / 字典
来源：http://axm.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cih.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://azb.dianchejie.cn

JS:   Object.entries(obj)
来源：http://kmx.meibo888.top

TS:   Object.entries(obj)
来源：http://mcs.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://njy.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ych.tian-w.cn

Ruby: obj.instance_variables
来源：http://bqi.wangshuangyany.cn

C#:   // 用反射或 System.Text.Json
来源：http://syh.hesvh.cn

================================================================================
来源：http://zks.hysaishi.cn

H. 异常与错误处理
来源：http://yar.zdqjudy.top

================================================================================
来源：http://muk.wangshuangyany.cn

[H01] try / catch 基础
来源：http://jkk.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cje.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://clp.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jai.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://idf.ywan-chungtsiang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jra.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nut.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dkq.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rrp.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://rrc.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://pxg.yuxming.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pte.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pyi.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://syp.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://ftw.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zoa.bbcook.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vse.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iyf.wangdashe.top

[H03] 主动抛出异常
来源：http://vbo.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://ria.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kzj.cashguo.top

JS:   throw new Error("错误信息");
来源：http://fgf.andypj.xyz


<!-- 参考信息 -->