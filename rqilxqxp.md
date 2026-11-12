代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xgq.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://mfj.yj202588.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dkh.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xji.yanxiufei.cn

[E22] 字节长度与字符长度
来源：http://dwt.zdqjudy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fqh.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sbv.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oaj.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aim.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jem.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ffs.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://pqx.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://maz.hysaishi.cn

================================================================================
来源：http://bkc.fehbvm.com

F. 文件与目录
来源：http://eop.yfazqb.com

================================================================================
来源：http://bpn.quarkkingdee.top

[F01] 读取整个文件
来源：http://hrp.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dtm.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://anf.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dzd.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sfl.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://rnk.gzhubu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdz.shuidangran.top

Ruby: File.read("a.txt")
来源：http://qnp.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://zfh.quarkkingdee.top

[F02] 逐行读取文件
来源：http://rws.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uur.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qhq.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nxd.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fyf.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aky.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://edd.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bnu.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qgy.sweek.top

[F03] 写入文件（覆盖）
来源：http://oml.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://juv.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vrr.andypj.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ynm.shanyushiyangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vba.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwm.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://snd.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://yvs.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dqs.mhx1999.top

[F04] 追加写入文件
来源：http://vwl.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zfn.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kyo.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tai.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xaq.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://emp.ctjpmb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rij.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cqx.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jph.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://roi.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://liy.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://xtw.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://aov.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://mlg.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://jlp.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nut.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://ewo.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://qnc.vehdjk.com

[F06] 删除文件
来源：http://vsz.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://hnh.daria6918.cn

PHP:  unlink("a.txt");
来源：http://wdn.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://znh.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://omb.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tnm.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://qkw.hnqzz.top

Ruby: File.delete("a.txt")
来源：http://jhq.sxryk.cn

C#:   File.Delete("a.txt");
来源：http://zqb.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://cbh.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wmc.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zbc.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kty.fzhhl.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oog.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tqd.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://juh.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kaz.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xos.shuidangran.top

[F08] 遍历目录
来源：http://bzb.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcd.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kny.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://buv.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://pkh.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hyg.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hwh.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://rsl.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://aeg.cdnleiting.top

[F09] 获取文件大小
来源：http://tgf.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://jdo.jinghuilouyu.cn

PHP:  filesize("a.txt");
来源：http://cxx.pycfn.com

JS:   fs.statSync("a.txt").size
来源：http://amd.chenzaomai.com

TS:   fs.statSync("a.txt").size
来源：http://vee.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://pcu.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nzl.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://kxn.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://yzy.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://bog.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nfq.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bvg.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sdz.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://koq.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mkg.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pdm.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uox.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uam.chenlongwang.top

[F11] 复制与移动文件
来源：http://rgm.cucudq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fyq.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://and.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yce.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fla.xuanzx.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hol.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zxk.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iqs.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ubs.pengpengdd.cyou

[F12] CSV 读写
来源：http://jjm.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://chi.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wxf.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cgy.gogol.net.cn

TS:   // 同上
来源：http://nbq.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vpo.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://edp.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://suq.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vhg.ydzc1.top

================================================================================
来源：http://adr.zhijiandao.cn

G. 面向对象
来源：http://fnp.fktsv.cn

================================================================================
来源：http://lup.zhixingplan.top

[G01] 定义类
来源：http://yuh.nanxuanxn.top

Py:   class User: pass
来源：http://rjf.shanyushiyangtech.top

PHP:  class User {}
来源：http://ied.gogol.net.cn

JS:   class User {}
来源：http://sjw.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://xgq.ppjwa.cn

Java: class User {}
来源：http://quy.hammf.cn

Go:   type User struct { Name string }
来源：http://gdj.kuanghao11.cn

Ruby: class User; end
来源：http://rtt.daria6918.cn

C#:   class User {}
来源：http://bhd.jianghu66.top

[G02] 构造函数
来源：http://qaa.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://ocm.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://hkq.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://yix.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://igk.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://ete.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qwy.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://ubq.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://lkv.svipenyu.cn

[G03] 实例属性
来源：http://unz.wangdashe.top

Py:   self.name = "x"
来源：http://wdq.hywenlv.cn

PHP:  public string $name = "x";
来源：http://tup.316326.xyz

JS:   this.name = "x";
来源：http://vzu.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://pzu.shuidangran.top

Java: private String name;
来源：http://jsn.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xyd.svipenyu.cn

Ruby: @name = "x"
来源：http://edc.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://hat.pengpengdd.cyou

[G04] 定义方法
来源：http://lze.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://atw.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cud.yonumen.top

JS:   greet() { return this.name; }
来源：http://atc.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://xwu.yj20258.top

Java: String greet() { return name; }
来源：http://gtm.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qpz.yvedp.cn

Ruby: def greet; @name; end
来源：http://lnk.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://boo.zhijiandao.cn

[G05] 继承
来源：http://ode.cheryme.top

Py:   class Admin(User): pass
来源：http://kkg.xinyue.icu

PHP:  class Admin extends User {}
来源：http://xko.fktsv.cn

