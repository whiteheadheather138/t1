代发 wailian999

[F01] 读取整个文件
来源：http://sbq.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qaw.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://yub.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hjv.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oer.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jba.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oer.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://yse.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://nur.gotoacloud.top

[F02] 逐行读取文件
来源：http://ibg.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ebc.jinghuilouyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pry.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bwh.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lgt.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fra.xingfuxueyuan.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pth.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qvz.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fli.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://jki.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oje.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jwt.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://clr.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vss.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ags.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jza.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ivr.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dxe.aizwys.cn

[F04] 追加写入文件
来源：http://lya.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mqh.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lrf.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rrh.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mvp.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://agp.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ytr.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iqe.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yli.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://luq.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pwv.sxryk.cn

PHP:  file_exists("a.txt");
来源：http://fhz.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://mpn.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://zzv.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gon.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vdr.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://cyn.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://nfd.sufxvd.cn

[F06] 删除文件
来源：http://gqs.yueranfly.top

Py:   os.remove("a.txt")
来源：http://adp.yj20258.top

PHP:  unlink("a.txt");
来源：http://kte.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://uwa.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://hrd.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://axs.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://tuz.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://wjf.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://zvr.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://rty.hongshengwenyu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://myd.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dag.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ity.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kmj.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qmm.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://scr.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lzr.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tpf.sysykeji.top

[F08] 遍历目录
来源：http://oud.gotoacloud.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zki.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfh.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://pkb.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://cxp.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ugt.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zud.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://hag.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://sdg.hnxiangtu.top

[F09] 获取文件大小
来源：http://jex.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://fph.gzhubu.top

PHP:  filesize("a.txt");
来源：http://wiu.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://hbb.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://caq.chenlongwang.top

Java: Files.size(Path.of("a.txt"))
来源：http://myh.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rmw.iojbl.cn

Ruby: File.size("a.txt")
来源：http://kzq.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://nfj.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://xuo.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ugi.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://awi.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ljy.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://hqx.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ryx.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uhh.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxy.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eht.havefunace.top

[F11] 复制与移动文件
来源：http://zuv.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gfs.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tid.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aud.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zij.hywenlv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uhm.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jwv.xylfe.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://igc.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://paf.xylfe.cn

[F12] CSV 读写
来源：http://iff.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xsd.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ijv.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qhi.c1oappe.top

TS:   // 同上
来源：http://lnr.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dzt.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yqd.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ucx.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eyn.guannengcc.top

================================================================================
来源：http://jfj.zdqjudy.top

G. 面向对象
来源：http://kta.shanyushiyangtech.top

================================================================================
来源：http://ybu.yvedp.cn

[G01] 定义类
来源：http://nlz.zhijiandao.cn

Py:   class User: pass
来源：http://vhs.chenzaomai.com

PHP:  class User {}
来源：http://lcx.fzhhl.top

JS:   class User {}
来源：http://jus.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://fgi.zdqjudy.top

Java: class User {}
来源：http://gfh.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://lsq.cqqwz.cn

Ruby: class User; end
来源：http://xvg.bbcook.cn

C#:   class User {}
来源：http://ryq.daria6918.cn

[G02] 构造函数
来源：http://tvj.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://ypo.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://fmu.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://wws.hysaishi.cn

TS:   constructor(public name: string) {}
来源：http://cgn.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://ckm.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bfq.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://abk.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://iim.jinghuilouyu.cn

[G03] 实例属性
来源：http://qqa.xinyue.icu

Py:   self.name = "x"
来源：http://azh.andypj.xyz

PHP:  public string $name = "x";
来源：http://nrl.gotoacloud.top

JS:   this.name = "x";
来源：http://fxd.nanxinkj.top

TS:   name: string = "x";
来源：http://asg.hesvh.cn

Java: private String name;
来源：http://wgg.aibaodan.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsf.sjlbkw.cn

Ruby: @name = "x"
来源：http://uvz.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://pjp.wangdashe.top

[G04] 定义方法
来源：http://xvr.yj202588.top

Py:   def greet(self): return self.name
来源：http://uar.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eld.cashguo.top

JS:   greet() { return this.name; }
来源：http://jxv.fzhhl.top

TS:   greet(): string { return this.name; }
来源：http://sjm.zdbjq.cn

Java: String greet() { return name; }
来源：http://dhf.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bfk.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://okk.aizwys.cn

C#:   public string Greet() => Name;
来源：http://egb.chenjidiqi.icu

[G05] 继承
来源：http://hyf.guannengcc.top

Py:   class Admin(User): pass
来源：http://qfi.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://pcm.zdqjudy.top

JS:   class Admin extends User {}
来源：http://tfp.tarul.cn

TS:   class Admin extends User {}
来源：http://kda.yuanzhike.top

Java: class Admin extends User {}
来源：http://eaa.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://clk.yj20258888.top

Ruby: class Admin < User; end
来源：http://syh.jyoumei.cn

C#:   class Admin : User {}
来源：http://euo.sxryk.cn

[G06] 重写方法
来源：http://zax.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://sze.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vcd.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://qjj.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://vle.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://dlv.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qhw.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://apn.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://dft.ppjwa.cn

