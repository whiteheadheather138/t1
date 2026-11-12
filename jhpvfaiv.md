代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xsn.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blj.yongpay.top

[F03] 写入文件（覆盖）
来源：http://ooi.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xum.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rsg.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tmt.yj20258888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xod.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bfc.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxm.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://bow.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zwy.kuanghao11.cn

[F04] 追加写入文件
来源：http://gwj.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ksu.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tka.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oet.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uev.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://llb.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jrw.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrh.chenjidiqi.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rmc.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://txs.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ojn.fengsongda.top

PHP:  file_exists("a.txt");
来源：http://jqq.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://lkb.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://aiq.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://elu.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rcy.sweek.top

Ruby: File.exist?("a.txt")
来源：http://uoh.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://eys.xuetiantiany.cn

[F06] 删除文件
来源：http://ppp.yonumen.top

Py:   os.remove("a.txt")
来源：http://nwr.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://amr.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uyy.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://pvu.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggy.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://hge.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://ndf.birdmap.top

C#:   File.Delete("a.txt");
来源：http://gza.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://pfb.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ops.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://brb.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lev.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dsn.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rce.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fiq.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tju.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bhm.zhiwuduotai.top

[F08] 遍历目录
来源：http://ivf.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jkv.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yfb.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://fvd.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://khi.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://msr.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nkz.tian-w.cn

Ruby: Dir.children("dir")
来源：http://gor.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://lrj.daxiang520.top

[F09] 获取文件大小
来源：http://aas.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://hoj.gzhubu.top

PHP:  filesize("a.txt");
来源：http://uep.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://nuf.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://xeb.tanke756.top

Java: Files.size(Path.of("a.txt"))
来源：http://qtw.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gyg.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://hos.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://fla.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://qlf.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hvp.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ezr.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ahw.sxryk.cn

TS:   path.extname("a.txt")
来源：http://uri.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://guh.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hpa.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://esj.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aqh.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://fqp.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pkd.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kbx.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dfr.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pgq.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://shf.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tym.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eeg.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iil.feifeiyinyue.top

[F12] CSV 读写
来源：http://prp.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fzk.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kws.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ssm.fanxiaobao.xyz

TS:   // 同上
来源：http://lbh.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qwa.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxb.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://szj.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://grz.jyoumei.cn

================================================================================
来源：http://gal.xuetiantiany.cn

G. 面向对象
来源：http://dhx.nanxinkj.top

================================================================================
来源：http://cvo.yj20258888.top

[G01] 定义类
来源：http://ciz.snrcjt.cn

Py:   class User: pass
来源：http://dei.feifeiyinyue.top

PHP:  class User {}
来源：http://ngp.chenjidiqi.icu

JS:   class User {}
来源：http://zpf.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://tep.shangyingyoupin.top

Java: class User {}
来源：http://yof.cheryme.top

Go:   type User struct { Name string }
来源：http://xgs.hongshengwenyu.top

Ruby: class User; end
来源：http://vgs.jlsjyb.cn

C#:   class User {}
来源：http://uwg.yanxiufei.cn

[G02] 构造函数
来源：http://zss.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://kdc.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://foq.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://ard.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://yqb.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://irq.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vuh.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://zjs.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://bdb.fehbvm.com

[G03] 实例属性
来源：http://ukb.aibaodan.cn

Py:   self.name = "x"
来源：http://brc.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://rql.jqgufenzy.top

JS:   this.name = "x";
来源：http://idd.jqgfzy.top

TS:   name: string = "x";
来源：http://ggp.zhengqikj.top

Java: private String name;
来源：http://bqd.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qfc.chenzaomai.com

Ruby: @name = "x"
来源：http://hfw.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://mfp.hammf.cn

[G04] 定义方法
来源：http://lji.iojbl.cn

Py:   def greet(self): return self.name
来源：http://kgk.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wms.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://ixp.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://lat.9152youxi.cn

Java: String greet() { return name; }
来源：http://wtl.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://osv.yonumen.top

Ruby: def greet; @name; end
来源：http://xbu.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://ocs.hongshengwenyu.top

[G05] 继承
来源：http://vwl.andypj.xyz

Py:   class Admin(User): pass
来源：http://jaq.xziqi.cn

PHP:  class Admin extends User {}
来源：http://cns.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://ltu.cqqwz.cn

TS:   class Admin extends User {}
来源：http://edr.jianghu66.top

Java: class Admin extends User {}
来源：http://xox.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mnt.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://uvg.sjlbkw.cn

C#:   class Admin : User {}
来源：http://jdk.epnwcf.com

[G06] 重写方法
来源：http://rix.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://wvc.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://wfa.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://cly.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://sab.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://eoe.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vud.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://yzz.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://sqq.guannengcc.top

[G07] 调用父类方法
来源：http://nvc.yueranfly.top

Py:   super().greet()
来源：http://tmg.dianchejie.cn

PHP:  parent::greet();
来源：http://fxs.shangyingyoupin.top

JS:   super.greet();
来源：http://xwb.havefunace.top

TS:   super.greet();
来源：http://bhg.hywenlv.cn

