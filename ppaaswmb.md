代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xrs.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ruf.jlsjyb.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsv.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://npk.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ioz.jqgfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://lpp.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uzh.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lzc.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://lfb.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nzq.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kca.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://msz.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yqx.316326.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zwv.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eop.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://owt.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jnw.jlsjyb.cn

================================================================================
来源：http://nik.shangyingyoupin.top

F. 文件与目录
来源：http://ljm.ehwqpu.com

================================================================================
来源：http://izd.jinqigfzy.top

[F01] 读取整个文件
来源：http://pbo.fengsongda.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dti.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://wmi.nanxinkj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vzi.birdmap.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vnx.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://mto.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iom.ydzc1.top

Ruby: File.read("a.txt")
来源：http://lsq.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://azz.yueranfly.top

[F02] 逐行读取文件
来源：http://dmx.meibo888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xzx.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://odj.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://asw.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smh.sufxvd.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jzx.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zsh.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ltj.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jrn.guowangkeji.top

[F03] 写入文件（覆盖）
来源：http://whi.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ujv.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fua.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukg.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://djj.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mnw.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xps.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://mei.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jxg.jqgfzy.top

[F04] 追加写入文件
来源：http://tdd.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qxj.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hki.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ksg.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kih.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajw.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wuu.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jll.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://odu.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://aet.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dqh.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://fef.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://jyi.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://ywp.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://zeo.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pjk.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://nkf.xuanzx.com

C#:   File.Exists("a.txt")
来源：http://dlj.yj20258.top

[F06] 删除文件
来源：http://qrj.tanke756.top

Py:   os.remove("a.txt")
来源：http://sou.xylfe.cn

PHP:  unlink("a.txt");
来源：http://der.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://gka.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uce.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://orl.birdmap.top

Go:   os.Remove("a.txt")
来源：http://gam.kuanghao11.cn

Ruby: File.delete("a.txt")
来源：http://onc.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://qio.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://vmz.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kaw.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pfc.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjz.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmr.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vlg.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wkf.jlsjyb.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zge.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xkb.guannengcc.top

[F08] 遍历目录
来源：http://fdo.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yzv.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sjp.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://btv.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://lze.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://seu.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mpt.birdmap.top

Ruby: Dir.children("dir")
来源：http://usz.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://cub.jyoumei.cn

[F09] 获取文件大小
来源：http://qpu.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://mtu.shuidangran.top

PHP:  filesize("a.txt");
来源：http://fiy.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://oes.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://tnv.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://fjp.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://odi.gzhubu.top

Ruby: File.size("a.txt")
来源：http://zde.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://vsc.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://kbx.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xjg.cashguo.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ljg.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aff.wangdashe.top

TS:   path.extname("a.txt")
来源：http://hnl.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jju.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://via.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kvg.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://neb.ehwqpu.com

[F11] 复制与移动文件
来源：http://cvt.cheryme.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xuf.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hxh.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gjg.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://inf.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iwu.zhongyouzk.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://inw.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jal.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psp.zdbjq.cn

[F12] CSV 读写
来源：http://yey.zhijiandao.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xcz.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xex.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dnr.vehdjk.com

TS:   // 同上
来源：http://hki.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cya.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ovp.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iin.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rxp.tarul.cn

================================================================================
来源：http://qdg.xuetiantiany.cn

G. 面向对象
来源：http://gno.redwolf501.top

================================================================================
来源：http://hoc.ybcxt.top

[G01] 定义类
来源：http://kpc.cucudq.cn

Py:   class User: pass
来源：http://hja.guannengcc.top

PHP:  class User {}
来源：http://cgk.pycfn.com

JS:   class User {}
来源：http://qgd.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://cqs.gotoacloud.top

Java: class User {}
来源：http://kqv.hnqzz.top

Go:   type User struct { Name string }
来源：http://apn.vehdjk.com

Ruby: class User; end
来源：http://izo.feifeiyinyue.top

C#:   class User {}
来源：http://rep.hysaishi.cn

[G02] 构造函数
来源：http://fqg.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://kaa.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://trh.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://uzy.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://nir.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://wcu.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tdd.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://lqh.daxiang520.top

C#:   public User(string name) { Name = name; }
来源：http://kyx.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://lwr.fengsongda.top

Py:   self.name = "x"
来源：http://jxh.epnwcf.com

PHP:  public string $name = "x";
来源：http://xrk.cashguo.top

JS:   this.name = "x";
来源：http://blo.yanxiufei.cn

TS:   name: string = "x";
来源：http://pss.jyoumei.cn

Java: private String name;
来源：http://cli.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wev.vehdjk.com

Ruby: @name = "x"
来源：http://hua.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://dml.tianlin.xyz

[G04] 定义方法
来源：http://xtb.gzhubu.top

Py:   def greet(self): return self.name
来源：http://fyo.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yiy.hcnkem.com

JS:   greet() { return this.name; }
来源：http://jup.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://vtp.nanxinkj.top

Java: String greet() { return name; }
来源：http://fry.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://awc.snrcjt.cn

Ruby: def greet; @name; end
来源：http://hqh.daxiang520.top

C#:   public string Greet() => Name;
来源：http://bco.yueranfly.top

[G05] 继承
来源：http://uks.daxiang520.top

