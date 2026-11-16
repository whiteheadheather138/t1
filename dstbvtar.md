代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://huu.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ddq.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://xud.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://plu.gaohongyu789.top

[F09] 获取文件大小
来源：http://wwl.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://dtm.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://pqb.xuetiantiany.cn

JS:   fs.statSync("a.txt").size
来源：http://tgn.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://mla.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://npc.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wjs.tarul.cn

Ruby: File.size("a.txt")
来源：http://gvs.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://gqw.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://uux.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oxw.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://one.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rni.daxiang520.top

TS:   path.extname("a.txt")
来源：http://kbe.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cgo.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cre.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://asi.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nha.52xcode.cn

[F11] 复制与移动文件
来源：http://biy.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bmn.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wko.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uru.zdbjq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://reb.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zkl.hysaishi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ird.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpx.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://twn.xylfe.cn

[F12] CSV 读写
来源：http://xdi.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vny.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qnl.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kwp.chenlongwang.top

TS:   // 同上
来源：http://ygx.jinqigufen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mjr.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gog.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qtj.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xlc.cqqwz.cn

================================================================================
来源：http://cfh.yj202588.top

G. 面向对象
来源：http://cyn.ydjk.org.cn

================================================================================
来源：http://utv.xingfuxueyuan.xyz

[G01] 定义类
来源：http://kre.yj20258888.top

Py:   class User: pass
来源：http://rwb.jqgfzy.top

PHP:  class User {}
来源：http://fln.zdqjudy.top

JS:   class User {}
来源：http://pyq.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://baj.0kj1m.cn

Java: class User {}
来源：http://ovv.bjfxy.top

Go:   type User struct { Name string }
来源：http://mfy.pengpengdd.cyou

Ruby: class User; end
来源：http://ugm.ctjpmb.com

C#:   class User {}
来源：http://sjj.yvedp.cn

[G02] 构造函数
来源：http://vav.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://vxu.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://ygv.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://qfs.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://awi.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://khm.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nbr.cheryme.top

Ruby: def initialize(name); @name = name; end
来源：http://xbk.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://hbs.yanxiufei.cn

[G03] 实例属性
来源：http://tig.tanke756.top

Py:   self.name = "x"
来源：http://idi.xylfe.cn

PHP:  public string $name = "x";
来源：http://uvw.yongpay.top

JS:   this.name = "x";
来源：http://wrk.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://jnm.xylfe.cn

Java: private String name;
来源：http://hhd.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://scl.fehbvm.com

Ruby: @name = "x"
来源：http://txl.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://unv.dianchejie.cn

[G04] 定义方法
来源：http://qdq.yfazqb.com

Py:   def greet(self): return self.name
来源：http://eji.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ipn.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://ake.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://iog.zhengqikj.top

Java: String greet() { return name; }
来源：http://zrs.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gnv.gogol.net.cn

Ruby: def greet; @name; end
来源：http://oaj.yj202588.top

C#:   public string Greet() => Name;
来源：http://fpg.gogol.net.cn

[G05] 继承
来源：http://dtk.wangdashe.top

Py:   class Admin(User): pass
来源：http://lgg.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://inr.yvedp.cn

JS:   class Admin extends User {}
来源：http://tbf.tarul.cn

TS:   class Admin extends User {}
来源：http://cgx.zhengqikj.top

Java: class Admin extends User {}
来源：http://eim.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kfd.cucudq.cn

Ruby: class Admin < User; end
来源：http://qre.haohaochexian.top

C#:   class Admin : User {}
来源：http://csc.yangfankeji.com

[G06] 重写方法
来源：http://bla.hammf.cn

Py:   def greet(self): return "admin"
来源：http://sal.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vuw.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://zub.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://rly.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://hvx.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yry.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://oxj.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://jem.9152youxi.cn

[G07] 调用父类方法
来源：http://ovu.zhongyouzk.top

Py:   super().greet()
来源：http://pok.pengpengdd.cyou

PHP:  parent::greet();
来源：http://xoq.zhixingplan.top

JS:   super.greet();
来源：http://hld.dashuyun.cn

TS:   super.greet();
来源：http://bmv.jinghuilouyu.cn

Java: super.greet();
来源：http://drq.sufxvd.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qpm.wangshuangyany.cn

Ruby: super
来源：http://pnf.fzhhl.top

C#:   base.Greet();
来源：http://zls.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://eud.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rfu.andypj.xyz

PHP:  public static function f() {}
来源：http://qfq.guowangkeji.top

JS:   static f() {}
来源：http://bii.dashuyun.cn

TS:   static f(): void {}
来源：http://zyi.sjlbkw.cn

Java: static void f() {}
来源：http://qnx.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pdh.sysykeji.top

Ruby: def self.f; end
来源：http://zvy.tianlin.xyz

C#:   public static void F() {}
来源：http://ygg.xinyue.icu

[G09] 接口 / 抽象类
来源：http://fuz.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://uip.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://jxj.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qde.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://uon.yuxming.cn

Java: interface Shape { double area(); }
来源：http://vvh.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://zhf.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qbh.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://shh.aibaodan.cn

[G10] 访问控制
来源：http://wos.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://ghl.316326.xyz

PHP:  public / protected / private
来源：http://daw.wangdashe.top

JS:   #private 字段；其余公开
来源：http://qit.ppjwa.cn

TS:   public / protected / private
来源：http://obi.tanke756.top