Java: super.greet();
来源：http://wbo.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bar.yuxming.cn

Ruby: super
来源：http://eyq.sysykeji.top

C#:   base.Greet();
来源：http://eqf.jinqigufen.top

[G08] 静态方法与属性
来源：http://naz.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cor.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://gbf.zhixingplan.top

JS:   static f() {}
来源：http://wgt.yuanzhike.top

TS:   static f(): void {}
来源：http://qpk.jinqigfzy.top

Java: static void f() {}
来源：http://epf.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujg.gaohongyu789.top

Ruby: def self.f; end
来源：http://xbi.jianghu66.top

C#:   public static void F() {}
来源：http://xhc.bbcook.cn

[G09] 接口 / 抽象类
来源：http://tzz.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://clt.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://trz.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dol.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://zja.cucudq.cn

Java: interface Shape { double area(); }
来源：http://xpz.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://tef.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wwm.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://voa.bbcook.cn

[G10] 访问控制
来源：http://lir.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://xyz.shangyingyoupin.top

PHP:  public / protected / private
来源：http://dbu.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://wkv.sufxvd.cn

TS:   public / protected / private
来源：http://cno.316326.xyz

Java: public / protected / private / 默认包级
来源：http://ffs.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ypx.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://vtt.yueranfly.top

C#:   public / protected / private / internal
来源：http://wbn.gzhubu.top

[G11] getter / setter
来源：http://xhx.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://ahx.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ioe.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://osh.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://kjq.9152youxi.cn

Java: public String getName() { return name; }
来源：http://owu.guannengcc.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ygl.9152youxi.cn

Ruby: attr_accessor :name
来源：http://due.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://kyj.0kj1m.cn

[G12] 对象转字符串
来源：http://qke.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://sok.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vrr.vehdjk.com

JS:   toString() { return this.name; }
来源：http://njs.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://lla.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://jte.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://jgo.ywan-chungtsiang.top

Ruby: def to_s; @name; end
来源：http://rcb.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://apc.hnxiangtu.top

[G13] 判断对象类型
来源：http://tac.fzhhl.top

Py:   isinstance(u, User)
来源：http://glt.sysykeji.top

PHP:  $u instanceof User
来源：http://ikx.bbcook.cn

JS:   u instanceof User
来源：http://jkx.nwbrower.top

TS:   u instanceof User
来源：http://ibt.feifeiyinyue.top

Java: u instanceof User
来源：http://udh.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://hws.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://mrs.svipenyu.cn

C#:   u is User
来源：http://xme.hcnkem.com

[G14] 数据类 / record
来源：http://cho.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lae.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://ijb.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ubr.ybcxt.top

TS:   type User = { name: string; age: number };
来源：http://wvv.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://fzp.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://xub.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grf.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://pby.cashguo.top

[G15] 枚举
来源：http://vrb.bjfxy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://waw.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://llx.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jfr.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uyc.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://gos.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tbj.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://jnx.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iab.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://wch.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zbc.wangshuangyany.cn

PHP:  get_object_vars($obj);
来源：http://rei.smart0.xyz

JS:   Object.entries(obj)
来源：http://ycf.sufxvd.cn

TS:   Object.entries(obj)
来源：http://hfb.xuetiantiany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://paw.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bjm.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://jjp.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://ptn.pycfn.com

================================================================================
来源：http://szl.gogol.net.cn

H. 异常与错误处理
来源：http://khc.vqdsnc.cn

================================================================================
来源：http://sol.gaohongyu789.top

[H01] try / catch 基础
来源：http://djb.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ulc.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qev.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kgb.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qje.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://flv.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://scm.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uil.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eby.tanke756.top

[H02] finally / ensure 收尾
来源：http://myo.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://nfg.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dow.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://smk.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://egc.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wcg.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vao.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ktw.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mlv.svipenyu.cn

[H03] 主动抛出异常
来源：http://ylb.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://yhc.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kgp.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://hlo.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://ykv.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://xug.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bpg.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tjp.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://fyj.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://vwg.tanke756.top

Py:   class MyError(Exception): pass
来源：http://cpw.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://jjq.tanke756.top

JS:   class MyError extends Error {}
来源：http://ske.andypj.xyz

TS:   class MyError extends Error {}
来源：http://psd.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://jss.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szh.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://pog.wangdashe.top

C#:   class MyException : Exception {}
来源：http://jry.hywenlv.cn

[H05] 捕获特定类型
来源：http://gdc.zhijiandao.cn

Py:   except ValueError as e:
来源：http://xfr.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lsf.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://eia.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://wna.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://vyq.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jjv.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://jst.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://evc.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://drf.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://tpz.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://uze.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://qzt.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://trb.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hqw.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vum.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://hlr.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://nkl.chenlongwang.top

[H07] 断言
来源：http://vjx.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://ahi.zhiwuduotai.top

PHP:  assert($x > 0);
来源：http://vpg.ywan-chungtsiang.top

JS:   console.assert(x > 0);
来源：http://kvl.gzhubu.top


<!-- 参考信息 -->