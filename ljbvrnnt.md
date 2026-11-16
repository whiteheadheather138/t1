代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bsm.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xwb.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://ewu.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ndw.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uok.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zpw.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wva.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ikx.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://czk.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://xjh.haohaochexian.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oym.chenlongwang.top

[F04] 追加写入文件
来源：http://gnb.0kj1m.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ueb.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ixi.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://irc.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkv.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qfe.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://quv.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tnb.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hdm.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://lve.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://odz.c1oappe.top

PHP:  file_exists("a.txt");
来源：http://als.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://uar.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://mry.guannengcc.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lou.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xkp.xylfe.cn

Ruby: File.exist?("a.txt")
来源：http://oci.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://jvt.vqdsnc.cn

[F06] 删除文件
来源：http://jrs.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://tow.fehbvm.com

PHP:  unlink("a.txt");
来源：http://loh.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://sry.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://gdf.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qli.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://fjo.iojbl.cn

Ruby: File.delete("a.txt")
来源：http://bgz.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://wus.yonumen.top

[F07] 创建目录（含多级）
来源：http://cvy.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zww.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qvn.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aqw.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qgj.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hew.xylfe.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mkh.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://apt.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vin.hysaishi.cn

[F08] 遍历目录
来源：http://fzl.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lco.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fdo.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://cut.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://iqs.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bwh.wangdashe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ood.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://jgc.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://tbt.jyoumei.cn

[F09] 获取文件大小
来源：http://bvt.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://bmy.hnqzz.top

PHP:  filesize("a.txt");
来源：http://nyk.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://rxy.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://abp.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://iiv.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hig.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://nfc.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://nne.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://zju.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mtx.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pxc.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vep.jianghu66.top

TS:   path.extname("a.txt")
来源：http://vhd.fktsv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uvo.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nsf.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pdb.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qtg.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://vvq.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wwz.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bsw.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://amg.aibaodan.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mte.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zqc.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgl.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbo.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qyq.sufxvd.cn

[F12] CSV 读写
来源：http://dyy.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zdw.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://clh.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://abq.yongpay.top

TS:   // 同上
来源：http://rmg.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ecs.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ukm.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mmx.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bpe.jinghuilouyu.cn

================================================================================
来源：http://jbs.gzhubu.top

G. 面向对象
来源：http://qtj.cdnleiting.top

================================================================================
来源：http://oox.gogol.net.cn

[G01] 定义类
来源：http://uku.shangyingyoupin.top

Py:   class User: pass
来源：http://gwz.hnxiangtu.top

PHP:  class User {}
来源：http://piz.uphjek.com

JS:   class User {}
来源：http://zlz.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://dks.vehdjk.com

Java: class User {}
来源：http://wgt.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://bmd.sysykeji.top

Ruby: class User; end
来源：http://oyx.zhiwuduotai.top

C#:   class User {}
来源：http://xdv.chenzaomai.com

[G02] 构造函数
来源：http://fnk.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://cax.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://wvm.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://jtb.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://yxz.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://hus.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pwy.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://vol.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://hfk.hesvh.cn

[G03] 实例属性
来源：http://uqf.ybcxt.top

Py:   self.name = "x"
来源：http://ysn.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://lxx.hnxiangtu.top

JS:   this.name = "x";
来源：http://chy.hysaishi.cn

TS:   name: string = "x";
来源：http://njz.shzxlz.cn

Java: private String name;
来源：http://fnc.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nwm.fengsongda.top

Ruby: @name = "x"
来源：http://dbe.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://mfm.nanxinkj.top

[G04] 定义方法
来源：http://uuu.jianghu66.top

Py:   def greet(self): return self.name
来源：http://aav.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rpr.ivvv.top

JS:   greet() { return this.name; }
来源：http://qoe.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://wqw.aibaodan.cn

Java: String greet() { return name; }
来源：http://qqc.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hqr.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://csk.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://pca.xuanzx.com

[G05] 继承
来源：http://fdo.bjfxy.top

Py:   class Admin(User): pass
来源：http://zhp.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://cbm.316326.xyz

JS:   class Admin extends User {}
来源：http://pge.yfazqb.com

TS:   class Admin extends User {}
来源：http://uuj.nanxuanxn.top

Java: class Admin extends User {}
来源：http://fvc.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vdg.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://dae.ehwqpu.com

C#:   class Admin : User {}
来源：http://sym.cashguo.top

[G06] 重写方法
来源：http://pjv.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://ehv.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ged.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://rtc.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://vni.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://kou.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jwt.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://avc.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://jwf.52xcode.cn

[G07] 调用父类方法
来源：http://zdf.guowangkeji.top

Py:   super().greet()
来源：http://lbm.jlsjyb.cn

PHP:  parent::greet();
来源：http://uqf.shuidangran.top

JS:   super.greet();
来源：http://xlo.pycfn.com

