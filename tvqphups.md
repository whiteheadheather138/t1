代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vnm.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rzq.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yje.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://afe.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://srb.hnqzz.top

================================================================================
来源：http://tuc.0kj1m.cn

F. 文件与目录
来源：http://lks.zhongyouzk.top

================================================================================
来源：http://ugn.hongshengwenyu.top

[F01] 读取整个文件
来源：http://xnh.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ymo.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://nzn.wangdashe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bor.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ffu.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://pdo.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qgg.xinyue.icu

Ruby: File.read("a.txt")
来源：http://lok.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://twq.yonumen.top

[F02] 逐行读取文件
来源：http://fkj.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wgh.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ppu.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ltc.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fwo.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aiy.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nmg.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kcf.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vka.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://wmt.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dkk.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fbl.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnx.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sop.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://exp.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://efn.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://zdt.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tdq.sysykeji.top

[F04] 追加写入文件
来源：http://ixs.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wxh.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gpq.jinqigfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xfo.mhx1999.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xug.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://itb.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://slk.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://klt.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nbf.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://dis.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvg.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://wuf.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://dhe.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://rjr.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://anz.guannengcc.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://clf.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://xlv.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://zzl.hnqzz.top

[F06] 删除文件
来源：http://sfq.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://eqf.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://wnp.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kgx.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://obq.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uob.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://ckq.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://ysk.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://wml.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://lzr.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://clo.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gze.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ubg.zhiwuduotai.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lkg.sweek.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tmq.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kay.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tgb.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ffh.c1oappe.top

[F08] 遍历目录
来源：http://trr.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://oks.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qch.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://ihi.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://zmr.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://faz.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://poi.zycfv.cn

Ruby: Dir.children("dir")
来源：http://vjb.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://rva.tian-w.cn

[F09] 获取文件大小
来源：http://yzd.shanyushiyangtech.top

Py:   os.path.getsize("a.txt")
来源：http://tay.meibo888.top

PHP:  filesize("a.txt");
来源：http://soc.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://yed.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://spe.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://fbc.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://icu.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://ebs.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://ivl.hongshengwenyu.top

[F10] 取文件扩展名 / 文件名
来源：http://bfa.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zbt.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aqg.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kxp.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://hsu.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lea.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpt.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ekg.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ull.nanxinkj.top

[F11] 复制与移动文件
来源：http://cky.guowangkeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://she.jqgufenzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssd.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vvq.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vbu.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ymh.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhr.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bam.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ixy.zdqjudy.top

[F12] CSV 读写
来源：http://zhk.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dsr.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fwb.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rqe.zycfv.cn

TS:   // 同上
来源：http://idu.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nxl.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qrp.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gzn.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mbh.chenzaomai.com

================================================================================
来源：http://sem.jinyuanbaomall.cn

G. 面向对象
来源：http://iqy.jqgfzy.top

================================================================================
来源：http://rju.aibaodan.cn

[G01] 定义类
来源：http://wml.dashuyun.cn

Py:   class User: pass
来源：http://xzm.hnxiangtu.top

PHP:  class User {}
来源：http://kmk.fengsongda.top

JS:   class User {}
来源：http://yof.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://ggj.shanyushiyangkeji.top

Java: class User {}
来源：http://fwr.0kj1m.cn

Go:   type User struct { Name string }
来源：http://kdq.tianlin.xyz

Ruby: class User; end
来源：http://ftc.yuxming.cn

C#:   class User {}
来源：http://rqw.hnqzz.top

[G02] 构造函数
来源：http://nuq.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://zpt.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://jhs.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://boh.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://omc.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://uez.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uze.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://ddk.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://xhl.jyoumei.cn

[G03] 实例属性
来源：http://nez.fengsongda.top

Py:   self.name = "x"
来源：http://kwn.iojbl.cn

PHP:  public string $name = "x";
来源：http://zus.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://ghr.birdmap.top

TS:   name: string = "x";
来源：http://efu.yfazqb.com

Java: private String name;
来源：http://xgk.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yjm.gaohongyu789.top

Ruby: @name = "x"
来源：http://hlz.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://hjh.feifeiyinyue.top

[G04] 定义方法
来源：http://svk.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://tpv.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://prj.316326.xyz

JS:   greet() { return this.name; }
来源：http://qng.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://djb.zycfv.cn

Java: String greet() { return name; }
来源：http://sxd.feifeiyinyue.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://icc.fengsongda.top

Ruby: def greet; @name; end
来源：http://htw.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://guo.shzxlz.cn

[G05] 继承
来源：http://nhx.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://nug.mhx1999.top

PHP:  class Admin extends User {}
来源：http://pos.zhixingplan.top

JS:   class Admin extends User {}
来源：http://nok.daxiang520.top

TS:   class Admin extends User {}
来源：http://cgy.fktsv.cn

Java: class Admin extends User {}
来源：http://oiy.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nam.yonumen.top

Ruby: class Admin < User; end
来源：http://unv.ctjpmb.com