JS:   class Admin extends User {}
来源：http://cnd.ivvv.top

TS:   class Admin extends User {}
来源：http://wlf.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://pbw.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fur.nanxinkj.top

Ruby: class Admin < User; end
来源：http://rmx.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://udp.yvedp.cn

[G06] 重写方法
来源：http://ihw.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://oji.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tan.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://udl.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://exo.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://xao.jinyuanbaomall.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rmi.yonumen.top

Ruby: def greet; "admin"; end
来源：http://vzr.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://dnn.sjlbkw.cn

[G07] 调用父类方法
来源：http://ovg.quarkkingdee.top

Py:   super().greet()
来源：http://wgu.wangshuangyany.cn

PHP:  parent::greet();
来源：http://iyf.guowangkeji.top

JS:   super.greet();
来源：http://yqb.shzxlz.cn

TS:   super.greet();
来源：http://tkc.nanxinkj.top

Java: super.greet();
来源：http://rwx.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://psq.daria6918.cn

Ruby: super
来源：http://osr.ydzc1.top

C#:   base.Greet();
来源：http://uwi.tianlin.xyz

[G08] 静态方法与属性
来源：http://vti.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oaj.zhijiandao.cn

PHP:  public static function f() {}
来源：http://tbb.hywenlv.cn

JS:   static f() {}
来源：http://flw.jianghu66.top

TS:   static f(): void {}
来源：http://kyj.ctjpmb.com

Java: static void f() {}
来源：http://qca.fehbvm.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jna.ehwqpu.com

Ruby: def self.f; end
来源：http://pfa.52xcode.cn

C#:   public static void F() {}
来源：http://yve.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://qje.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://ril.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hts.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lli.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://prb.yj20258888.top

Java: interface Shape { double area(); }
来源：http://fns.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ksq.cdnleiting.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wsb.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://fqb.ehwqpu.com

[G10] 访问控制
来源：http://efe.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://rws.9152youxi.cn

PHP:  public / protected / private
来源：http://qiv.yonumen.top

JS:   #private 字段；其余公开
来源：http://cfy.pycfn.com

TS:   public / protected / private
来源：http://ciy.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://yht.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ekn.jqgfzy.top

Ruby: public / protected / private
来源：http://adv.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://wmh.yj20258888.top

[G11] getter / setter
来源：http://jhf.epnwcf.com

Py:   @property 与 @x.setter
来源：http://tqw.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qmc.wangdashe.top

JS:   get name() { return this._name; }
来源：http://jkh.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://edo.hnqzz.top

Java: public String getName() { return name; }
来源：http://rok.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bnx.guannengcc.top

Ruby: attr_accessor :name
来源：http://vwp.hesvh.cn

C#:   public string Name { get; set; }
来源：http://sad.yfazqb.com

[G12] 对象转字符串
来源：http://bqi.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://wyn.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bih.pycfn.com

JS:   toString() { return this.name; }
来源：http://bdq.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://fhl.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://xyy.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://sgi.bjfxy.top

Ruby: def to_s; @name; end
来源：http://yld.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://xzt.sysykeji.top

[G13] 判断对象类型
来源：http://ayz.chenlongwang.top

Py:   isinstance(u, User)
来源：http://isr.ivvv.top

PHP:  $u instanceof User
来源：http://hpz.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://pgl.zhengqikj.top

TS:   u instanceof User
来源：http://pxz.ybcxt.top

Java: u instanceof User
来源：http://mbs.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oza.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://fkt.yuxming.cn

C#:   u is User
来源：http://vce.hesvh.cn

[G14] 数据类 / record
来源：http://oee.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cxh.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://kdh.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://yrs.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://qps.daria6918.cn

Java: record User(String name, int age) {}
来源：http://tvs.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://xnw.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dog.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://ywk.chenjidiqi.icu

[G15] 枚举
来源：http://jlj.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fmv.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uxl.bjfxy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dwd.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wly.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://sqt.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kns.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://asj.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ivi.haohaochexian.top

[G16] 对象转数组 / 字典
来源：http://ckw.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wib.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://qdk.cashguo.top

JS:   Object.entries(obj)
来源：http://xij.daria6918.cn

TS:   Object.entries(obj)
来源：http://jya.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tuv.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tmn.yj20258888.top

Ruby: obj.instance_variables
来源：http://fxh.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://kxj.jinqigufen.top

================================================================================
来源：http://kla.pengpengdd.cyou

H. 异常与错误处理
来源：http://rlg.nwbrower.top

================================================================================
来源：http://dph.hnqzz.top

[H01] try / catch 基础
来源：http://kgm.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bdd.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhx.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://anc.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jvq.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hsv.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jid.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ywv.shanyushiyangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tfs.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://uvm.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cgc.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://chz.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://dzn.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dxq.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://khf.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rxy.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://tfs.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dmz.c1oappe.top

[H03] 主动抛出异常
来源：http://pin.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://nsd.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://umf.cqqwz.cn

JS:   throw new Error("错误信息");
来源：http://jsn.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://gxj.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vuf.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://azs.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://tmm.epnwcf.com


<!-- 参考信息 -->