TS:   super.greet();
来源：http://gwe.ydzc1.top

Java: super.greet();
来源：http://vrg.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dbh.shzxlz.cn

Ruby: super
来源：http://krz.jinqigfzy.top

C#:   base.Greet();
来源：http://rdq.cucudq.cn

[G08] 静态方法与属性
来源：http://xrj.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://shd.nwbrower.top

PHP:  public static function f() {}
来源：http://yni.yj20258.top

JS:   static f() {}
来源：http://zba.yvedp.cn

TS:   static f(): void {}
来源：http://whx.gotoacloud.top

Java: static void f() {}
来源：http://caz.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://qfk.zdqjudy.top

Ruby: def self.f; end
来源：http://aut.tarul.cn

C#:   public static void F() {}
来源：http://nga.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://hgj.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://sbi.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qrf.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tbn.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://noc.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://qmd.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://veh.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://giu.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://rlt.guannengcc.top

[G10] 访问控制
来源：http://fdi.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://ftf.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://djf.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://him.pycfn.com

TS:   public / protected / private
来源：http://jnn.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://brz.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bdj.redwolf501.top

Ruby: public / protected / private
来源：http://tjm.gotoacloud.top

C#:   public / protected / private / internal
来源：http://kff.yueranfly.top

[G11] getter / setter
来源：http://pap.tian-w.cn

Py:   @property 与 @x.setter
来源：http://lyo.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mpf.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://vse.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://fgx.zycfv.cn

Java: public String getName() { return name; }
来源：http://uwj.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hyr.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://gqv.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://ucn.shanyushiyangtech.top

[G12] 对象转字符串
来源：http://jbl.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://bte.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mlq.jianghu66.top

JS:   toString() { return this.name; }
来源：http://szw.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://bbi.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://gzm.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://xul.hnqzz.top

Ruby: def to_s; @name; end
来源：http://lvl.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://wtb.zhengqikj.top

[G13] 判断对象类型
来源：http://wad.pycfn.com

Py:   isinstance(u, User)
来源：http://ivn.yfazqb.com

PHP:  $u instanceof User
来源：http://rcd.cqqwz.cn

JS:   u instanceof User
来源：http://vbd.gaohongyu789.top

TS:   u instanceof User
来源：http://clw.yvedp.cn

Java: u instanceof User
来源：http://bmz.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mpp.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://egv.pengpengdd.cyou

C#:   u is User
来源：http://fgg.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://jnq.fengsongda.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sxj.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://yan.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zti.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://kua.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://uva.sweek.top

Go:   type User struct { Name string; Age int }
来源：http://jjj.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tsx.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://rxg.chenjidiqi.icu

[G15] 枚举
来源：http://fxr.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yxz.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mik.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tip.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eay.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://nwo.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kvf.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://gtz.hfpthk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gbj.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://lao.sweek.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://htw.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://zkb.fktsv.cn

JS:   Object.entries(obj)
来源：http://frh.sysykeji.top

TS:   Object.entries(obj)
来源：http://bxt.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kuf.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://brf.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://afl.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://hna.xuetiantiany.cn

================================================================================
来源：http://gfw.shanyushiyangtech.top

H. 异常与错误处理
来源：http://qzl.gzhubu.top

================================================================================
来源：http://suq.pycfn.com

[H01] try / catch 基础
来源：http://grd.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iuk.sxryk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kny.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jop.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://iwv.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hlv.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://owx.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fqj.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gmk.tian-w.cn

[H02] finally / ensure 收尾
来源：http://gnw.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://kxg.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kgl.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ztv.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://nmc.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zxa.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fxh.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://zcz.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wyj.gotoacloud.top

[H03] 主动抛出异常
来源：http://fgo.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://jsx.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bnh.jinghuilouyu.cn

JS:   throw new Error("错误信息");
来源：http://kpm.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://tmr.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vcs.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fgb.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bef.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://bxa.yueranfly.top

[H04] 自定义异常类型
来源：http://npl.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://fjw.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://jul.guowangkeji.top

JS:   class MyError extends Error {}
来源：http://hhm.wangdashe.top

TS:   class MyError extends Error {}
来源：http://upf.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://tiz.iojbl.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xhr.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://zzt.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://zvt.zhixingplan.top

[H05] 捕获特定类型
来源：http://mqc.hesvh.cn

Py:   except ValueError as e:
来源：http://ndk.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qdf.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://fxg.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://edr.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://zgp.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tpm.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://qcn.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pnt.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://uqf.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://nje.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://qvq.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xhz.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://qwn.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dma.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ecb.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://frh.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://jba.dianchejie.cn

[H07] 断言
来源：http://ovu.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://jrv.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://lqj.andypj.xyz

JS:   console.assert(x > 0);
来源：http://paq.xingfuxueyuan.xyz


<!-- 参考信息 -->