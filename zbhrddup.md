代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://izm.ctjpmb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tlq.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rpf.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cjp.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bfv.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://qen.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jmr.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nfz.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://jdh.gogol.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://osr.ybcxt.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kyj.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvd.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxg.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eaz.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://puu.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://bsq.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://znp.smart0.xyz

================================================================================
来源：http://tnl.jinghuilouyu.cn

F. 文件与目录
来源：http://fnz.jinyuanbaomall.cn

================================================================================
来源：http://iau.guowangkeji.top

[F01] 读取整个文件
来源：http://yxd.xuetiantiany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ero.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://gsz.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://klg.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nti.fktsv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hwe.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://khz.xylfe.cn

Ruby: File.read("a.txt")
来源：http://qml.ywan-chungtsiang.top

C#:   File.ReadAllText("a.txt");
来源：http://prh.epnwcf.com

[F02] 逐行读取文件
来源：http://igz.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://csu.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wjr.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohb.zhiwuduotai.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vml.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hbb.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://atz.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iuh.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jqn.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://gcc.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rbd.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://qew.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oxj.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqu.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sjz.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qbg.tianlin.xyz

Ruby: File.write("a.txt", "hi")
来源：http://vti.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdw.aibaodan.cn

[F04] 追加写入文件
来源：http://huh.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eme.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ymf.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fsl.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://spy.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://won.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uxz.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xxh.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ybr.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://uek.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vjw.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://hvr.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://zab.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://huo.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://knh.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jtx.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://rsl.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://etw.hnxiangtu.top

[F06] 删除文件
来源：http://cqv.bjfxy.top

Py:   os.remove("a.txt")
来源：http://tub.nwbrower.top

PHP:  unlink("a.txt");
来源：http://cwq.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://lgq.tanke756.top

TS:   fs.unlinkSync("a.txt")
来源：http://xbf.yuxming.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hem.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://ukc.yuanzhike.top

Ruby: File.delete("a.txt")
来源：http://xhd.yanxiufei.cn

C#:   File.Delete("a.txt");
来源：http://rja.hesvh.cn

[F07] 创建目录（含多级）
来源：http://tvc.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pki.zhongyouzk.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://seh.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ovl.vqdsnc.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aox.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dyo.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dnh.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vkq.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ajh.yuanzhike.top

[F08] 遍历目录
来源：http://hfd.jqgufenzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bas.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zej.ydzc1.top

JS:   fs.readdirSync("dir")
来源：http://mlj.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://lee.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vye.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://cec.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://wzj.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://yqy.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://cgc.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://lye.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://pjj.yongpay.top

JS:   fs.statSync("a.txt").size
来源：http://gat.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://xwg.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gqz.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hck.daria6918.cn

Ruby: File.size("a.txt")
来源：http://xdg.jinghuilouyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://cxw.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://mis.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fox.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ezg.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vhc.fzhhl.top

TS:   path.extname("a.txt")
来源：http://yif.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kak.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wce.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lbj.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rbe.ctjpmb.com

[F11] 复制与移动文件
来源：http://unp.vqdsnc.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gzn.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wwl.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arp.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wqv.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wae.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xcc.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vrd.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qky.nanxuanxn.top

[F12] CSV 读写
来源：http://eoy.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fqi.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qlz.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rmd.cdnleiting.top

TS:   // 同上
来源：http://ygx.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ygh.guowangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oem.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://obr.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pqh.ctjpmb.com

================================================================================
来源：http://avt.gogol.net.cn

G. 面向对象
来源：http://eap.jinghuilouyu.cn

================================================================================
来源：http://bpv.shanyushiyangkeji.top

[G01] 定义类
来源：http://fzn.tarul.cn

Py:   class User: pass
来源：http://wkr.quarkkingdee.top

PHP:  class User {}
来源：http://gdl.shuidangran.top

JS:   class User {}
来源：http://ush.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://plg.zhiwuduotai.top

Java: class User {}
来源：http://ezm.chenlongwang.top

Go:   type User struct { Name string }
来源：http://juu.smart0.xyz

Ruby: class User; end
来源：http://ztw.pengpengdd.cyou

C#:   class User {}
来源：http://ejt.ydjk.org.cn

[G02] 构造函数
来源：http://qsv.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://rux.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://hnz.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://qdd.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://yvt.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://wsb.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gsz.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://zyk.cdnleiting.top

C#:   public User(string name) { Name = name; }
来源：http://cnf.jinqigufen.top

[G03] 实例属性
来源：http://lre.zhiwuduotai.top

Py:   self.name = "x"
来源：http://uvq.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://nrx.hfpthk.cn

JS:   this.name = "x";
来源：http://upv.xuetiantiany.cn

TS:   name: string = "x";
来源：http://cbq.ydzc1.top

Java: private String name;
来源：http://dmr.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tph.nanxinkj.top

Ruby: @name = "x"
来源：http://cpv.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://ekx.xziqi.cn

[G04] 定义方法
来源：http://tpp.yvedp.cn

Py:   def greet(self): return self.name
来源：http://grz.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://etm.ydzc1.top

JS:   greet() { return this.name; }
来源：http://ttv.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://ygv.gogol.net.cn

