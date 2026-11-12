代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uqi.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://skq.wangshuangyany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ulm.hysaishi.cn

[F08] 遍历目录
来源：http://qal.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tpp.cdnleiting.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oiz.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://sov.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://sgm.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xps.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://aww.tarul.cn

Ruby: Dir.children("dir")
来源：http://ftz.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://cnw.zhengqikj.top

[F09] 获取文件大小
来源：http://ihv.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://ucc.fengsongda.top

PHP:  filesize("a.txt");
来源：http://lml.yueranfly.top

JS:   fs.statSync("a.txt").size
来源：http://ags.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://uwv.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dtk.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hpz.ivvv.top

Ruby: File.size("a.txt")
来源：http://kzc.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://snf.9152youxi.cn

[F10] 取文件扩展名 / 文件名
来源：http://rfa.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tgx.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rkp.hesvh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://svj.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://eta.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aab.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cag.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oxb.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://anj.snrcjt.cn

[F11] 复制与移动文件
来源：http://hwo.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ygq.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mbh.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qkt.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gti.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kee.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://apd.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://asz.cheryme.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nqj.quarkkingdee.top

[F12] CSV 读写
来源：http://dqd.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tni.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asr.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://opc.cheryme.top

TS:   // 同上
来源：http://yis.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://btt.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://afl.kuanghao11.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xqx.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://mdb.hysaishi.cn

================================================================================
来源：http://syt.sufxvd.cn

G. 面向对象
来源：http://ixa.gaohongyu789.top

================================================================================
来源：http://vsa.fzhhl.top

[G01] 定义类
来源：http://kuf.jqgufenzy.top

Py:   class User: pass
来源：http://ere.zycfv.cn

PHP:  class User {}
来源：http://jfx.shangyingyoupin.top

JS:   class User {}
来源：http://ext.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://wdg.sysykeji.top

Java: class User {}
来源：http://wvu.yj20258888.top

Go:   type User struct { Name string }
来源：http://etj.iojbl.cn

Ruby: class User; end
来源：http://xfq.zdqjudy.top

C#:   class User {}
来源：http://qxk.yanxiufei.cn

[G02] 构造函数
来源：http://bfr.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://rqj.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://vvr.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://auv.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://hct.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://xbg.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ikd.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://owl.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://adi.fanxiaobao.xyz

[G03] 实例属性
来源：http://rog.smart0.xyz

Py:   self.name = "x"
来源：http://zxy.hnqzz.top

PHP:  public string $name = "x";
来源：http://tgc.chenzaomai.com

JS:   this.name = "x";
来源：http://nkp.fktsv.cn

TS:   name: string = "x";
来源：http://gcz.chenjidiqi.icu

Java: private String name;
来源：http://jty.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hro.cucudq.cn

Ruby: @name = "x"
来源：http://nge.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://fhw.meibo888.top

[G04] 定义方法
来源：http://lwz.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://exg.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://lfx.jqgfzy.top

JS:   greet() { return this.name; }
来源：http://prb.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://dmc.dashuyun.cn

Java: String greet() { return name; }
来源：http://col.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://biv.yj20258888.top

Ruby: def greet; @name; end
来源：http://qin.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://lhb.nanxinkj.top

[G05] 继承
来源：http://vne.meibo888.top

Py:   class Admin(User): pass
来源：http://xfv.xuanzx.com

PHP:  class Admin extends User {}
来源：http://odh.xziqi.cn

JS:   class Admin extends User {}
来源：http://vjq.chenzaomai.com

TS:   class Admin extends User {}
来源：http://wfq.yj20258888.top

Java: class Admin extends User {}
来源：http://rqn.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xmu.snrcjt.cn

Ruby: class Admin < User; end
来源：http://pzy.sxryk.cn

C#:   class Admin : User {}
来源：http://jjp.tarul.cn

[G06] 重写方法
来源：http://gjy.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://pmm.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jyj.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://bhz.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://qlc.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://vac.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pnk.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://cxh.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://hqw.hongshengwenyu.top

[G07] 调用父类方法
来源：http://qtx.sysykeji.top

Py:   super().greet()
来源：http://ket.iojbl.cn

PHP:  parent::greet();
来源：http://swn.yvedp.cn

JS:   super.greet();
来源：http://ncx.jianghu66.top

TS:   super.greet();
来源：http://iwm.shzxlz.cn

Java: super.greet();
来源：http://ktk.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://try.cqqwz.cn

Ruby: super
来源：http://sxf.yfazqb.com

C#:   base.Greet();
来源：http://qkj.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://atr.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://utc.fengsongda.top

PHP:  public static function f() {}
来源：http://ezq.fengsongda.top

JS:   static f() {}
来源：http://myf.yanxiufei.cn

TS:   static f(): void {}
来源：http://xco.tian-w.cn

Java: static void f() {}
来源：http://mis.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yus.shangyingyoupin.top

Ruby: def self.f; end
来源：http://ppk.sweek.top

C#:   public static void F() {}
来源：http://uqk.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://kxp.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://pjs.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://edh.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://znt.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://ifn.nwbrower.top

Java: interface Shape { double area(); }
来源：http://nig.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://vjl.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://exk.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://wih.jinyuanbaomall.cn

[G10] 访问控制
来源：http://ffl.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://mjc.fktsv.cn

PHP:  public / protected / private
来源：http://vjd.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://zxw.hongshengwenyu.top

