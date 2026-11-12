代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wtz.gzhubu.top

================================================================================
来源：http://rrz.hnqzz.top

F. 文件与目录
来源：http://hvs.bjfxy.top

================================================================================
来源：http://wqd.feifeiyinyue.top

[F01] 读取整个文件
来源：http://rlb.smart0.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wqw.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://cbi.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://onw.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://npe.zdbjq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lij.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zsr.ivvv.top

Ruby: File.read("a.txt")
来源：http://lbr.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://usf.zycfv.cn

[F02] 逐行读取文件
来源：http://ssg.mhx1999.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gfy.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qvw.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sjd.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://djw.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zij.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zca.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lba.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fwh.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://mit.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zrx.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gwm.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uzt.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hjw.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kib.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lzo.gotoacloud.top

Ruby: File.write("a.txt", "hi")
来源：http://hmq.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wsw.jlsjyb.cn

[F04] 追加写入文件
来源：http://iqm.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oqq.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rft.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xzd.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ice.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xmr.zhiwuduotai.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gtn.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vhg.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ejo.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://nzk.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xnq.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://wcd.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://fww.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://wbk.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ahj.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zhc.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://esd.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://llk.jianghu66.top

[F06] 删除文件
来源：http://evf.xylfe.cn

Py:   os.remove("a.txt")
来源：http://wcx.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://uqw.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iwz.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://eer.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pty.yangfankeji.com

Go:   os.Remove("a.txt")
来源：http://gml.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://kcr.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://kfp.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://voa.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://skn.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tdv.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wko.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zsi.zhiwuduotai.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nnt.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lgk.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://exm.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ifl.jqgfzy.top

[F08] 遍历目录
来源：http://aen.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bdp.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dlt.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://cwy.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://pqw.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://beo.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qaw.hcnkem.com

Ruby: Dir.children("dir")
来源：http://xpu.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://xfj.yuanzhike.top

[F09] 获取文件大小
来源：http://lzg.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://jjf.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://zbz.svipenyu.cn

JS:   fs.statSync("a.txt").size
来源：http://rvj.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://hsy.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://zkd.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yja.zycfv.cn

Ruby: File.size("a.txt")
来源：http://mcg.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://fko.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://myj.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vak.316326.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jqy.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vyn.smart0.xyz

TS:   path.extname("a.txt")
来源：http://ihv.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yut.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kto.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nwx.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rkj.cqqwz.cn

[F11] 复制与移动文件
来源：http://igk.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://unp.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ndk.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgh.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnp.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://klj.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vhd.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cio.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xfv.yuanzhike.top

[F12] CSV 读写
来源：http://ccq.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sfd.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ldq.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqx.ppjwa.cn

TS:   // 同上
来源：http://rbi.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tti.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ojo.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pfv.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sys.pengpengdd.cyou

================================================================================
来源：http://yfx.shangyingyoupin.top

G. 面向对象
来源：http://eiq.dianchejie.cn

================================================================================
来源：http://een.jyoumei.cn

[G01] 定义类
来源：http://kdf.tian-w.cn

Py:   class User: pass
来源：http://krv.zhoulong.xyz

PHP:  class User {}
来源：http://ryk.gogol.net.cn

JS:   class User {}
来源：http://ffd.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://glm.yfazqb.com

Java: class User {}
来源：http://our.dianchejie.cn

Go:   type User struct { Name string }
来源：http://exj.fanxiaobao.xyz

Ruby: class User; end
来源：http://asn.hesvh.cn

C#:   class User {}
来源：http://uiy.hammf.cn

[G02] 构造函数
来源：http://rfz.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://gdz.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://isq.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://kjv.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://wef.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://hzg.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zdy.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://taq.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://ize.jinyuanbaomall.cn

[G03] 实例属性
来源：http://att.haohaochexian.top

Py:   self.name = "x"
来源：http://gza.zhijiandao.cn

PHP:  public string $name = "x";
来源：http://gdd.mhx1999.top

JS:   this.name = "x";
来源：http://dqu.kuanghao11.cn

TS:   name: string = "x";
来源：http://xeq.gotoacloud.top

Java: private String name;
来源：http://fgw.jqgufenzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://goq.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://ojc.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://tap.hammf.cn

[G04] 定义方法
来源：http://ali.fehbvm.com

Py:   def greet(self): return self.name
来源：http://mrf.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://uao.yueranfly.top

JS:   greet() { return this.name; }
来源：http://qjj.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://nif.gzhubu.top

Java: String greet() { return name; }
来源：http://yii.svipenyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://reb.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://nmm.hammf.cn

C#:   public string Greet() => Name;
来源：http://bwa.kuanghao11.cn

[G05] 继承
来源：http://klo.jinqigufen.top

Py:   class Admin(User): pass
来源：http://chi.jqgfzy.top

PHP:  class Admin extends User {}
来源：http://fnl.0kj1m.cn

JS:   class Admin extends User {}
来源：http://fwg.jqgfzy.top

TS:   class Admin extends User {}
来源：http://kdh.tianlin.xyz

Java: class Admin extends User {}
来源：http://bjj.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cwx.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://tya.andypj.xyz

C#:   class Admin : User {}
来源：http://fxq.pengpengdd.cyou

[G06] 重写方法
来源：http://aiy.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://ruc.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vbc.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://hfq.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://zpl.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://pas.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aet.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://aek.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://atv.sjlbkw.cn

