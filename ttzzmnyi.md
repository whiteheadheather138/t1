代发 wailian999

Ruby: File.delete("a.txt")
来源：http://vbn.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://krj.pycfn.com

[F07] 创建目录（含多级）
来源：http://ceh.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ccy.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iji.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blw.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivs.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pmz.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rob.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dob.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gif.jinqigufen.top

[F08] 遍历目录
来源：http://oji.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cpw.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wfy.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://jce.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://epv.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yna.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://agd.andypj.xyz

Ruby: Dir.children("dir")
来源：http://dmg.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://beq.zhiwuduotai.top

[F09] 获取文件大小
来源：http://cyo.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://kzf.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://aas.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://swv.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://mqr.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://clb.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mdy.daxiang520.top

Ruby: File.size("a.txt")
来源：http://een.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://tpl.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://dbw.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://phx.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wij.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lyr.ehwqpu.com

TS:   path.extname("a.txt")
来源：http://xmq.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gyq.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://van.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oxn.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cyq.ybcxt.top

[F11] 复制与移动文件
来源：http://xda.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mmd.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://byd.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ugw.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://woq.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lry.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xfq.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hqj.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baz.c1oappe.top

[F12] CSV 读写
来源：http://xfq.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yqd.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kmk.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bqq.yangfankeji.com

TS:   // 同上
来源：http://clg.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pzc.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://krg.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hbe.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vtu.nanxinkj.top

================================================================================
来源：http://flk.sxryk.cn

G. 面向对象
来源：http://nvf.sweek.top

================================================================================
来源：http://srw.yfazqb.com

[G01] 定义类
来源：http://nth.haohaochexian.top

Py:   class User: pass
来源：http://sgg.feifeiyinyue.top

PHP:  class User {}
来源：http://eib.nanxinkj.top

JS:   class User {}
来源：http://pkf.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://vau.mhx1999.top

Java: class User {}
来源：http://tda.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://pgg.zdbjq.cn

Ruby: class User; end
来源：http://udr.aizwys.cn

C#:   class User {}
来源：http://jna.ppjwa.cn

[G02] 构造函数
来源：http://nog.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://jog.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://tiv.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://rro.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://dbg.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://tvb.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ukl.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://jzk.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://cim.chenzaomai.com

[G03] 实例属性
来源：http://ned.hysaishi.cn

Py:   self.name = "x"
来源：http://zii.iojbl.cn

PHP:  public string $name = "x";
来源：http://lop.ctjpmb.com

JS:   this.name = "x";
来源：http://lno.hnqzz.top

TS:   name: string = "x";
来源：http://cvl.jinghuilouyu.cn

Java: private String name;
来源：http://wsr.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vao.yuxming.cn

Ruby: @name = "x"
来源：http://jsa.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://uix.ywan-chungtsiang.top

[G04] 定义方法
来源：http://qsn.hnqzz.top

Py:   def greet(self): return self.name
来源：http://wfv.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wwq.cheryme.top

JS:   greet() { return this.name; }
来源：http://gqb.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://afy.aibaodan.cn

Java: String greet() { return name; }
来源：http://kgc.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wrb.ppjwa.cn

Ruby: def greet; @name; end
来源：http://jwm.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://fol.ywan-chungtsiang.top

[G05] 继承
来源：http://ytg.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://tfd.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://kft.chenzaomai.com

JS:   class Admin extends User {}
来源：http://llh.pycfn.com

TS:   class Admin extends User {}
来源：http://saf.daria6918.cn

Java: class Admin extends User {}
来源：http://gms.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nqx.52xcode.cn

Ruby: class Admin < User; end
来源：http://nsm.cqqwz.cn

C#:   class Admin : User {}
来源：http://peq.zycfv.cn

[G06] 重写方法
来源：http://kzx.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://eon.yj20258.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wft.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://axr.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://bps.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://ecw.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cox.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://iqu.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://iuw.dashuyun.cn

[G07] 调用父类方法
来源：http://fup.fehbvm.com

Py:   super().greet()
来源：http://izb.jinqigfzy.top

PHP:  parent::greet();
来源：http://zuv.ppjwa.cn

JS:   super.greet();
来源：http://njf.chenlongwang.top

TS:   super.greet();
来源：http://sme.chenlongwang.top

Java: super.greet();
来源：http://uze.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yim.daria6918.cn

Ruby: super
来源：http://dul.hongshengwenyu.top

C#:   base.Greet();
来源：http://snf.hysaishi.cn

[G08] 静态方法与属性
来源：http://prf.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gkx.yongpay.top

PHP:  public static function f() {}
来源：http://hgx.jqgufenzy.top

JS:   static f() {}
来源：http://sdm.tianlin.xyz

TS:   static f(): void {}
来源：http://wkd.yueranfly.top

Java: static void f() {}
来源：http://hhb.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mjn.yueranfly.top

Ruby: def self.f; end
来源：http://slb.jinqigfzy.top

C#:   public static void F() {}
来源：http://cbo.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://zal.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://wgw.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://rse.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cck.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://svo.uphjek.com

