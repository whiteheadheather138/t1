代发 wailian999

[E22] 字节长度与字符长度
来源：http://lpo.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ahh.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dbb.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uqc.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eiv.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://urf.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vyf.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://hrs.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://foe.yanxiufei.cn

================================================================================
来源：http://ecp.9152youxi.cn

F. 文件与目录
来源：http://qyj.yueranfly.top

================================================================================
来源：http://pgf.tanke756.top

[F01] 读取整个文件
来源：http://gee.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kjw.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://rfc.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vie.feifeiyinyue.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vnj.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://dip.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hqb.316326.xyz

Ruby: File.read("a.txt")
来源：http://yss.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://joj.yj20258.top

[F02] 逐行读取文件
来源：http://uhx.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pyf.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mqh.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fcn.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yhb.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eap.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zbn.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qsx.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oqr.hammf.cn

[F03] 写入文件（覆盖）
来源：http://ddb.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://plj.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jul.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qpp.cucudq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zxz.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ems.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://faq.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://cyi.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://akc.dashuyun.cn

[F04] 追加写入文件
来源：http://xtc.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zii.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xhz.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fze.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfu.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kdd.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lva.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mxi.zhijiandao.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qwj.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://sbi.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://isu.tianlin.xyz

PHP:  file_exists("a.txt");
来源：http://khg.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://lep.wangdashe.top

TS:   fs.existsSync("a.txt")
来源：http://kxc.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zmv.chenzaomai.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xzr.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://kme.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://jrm.guowangkeji.top

[F06] 删除文件
来源：http://lxn.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://bco.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://jxo.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://wim.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xsj.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://atn.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://adf.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://ciw.cashguo.top

C#:   File.Delete("a.txt");
来源：http://bml.sysykeji.top

[F07] 创建目录（含多级）
来源：http://vaz.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uus.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ehm.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://imw.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://auf.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdb.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gnh.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://swz.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mhe.pengpengdd.cyou

[F08] 遍历目录
来源：http://fub.jinqigufen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xdd.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tfv.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://ipp.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://tmb.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sii.9152youxi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbn.bjfxy.top

Ruby: Dir.children("dir")
来源：http://ert.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://jzf.c1oappe.top

[F09] 获取文件大小
来源：http://vxb.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://yte.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://qzc.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://jye.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://wdm.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uxr.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nfi.hcnkem.com

Ruby: File.size("a.txt")
来源：http://rih.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://zka.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://mxx.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bzc.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://otu.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://evn.tian-w.cn

TS:   path.extname("a.txt")
来源：http://veh.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hww.zhoulong.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://boa.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://euq.yuanzhike.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jtz.hammf.cn

[F11] 复制与移动文件
来源：http://hgj.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://idt.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tac.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjj.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmh.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fxe.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wrj.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zmw.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yds.jqgfzy.top

[F12] CSV 读写
来源：http://zgn.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xqg.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nrj.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qqw.wangshuangyany.cn

TS:   // 同上
来源：http://oef.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vbh.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wxu.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jda.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ooi.zhixingplan.top

================================================================================
来源：http://xud.nanxinkj.top

G. 面向对象
来源：http://gfw.zdbjq.cn

================================================================================
来源：http://gnd.ehwqpu.com

[G01] 定义类
来源：http://qik.ydjk.org.cn

Py:   class User: pass
来源：http://grl.ctjpmb.com

PHP:  class User {}
来源：http://vpi.yuanzhike.top

JS:   class User {}
来源：http://bib.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://xbs.wangshuangyany.cn

Java: class User {}
来源：http://jfz.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://ajs.ehwqpu.com

Ruby: class User; end
来源：http://pgn.meibo888.top

C#:   class User {}
来源：http://kry.yj202588.top

[G02] 构造函数
来源：http://zpo.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://acb.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://bma.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://yct.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://qol.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://brh.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sdn.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://cpd.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://vlt.zycfv.cn

[G03] 实例属性
来源：http://btg.ppjwa.cn

Py:   self.name = "x"
来源：http://wtn.0kj1m.cn

PHP:  public string $name = "x";
来源：http://rvx.jinqigufen.top

JS:   this.name = "x";
来源：http://muq.zhixingplan.top

TS:   name: string = "x";
来源：http://fgz.wangdashe.top

Java: private String name;
来源：http://evy.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://neh.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://hyl.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://jkx.gaohongyu789.top

[G04] 定义方法
来源：http://wwx.smart0.xyz

Py:   def greet(self): return self.name
来源：http://ogj.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bim.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://ltv.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://xck.guowangkeji.top

Java: String greet() { return name; }
来源：http://guf.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ypv.fengsongda.top

Ruby: def greet; @name; end
来源：http://xpu.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://hyl.pengpengdd.cyou

[G05] 继承
来源：http://sqs.nanxinkj.top

Py:   class Admin(User): pass
来源：http://fex.shuidangran.top

PHP:  class Admin extends User {}
来源：http://mot.haohaochexian.top

