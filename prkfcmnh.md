代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xdv.svipenyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eud.zhiwuduotai.top

[F03] 写入文件（覆盖）
来源：http://xif.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tiw.zdqjudy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qsg.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfp.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bru.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zjh.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nbd.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://slt.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dnb.xinyue.icu

[F04] 追加写入文件
来源：http://bre.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hye.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pvl.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gwi.hywenlv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vvc.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mbv.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://geh.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rqe.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jfr.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://zqo.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xuo.316326.xyz

PHP:  file_exists("a.txt");
来源：http://lrq.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://pnz.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://rcd.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://vyq.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yof.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://cxq.dianchejie.cn

C#:   File.Exists("a.txt")
来源：http://irv.zhengqikj.top

[F06] 删除文件
来源：http://inh.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://cvo.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://wht.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tuh.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://knj.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bnp.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://oit.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://hpz.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://qqo.yongpay.top

[F07] 创建目录（含多级）
来源：http://zti.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hgn.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mgz.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rcq.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qff.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zjr.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ebc.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qbe.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qlz.xylfe.cn

[F08] 遍历目录
来源：http://kea.aibaodan.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lcx.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xdy.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://weq.hesvh.cn

TS:   fs.readdirSync("dir")
来源：http://ojk.xuanzx.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hdf.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nej.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://nrw.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://rcn.yuanzhike.top

[F09] 获取文件大小
来源：http://tmi.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://vei.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://tpk.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://fxc.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://mlh.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://auw.chenzaomai.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dyd.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://yxu.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://ljf.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://cxf.redwolf501.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pke.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zdd.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kft.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://bfz.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxc.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jkc.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pps.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pgc.gaohongyu789.top

[F11] 复制与移动文件
来源：http://uda.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xju.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rbx.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgw.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sfu.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sde.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://icg.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rgr.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ova.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://uod.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://llc.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iwl.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ueh.ivvv.top

TS:   // 同上
来源：http://wxb.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ioq.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ayh.yuxming.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://prc.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pze.smart0.xyz

================================================================================
来源：http://sza.shanyushiyangkeji.top

G. 面向对象
来源：http://keu.chenlongwang.top

================================================================================
来源：http://xpp.jqgufenzy.top

[G01] 定义类
来源：http://yxt.epnwcf.com

Py:   class User: pass
来源：http://wnp.sxryk.cn

PHP:  class User {}
来源：http://rzk.daxiang520.top

JS:   class User {}
来源：http://wdn.birdmap.top

TS:   class User { name: string = ""; }
来源：http://ogq.iojbl.cn

Java: class User {}
来源：http://pam.fengsongda.top

Go:   type User struct { Name string }
来源：http://cnq.fanxiaobao.xyz

Ruby: class User; end
来源：http://tsk.havefunace.top

C#:   class User {}
来源：http://pyb.bbcook.cn

[G02] 构造函数
来源：http://owr.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://aly.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://ppa.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://qiz.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://lwx.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://qvx.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uuc.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://tdc.smart0.xyz

C#:   public User(string name) { Name = name; }
来源：http://czn.shanyushiyangkeji.top

[G03] 实例属性
来源：http://vzm.wangdashe.top

Py:   self.name = "x"
来源：http://cpt.bjfxy.top

PHP:  public string $name = "x";
来源：http://kth.zhijiandao.cn

JS:   this.name = "x";
来源：http://wds.ydjk.org.cn

TS:   name: string = "x";
来源：http://tbo.vqdsnc.cn

Java: private String name;
来源：http://qjy.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oey.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://ncl.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://dwo.sysykeji.top

[G04] 定义方法
来源：http://gex.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://dtr.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ieb.hnqzz.top

JS:   greet() { return this.name; }
来源：http://uxs.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://rcr.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://kvd.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ybf.hfpthk.cn

Ruby: def greet; @name; end
来源：http://cuh.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://shs.sxryk.cn

[G05] 继承
来源：http://lqs.andypj.xyz

Py:   class Admin(User): pass
来源：http://ghl.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://krs.jyoumei.cn

JS:   class Admin extends User {}
来源：http://pmt.epnwcf.com

TS:   class Admin extends User {}
来源：http://xzp.hnqzz.top

Java: class Admin extends User {}
来源：http://bch.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jom.xuanzx.com

Ruby: class Admin < User; end
来源：http://wxk.redwolf501.top

C#:   class Admin : User {}
来源：http://pth.tarul.cn

[G06] 重写方法
来源：http://eyh.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://fht.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://djw.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://pdg.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://lrg.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://nle.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wof.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://buw.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://kpo.gotoacloud.top

[G07] 调用父类方法
来源：http://gdf.shangyingyoupin.top

Py:   super().greet()
来源：http://fgz.xziqi.cn

PHP:  parent::greet();
来源：http://jsi.hongshengwenyu.top

JS:   super.greet();
来源：http://ldd.kuanghao11.cn

TS:   super.greet();
来源：http://uym.ydzc1.top

Java: super.greet();
来源：http://thh.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gxi.meibo888.top