Py:   class Admin(User): pass
来源：http://rkg.sysykeji.top

PHP:  class Admin extends User {}
来源：http://xhc.aizwys.cn

JS:   class Admin extends User {}
来源：http://kxp.hnqzz.top

TS:   class Admin extends User {}
来源：http://kvo.cheryme.top

Java: class Admin extends User {}
来源：http://jkw.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vod.iojbl.cn

Ruby: class Admin < User; end
来源：http://for.zdbjq.cn

C#:   class Admin : User {}
来源：http://vtr.shzxlz.cn

[G06] 重写方法
来源：http://xjz.sweek.top

Py:   def greet(self): return "admin"
来源：http://puc.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tsi.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://obq.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://ngo.uphjek.com

Java: @Override String greet() { return "admin"; }
来源：http://wxd.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rkf.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://ztw.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://dpa.birdmap.top

[G07] 调用父类方法
来源：http://hov.zhiwuduotai.top

Py:   super().greet()
来源：http://ydn.feifeiyinyue.top

PHP:  parent::greet();
来源：http://gxb.smart0.xyz

JS:   super.greet();
来源：http://ygb.zhaomingkeji.xyz

TS:   super.greet();
来源：http://prc.haohaochexian.top

Java: super.greet();
来源：http://bjn.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gpe.shuidangran.top

Ruby: super
来源：http://zbs.yvedp.cn

C#:   base.Greet();
来源：http://fms.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://dzg.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yyv.dianchejie.cn

PHP:  public static function f() {}
来源：http://fzx.chenzaomai.com

JS:   static f() {}
来源：http://ize.havefunace.top

TS:   static f(): void {}
来源：http://cku.wangdashe.top

Java: static void f() {}
来源：http://nkv.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ewk.shanyushiyangtech.top

Ruby: def self.f; end
来源：http://vfk.yfazqb.com

C#:   public static void F() {}
来源：http://kuf.yj20258888.top

[G09] 接口 / 抽象类
来源：http://mdr.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://geo.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://zgh.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qsv.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://hip.bbcook.cn

Java: interface Shape { double area(); }
来源：http://hgs.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://knv.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dpv.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://pql.tanke756.top

[G10] 访问控制
来源：http://yab.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://zhg.jlsjyb.cn

PHP:  public / protected / private
来源：http://ncp.c1oappe.top

JS:   #private 字段；其余公开
来源：http://doa.xuanzx.com

TS:   public / protected / private
来源：http://iyg.birdmap.top

Java: public / protected / private / 默认包级
来源：http://jvm.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://stg.zhoulong.xyz

Ruby: public / protected / private
来源：http://amf.redwolf501.top

C#:   public / protected / private / internal
来源：http://sis.iojbl.cn

[G11] getter / setter
来源：http://qkd.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://aum.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://bgo.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://tqp.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://cdv.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://wzt.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://egr.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://ajc.uphjek.com

C#:   public string Name { get; set; }
来源：http://cqr.zhixingplan.top

[G12] 对象转字符串
来源：http://ogb.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://pdz.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://kbb.aizwys.cn

JS:   toString() { return this.name; }
来源：http://kwt.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://mjp.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://wza.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://owq.yongpay.top

Ruby: def to_s; @name; end
来源：http://blp.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://ikf.sxryk.cn

[G13] 判断对象类型
来源：http://fmz.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://dit.ctjpmb.com

PHP:  $u instanceof User
来源：http://dya.sufxvd.cn

JS:   u instanceof User
来源：http://swc.zhiwuduotai.top

TS:   u instanceof User
来源：http://pbo.52xcode.cn

Java: u instanceof User
来源：http://zds.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://amm.smart0.xyz

Ruby: u.is_a?(User)
来源：http://fal.jiagoushi.top

C#:   u is User
来源：http://msm.tian-w.cn

[G14] 数据类 / record
来源：http://cwu.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vry.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://qxb.hongshengwenyu.top

JS:   // 无内置：普通类或对象字面量
来源：http://rwg.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://ale.mhx1999.top

Java: record User(String name, int age) {}
来源：http://gdc.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://ons.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jvd.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://osv.gotoacloud.top

[G15] 枚举
来源：http://pms.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tbf.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://otj.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ksi.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ise.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://aze.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekf.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://tfj.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xqg.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://ktb.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kpn.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://gvw.jinqigufen.top

JS:   Object.entries(obj)
来源：http://jih.gogol.net.cn

TS:   Object.entries(obj)
来源：http://tqt.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vyi.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lph.daxiang520.top

Ruby: obj.instance_variables
来源：http://sjv.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://bhq.jyoumei.cn

================================================================================
来源：http://pyg.cucudq.cn

H. 异常与错误处理
来源：http://yqs.yj20258888.top

================================================================================
来源：http://srf.52xcode.cn

[H01] try / catch 基础
来源：http://pun.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ggs.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gxr.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eld.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bda.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ptf.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nkf.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uez.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://faz.xinyue.icu

[H02] finally / ensure 收尾
来源：http://jmc.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pzk.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gmk.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jgm.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eyn.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://qom.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://ant.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mth.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pse.yueranfly.top

[H03] 主动抛出异常
来源：http://ruv.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://sus.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixe.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://geq.tanke756.top


<!-- 参考信息 -->