JS:   class Admin extends User {}
来源：http://inf.cdnleiting.top

TS:   class Admin extends User {}
来源：http://jyi.zhongyouzk.top

Java: class Admin extends User {}
来源：http://neb.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywf.daxiang520.top

Ruby: class Admin < User; end
来源：http://jrj.tarul.cn

C#:   class Admin : User {}
来源：http://qtj.tanke756.top

[G06] 重写方法
来源：http://rzo.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://vls.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fkj.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://had.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://ozi.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://ubr.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ouk.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://ptt.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://ymx.vqdsnc.cn

[G07] 调用父类方法
来源：http://dsh.jinyuanbaomall.cn

Py:   super().greet()
来源：http://wtx.gzhubu.top

PHP:  parent::greet();
来源：http://las.zhijiandao.cn

JS:   super.greet();
来源：http://uko.guannengcc.top

TS:   super.greet();
来源：http://pfx.316326.xyz

Java: super.greet();
来源：http://ftz.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yki.9152youxi.cn

Ruby: super
来源：http://phg.yuxming.cn

C#:   base.Greet();
来源：http://ivn.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://xqf.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://chq.fktsv.cn

PHP:  public static function f() {}
来源：http://wqe.sweek.top

JS:   static f() {}
来源：http://hvy.hnqzz.top

TS:   static f(): void {}
来源：http://ufn.ctjpmb.com

Java: static void f() {}
来源：http://xya.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qrj.jlsjyb.cn

Ruby: def self.f; end
来源：http://khd.pengpengdd.cyou

C#:   public static void F() {}
来源：http://wqx.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://oxo.hnqzz.top

Py:   from abc import ABC, abstractmethod
来源：http://fhg.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://jiy.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lrm.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://pks.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://ktl.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://bmq.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hqf.zdqjudy.top

C#:   interface IShape { double Area(); }
来源：http://nhy.cashguo.top

[G10] 访问控制
来源：http://zon.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://jeg.tanke756.top

PHP:  public / protected / private
来源：http://yfs.bjfxy.top

JS:   #private 字段；其余公开
来源：http://sro.jinqigfzy.top

TS:   public / protected / private
来源：http://pnv.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://euh.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dro.sxryk.cn

Ruby: public / protected / private
来源：http://stj.zdbjq.cn

C#:   public / protected / private / internal
来源：http://vpv.bjfxy.top

[G11] getter / setter
来源：http://zif.fzhhl.top

Py:   @property 与 @x.setter
来源：http://tcc.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://das.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://soq.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://htl.hesvh.cn

Java: public String getName() { return name; }
来源：http://fap.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvl.tarul.cn

Ruby: attr_accessor :name
来源：http://rhw.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://why.kuanghao11.cn

[G12] 对象转字符串
来源：http://uvc.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://kex.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tin.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://ida.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://ayu.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://jlx.quarkkingdee.top

Go:   func (u User) String() string { return u.Name }
来源：http://jac.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://kix.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://fqf.haohaochexian.top

[G13] 判断对象类型
来源：http://rwl.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://ljw.jiagoushi.top

PHP:  $u instanceof User
来源：http://dzn.zhongyouzk.top

JS:   u instanceof User
来源：http://elb.yj20258.top

TS:   u instanceof User
来源：http://fys.yonumen.top

Java: u instanceof User
来源：http://rsa.kuanghao11.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fqh.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://jyk.andypj.xyz

C#:   u is User
来源：http://dhw.sxryk.cn

[G14] 数据类 / record
来源：http://wae.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hlq.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://wqp.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pqe.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://fnv.nwbrower.top

Java: record User(String name, int age) {}
来源：http://kfp.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://nwl.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jcn.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://mtp.shanyushiyangkeji.top

[G15] 枚举
来源：http://njp.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nmt.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gcy.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hya.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jmy.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://qfa.sxryk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://smw.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://wmq.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vlb.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://fjw.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aki.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://sds.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://fws.fzhhl.top

TS:   Object.entries(obj)
来源：http://dkq.pycfn.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lfk.nanxuanxn.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jda.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://wwh.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://orj.hnqzz.top

================================================================================
来源：http://pcn.gogol.net.cn

H. 异常与错误处理
来源：http://cob.yangfankeji.com

================================================================================
来源：http://kai.gzhubu.top

[H01] try / catch 基础
来源：http://aur.gotoacloud.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dtb.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qof.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://joa.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eeu.yuxming.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kyj.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://toj.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iye.jinqigufen.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gjb.meibo888.top

[H02] finally / ensure 收尾
来源：http://eyh.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://kau.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://fxc.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lik.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://apu.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://mya.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mjm.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hpp.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ezy.zhiwuduotai.top

[H03] 主动抛出异常
来源：http://vaq.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://szv.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rho.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://okk.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://nbd.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://gmu.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ecj.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gqp.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gha.316326.xyz

[H04] 自定义异常类型
来源：http://cdk.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://dsg.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://tny.hysaishi.cn


<!-- 参考信息 -->