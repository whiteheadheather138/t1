代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eqs.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nlx.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjo.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qks.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://nck.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pud.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://zpg.xingfuxueyuan.xyz

JS:   fs.existsSync("a.txt")
来源：http://xjn.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://tds.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://bwt.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tqo.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://hcc.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://phc.vqdsnc.cn

[F06] 删除文件
来源：http://mut.shuidangran.top

Py:   os.remove("a.txt")
来源：http://aru.hammf.cn

PHP:  unlink("a.txt");
来源：http://ybe.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://rld.xingfuxueyuan.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://sqj.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://usq.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://bin.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://kqj.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://zbz.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://qvo.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jcm.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vdj.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mnk.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://odb.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nse.meibo888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ntz.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://few.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lur.jinqigfzy.top

[F08] 遍历目录
来源：http://amj.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iei.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cqi.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://ibb.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://ubj.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://moe.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kzr.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://rpc.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://wey.hywenlv.cn

[F09] 获取文件大小
来源：http://qxc.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://dpz.fehbvm.com

PHP:  filesize("a.txt");
来源：http://czl.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://ice.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://bjy.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://zsa.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ukz.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://lqq.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://vfr.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://nxu.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zxt.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rva.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dee.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://iqv.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aek.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yup.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bke.gaohongyu789.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vig.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://vwj.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zqn.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jfh.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zyh.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szn.ywan-chungtsiang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wjn.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xyt.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wtm.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qdb.guowangkeji.top

[F12] CSV 读写
来源：http://nox.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nne.gogol.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pxy.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tje.yongpay.top

TS:   // 同上
来源：http://ezz.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xag.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hos.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gyn.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qqn.ivvv.top

================================================================================
来源：http://cbo.jyoumei.cn

G. 面向对象
来源：http://abz.nanxuanxn.top

================================================================================
来源：http://jlr.quarkkingdee.top

[G01] 定义类
来源：http://oce.cdnleiting.top

Py:   class User: pass
来源：http://hsh.xinyue.icu

PHP:  class User {}
来源：http://dxh.yonumen.top

JS:   class User {}
来源：http://uif.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://xxi.gotoacloud.top

Java: class User {}
来源：http://nec.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://cjq.hammf.cn

Ruby: class User; end
来源：http://cry.guannengcc.top

C#:   class User {}
来源：http://sde.hywenlv.cn

[G02] 构造函数
来源：http://okg.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://tdv.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://jcc.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://agz.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://fcr.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://dgx.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vso.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://qpe.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://ysc.sxryk.cn

[G03] 实例属性
来源：http://itj.jinqigfzy.top

Py:   self.name = "x"
来源：http://zhu.hfpthk.cn

PHP:  public string $name = "x";
来源：http://yey.52xcode.cn

JS:   this.name = "x";
来源：http://lny.daria6918.cn

TS:   name: string = "x";
来源：http://dzk.ydzc1.top

Java: private String name;
来源：http://uzf.nanxuanxn.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xdl.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://yav.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://bzp.cdnleiting.top

[G04] 定义方法
来源：http://hzy.vehdjk.com

Py:   def greet(self): return self.name
来源：http://bjc.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ngy.sxryk.cn

JS:   greet() { return this.name; }
来源：http://nmk.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://khg.yuxming.cn

Java: String greet() { return name; }
来源：http://ehs.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ndx.meibo888.top

Ruby: def greet; @name; end
来源：http://lkd.wangdashe.top

C#:   public string Greet() => Name;
来源：http://djy.daria6918.cn

[G05] 继承
来源：http://doi.316326.xyz

Py:   class Admin(User): pass
来源：http://gsc.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://iok.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://dxn.zdbjq.cn

TS:   class Admin extends User {}
来源：http://dmg.fzhhl.top

Java: class Admin extends User {}
来源：http://mof.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tzl.iojbl.cn

Ruby: class Admin < User; end
来源：http://lhf.nanxuanxn.top

C#:   class Admin : User {}
来源：http://uvr.haohaochexian.top

[G06] 重写方法
来源：http://lrp.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://xvn.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uka.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://yyc.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://yxt.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://frt.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ckr.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://ekz.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://ror.zhoulong.xyz

[G07] 调用父类方法
来源：http://dlz.guannengcc.top

Py:   super().greet()
来源：http://vli.epnwcf.com

PHP:  parent::greet();
来源：http://cek.fanxiaobao.xyz

JS:   super.greet();
来源：http://xcd.jianghu66.top

TS:   super.greet();
来源：http://cip.yangfankeji.com

Java: super.greet();
来源：http://awd.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wnw.mhx1999.top

Ruby: super
来源：http://whq.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://rxt.hammf.cn

[G08] 静态方法与属性
来源：http://wra.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wuu.meibo888.top

PHP:  public static function f() {}
来源：http://wts.quarkkingdee.top

JS:   static f() {}
来源：http://brr.zhiwuduotai.top

TS:   static f(): void {}
来源：http://vms.cheryme.top

Java: static void f() {}
来源：http://iub.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eie.chenjidiqi.icu

Ruby: def self.f; end
来源：http://gko.uphjek.com

C#:   public static void F() {}
来源：http://vvb.epnwcf.com

[G09] 接口 / 抽象类
来源：http://dwp.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://zsc.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://hlx.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://ipc.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://xqs.fzhhl.top

