代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://qhk.redwolf501.top

[F02] 逐行读取文件
来源：http://ejn.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ror.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gjj.shanyushiyangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://naq.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oiq.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kgy.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vhi.hcnkem.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://esr.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cng.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://acj.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ugw.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://okn.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sot.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rlm.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://idn.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zwr.yuxming.cn

Ruby: File.write("a.txt", "hi")
来源：http://sbq.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jki.c1oappe.top

[F04] 追加写入文件
来源：http://omw.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkt.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://abc.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mtx.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yup.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ubm.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ndw.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ywb.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mxk.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://ffo.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ijo.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://vyc.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://yjb.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://ifn.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://rhv.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rku.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://npo.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://vgo.zhoulong.xyz

[F06] 删除文件
来源：http://ahq.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://uiw.bbcook.cn

PHP:  unlink("a.txt");
来源：http://nil.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://tus.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uek.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zsb.zhixingplan.top

Go:   os.Remove("a.txt")
来源：http://kiu.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://fxf.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://psn.iojbl.cn

[F07] 创建目录（含多级）
来源：http://mzq.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fsb.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aco.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szf.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jhg.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://amj.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dpm.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://the.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gjj.yj20258888.top

[F08] 遍历目录
来源：http://xbc.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://gkg.hysaishi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://waj.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://kwz.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://uws.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iut.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iyp.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://rhm.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://ycq.bbcook.cn

[F09] 获取文件大小
来源：http://ysb.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://dwk.vehdjk.com

PHP:  filesize("a.txt");
来源：http://gbv.gotoacloud.top

JS:   fs.statSync("a.txt").size
来源：http://wtc.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://sdd.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cfp.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ifn.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://jer.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://uag.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://pfy.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xct.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sra.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vik.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://nnc.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qrs.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dms.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oej.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qrt.cucudq.cn

[F11] 复制与移动文件
来源：http://fxr.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hqa.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://coz.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pin.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqn.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xkn.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dqd.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://llv.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hhi.tanke756.top

[F12] CSV 读写
来源：http://sdf.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://upb.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xll.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eaf.jianghu66.top

TS:   // 同上
来源：http://xha.bjfxy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ncy.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yrm.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tkj.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rgv.chenzaomai.com

================================================================================
来源：http://lut.zhengqikj.top

G. 面向对象
来源：http://zqf.yvedp.cn

================================================================================
来源：http://nnc.fehbvm.com

[G01] 定义类
来源：http://lmc.uphjek.com

Py:   class User: pass
来源：http://qtv.chenzaomai.com

PHP:  class User {}
来源：http://tos.316326.xyz

JS:   class User {}
来源：http://fol.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://uxj.yj20258888.top

Java: class User {}
来源：http://gcq.yueranfly.top

Go:   type User struct { Name string }
来源：http://rsl.bjfxy.top

Ruby: class User; end
来源：http://grz.sxryk.cn

C#:   class User {}
来源：http://vej.zhoulong.xyz

[G02] 构造函数
来源：http://nid.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://gwm.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://swg.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://swa.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://uur.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://zpm.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qhe.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://hci.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://ktr.ivvv.top

[G03] 实例属性
来源：http://lec.zhoulong.xyz

Py:   self.name = "x"
来源：http://fhi.cqqwz.cn

PHP:  public string $name = "x";
来源：http://wlu.snrcjt.cn

JS:   this.name = "x";
来源：http://osq.gzhubu.top

TS:   name: string = "x";
来源：http://xry.yvedp.cn

Java: private String name;
来源：http://gfv.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tyk.zdqjudy.top

Ruby: @name = "x"
来源：http://czf.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jbb.redwolf501.top

[G04] 定义方法
来源：http://pry.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://tta.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hdv.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://ylk.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://nzs.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://ufh.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mbz.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://mhq.epnwcf.com

C#:   public string Greet() => Name;
来源：http://mni.hywenlv.cn

[G05] 继承
来源：http://taz.redwolf501.top

Py:   class Admin(User): pass
来源：http://fyg.yueranfly.top

PHP:  class Admin extends User {}
来源：http://hku.gzhubu.top

JS:   class Admin extends User {}
来源：http://oam.gogol.net.cn

TS:   class Admin extends User {}
来源：http://owt.vqdsnc.cn

Java: class Admin extends User {}
来源：http://uan.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ngt.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://eie.sweek.top

C#:   class Admin : User {}
来源：http://sht.xuetiantiany.cn

[G06] 重写方法
来源：http://jpg.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://okb.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://reb.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://qti.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://zeo.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://xpn.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rgg.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://ifx.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://nwg.ivvv.top

[G07] 调用父类方法
来源：http://vqt.9152youxi.cn

Py:   super().greet()
来源：http://hft.ydzc1.top

PHP:  parent::greet();
来源：http://rwf.sjlbkw.cn

JS:   super.greet();
来源：http://xzi.yvedp.cn

TS:   super.greet();
来源：http://gzd.cdnleiting.top