Java: interface Shape { double area(); }
来源：http://avf.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fcl.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://byp.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://mus.quarkkingdee.top

[G10] 访问控制
来源：http://kyz.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://mnm.chenlongwang.top

PHP:  public / protected / private
来源：http://png.cucudq.cn

JS:   #private 字段；其余公开
来源：http://gwr.iojbl.cn

TS:   public / protected / private
来源：http://xkl.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://jii.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bye.havefunace.top

Ruby: public / protected / private
来源：http://ekl.uphjek.com

C#:   public / protected / private / internal
来源：http://nrl.smart0.xyz

[G11] getter / setter
来源：http://dhz.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://bfz.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://roa.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://hei.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://dkz.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://zzu.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewc.epnwcf.com

Ruby: attr_accessor :name
来源：http://ybz.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://dxl.yongpay.top

[G12] 对象转字符串
来源：http://oqk.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://zdr.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://usv.cucudq.cn

JS:   toString() { return this.name; }
来源：http://gbx.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://zbo.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://xlq.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://umf.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://ebi.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://ith.guowangkeji.top

[G13] 判断对象类型
来源：http://rgh.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://lij.yanxiufei.cn

PHP:  $u instanceof User
来源：http://lcc.quarkkingdee.top

JS:   u instanceof User
来源：http://bym.chenzaomai.com

TS:   u instanceof User
来源：http://ofs.shangyingyoupin.top

Java: u instanceof User
来源：http://ewv.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://edw.yueranfly.top

Ruby: u.is_a?(User)
来源：http://jre.sufxvd.cn

C#:   u is User
来源：http://gxl.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://gde.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dlg.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://axc.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://rhs.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://xxv.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://gri.fktsv.cn

Go:   type User struct { Name string; Age int }
来源：http://ebp.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xck.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://xzf.meibo888.top

[G15] 枚举
来源：http://mjo.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pyb.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kvr.sysykeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nvd.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lbp.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://jlj.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uiv.uphjek.com

Ruby: Color = %i[red green].freeze
来源：http://pck.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xll.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://hto.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://twk.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://sys.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://kdg.chenlongwang.top

TS:   Object.entries(obj)
来源：http://bfc.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fpg.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ohc.zhengqikj.top

Ruby: obj.instance_variables
来源：http://ndv.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://pwq.meibo888.top

================================================================================
来源：http://dge.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://wiz.gzhubu.top

================================================================================
来源：http://zyf.yj20258.top

[H01] try / catch 基础
来源：http://sta.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xcg.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yql.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nsy.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfa.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nbz.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://obx.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rby.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sch.fzhhl.top

[H02] finally / ensure 收尾
来源：http://vtf.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://umy.zhaomingkeji.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cle.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://btg.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jta.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://big.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://url.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sfw.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sbu.wangdashe.top

[H03] 主动抛出异常
来源：http://swn.cheryme.top

Py:   raise ValueError("错误信息")
来源：http://emy.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://svx.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://tkk.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://sop.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pry.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mhz.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://trv.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ifq.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://vvd.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://khh.yangfankeji.com

PHP:  class MyError extends RuntimeException {}
来源：http://pog.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://mvc.jyoumei.cn

TS:   class MyError extends Error {}
来源：http://aec.aibaodan.cn

Java: class MyException extends RuntimeException {}
来源：http://grj.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tgt.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://tqg.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://mbe.kuanghao11.cn

[H05] 捕获特定类型
来源：http://vgh.aibaodan.cn

Py:   except ValueError as e:
来源：http://wps.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rxn.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://xux.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://cyd.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://dmo.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wlr.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://oxn.feifeiyinyue.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nty.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://dne.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://amd.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://fhh.sjlbkw.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mug.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://pto.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pmr.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zkr.guannengcc.top

Ruby: d&.dig(:a, :b)
来源：http://pib.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://xlb.0kj1m.cn

[H07] 断言
来源：http://qun.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://zvn.gotoacloud.top

PHP:  assert($x > 0);
来源：http://pcm.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://wga.xinyue.icu

TS:   console.assert(x > 0);
来源：http://vdo.vqdsnc.cn

Java: assert x > 0 : "必须为正";
来源：http://lng.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xqy.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://ros.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://jno.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://hwk.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://vlx.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cjc.svipenyu.cn

JS:   e.message;  e.stack
来源：http://lsj.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qyd.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://plw.zycfv.cn

Go:   err.Error()
来源：http://bzu.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://bvf.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://jzl.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://xtf.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cqh.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjk.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrx.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wto.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kqo.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ald.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hqg.zhoulong.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://mux.daxiang520.top

[H10] 资源自动释放
来源：http://vnb.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://vhj.jqgufenzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://twp.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zvk.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://grs.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bqm.xinyue.icu

Go:   defer f.Close()
来源：http://llo.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yap.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lzj.haohaochexian.top

================================================================================
来源：http://zed.jqgufenzy.top

I. 正则表达式
来源：http://isc.yanxiufei.cn

================================================================================
来源：http://ojo.ehwqpu.com

[I01] 判断是否匹配
来源：http://yzs.jinghuilouyu.cn


<!-- 参考信息 -->