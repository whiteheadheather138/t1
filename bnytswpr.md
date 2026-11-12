代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tyo.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://myo.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mgx.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wnk.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://rid.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pwt.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xsf.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtk.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jhp.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hcy.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zth.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://tmb.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hjb.yonumen.top

================================================================================
来源：http://vwc.dashuyun.cn

F. 文件与目录
来源：http://dzp.tianlin.xyz

================================================================================
来源：http://ksk.daxiang520.top

[F01] 读取整个文件
来源：http://acj.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kir.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://fca.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mrw.xylfe.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://axn.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://efw.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mzx.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://unt.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://iwo.sweek.top

[F02] 逐行读取文件
来源：http://cfk.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eki.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mci.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ztd.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ckf.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nek.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ocn.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jot.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mko.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://rhk.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ane.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rca.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztr.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://soc.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hhb.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mqw.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://pwe.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://adp.zhoulong.xyz

[F04] 追加写入文件
来源：http://rfz.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blb.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vnw.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vxb.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zzj.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xav.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://izg.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qff.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pkp.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://iny.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zdi.316326.xyz

PHP:  file_exists("a.txt");
来源：http://net.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://zbo.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://bby.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://whm.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yce.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://jjk.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://uci.mhx1999.top

[F06] 删除文件
来源：http://ssc.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://wdo.yj20258888.top

PHP:  unlink("a.txt");
来源：http://ngx.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://jbu.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wxq.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nwr.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://qbo.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://uqa.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://eyw.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://mzw.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ujy.yvedp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kdm.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://din.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqr.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vpr.yanxiufei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lol.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwf.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vld.iojbl.cn

[F08] 遍历目录
来源：http://xej.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ltj.sjlbkw.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jqa.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://bpp.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://mot.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://teo.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vah.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://kui.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://vlg.jiagoushi.top

[F09] 获取文件大小
来源：http://jnu.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://akk.gzhubu.top

PHP:  filesize("a.txt");
来源：http://sga.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://ydw.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://rxx.hnxiangtu.top

Java: Files.size(Path.of("a.txt"))
来源：http://sww.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ohx.fehbvm.com

Ruby: File.size("a.txt")
来源：http://kpg.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://gek.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://jie.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://roa.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dqj.hysaishi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xkd.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://ebw.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fpi.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfv.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yri.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nta.iojbl.cn

[F11] 复制与移动文件
来源：http://jfj.vehdjk.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xsm.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xax.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jcz.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gin.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://knp.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wyv.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bgw.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xke.sysykeji.top

[F12] CSV 读写
来源：http://czc.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wkh.iojbl.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hvr.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oub.cucudq.cn

TS:   // 同上
来源：http://hyk.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://osh.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lws.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rup.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://wqd.nanxuanxn.top

================================================================================
来源：http://wyx.guannengcc.top

G. 面向对象
来源：http://fit.xylfe.cn

================================================================================
来源：http://vft.jinqigufen.top

[G01] 定义类
来源：http://mrb.meibo888.top

Py:   class User: pass
来源：http://meq.birdmap.top

PHP:  class User {}
来源：http://yur.cqqwz.cn

JS:   class User {}
来源：http://bdn.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://nrj.kuanghao11.cn

Java: class User {}
来源：http://bto.0kj1m.cn

Go:   type User struct { Name string }
来源：http://hak.fktsv.cn

Ruby: class User; end
来源：http://xlm.zhaomingkeji.xyz

C#:   class User {}
来源：http://vns.redwolf501.top

[G02] 构造函数
来源：http://qax.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://aqk.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://oen.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://abh.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://kzd.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://zns.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://est.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://gst.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://tta.yfazqb.com

[G03] 实例属性
来源：http://xdr.ybcxt.top

Py:   self.name = "x"
来源：http://zpz.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://yjz.yuanzhike.top

JS:   this.name = "x";
来源：http://ojk.hysaishi.cn

TS:   name: string = "x";
来源：http://iim.xuetiantiany.cn

Java: private String name;
来源：http://jve.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uxr.sjlbkw.cn

Ruby: @name = "x"
来源：http://dul.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://myl.sweek.top

[G04] 定义方法
来源：http://uwg.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://dkz.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lzo.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://zxd.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://dgz.xuanzx.com

Java: String greet() { return name; }
来源：http://btl.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dcf.fehbvm.com

Ruby: def greet; @name; end
来源：http://vzd.birdmap.top

C#:   public string Greet() => Name;
来源：http://bfk.hnqzz.top

[G05] 继承
来源：http://wgh.nwbrower.top

Py:   class Admin(User): pass
来源：http://ujz.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://gez.hywenlv.cn

JS:   class Admin extends User {}
来源：http://ath.ydzc1.top

