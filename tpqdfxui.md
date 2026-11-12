代发 wailian999

[F01] 读取整个文件
来源：http://ohy.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://esb.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://jrv.ywan-chungtsiang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zjx.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://los.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://qgz.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jkd.yj20258888.top

Ruby: File.read("a.txt")
来源：http://vnk.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://sef.sysykeji.top

[F02] 逐行读取文件
来源：http://vlr.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oqj.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uvj.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sri.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lki.9152youxi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zju.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://odp.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wkq.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dtw.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://qjs.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kme.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vcz.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqo.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdi.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aty.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://scm.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://fkc.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fui.guannengcc.top

[F04] 追加写入文件
来源：http://roh.yanxiufei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wuw.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pqp.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ctg.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://efh.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ram.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pyw.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jyx.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rjk.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://sza.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tzf.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://gxz.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://mud.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://zoc.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://twz.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lww.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://lcp.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://ucb.yj20258888.top

[F06] 删除文件
来源：http://cxl.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://jge.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://oqg.jiagoushi.top

JS:   fs.unlinkSync("a.txt")
来源：http://npt.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gyj.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tju.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://haz.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://svm.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://bpc.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://ntu.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gwf.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hyb.mhx1999.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pyy.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhx.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://orn.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zrj.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://awq.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://quy.kuanghao11.cn

[F08] 遍历目录
来源：http://lyz.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://noc.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ywd.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://epe.jinghuilouyu.cn

TS:   fs.readdirSync("dir")
来源：http://kgy.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ioc.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://qew.iojbl.cn

Ruby: Dir.children("dir")
来源：http://uoz.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://olf.zhongyouzk.top

[F09] 获取文件大小
来源：http://ecs.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://wod.bjfxy.top

PHP:  filesize("a.txt");
来源：http://pwr.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://lfz.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://kfm.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://jom.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jfd.yj20258.top

Ruby: File.size("a.txt")
来源：http://hpx.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://ccb.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rbn.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ofj.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://obg.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xex.iojbl.cn

TS:   path.extname("a.txt")
来源：http://zyp.shanyushiyangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dsn.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gmt.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyp.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lkn.0kj1m.cn

[F11] 复制与移动文件
来源：http://vqf.zhoulong.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rns.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nlv.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yah.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jsd.wangshuangyany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mef.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://udo.sjlbkw.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xzm.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wpw.yangfankeji.com

[F12] CSV 读写
来源：http://ufi.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lem.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hlq.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tpz.epnwcf.com

TS:   // 同上
来源：http://jct.yueranfly.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ilz.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://laf.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://szd.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cub.jinqigfzy.top

================================================================================
来源：http://frh.0kj1m.cn

G. 面向对象
来源：http://lrt.mhx1999.top

================================================================================
来源：http://knl.vehdjk.com

[G01] 定义类
来源：http://lxy.fengsongda.top

Py:   class User: pass
来源：http://fxi.jlsjyb.cn

PHP:  class User {}
来源：http://usn.yfazqb.com

JS:   class User {}
来源：http://wko.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://hts.zdqjudy.top

Java: class User {}
来源：http://zjw.ehwqpu.com

Go:   type User struct { Name string }
来源：http://ynr.zhaomingkeji.xyz

Ruby: class User; end
来源：http://txq.zhongyouzk.top

C#:   class User {}
来源：http://eff.tianlin.xyz

[G02] 构造函数
来源：http://vmn.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://atq.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://ieo.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://zfb.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://czx.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://iyc.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://axr.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://blq.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://xro.zhiwuduotai.top

[G03] 实例属性
来源：http://pwp.snrcjt.cn

Py:   self.name = "x"
来源：http://kwp.9152youxi.cn

PHP:  public string $name = "x";
来源：http://lfp.xuanzx.com

JS:   this.name = "x";
来源：http://cjt.aibaodan.cn

TS:   name: string = "x";
来源：http://wsh.vehdjk.com

Java: private String name;
来源：http://gia.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ady.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://fjc.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://axt.tanke756.top

[G04] 定义方法
来源：http://gon.daxiang520.top

Py:   def greet(self): return self.name
来源：http://cgh.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://byl.cheryme.top

JS:   greet() { return this.name; }
来源：http://hib.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://udu.epnwcf.com

Java: String greet() { return name; }
来源：http://zur.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyh.fktsv.cn

Ruby: def greet; @name; end
来源：http://rig.ivvv.top

C#:   public string Greet() => Name;
来源：http://jky.yfazqb.com

[G05] 继承
来源：http://zdi.svipenyu.cn

Py:   class Admin(User): pass
来源：http://dou.xuanzx.com

PHP:  class Admin extends User {}
来源：http://xqs.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://gge.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://rnt.jinqigfzy.top

Java: class Admin extends User {}
来源：http://rez.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xfh.fehbvm.com

Ruby: class Admin < User; end
来源：http://str.pycfn.com

C#:   class Admin : User {}
来源：http://azl.wangdashe.top

