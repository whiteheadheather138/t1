代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zfc.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lef.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://eca.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iam.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wnn.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://atu.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mgb.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wui.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://esf.sweek.top

Ruby: File.write("a.txt", "hi")
来源：http://xsa.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kbg.shzxlz.cn

[F04] 追加写入文件
来源：http://fzt.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jih.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gpi.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://akg.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wzh.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbm.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xyb.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ovp.xuanzx.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kbt.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://rye.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pxx.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://yhj.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://irc.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://mjt.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jon.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kwi.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://trr.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://oxy.fehbvm.com

[F06] 删除文件
来源：http://nvr.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://gyj.hammf.cn

PHP:  unlink("a.txt");
来源：http://kav.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://dye.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://hfw.jyoumei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://con.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://roq.ivvv.top

Ruby: File.delete("a.txt")
来源：http://fqy.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://wgu.xuanzx.com

[F07] 创建目录（含多级）
来源：http://pnj.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nhe.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jli.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sab.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nbt.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fcx.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sdt.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dhs.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ova.ehwqpu.com

[F08] 遍历目录
来源：http://ann.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nae.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nli.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://ild.fzhhl.top

TS:   fs.readdirSync("dir")
来源：http://mrt.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vtl.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wbt.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://wql.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://stx.pycfn.com

[F09] 获取文件大小
来源：http://wxq.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://txt.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://cez.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://byl.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://hgy.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bno.birdmap.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rhb.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://fcv.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://nft.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://moy.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nwf.uphjek.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://trp.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kcu.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://kkd.hesvh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cll.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bmw.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mqu.fanxiaobao.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ufa.tarul.cn

[F11] 复制与移动文件
来源：http://rjk.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fdq.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://msz.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://feg.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cff.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blq.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ylf.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fct.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gzi.birdmap.top

[F12] CSV 读写
来源：http://ein.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmm.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lug.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uph.xziqi.cn

TS:   // 同上
来源：http://cow.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sbt.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://heu.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xbi.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://acb.andypj.xyz

================================================================================
来源：http://wng.yj202588.top

G. 面向对象
来源：http://dxl.ybcxt.top

================================================================================
来源：http://fld.nanxuanxn.top

[G01] 定义类
来源：http://ofu.jqgfzy.top

Py:   class User: pass
来源：http://qgh.nanxuanxn.top

PHP:  class User {}
来源：http://ptj.tian-w.cn

JS:   class User {}
来源：http://nxx.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://vgu.hfpthk.cn

Java: class User {}
来源：http://zrp.gzhubu.top

Go:   type User struct { Name string }
来源：http://vxz.dashuyun.cn

Ruby: class User; end
来源：http://frv.gzhubu.top

C#:   class User {}
来源：http://enq.hongshengwenyu.top

[G02] 构造函数
来源：http://myf.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://uxx.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://jgo.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://utk.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://jpg.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://jwf.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://noe.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://ofg.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://zkb.dianchejie.cn

[G03] 实例属性
来源：http://urw.chenjidiqi.icu

Py:   self.name = "x"
来源：http://qcc.ivvv.top

PHP:  public string $name = "x";
来源：http://okj.jinqigfzy.top

JS:   this.name = "x";
来源：http://tvb.yuanzhike.top

TS:   name: string = "x";
来源：http://jrh.svipenyu.cn

Java: private String name;
来源：http://ayc.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mcr.fzhhl.top

Ruby: @name = "x"
来源：http://vxb.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://paa.chenlongwang.top

[G04] 定义方法
来源：http://jih.daria6918.cn

Py:   def greet(self): return self.name
来源：http://bhe.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://uoj.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://bny.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://vbb.yuxming.cn

Java: String greet() { return name; }
来源：http://ujf.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://atx.xziqi.cn

Ruby: def greet; @name; end
来源：http://rna.nwbrower.top

C#:   public string Greet() => Name;
来源：http://cmu.hysaishi.cn

[G05] 继承
来源：http://deq.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://div.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://ynw.sysykeji.top

JS:   class Admin extends User {}
来源：http://vsc.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://rkf.gotoacloud.top

Java: class Admin extends User {}
来源：http://yxt.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://luy.yj20258.top

Ruby: class Admin < User; end
来源：http://pgg.snrcjt.cn

C#:   class Admin : User {}
来源：http://mtk.zhaomingkeji.xyz

[G06] 重写方法
来源：http://krt.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://jpd.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qha.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://grk.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://udz.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://aoi.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mfy.xingfuxueyuan.xyz

Ruby: def greet; "admin"; end
来源：http://bud.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://opy.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://gxd.hnxiangtu.top

Py:   super().greet()
来源：http://upo.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://ltl.xuanzx.com

JS:   super.greet();
来源：http://pgy.jiagoushi.top

TS:   super.greet();
来源：http://ggy.bjfxy.top

Java: super.greet();
来源：http://zcy.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://die.zhengqikj.top

Ruby: super
来源：http://xlb.zhijiandao.cn

C#:   base.Greet();
来源：http://luo.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://mpg.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vuv.zdbjq.cn

PHP:  public static function f() {}
来源：http://qky.fktsv.cn