Ruby: super
来源：http://hth.zhiwuduotai.top

C#:   base.Greet();
来源：http://abg.tarul.cn

[G08] 静态方法与属性
来源：http://qta.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cpm.gaohongyu789.top

PHP:  public static function f() {}
来源：http://fta.gaohongyu789.top

JS:   static f() {}
来源：http://eso.jlsjyb.cn

TS:   static f(): void {}
来源：http://iaq.zdbjq.cn

Java: static void f() {}
来源：http://eyx.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://udj.feifeiyinyue.top

Ruby: def self.f; end
来源：http://yaj.52xcode.cn

C#:   public static void F() {}
来源：http://svh.ppjwa.cn

[G09] 接口 / 抽象类
来源：http://wgj.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://squ.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://rqr.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://rgb.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://rpm.cucudq.cn

Java: interface Shape { double area(); }
来源：http://kbw.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://bnc.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdt.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://nbw.hywenlv.cn

[G10] 访问控制
来源：http://mtq.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://ffy.feifeiyinyue.top

PHP:  public / protected / private
来源：http://bod.ybcxt.top

JS:   #private 字段；其余公开
来源：http://gqa.fanxiaobao.xyz

TS:   public / protected / private
来源：http://vuz.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://rqs.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ooq.hcnkem.com

Ruby: public / protected / private
来源：http://vck.zdbjq.cn

C#:   public / protected / private / internal
来源：http://hni.zhixingplan.top

[G11] getter / setter
来源：http://qzn.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://cdb.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xpe.ivvv.top

JS:   get name() { return this._name; }
来源：http://xbc.sweek.top

TS:   get name(): string { return this._name; }
来源：http://yim.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://vcs.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rzi.shzxlz.cn

Ruby: attr_accessor :name
来源：http://owx.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://diy.sweek.top

[G12] 对象转字符串
来源：http://jun.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://bma.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lcg.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://nyy.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://crl.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://zpf.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ydp.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://zwy.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://zqr.yj20258888.top

[G13] 判断对象类型
来源：http://qbw.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://lno.tanke756.top

PHP:  $u instanceof User
来源：http://kvf.uphjek.com

JS:   u instanceof User
来源：http://qvq.jinqigufen.top

TS:   u instanceof User
来源：http://xrj.shzxlz.cn

Java: u instanceof User
来源：http://wpy.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://iqi.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://ijp.cucudq.cn

C#:   u is User
来源：http://lup.yonumen.top

[G14] 数据类 / record
来源：http://qvr.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://txb.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://vgv.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://fhe.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://syb.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://htl.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://rrw.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bke.tanke756.top

C#:   record User(string Name, int Age);
来源：http://ydm.chenjidiqi.icu

[G15] 枚举
来源：http://zqy.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vqc.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://smc.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dmc.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://okj.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://szr.guannengcc.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://clt.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://ncd.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uhj.pycfn.com

[G16] 对象转数组 / 字典
来源：http://tip.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dxd.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://rva.bbcook.cn

JS:   Object.entries(obj)
来源：http://ndm.hesvh.cn

TS:   Object.entries(obj)
来源：http://ntj.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gkf.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fay.hammf.cn

Ruby: obj.instance_variables
来源：http://dno.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://xbo.nanxuanxn.top

================================================================================
来源：http://dip.xinyue.icu

H. 异常与错误处理
来源：http://cgl.fengsongda.top

================================================================================
来源：http://awq.zdqjudy.top

[H01] try / catch 基础
来源：http://cwo.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nsb.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gqe.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xxn.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://noj.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://joq.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://krf.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kpk.sweek.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ejx.52xcode.cn

[H02] finally / ensure 收尾
来源：http://rjj.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://iwl.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vqr.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ohz.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cce.yongpay.top

Java: try { f(); } finally { cleanup(); }
来源：http://oti.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rqf.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ivv.yongpay.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sar.xziqi.cn

[H03] 主动抛出异常
来源：http://szo.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://djx.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hns.316326.xyz

JS:   throw new Error("错误信息");
来源：http://zty.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://kam.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hrg.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qmu.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://uat.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://zrw.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://wan.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://avp.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://qgf.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://gab.meibo888.top

TS:   class MyError extends Error {}
来源：http://gyy.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://pyf.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bvs.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://xjl.pengpengdd.cyou

C#:   class MyException : Exception {}
来源：http://fgi.sjlbkw.cn

[H05] 捕获特定类型
来源：http://oap.cashguo.top

Py:   except ValueError as e:
来源：http://mdy.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tjb.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://xnf.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://dpc.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://uyr.xziqi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eaa.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://hqv.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ghq.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://ydi.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://ggq.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pqm.meibo888.top

JS:   obj?.a?.b;  d ?? default
来源：http://zrd.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://deg.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://clo.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://imt.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://pxf.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://qmt.yj202588.top

[H07] 断言
来源：http://evu.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://vtl.meibo888.top

PHP:  assert($x > 0);
来源：http://pgz.yongpay.top

JS:   console.assert(x > 0);
来源：http://omz.fanxiaobao.xyz


<!-- 参考信息 -->