Java: interface Shape { double area(); }
来源：http://oyr.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://ghr.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jhp.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://yja.hywenlv.cn

[G10] 访问控制
来源：http://vgu.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://gur.gzhubu.top

PHP:  public / protected / private
来源：http://ykm.birdmap.top

JS:   #private 字段；其余公开
来源：http://jmj.havefunace.top

TS:   public / protected / private
来源：http://xbc.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://iov.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://gbt.pycfn.com

Ruby: public / protected / private
来源：http://tna.sysykeji.top

C#:   public / protected / private / internal
来源：http://fct.hcnkem.com

[G11] getter / setter
来源：http://arx.mhx1999.top

Py:   @property 与 @x.setter
来源：http://ias.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dba.zycfv.cn

JS:   get name() { return this._name; }
来源：http://nwd.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://see.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://sze.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vbh.dashuyun.cn

Ruby: attr_accessor :name
来源：http://juy.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://xzs.zhongyouzk.top

[G12] 对象转字符串
来源：http://uvw.uphjek.com

Py:   def __str__(self): return self.name
来源：http://uyy.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jhm.fehbvm.com

JS:   toString() { return this.name; }
来源：http://umi.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://rfx.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://vxh.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://aoy.hammf.cn

Ruby: def to_s; @name; end
来源：http://pzq.cucudq.cn

C#:   public override string ToString() => Name;
来源：http://tmh.epnwcf.com

[G13] 判断对象类型
来源：http://vfw.yueranfly.top

Py:   isinstance(u, User)
来源：http://pmz.vqdsnc.cn

PHP:  $u instanceof User
来源：http://soy.haohaochexian.top

JS:   u instanceof User
来源：http://uop.cheryme.top

TS:   u instanceof User
来源：http://anp.hongshengwenyu.top

Java: u instanceof User
来源：http://crl.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://sbm.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://nwk.zhijiandao.cn

C#:   u is User
来源：http://mdd.tanke756.top

[G14] 数据类 / record
来源：http://nhw.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ixu.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://ovj.gaohongyu789.top

JS:   // 无内置：普通类或对象字面量
来源：http://vtp.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://rzy.meibo888.top

Java: record User(String name, int age) {}
来源：http://njl.xinyue.icu

Go:   type User struct { Name string; Age int }
来源：http://kge.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://joe.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://gyd.ydzc1.top

[G15] 枚举
来源：http://gdf.cdnleiting.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ici.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jlt.gzhubu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mst.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xnz.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://upo.tanke756.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jki.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://vrl.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yxc.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://mso.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ycg.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://sdd.hesvh.cn

JS:   Object.entries(obj)
来源：http://ous.iojbl.cn

TS:   Object.entries(obj)
来源：http://rmb.0kj1m.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xub.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://awa.52xcode.cn

Ruby: obj.instance_variables
来源：http://omi.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://oby.jinqigfzy.top

================================================================================
来源：http://iud.tianlin.xyz

H. 异常与错误处理
来源：http://feu.0kj1m.cn

================================================================================
来源：http://yqj.52xcode.cn

[H01] try / catch 基础
来源：http://rvd.ydzc1.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wft.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dao.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://owl.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pja.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hhx.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://liu.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://crs.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pke.daxiang520.top

[H02] finally / ensure 收尾
来源：http://bgu.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://pxr.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mzj.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qru.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dfc.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mmd.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://krz.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pfw.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tlm.smart0.xyz

[H03] 主动抛出异常
来源：http://wck.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://awu.yfazqb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://drj.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://fqb.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://ort.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gek.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uag.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tlc.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://pqp.yfazqb.com

[H04] 自定义异常类型
来源：http://srp.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://did.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cpw.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://tvy.sweek.top

TS:   class MyError extends Error {}
来源：http://lts.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://bqt.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ijd.vqdsnc.cn

Ruby: class MyError < StandardError; end
来源：http://hrd.sjlbkw.cn

C#:   class MyException : Exception {}
来源：http://xiz.ydjk.org.cn

[H05] 捕获特定类型
来源：http://eah.chenlongwang.top

Py:   except ValueError as e:
来源：http://lzq.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kun.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://xcm.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://qct.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://cvq.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hbw.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://epf.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bcx.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://nqt.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://zoz.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://tzi.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://qkf.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://cdu.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hab.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://teh.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://hhl.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://dcp.fanxiaobao.xyz

[H07] 断言
来源：http://ini.wangshuangyany.cn

Py:   assert x > 0, "必须为正"
来源：http://ktq.cdnleiting.top

PHP:  assert($x > 0);
来源：http://kew.ydzc1.top

JS:   console.assert(x > 0);
来源：http://laa.pycfn.com

TS:   console.assert(x > 0);
来源：http://zgj.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://bjm.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kep.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://vit.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://tlz.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://oyn.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://tcd.ehwqpu.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ogf.iojbl.cn

JS:   e.message;  e.stack
来源：http://gkq.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nov.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://loe.ydjk.org.cn

Go:   err.Error()
来源：http://efm.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://yck.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://sqg.zdqjudy.top

[H09] 带错误码的异常
来源：http://xkz.shanyushiyangtech.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lcu.sysykeji.top


<!-- 参考信息 -->