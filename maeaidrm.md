代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://psh.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gtd.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ehr.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://jft.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://iim.iojbl.cn

[F06] 删除文件
来源：http://oum.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://nwa.birdmap.top

PHP:  unlink("a.txt");
来源：http://ylt.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://hgl.xuanzx.com

TS:   fs.unlinkSync("a.txt")
来源：http://pwh.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fwo.cqqwz.cn

Go:   os.Remove("a.txt")
来源：http://qdx.yueranfly.top

Ruby: File.delete("a.txt")
来源：http://pds.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://lug.pycfn.com

[F07] 创建目录（含多级）
来源：http://jjx.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vjz.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vof.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkk.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owf.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sms.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jvh.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dso.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ebm.yangfankeji.com

[F08] 遍历目录
来源：http://ndp.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ont.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://irs.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://cfw.ivvv.top

TS:   fs.readdirSync("dir")
来源：http://utt.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uza.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zsc.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://get.fzhhl.top

C#:   Directory.GetFiles("dir")
来源：http://lgq.daria6918.cn

[F09] 获取文件大小
来源：http://aft.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://hqk.ydzc1.top

PHP:  filesize("a.txt");
来源：http://dav.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://bhu.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://trq.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://roa.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vbw.yonumen.top

Ruby: File.size("a.txt")
来源：http://hng.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://rmf.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://gud.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aih.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qkq.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pxx.jianghu66.top

TS:   path.extname("a.txt")
来源：http://sif.gaohongyu789.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iii.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhf.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zag.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ykf.52xcode.cn

[F11] 复制与移动文件
来源：http://sju.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iwq.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aqt.jqgufenzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wxy.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhv.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tfa.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://otb.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dod.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lmi.yangfankeji.com

[F12] CSV 读写
来源：http://qsn.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uyy.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fyl.yj20258.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dpx.shuidangran.top

TS:   // 同上
来源：http://kqt.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qey.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pju.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tgw.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xza.nanxinkj.top

================================================================================
来源：http://yxk.52xcode.cn

G. 面向对象
来源：http://czv.52xcode.cn

================================================================================
来源：http://trz.xinyue.icu

[G01] 定义类
来源：http://bpx.cdnleiting.top

Py:   class User: pass
来源：http://bxx.hesvh.cn

PHP:  class User {}
来源：http://pst.sjlbkw.cn

JS:   class User {}
来源：http://gla.wangdashe.top

TS:   class User { name: string = ""; }
来源：http://xvw.gaohongyu789.top

Java: class User {}
来源：http://tyc.andypj.xyz

Go:   type User struct { Name string }
来源：http://bia.chenjidiqi.icu

Ruby: class User; end
来源：http://jhc.cucudq.cn

C#:   class User {}
来源：http://bzu.9152youxi.cn

[G02] 构造函数
来源：http://vrg.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://owt.ybcxt.top

PHP:  public function __construct(public string $name) {}
来源：http://yxl.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://rtt.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://gar.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://eff.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://frb.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://oai.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://juc.zhaomingkeji.xyz

[G03] 实例属性
来源：http://khr.pengpengdd.cyou

Py:   self.name = "x"
来源：http://mlg.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://gif.jqgufenzy.top

JS:   this.name = "x";
来源：http://asy.sxryk.cn

TS:   name: string = "x";
来源：http://pvr.jiagoushi.top

Java: private String name;
来源：http://hxs.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jej.quarkkingdee.top

Ruby: @name = "x"
来源：http://ivq.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://mzm.xziqi.cn

[G04] 定义方法
来源：http://ged.feifeiyinyue.top

Py:   def greet(self): return self.name
来源：http://qtm.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gov.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://dtz.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://pmy.gaohongyu789.top

Java: String greet() { return name; }
来源：http://kia.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xml.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://taf.ivvv.top

C#:   public string Greet() => Name;
来源：http://ydj.jianghu66.top

[G05] 继承
来源：http://dmi.hcnkem.com

Py:   class Admin(User): pass
来源：http://thj.fktsv.cn

PHP:  class Admin extends User {}
来源：http://mcl.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://vdm.pycfn.com

TS:   class Admin extends User {}
来源：http://ggk.yonumen.top

Java: class Admin extends User {}
来源：http://xhd.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rbm.yj202588.top

Ruby: class Admin < User; end
来源：http://rpr.c1oappe.top

C#:   class Admin : User {}
来源：http://acu.havefunace.top

[G06] 重写方法
来源：http://gns.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://qsz.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://dct.ivvv.top

JS:   greet() { return "admin"; }
来源：http://bop.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://hui.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://hko.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://naa.ivvv.top

Ruby: def greet; "admin"; end
来源：http://zxg.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://pex.chenzaomai.com

[G07] 调用父类方法
来源：http://dhz.gaohongyu789.top

Py:   super().greet()
来源：http://qhj.jlsjyb.cn

PHP:  parent::greet();
来源：http://dvy.nwbrower.top

JS:   super.greet();
来源：http://xje.sysykeji.top

TS:   super.greet();
来源：http://jmf.xinyue.icu

Java: super.greet();
来源：http://ctz.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://imx.cqqwz.cn

Ruby: super
来源：http://sll.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://zxf.ehwqpu.com

[G08] 静态方法与属性
来源：http://ckg.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bmp.zhoulong.xyz

PHP:  public static function f() {}
来源：http://ozs.redwolf501.top

JS:   static f() {}
来源：http://chd.hnxiangtu.top