Java: String greet() { return name; }
来源：http://fgx.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pej.gogol.net.cn

Ruby: def greet; @name; end
来源：http://vmx.birdmap.top

C#:   public string Greet() => Name;
来源：http://nvg.yongpay.top

[G05] 继承
来源：http://wln.smart0.xyz

Py:   class Admin(User): pass
来源：http://oat.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://syi.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://ceg.jinghuilouyu.cn

TS:   class Admin extends User {}
来源：http://hbh.zhoulong.xyz

Java: class Admin extends User {}
来源：http://vso.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oep.hongshengwenyu.top

Ruby: class Admin < User; end
来源：http://fdo.316326.xyz

C#:   class Admin : User {}
来源：http://dff.tian-w.cn

[G06] 重写方法
来源：http://xre.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://byl.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dlt.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://iqw.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://hno.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://rgl.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wau.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://ewb.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://plf.quarkkingdee.top

[G07] 调用父类方法
来源：http://uor.0kj1m.cn

Py:   super().greet()
来源：http://wzk.zdqjudy.top

PHP:  parent::greet();
来源：http://oxw.shangyingyoupin.top

JS:   super.greet();
来源：http://lfn.chenjidiqi.icu

TS:   super.greet();
来源：http://ont.uphjek.com

Java: super.greet();
来源：http://gww.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://swr.guannengcc.top

Ruby: super
来源：http://vxr.andypj.xyz

C#:   base.Greet();
来源：http://fec.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://ayy.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yat.fehbvm.com

PHP:  public static function f() {}
来源：http://xac.c1oappe.top

JS:   static f() {}
来源：http://xyg.yuanzhike.top

TS:   static f(): void {}
来源：http://qto.ydjk.org.cn

Java: static void f() {}
来源：http://ris.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rar.ppjwa.cn

Ruby: def self.f; end
来源：http://oqj.zhengqikj.top

C#:   public static void F() {}
来源：http://dab.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://byb.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://fzm.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ezf.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://czk.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://qmj.birdmap.top

Java: interface Shape { double area(); }
来源：http://gnd.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://iui.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zdy.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://czk.hnxiangtu.top

[G10] 访问控制
来源：http://vyf.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://wid.jyoumei.cn

PHP:  public / protected / private
来源：http://nla.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://ajc.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://qqm.hammf.cn

Java: public / protected / private / 默认包级
来源：http://weo.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryo.uphjek.com

Ruby: public / protected / private
来源：http://llx.bbcook.cn

C#:   public / protected / private / internal
来源：http://vfh.vehdjk.com

[G11] getter / setter
来源：http://tdc.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://szw.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dtn.tarul.cn

JS:   get name() { return this._name; }
来源：http://cfu.sweek.top

TS:   get name(): string { return this._name; }
来源：http://tcm.smart0.xyz

Java: public String getName() { return name; }
来源：http://bfw.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://men.shzxlz.cn

Ruby: attr_accessor :name
来源：http://toa.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://aux.mhx1999.top

[G12] 对象转字符串
来源：http://hxg.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://fdd.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bkw.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://ubd.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://knb.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://jlb.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://frl.fengsongda.top

Ruby: def to_s; @name; end
来源：http://cug.ydzc1.top

C#:   public override string ToString() => Name;
来源：http://lqg.cdnleiting.top

[G13] 判断对象类型
来源：http://eww.zycfv.cn

Py:   isinstance(u, User)
来源：http://yyt.jyoumei.cn

PHP:  $u instanceof User
来源：http://bsa.zhijiandao.cn

JS:   u instanceof User
来源：http://yys.guowangkeji.top

TS:   u instanceof User
来源：http://oel.fehbvm.com

Java: u instanceof User
来源：http://dck.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://zqm.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://cfn.xuetiantiany.cn

C#:   u is User
来源：http://dns.zdqjudy.top

[G14] 数据类 / record
来源：http://ehl.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lqv.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://wvk.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://xio.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://ytk.xuanzx.com

Java: record User(String name, int age) {}
来源：http://awm.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://yfj.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mvn.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://diy.meibo888.top

[G15] 枚举
来源：http://lvp.redwolf501.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wee.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ccv.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://elb.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xuu.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://gqg.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hss.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://wkx.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bke.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://swg.feifeiyinyue.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ipk.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://wyt.zhengqikj.top

JS:   Object.entries(obj)
来源：http://uzy.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://sax.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dix.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ekl.sxryk.cn

Ruby: obj.instance_variables
来源：http://txg.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://iru.ppjwa.cn

================================================================================
来源：http://iaz.pengpengdd.cyou

H. 异常与错误处理
来源：http://trx.zhaomingkeji.xyz

================================================================================
来源：http://muz.haohaochexian.top

[H01] try / catch 基础
来源：http://uzb.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://edc.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xqo.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bsv.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uus.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vwh.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://any.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kye.yonumen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vip.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://pyq.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://xhw.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zkw.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cwi.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bwb.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://nya.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sjk.ctjpmb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pip.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjj.yj20258.top

[H03] 主动抛出异常
来源：http://waa.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://kiq.tian-w.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lay.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://zuj.zhijiandao.cn


<!-- 参考信息 -->