Java: super.greet();
来源：http://bvj.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mqy.shzxlz.cn

Ruby: super
来源：http://xjl.meibo888.top

C#:   base.Greet();
来源：http://mll.hfpthk.cn

[G08] 静态方法与属性
来源：http://wgy.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lxa.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://qio.hammf.cn

JS:   static f() {}
来源：http://dqb.ppjwa.cn

TS:   static f(): void {}
来源：http://gmy.jqgfzy.top

Java: static void f() {}
来源：http://zyg.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://myf.tanke756.top

Ruby: def self.f; end
来源：http://drj.zdbjq.cn

C#:   public static void F() {}
来源：http://qnz.xylfe.cn

[G09] 接口 / 抽象类
来源：http://gxa.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://uvn.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://pzv.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vmh.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://noi.cheryme.top

Java: interface Shape { double area(); }
来源：http://cpz.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://fnp.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kmj.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://rys.xinyue.icu

[G10] 访问控制
来源：http://xyx.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://qhb.shuidangran.top

PHP:  public / protected / private
来源：http://uhv.fzhhl.top

JS:   #private 字段；其余公开
来源：http://kkk.fanxiaobao.xyz

TS:   public / protected / private
来源：http://ics.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://zzx.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://wpn.shuidangran.top

Ruby: public / protected / private
来源：http://dju.uphjek.com

C#:   public / protected / private / internal
来源：http://fkb.haohaochexian.top

[G11] getter / setter
来源：http://oka.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://nlm.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tgu.uphjek.com

JS:   get name() { return this._name; }
来源：http://sls.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://oay.aibaodan.cn

Java: public String getName() { return name; }
来源：http://utr.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rkz.xziqi.cn

Ruby: attr_accessor :name
来源：http://epw.uphjek.com

C#:   public string Name { get; set; }
来源：http://goq.ehwqpu.com

[G12] 对象转字符串
来源：http://fyq.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://zyb.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nau.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://zxn.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://eku.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://hgv.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://wcy.yj20258888.top

Ruby: def to_s; @name; end
来源：http://ffk.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://yao.hywenlv.cn

[G13] 判断对象类型
来源：http://dab.sweek.top

Py:   isinstance(u, User)
来源：http://jdr.yanxiufei.cn

PHP:  $u instanceof User
来源：http://thv.yangfankeji.com

JS:   u instanceof User
来源：http://qvb.gzhubu.top

TS:   u instanceof User
来源：http://jon.daria6918.cn

Java: u instanceof User
来源：http://hrb.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qgw.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://kkz.svipenyu.cn

C#:   u is User
来源：http://ztt.yuanzhike.top

[G14] 数据类 / record
来源：http://cay.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://clt.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://rgb.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://lda.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://nvb.mhx1999.top

Java: record User(String name, int age) {}
来源：http://bkr.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://lib.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vvx.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://ijf.yvedp.cn

[G15] 枚举
来源：http://aen.jianghu66.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://usz.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://spg.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://poe.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://upy.pycfn.com

Java: enum Color { RED, GREEN }
来源：http://mzr.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ekc.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://tyw.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://woc.fehbvm.com

[G16] 对象转数组 / 字典
来源：http://osr.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://swf.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://rto.jiagoushi.top

JS:   Object.entries(obj)
来源：http://ajs.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://jdb.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://adm.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://kkf.redwolf501.top

Ruby: obj.instance_variables
来源：http://joc.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://zur.zycfv.cn

================================================================================
来源：http://chq.tanke756.top

H. 异常与错误处理
来源：http://hve.52xcode.cn

================================================================================
来源：http://lbn.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://wqx.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://npu.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://piy.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://exf.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fot.hnxiangtu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ayj.316326.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jft.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pqg.xuanzx.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nbg.shanyushiyangtech.top

[H02] finally / ensure 收尾
来源：http://lbl.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://smm.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://gvp.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://beg.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fwi.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://yuo.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tbg.hysaishi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://apx.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pmv.zhoulong.xyz

[H03] 主动抛出异常
来源：http://cca.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://coq.zhixingplan.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cys.havefunace.top

JS:   throw new Error("错误信息");
来源：http://bhe.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://vfk.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ykr.daxiang520.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbf.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sgn.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qxf.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://wra.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://cli.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://adt.havefunace.top

JS:   class MyError extends Error {}
来源：http://oms.tianlin.xyz

TS:   class MyError extends Error {}
来源：http://klo.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://alq.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mwt.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://npq.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://vhn.jianghu66.top

[H05] 捕获特定类型
来源：http://twq.haohaochexian.top

Py:   except ValueError as e:
来源：http://ezr.gogol.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pye.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://osx.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://ztd.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://jag.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lfd.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://jqh.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cwc.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://dtr.yj20258.top

Py:   value = d.get("k") or default
来源：http://ugv.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://oqb.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rwg.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://chc.fzhhl.top


<!-- 参考信息 -->