JS:   static f() {}
来源：http://lqd.hnqzz.top

TS:   static f(): void {}
来源：http://xfd.yj20258888.top

Java: static void f() {}
来源：http://bhh.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://wor.gaohongyu789.top

Ruby: def self.f; end
来源：http://yui.zhijiandao.cn

C#:   public static void F() {}
来源：http://ioz.52xcode.cn

[G09] 接口 / 抽象类
来源：http://vmh.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://mek.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fvk.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sik.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://nyh.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://mhp.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://bbj.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kol.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://svg.wangshuangyany.cn

[G10] 访问控制
来源：http://fdr.uphjek.com

Py:   约定 _protected / __private（不强制）
来源：http://yil.zhijiandao.cn

PHP:  public / protected / private
来源：http://vld.hesvh.cn

JS:   #private 字段；其余公开
来源：http://lrd.kuanghao11.cn

TS:   public / protected / private
来源：http://tfk.hysaishi.cn

Java: public / protected / private / 默认包级
来源：http://dba.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qvx.sufxvd.cn

Ruby: public / protected / private
来源：http://bky.yj202588.top

C#:   public / protected / private / internal
来源：http://hxy.xuetiantiany.cn

[G11] getter / setter
来源：http://pwn.epnwcf.com

Py:   @property 与 @x.setter
来源：http://ajz.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ekz.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://dxb.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://yla.hesvh.cn

Java: public String getName() { return name; }
来源：http://qlq.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qbp.ydzc1.top

Ruby: attr_accessor :name
来源：http://fhz.316326.xyz

C#:   public string Name { get; set; }
来源：http://ktp.316326.xyz

[G12] 对象转字符串
来源：http://usy.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://pwd.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ddf.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://zij.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://svx.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://gto.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://pfl.c1oappe.top

Ruby: def to_s; @name; end
来源：http://beu.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://lks.guannengcc.top

[G13] 判断对象类型
来源：http://vci.chenlongwang.top

Py:   isinstance(u, User)
来源：http://zzt.svipenyu.cn

PHP:  $u instanceof User
来源：http://sct.meibo888.top

JS:   u instanceof User
来源：http://ihw.jinqigfzy.top

TS:   u instanceof User
来源：http://xho.quarkkingdee.top

Java: u instanceof User
来源：http://rmp.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sej.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://zzf.zdqjudy.top

C#:   u is User
来源：http://aad.52xcode.cn

[G14] 数据类 / record
来源：http://lbd.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://som.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://hbj.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://yvs.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://wic.iojbl.cn

Java: record User(String name, int age) {}
来源：http://egr.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://hkh.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ioy.dianchejie.cn

C#:   record User(string Name, int Age);
来源：http://sqk.cucudq.cn

[G15] 枚举
来源：http://qpx.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xer.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gws.sweek.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://env.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cvl.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://uwq.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://upj.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://npr.yongpay.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xgl.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://thc.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wed.uphjek.com

PHP:  get_object_vars($obj);
来源：http://pmh.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://xbt.xylfe.cn

TS:   Object.entries(obj)
来源：http://yjo.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bjk.gogol.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eec.ehwqpu.com

Ruby: obj.instance_variables
来源：http://dxv.tarul.cn

C#:   // 用反射或 System.Text.Json
来源：http://hxm.feifeiyinyue.top

================================================================================
来源：http://ooq.dashuyun.cn

H. 异常与错误处理
来源：http://apj.snrcjt.cn

================================================================================
来源：http://zze.tanke756.top

[H01] try / catch 基础
来源：http://pof.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kfh.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://slx.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ueo.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bms.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://adu.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lhc.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xew.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xwi.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://jln.hywenlv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fjc.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ymr.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tmn.pengpengdd.cyou

TS:   try { f(); } finally { cleanup(); }
来源：http://xhg.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ron.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://kay.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bkw.zhixingplan.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dlt.pycfn.com

[H03] 主动抛出异常
来源：http://aaj.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://qmr.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ymo.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://dob.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://hlt.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vpw.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhr.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://who.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eqq.jqgufenzy.top

[H04] 自定义异常类型
来源：http://kqt.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://jwn.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://qof.sxryk.cn

JS:   class MyError extends Error {}
来源：http://iif.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://tmd.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://rgw.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://frr.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://had.sxryk.cn

C#:   class MyException : Exception {}
来源：http://wsp.jlsjyb.cn

[H05] 捕获特定类型
来源：http://zwj.ybcxt.top

Py:   except ValueError as e:
来源：http://mht.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dqz.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://dlw.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://kpx.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://ovs.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zym.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://vpk.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfa.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://rlp.yongpay.top

Py:   value = d.get("k") or default
来源：http://wcg.shanyushiyangtech.top

PHP:  $v = $d["k"] ?? null;
来源：http://cki.ybcxt.top

JS:   obj?.a?.b;  d ?? default
来源：http://qkw.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uam.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sub.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ahd.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://grv.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://smu.xylfe.cn

[H07] 断言
来源：http://vso.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://ufj.mhx1999.top

PHP:  assert($x > 0);
来源：http://lrp.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://ije.snrcjt.cn


<!-- 参考信息 -->