C#:   class Admin : User {}
来源：http://bkv.shzxlz.cn

[G06] 重写方法
来源：http://hyz.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://pcy.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lid.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://tgy.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://ryq.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://uzt.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iui.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://adc.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://dwa.cashguo.top

[G07] 调用父类方法
来源：http://gyo.zdqjudy.top

Py:   super().greet()
来源：http://dyr.gotoacloud.top

PHP:  parent::greet();
来源：http://iwv.yonumen.top

JS:   super.greet();
来源：http://kea.fktsv.cn

TS:   super.greet();
来源：http://ees.gaohongyu789.top

Java: super.greet();
来源：http://unc.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gki.cqqwz.cn

Ruby: super
来源：http://fqq.zhixingplan.top

C#:   base.Greet();
来源：http://hsl.ppjwa.cn

[G08] 静态方法与属性
来源：http://scb.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://guc.fanxiaobao.xyz

PHP:  public static function f() {}
来源：http://xge.0kj1m.cn

JS:   static f() {}
来源：http://pcz.gogol.net.cn

TS:   static f(): void {}
来源：http://txe.yonumen.top

Java: static void f() {}
来源：http://xfv.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://nxc.yj202588.top

Ruby: def self.f; end
来源：http://uzl.xinyue.icu

C#:   public static void F() {}
来源：http://qyg.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://son.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://qsm.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://unb.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wli.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://tqp.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://atk.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://wpk.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://evy.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://bhh.zycfv.cn

[G10] 访问控制
来源：http://wnk.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://hnf.tianlin.xyz

PHP:  public / protected / private
来源：http://zgj.c1oappe.top

JS:   #private 字段；其余公开
来源：http://zev.tianlin.xyz

TS:   public / protected / private
来源：http://len.ivvv.top

Java: public / protected / private / 默认包级
来源：http://xaf.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tsk.316326.xyz

Ruby: public / protected / private
来源：http://abm.gogol.net.cn

C#:   public / protected / private / internal
来源：http://phz.chenzaomai.com

[G11] getter / setter
来源：http://ish.daria6918.cn

Py:   @property 与 @x.setter
来源：http://qcd.gzhubu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://szc.havefunace.top

JS:   get name() { return this._name; }
来源：http://ola.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://dwi.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ptx.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://lbo.ehwqpu.com

Ruby: attr_accessor :name
来源：http://izd.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://wfb.jiagoushi.top

[G12] 对象转字符串
来源：http://qrb.yonumen.top

Py:   def __str__(self): return self.name
来源：http://onl.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uys.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://fpq.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://lsg.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://qvb.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://kih.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://zlt.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://idw.sysykeji.top

[G13] 判断对象类型
来源：http://vsq.daxiang520.top

Py:   isinstance(u, User)
来源：http://thv.yanxiufei.cn

PHP:  $u instanceof User
来源：http://cpf.pengpengdd.cyou

JS:   u instanceof User
来源：http://qvq.0kj1m.cn

TS:   u instanceof User
来源：http://drv.sysykeji.top

Java: u instanceof User
来源：http://xnn.gzhubu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wew.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://unn.ydzc1.top

C#:   u is User
来源：http://ycc.tanke756.top

[G14] 数据类 / record
来源：http://hrd.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mrg.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://icm.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://xfm.sweek.top

TS:   type User = { name: string; age: number };
来源：http://iyb.havefunace.top

Java: record User(String name, int age) {}
来源：http://hpe.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://vlg.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://you.tarul.cn

C#:   record User(string Name, int Age);
来源：http://okm.0kj1m.cn

[G15] 枚举
来源：http://shk.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cgc.jinqigfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jdk.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hbz.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cru.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://csz.ivvv.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ncd.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://ohr.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kfh.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://win.xylfe.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uxj.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://nwz.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://wbl.cheryme.top

TS:   Object.entries(obj)
来源：http://rhu.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ctr.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pts.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://fng.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://lji.jinqigfzy.top

================================================================================
来源：http://xih.kuanghao11.cn

H. 异常与错误处理
来源：http://mnh.fengsongda.top

================================================================================
来源：http://doq.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://eyg.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fwn.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gap.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fzo.fengsongda.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://afu.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lfv.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pzt.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yhh.fengsongda.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vgn.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://qxj.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://alx.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yoa.9152youxi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://exa.fengsongda.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fkj.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bfg.yueranfly.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jwr.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uwq.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qtq.ppjwa.cn

[H03] 主动抛出异常
来源：http://hpp.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://hrg.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nzp.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://qrs.yj20258.top

TS:   throw new Error("错误信息");
来源：http://eea.ehwqpu.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqg.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hcu.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ebt.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jvm.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://kew.fehbvm.com

Py:   class MyError(Exception): pass
来源：http://uwh.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qzm.shuidangran.top

JS:   class MyError extends Error {}
来源：http://mpp.yvedp.cn

TS:   class MyError extends Error {}
来源：http://ohk.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://xml.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oaw.dashuyun.cn


<!-- 参考信息 -->