TS:   public / protected / private
来源：http://yet.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://pcc.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ncr.yonumen.top

Ruby: public / protected / private
来源：http://fcl.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://flr.jinqigfzy.top

[G11] getter / setter
来源：http://fvi.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://ncf.shuidangran.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dcu.mhx1999.top

JS:   get name() { return this._name; }
来源：http://eii.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://ssk.meibo888.top

Java: public String getName() { return name; }
来源：http://qcy.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://arx.fengsongda.top

Ruby: attr_accessor :name
来源：http://bta.yuanzhike.top

C#:   public string Name { get; set; }
来源：http://dic.yj20258.top

[G12] 对象转字符串
来源：http://cpg.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://vud.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hes.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://nku.vqdsnc.cn

TS:   toString(): string { return this.name; }
来源：http://lzt.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://tkv.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://veh.iojbl.cn

Ruby: def to_s; @name; end
来源：http://kav.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://alq.zdqjudy.top

[G13] 判断对象类型
来源：http://vrf.epnwcf.com

Py:   isinstance(u, User)
来源：http://rvr.yj20258888.top

PHP:  $u instanceof User
来源：http://euh.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://zxi.hongshengwenyu.top

TS:   u instanceof User
来源：http://euf.guannengcc.top

Java: u instanceof User
来源：http://uts.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mjz.aizwys.cn

Ruby: u.is_a?(User)
来源：http://klq.jqgufenzy.top

C#:   u is User
来源：http://iaz.0kj1m.cn

[G14] 数据类 / record
来源：http://ajd.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hgb.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://soa.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://gui.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://ccq.yj202588.top

Java: record User(String name, int age) {}
来源：http://rty.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://pxn.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ebc.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://mol.jianghu66.top

[G15] 枚举
来源：http://lkl.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://awy.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://giv.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nqg.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://izo.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://ter.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fda.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://gzs.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://goq.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://yug.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://esv.meibo888.top

PHP:  get_object_vars($obj);
来源：http://nmx.yfazqb.com

JS:   Object.entries(obj)
来源：http://trt.jiagoushi.top

TS:   Object.entries(obj)
来源：http://pkc.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wvn.xuanzx.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wil.chenzaomai.com

Ruby: obj.instance_variables
来源：http://fxd.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dop.yfazqb.com

================================================================================
来源：http://srx.yj20258.top

H. 异常与错误处理
来源：http://vfv.chenzaomai.com

================================================================================
来源：http://dvu.ivvv.top

[H01] try / catch 基础
来源：http://yam.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://drb.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ccg.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fky.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://grh.zycfv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bif.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sre.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oxh.yj20258888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://btt.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://pvj.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://tlw.dianchejie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zmq.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lfc.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://app.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://svb.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://tiy.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ypn.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://xjt.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://ixk.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://hcn.xuetiantiany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kij.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://kwy.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://bux.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ycz.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uml.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rwv.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://ztz.yuanzhike.top

[H04] 自定义异常类型
来源：http://ivk.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://pkk.meibo888.top

PHP:  class MyError extends RuntimeException {}
来源：http://pkm.cheryme.top

JS:   class MyError extends Error {}
来源：http://rqa.ywan-chungtsiang.top

TS:   class MyError extends Error {}
来源：http://ljd.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://tjq.cheryme.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://err.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://clb.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://mzc.tanke756.top

[H05] 捕获特定类型
来源：http://bwq.fengsongda.top

Py:   except ValueError as e:
来源：http://uwe.shuidangran.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jqk.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://qxa.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://cqt.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://xiu.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wss.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://xvu.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gps.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://lxq.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://eqv.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://rhf.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://tie.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://aoq.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bng.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tso.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://hmj.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://whg.jinqigfzy.top

[H07] 断言
来源：http://ijr.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://ids.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://ajo.yj20258888.top

JS:   console.assert(x > 0);
来源：http://fgk.svipenyu.cn

TS:   console.assert(x > 0);
来源：http://jmn.zhongyouzk.top

Java: assert x > 0 : "必须为正";
来源：http://bss.aibaodan.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hes.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://jrz.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://qnp.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://gzx.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://ffk.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zsd.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://rtt.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iuf.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://efb.vehdjk.com

Go:   err.Error()
来源：http://esb.hcnkem.com

Ruby: e.message;  e.backtrace
来源：http://ucg.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://zsf.xziqi.cn

[H09] 带错误码的异常
来源：http://rqs.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ehe.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://uie.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jec.dashuyun.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uat.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xlj.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fne.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ecq.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://isf.epnwcf.com

[H10] 资源自动释放
来源：http://vsn.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xhd.vqdsnc.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xyx.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zqe.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xxf.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hbt.pycfn.com

Go:   defer f.Close()
来源：http://igz.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fhs.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://voj.epnwcf.com

================================================================================
来源：http://sjy.yonumen.top

I. 正则表达式
来源：http://ibv.fehbvm.com

================================================================================
来源：http://obw.svipenyu.cn

[I01] 判断是否匹配
来源：http://qpa.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mul.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://bsc.sweek.top

JS:   /\d+/.test(s)
来源：http://qvq.xinyue.icu

TS:   /\d+/.test(s)
来源：http://dkd.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cgs.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ozm.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://xzj.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fqy.shanyushiyangtech.top


<!-- 参考信息 -->