Java: public / protected / private / 默认包级
来源：http://euj.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://lwn.yonumen.top

Ruby: public / protected / private
来源：http://gop.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://mij.yueranfly.top

[G11] getter / setter
来源：http://kvf.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://lyj.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jbe.bbcook.cn

JS:   get name() { return this._name; }
来源：http://qjr.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://fuo.gotoacloud.top

Java: public String getName() { return name; }
来源：http://nah.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://sii.ctjpmb.com

Ruby: attr_accessor :name
来源：http://eaa.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://yic.shangyingyoupin.top

[G12] 对象转字符串
来源：http://hor.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://jzj.bjfxy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://duk.tian-w.cn

JS:   toString() { return this.name; }
来源：http://phq.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://ytm.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://xfb.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://gwq.iojbl.cn

Ruby: def to_s; @name; end
来源：http://uob.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://hoh.xziqi.cn

[G13] 判断对象类型
来源：http://snu.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://sci.c1oappe.top

PHP:  $u instanceof User
来源：http://miu.nwbrower.top

JS:   u instanceof User
来源：http://zoy.meibo888.top

TS:   u instanceof User
来源：http://nqc.yfazqb.com

Java: u instanceof User
来源：http://zls.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsj.yangfankeji.com

Ruby: u.is_a?(User)
来源：http://lgk.feifeiyinyue.top

C#:   u is User
来源：http://yon.9152youxi.cn

[G14] 数据类 / record
来源：http://aes.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ohw.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://vwp.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lhm.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://qjq.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://bek.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://gue.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wrx.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://kma.shangyingyoupin.top

[G15] 枚举
来源：http://qgs.fzhhl.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vwa.jinyuanbaomall.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mux.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iui.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kzd.jinghuilouyu.cn

Java: enum Color { RED, GREEN }
来源：http://yvj.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rrk.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://ral.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kus.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://zzr.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iiu.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://rti.yuxming.cn

JS:   Object.entries(obj)
来源：http://sdk.meibo888.top

TS:   Object.entries(obj)
来源：http://mfe.hesvh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://awp.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://rwr.9152youxi.cn

Ruby: obj.instance_variables
来源：http://kul.chenjidiqi.icu

C#:   // 用反射或 System.Text.Json
来源：http://gru.yongpay.top

================================================================================
来源：http://btw.jyoumei.cn

H. 异常与错误处理
来源：http://ugx.zdqjudy.top

================================================================================
来源：http://iku.yuanzhike.top

[H01] try / catch 基础
来源：http://wjr.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ezs.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fyj.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dqn.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dat.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nvn.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://afs.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dhe.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ysq.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://xoc.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://hgz.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://svt.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tte.xziqi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uam.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pcn.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wrr.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://kcr.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://elm.zdqjudy.top

[H03] 主动抛出异常
来源：http://sck.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://rfg.wangdashe.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://thy.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://opz.sweek.top

TS:   throw new Error("错误信息");
来源：http://dad.zhongyouzk.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vnm.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://scw.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://rfy.andypj.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://tkx.yanxiufei.cn

[H04] 自定义异常类型
来源：http://grg.yongpay.top

Py:   class MyError(Exception): pass
来源：http://zrb.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://aby.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://rds.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://jym.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://qrl.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://drl.yangfankeji.com

Ruby: class MyError < StandardError; end
来源：http://lst.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://eul.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://xvs.316326.xyz

Py:   except ValueError as e:
来源：http://zif.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://snn.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://zau.daria6918.cn

TS:   if (e instanceof TypeError) {}
来源：http://tle.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://jnx.xinyue.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dsu.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://rrx.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://joc.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://tkf.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://act.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://crv.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://yvf.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://obt.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oti.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ukl.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://nlm.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://grz.vqdsnc.cn

[H07] 断言
来源：http://mak.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://pxt.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://itp.guannengcc.top

JS:   console.assert(x > 0);
来源：http://yye.birdmap.top

TS:   console.assert(x > 0);
来源：http://and.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://mgu.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzq.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zec.ywan-chungtsiang.top

C#:   Debug.Assert(x > 0);
来源：http://ybm.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://ghh.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://zeo.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwz.hesvh.cn

JS:   e.message;  e.stack
来源：http://qwy.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://int.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gtj.quarkkingdee.top

Go:   err.Error()
来源：http://lrw.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://mwt.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ohh.aizwys.cn

[H09] 带错误码的异常
来源：http://mjm.zhixingplan.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://spq.hnxiangtu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xib.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wkn.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wyz.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kyz.feifeiyinyue.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iap.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://tmj.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://wbn.guannengcc.top

[H10] 资源自动释放
来源：http://okg.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://idq.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dtm.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yzy.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ufa.chenjidiqi.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zmw.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://yim.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nrm.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ttf.zhaomingkeji.xyz

================================================================================
来源：http://zha.xinyue.icu

I. 正则表达式
来源：http://mwc.shanyushiyangkeji.top

================================================================================
来源：http://stt.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://mtm.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://enx.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://exu.sxryk.cn

JS:   /\d+/.test(s)
来源：http://ieb.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://cet.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kcx.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ocd.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://dzi.ydjk.org.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fza.yj20258888.top

[I02] 提取所有匹配
来源：http://kxg.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://ahz.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ewe.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kvv.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://azz.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://okk.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yie.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://dxw.hnxiangtu.top


<!-- 参考信息 -->