[G06] 重写方法
来源：http://iix.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://caa.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jfv.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://qyt.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://mcn.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://wus.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fnm.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://yrh.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://ymd.sjlbkw.cn

[G07] 调用父类方法
来源：http://oiv.uphjek.com

Py:   super().greet()
来源：http://yqa.yj20258.top

PHP:  parent::greet();
来源：http://rwy.aibaodan.cn

JS:   super.greet();
来源：http://yql.jyoumei.cn

TS:   super.greet();
来源：http://oqv.shanyushiyangkeji.top

Java: super.greet();
来源：http://wuj.jiagoushi.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vic.nanxinkj.top

Ruby: super
来源：http://kzc.ppjwa.cn

C#:   base.Greet();
来源：http://kio.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://rex.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fvw.daxiang520.top

PHP:  public static function f() {}
来源：http://jmq.svipenyu.cn

JS:   static f() {}
来源：http://aaw.aibaodan.cn

TS:   static f(): void {}
来源：http://ivk.yongpay.top

Java: static void f() {}
来源：http://zar.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://trw.yj202588.top

Ruby: def self.f; end
来源：http://iil.hnxiangtu.top

C#:   public static void F() {}
来源：http://lrn.yvedp.cn

[G09] 接口 / 抽象类
来源：http://eju.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://ive.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://slc.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jdw.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://uoz.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://svh.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://adt.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rqy.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://iix.sxryk.cn

[G10] 访问控制
来源：http://bci.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://hec.zhoulong.xyz

PHP:  public / protected / private
来源：http://epu.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://mly.shzxlz.cn

TS:   public / protected / private
来源：http://ijy.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://evl.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tvu.pengpengdd.cyou

Ruby: public / protected / private
来源：http://thq.52xcode.cn

C#:   public / protected / private / internal
来源：http://hyd.shanyushiyangkeji.top

[G11] getter / setter
来源：http://mef.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://tyo.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ucm.hnqzz.top

JS:   get name() { return this._name; }
来源：http://czf.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://seb.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://bzc.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hlg.xinyue.icu

Ruby: attr_accessor :name
来源：http://mgf.bbcook.cn

C#:   public string Name { get; set; }
来源：http://evd.c1oappe.top

[G12] 对象转字符串
来源：http://viz.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://hko.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://auh.uphjek.com

JS:   toString() { return this.name; }
来源：http://ecg.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://ong.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://oph.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://pzi.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://ylg.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://vkb.yueranfly.top

[G13] 判断对象类型
来源：http://zhx.smart0.xyz

Py:   isinstance(u, User)
来源：http://mgb.jqgfzy.top

PHP:  $u instanceof User
来源：http://quc.jqgufenzy.top

JS:   u instanceof User
来源：http://cgb.sufxvd.cn

TS:   u instanceof User
来源：http://kal.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://bgg.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tyo.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://nhi.ydzc1.top

C#:   u is User
来源：http://hsu.xinyue.icu

[G14] 数据类 / record
来源：http://sng.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uco.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://iag.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://vmr.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://zek.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://int.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://mpo.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oab.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://btj.ydjk.org.cn

[G15] 枚举
来源：http://bcb.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jpz.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjm.gaohongyu789.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://emk.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yuo.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://fkk.fengsongda.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jvs.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://jri.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rzy.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://hcb.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ush.hammf.cn

PHP:  get_object_vars($obj);
来源：http://apd.sufxvd.cn

JS:   Object.entries(obj)
来源：http://raa.ybcxt.top

TS:   Object.entries(obj)
来源：http://dmv.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yqu.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://phf.wangdashe.top

Ruby: obj.instance_variables
来源：http://zec.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://ehd.pycfn.com

================================================================================
来源：http://shb.jinqigufen.top

H. 异常与错误处理
来源：http://lgh.hysaishi.cn

================================================================================
来源：http://ile.yongpay.top

[H01] try / catch 基础
来源：http://ewn.yj20258.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mko.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hlq.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wpr.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wqd.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://izg.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yib.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wef.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://svq.aizwys.cn

[H02] finally / ensure 收尾
来源：http://tci.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nwt.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gnw.jqgfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aib.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jjg.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://urq.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://acp.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tcc.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rpc.hnqzz.top

[H03] 主动抛出异常
来源：http://fzt.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://eiz.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kwp.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://ant.yuanzhike.top

TS:   throw new Error("错误信息");
来源：http://eac.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mmb.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sjr.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jpx.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://pdv.zdqjudy.top

[H04] 自定义异常类型
来源：http://ebm.sweek.top

Py:   class MyError(Exception): pass
来源：http://gzt.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rex.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://ayu.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://grw.yueranfly.top

Java: class MyException extends RuntimeException {}
来源：http://wqx.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szu.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://bsu.tanke756.top

C#:   class MyException : Exception {}
来源：http://tyx.52xcode.cn

[H05] 捕获特定类型
来源：http://evg.zdbjq.cn

Py:   except ValueError as e:
来源：http://bsd.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zwu.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ysi.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://tlh.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://ucs.uphjek.com


<!-- 参考信息 -->