TS:   class Admin extends User {}
来源：http://fat.sysykeji.top

Java: class Admin extends User {}
来源：http://rin.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cni.gzhubu.top

Ruby: class Admin < User; end
来源：http://igg.ybcxt.top

C#:   class Admin : User {}
来源：http://pqb.mhx1999.top

[G06] 重写方法
来源：http://rnc.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://pxk.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bis.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://tsg.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://grz.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://hjv.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lzw.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://bqy.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://nxe.hywenlv.cn

[G07] 调用父类方法
来源：http://ecj.zhoulong.xyz

Py:   super().greet()
来源：http://mbb.zhongyouzk.top

PHP:  parent::greet();
来源：http://jpa.mhx1999.top

JS:   super.greet();
来源：http://cwk.vqdsnc.cn

TS:   super.greet();
来源：http://opq.zdbjq.cn

Java: super.greet();
来源：http://pwl.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rjp.dashuyun.cn

Ruby: super
来源：http://fbk.yangfankeji.com

C#:   base.Greet();
来源：http://btr.yonumen.top

[G08] 静态方法与属性
来源：http://qhg.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dlx.vehdjk.com

PHP:  public static function f() {}
来源：http://dxr.shangyingyoupin.top

JS:   static f() {}
来源：http://gdd.jyoumei.cn

TS:   static f(): void {}
来源：http://kcr.c1oappe.top

Java: static void f() {}
来源：http://chf.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vhd.aibaodan.cn

Ruby: def self.f; end
来源：http://csl.aibaodan.cn

C#:   public static void F() {}
来源：http://rrj.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://mup.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://kpv.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://rbz.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://djr.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://peo.hcnkem.com

Java: interface Shape { double area(); }
来源：http://xtn.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://zig.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ofd.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://mhk.jinyuanbaomall.cn

[G10] 访问控制
来源：http://sfh.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://aid.daria6918.cn

PHP:  public / protected / private
来源：http://rfe.havefunace.top

JS:   #private 字段；其余公开
来源：http://wvc.zhixingplan.top

TS:   public / protected / private
来源：http://xxs.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://rha.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xoa.cheryme.top

Ruby: public / protected / private
来源：http://epr.jqgfzy.top

C#:   public / protected / private / internal
来源：http://ijd.cqqwz.cn

[G11] getter / setter
来源：http://ltd.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://rtw.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kmp.sysykeji.top

JS:   get name() { return this._name; }
来源：http://luk.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://zth.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://gqr.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cki.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://thn.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://fgs.ydjk.org.cn

[G12] 对象转字符串
来源：http://yxz.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://nra.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://voi.ydzc1.top

JS:   toString() { return this.name; }
来源：http://yrk.wangshuangyany.cn

TS:   toString(): string { return this.name; }
来源：http://ldd.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://jwh.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://awf.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://flb.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://jbz.xylfe.cn

[G13] 判断对象类型
来源：http://vec.smart0.xyz

Py:   isinstance(u, User)
来源：http://ezt.xylfe.cn

PHP:  $u instanceof User
来源：http://jaw.yueranfly.top

JS:   u instanceof User
来源：http://ihc.hysaishi.cn

TS:   u instanceof User
来源：http://vpf.yueranfly.top

Java: u instanceof User
来源：http://hel.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://etv.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://cmu.svipenyu.cn

C#:   u is User
来源：http://faj.ppjwa.cn

[G14] 数据类 / record
来源：http://pci.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ffq.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://umn.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://rng.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://ysh.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://zss.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://qyi.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wps.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://fgx.andypj.xyz

[G15] 枚举
来源：http://cie.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fhc.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vzp.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vrw.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mqc.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://ujm.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xbn.daxiang520.top

Ruby: Color = %i[red green].freeze
来源：http://pze.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iyg.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://vjk.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://guu.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://ajt.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://hvv.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://juu.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vhv.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nil.jyoumei.cn

Ruby: obj.instance_variables
来源：http://ari.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://cdq.aibaodan.cn

================================================================================
来源：http://bkb.tanke756.top

H. 异常与错误处理
来源：http://wwx.ybcxt.top

================================================================================
来源：http://xba.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://ixj.52xcode.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oeh.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nko.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://erm.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eso.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jur.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vco.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zya.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://snq.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://cds.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://rra.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ocy.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ynu.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zvs.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://gqz.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mtv.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zzr.andypj.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://uey.fktsv.cn

[H03] 主动抛出异常
来源：http://tkh.cucudq.cn

Py:   raise ValueError("错误信息")
来源：http://yba.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://npg.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://lzq.yj20258.top

TS:   throw new Error("错误信息");
来源：http://uzz.epnwcf.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://twa.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xgx.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tcu.snrcjt.cn


<!-- 参考信息 -->