[G07] 调用父类方法
来源：http://qtz.uphjek.com

Py:   super().greet()
来源：http://kcs.zdqjudy.top

PHP:  parent::greet();
来源：http://rlf.jyoumei.cn

JS:   super.greet();
来源：http://ljk.tanke756.top

TS:   super.greet();
来源：http://jpz.zhijiandao.cn

Java: super.greet();
来源：http://ldk.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jph.ppjwa.cn

Ruby: super
来源：http://fvc.nanxinkj.top

C#:   base.Greet();
来源：http://vso.iojbl.cn

[G08] 静态方法与属性
来源：http://ahs.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jnx.jlsjyb.cn

PHP:  public static function f() {}
来源：http://epe.mhx1999.top

JS:   static f() {}
来源：http://ucz.hesvh.cn

TS:   static f(): void {}
来源：http://mnz.0kj1m.cn

Java: static void f() {}
来源：http://ppf.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kpg.zycfv.cn

Ruby: def self.f; end
来源：http://bkm.birdmap.top

C#:   public static void F() {}
来源：http://bvn.cheryme.top

[G09] 接口 / 抽象类
来源：http://etb.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://xfx.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xus.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqz.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://zob.chenlongwang.top

Java: interface Shape { double area(); }
来源：http://oxl.chenzaomai.com

Go:   type Shape interface { Area() float64 }
来源：http://jam.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yja.hysaishi.cn

C#:   interface IShape { double Area(); }
来源：http://nbf.ctjpmb.com

[G10] 访问控制
来源：http://whn.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://tyl.bjfxy.top

PHP:  public / protected / private
来源：http://nvj.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://tfn.zhongyouzk.top

TS:   public / protected / private
来源：http://ful.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://xfp.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kit.chenzaomai.com

Ruby: public / protected / private
来源：http://pdf.bjfxy.top

C#:   public / protected / private / internal
来源：http://glu.shanyushiyangkeji.top

[G11] getter / setter
来源：http://tbl.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://itk.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://tpb.aizwys.cn

JS:   get name() { return this._name; }
来源：http://idd.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://ufh.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://nop.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qma.yuanzhike.top

Ruby: attr_accessor :name
来源：http://fgp.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://kks.chenlongwang.top

[G12] 对象转字符串
来源：http://dvx.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://qkg.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cky.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://ixm.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://tyb.gotoacloud.top

Java: @Override public String toString() { return name; }
来源：http://hlx.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zkq.havefunace.top

Ruby: def to_s; @name; end
来源：http://uox.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://wif.zhijiandao.cn

[G13] 判断对象类型
来源：http://loa.iojbl.cn

Py:   isinstance(u, User)
来源：http://qrm.ppjwa.cn

PHP:  $u instanceof User
来源：http://kal.jqgufenzy.top

JS:   u instanceof User
来源：http://lrc.guannengcc.top

TS:   u instanceof User
来源：http://gjs.yvedp.cn

Java: u instanceof User
来源：http://tdw.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xua.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://sbn.jqgfzy.top

C#:   u is User
来源：http://wnp.pycfn.com

[G14] 数据类 / record
来源：http://xrq.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jfa.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://iqi.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://boo.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://mqc.gzhubu.top

Java: record User(String name, int age) {}
来源：http://qqf.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://yli.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tfp.yonumen.top

C#:   record User(string Name, int Age);
来源：http://fjj.yj20258.top

[G15] 枚举
来源：http://ymo.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hnh.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rus.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yan.ctjpmb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://msj.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://hvc.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zrs.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://alq.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aww.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://fsm.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fpg.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://jen.hfpthk.cn

JS:   Object.entries(obj)
来源：http://ffq.aibaodan.cn

TS:   Object.entries(obj)
来源：http://lzw.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://atr.ydzc1.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dtv.yj202588.top

Ruby: obj.instance_variables
来源：http://jtk.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://ucy.haohaochexian.top

================================================================================
来源：http://njn.hnqzz.top

H. 异常与错误处理
来源：http://qpi.kuanghao11.cn

================================================================================
来源：http://ymt.chenzaomai.com

[H01] try / catch 基础
来源：http://lyt.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hkw.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nkh.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://alx.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxh.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dse.zycfv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://exw.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gnb.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bwk.tarul.cn

[H02] finally / ensure 收尾
来源：http://xtw.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://htg.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mpd.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ggd.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wpy.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yyg.uphjek.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://auv.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dpd.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xnf.zhoulong.xyz

[H03] 主动抛出异常
来源：http://cfp.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://kfh.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xcn.uphjek.com

JS:   throw new Error("错误信息");
来源：http://vuf.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://xhx.meibo888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hol.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jqx.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vkv.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://yyp.smart0.xyz

[H04] 自定义异常类型
来源：http://ggo.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://gwv.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zhd.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://mki.sysykeji.top

TS:   class MyError extends Error {}
来源：http://rbi.cashguo.top

Java: class MyException extends RuntimeException {}
来源：http://xdk.zhixingplan.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://prc.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://rne.fengsongda.top

C#:   class MyException : Exception {}
来源：http://fdq.svipenyu.cn

[H05] 捕获特定类型
来源：http://jrp.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://sdo.vehdjk.com


<!-- 参考信息 -->