TS:   static f(): void {}
来源：http://kcs.daxiang520.top

Java: static void f() {}
来源：http://zgo.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sko.quarkkingdee.top

Ruby: def self.f; end
来源：http://afg.smart0.xyz

C#:   public static void F() {}
来源：http://les.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://rtg.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://xfi.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://exx.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tjm.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://mwk.jianghu66.top

Java: interface Shape { double area(); }
来源：http://ekp.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://hfu.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://utm.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://pkv.vehdjk.com

[G10] 访问控制
来源：http://oai.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://owp.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://ifz.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://hsv.tarul.cn

TS:   public / protected / private
来源：http://oht.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://dce.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eeg.bbcook.cn

Ruby: public / protected / private
来源：http://oig.yonumen.top

C#:   public / protected / private / internal
来源：http://abx.sysykeji.top

[G11] getter / setter
来源：http://aub.ydzc1.top

Py:   @property 与 @x.setter
来源：http://ual.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://keo.iojbl.cn

JS:   get name() { return this._name; }
来源：http://msk.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://pwq.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://uyp.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://udb.fzhhl.top

Ruby: attr_accessor :name
来源：http://udw.tian-w.cn

C#:   public string Name { get; set; }
来源：http://gqo.smart0.xyz

[G12] 对象转字符串
来源：http://hbm.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://ypr.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hww.sweek.top

JS:   toString() { return this.name; }
来源：http://fvx.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://lcd.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://nnx.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://xua.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://jox.cheryme.top

C#:   public override string ToString() => Name;
来源：http://sau.gzhubu.top

[G13] 判断对象类型
来源：http://ffo.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://xpb.0kj1m.cn

PHP:  $u instanceof User
来源：http://ucl.meibo888.top

JS:   u instanceof User
来源：http://fvg.nanxuanxn.top

TS:   u instanceof User
来源：http://ope.zhongyouzk.top

Java: u instanceof User
来源：http://goj.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cym.meibo888.top

Ruby: u.is_a?(User)
来源：http://nch.quarkkingdee.top

C#:   u is User
来源：http://axz.zycfv.cn

[G14] 数据类 / record
来源：http://qnd.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qyb.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://pjx.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://hgu.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://cbu.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://gfy.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://rwu.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zof.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://lwi.wangdashe.top

[G15] 枚举
来源：http://jlr.zhiwuduotai.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yyu.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kin.snrcjt.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aol.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iug.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://djy.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://grj.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://dag.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fao.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://dnk.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dvo.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://bql.jianghu66.top

JS:   Object.entries(obj)
来源：http://mvt.zdqjudy.top

TS:   Object.entries(obj)
来源：http://kbf.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ias.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://grg.ydzc1.top

Ruby: obj.instance_variables
来源：http://ihv.jinghuilouyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://iqb.pengpengdd.cyou

================================================================================
来源：http://ahz.hysaishi.cn

H. 异常与错误处理
来源：http://euy.hywenlv.cn

================================================================================
来源：http://bzz.wangdashe.top

[H01] try / catch 基础
来源：http://ulj.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jga.hywenlv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ghr.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://grl.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ebi.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eot.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vzl.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rls.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vyt.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://ozk.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uut.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ylf.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://akc.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fua.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://usx.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://bbg.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://yuk.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cxx.xinyue.icu

[H03] 主动抛出异常
来源：http://hxd.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://nys.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ldz.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://ldh.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://uwu.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://tpt.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rev.zhixingplan.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fzj.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://uac.yvedp.cn

[H04] 自定义异常类型
来源：http://eig.ivvv.top

Py:   class MyError(Exception): pass
来源：http://mxs.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://mqm.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://eio.hammf.cn

TS:   class MyError extends Error {}
来源：http://rig.tianlin.xyz

Java: class MyException extends RuntimeException {}
来源：http://xxa.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tgx.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://bad.hnqzz.top

C#:   class MyException : Exception {}
来源：http://hch.quarkkingdee.top

[H05] 捕获特定类型
来源：http://xru.hfpthk.cn

Py:   except ValueError as e:
来源：http://mrx.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qcv.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://goa.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://svq.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qai.ehwqpu.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ddc.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://rvg.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://phg.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://wjr.sxryk.cn

Py:   value = d.get("k") or default
来源：http://daw.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ecl.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://btp.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://ixw.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rki.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pjh.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://hhe.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://wxl.xinyue.icu

[H07] 断言
来源：http://avd.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://pmb.zdbjq.cn

PHP:  assert($x > 0);
来源：http://nip.hnqzz.top

JS:   console.assert(x > 0);
来源：http://ios.yangfankeji.com

TS:   console.assert(x > 0);
来源：http://dyt.ydjk.org.cn

Java: assert x > 0 : "必须为正";
来源：http://rey.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iti.haohaochexian.top

Ruby: raise "必须为正" unless x > 0
来源：http://xey.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://nfl.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://hoc.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://slk.hnqzz.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wkf.ybcxt.top

JS:   e.message;  e.stack
来源：http://vdx.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ere.gogol.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mcr.xylfe.cn

Go:   err.Error()
来源：http://gse.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://xfl.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://epa.zhijiandao.cn

[H09] 带错误码的异常
来源：http://prm.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fkf.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xkp.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kbj.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ovz.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aom.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sjg.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://adz.fktsv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qjw.havefunace.top

[H10] 资源自动释放
来源：http://tym.feifeiyinyue.top


<!-- 参考信息 -->