[G07] 调用父类方法
来源：http://usl.epnwcf.com

Py:   super().greet()
来源：http://nbm.svipenyu.cn

PHP:  parent::greet();
来源：http://qwp.zdbjq.cn

JS:   super.greet();
来源：http://dtx.hongshengwenyu.top

TS:   super.greet();
来源：http://cis.tarul.cn

Java: super.greet();
来源：http://sfl.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://elv.dashuyun.cn

Ruby: super
来源：http://xkm.fengsongda.top

C#:   base.Greet();
来源：http://wje.xziqi.cn

[G08] 静态方法与属性
来源：http://mxj.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ovz.gaohongyu789.top

PHP:  public static function f() {}
来源：http://ggq.yj202588.top

JS:   static f() {}
来源：http://ust.cqqwz.cn

TS:   static f(): void {}
来源：http://ikt.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://evr.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://kzl.yfazqb.com

Ruby: def self.f; end
来源：http://bbf.haohaochexian.top

C#:   public static void F() {}
来源：http://ogk.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://oue.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://zei.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://kqu.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://skc.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://pmn.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://wjj.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://wyu.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yzd.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://fpk.pycfn.com

[G10] 访问控制
来源：http://gmx.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://onr.nanxinkj.top

PHP:  public / protected / private
来源：http://viw.tarul.cn

JS:   #private 字段；其余公开
来源：http://kzb.hesvh.cn

TS:   public / protected / private
来源：http://xut.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://myn.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jyk.ydzc1.top

Ruby: public / protected / private
来源：http://orm.9152youxi.cn

C#:   public / protected / private / internal
来源：http://ctp.wangshuangyany.cn

[G11] getter / setter
来源：http://zvm.fehbvm.com

Py:   @property 与 @x.setter
来源：http://flx.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xmv.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://lmj.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://vnp.sufxvd.cn

Java: public String getName() { return name; }
来源：http://lav.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://waz.svipenyu.cn

Ruby: attr_accessor :name
来源：http://aup.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://vfd.zhiwuduotai.top

[G12] 对象转字符串
来源：http://tjg.pycfn.com

Py:   def __str__(self): return self.name
来源：http://vdz.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eyw.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://ydb.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://gie.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://lsi.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://fqv.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://vko.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://kqp.9152youxi.cn

[G13] 判断对象类型
来源：http://wxw.yangfankeji.com

Py:   isinstance(u, User)
来源：http://dgz.wangdashe.top

PHP:  $u instanceof User
来源：http://jzc.havefunace.top

JS:   u instanceof User
来源：http://yxx.0kj1m.cn

TS:   u instanceof User
来源：http://mag.jinqigfzy.top

Java: u instanceof User
来源：http://icl.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://voj.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://uij.zdqjudy.top

C#:   u is User
来源：http://qzr.zdqjudy.top

[G14] 数据类 / record
来源：http://kta.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vwf.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://uet.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://sih.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://sos.shanyushiyangtech.top

Java: record User(String name, int age) {}
来源：http://nzs.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://zcq.tianlin.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://knl.cheryme.top

C#:   record User(string Name, int Age);
来源：http://iaf.aibaodan.cn

[G15] 枚举
来源：http://myx.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nfq.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://jys.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ehl.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qul.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://kqo.52xcode.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yfu.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://jyb.cashguo.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fns.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://znm.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xho.tanke756.top

PHP:  get_object_vars($obj);
来源：http://sfx.tian-w.cn

JS:   Object.entries(obj)
来源：http://wle.mhx1999.top

TS:   Object.entries(obj)
来源：http://qgs.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bmq.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xnv.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://pgn.zycfv.cn

C#:   // 用反射或 System.Text.Json
来源：http://dne.nwbrower.top

================================================================================
来源：http://mwa.sufxvd.cn

H. 异常与错误处理
来源：http://qwa.zdbjq.cn

================================================================================
来源：http://bqj.fzhhl.top

[H01] try / catch 基础
来源：http://huo.cdnleiting.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jex.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fwc.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vwx.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zlb.c1oappe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ggm.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lte.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vlz.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mfa.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://cab.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://jgq.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gnc.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qkq.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lfb.zhengqikj.top

Java: try { f(); } finally { cleanup(); }
来源：http://tih.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://llf.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ssi.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ycc.jlsjyb.cn

[H03] 主动抛出异常
来源：http://wym.hywenlv.cn

Py:   raise ValueError("错误信息")
来源：http://cqo.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dtr.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://trm.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://uyn.daxiang520.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uxr.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hht.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://izf.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://ffb.yuanzhike.top

[H04] 自定义异常类型
来源：http://stj.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://jvh.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://kqf.epnwcf.com

JS:   class MyError extends Error {}
来源：http://inp.yongpay.top

TS:   class MyError extends Error {}
来源：http://tli.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://tzb.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://awt.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://vep.zhaomingkeji.xyz

C#:   class MyException : Exception {}
来源：http://asp.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://lwb.haohaochexian.top

Py:   except ValueError as e:
来源：http://ljk.cashguo.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qla.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://stm.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://pxu.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://hob.c1oappe.top


<!-- 参考信息 -->