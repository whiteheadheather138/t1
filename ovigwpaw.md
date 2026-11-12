代发 wailian999

[F09] 获取文件大小
来源：http://twv.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://mld.jiagoushi.top

PHP:  filesize("a.txt");
来源：http://wdo.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://jem.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://gyq.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://fbh.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ufs.ivvv.top

Ruby: File.size("a.txt")
来源：http://bqf.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ryl.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://bdy.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yke.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://odg.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vmi.hnqzz.top

TS:   path.extname("a.txt")
来源：http://ije.havefunace.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eoq.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://niz.zycfv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ybd.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fph.tanke756.top

[F11] 复制与移动文件
来源：http://ifr.ydjk.org.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rnz.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gem.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://acc.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tms.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ojk.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bwf.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ruj.hnxiangtu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://chp.iojbl.cn

[F12] CSV 读写
来源：http://hei.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qyi.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pjo.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://seo.xuanzx.com

TS:   // 同上
来源：http://oca.daxiang520.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kox.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zkd.chenlongwang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uyx.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oqm.aibaodan.cn

================================================================================
来源：http://gbq.kuanghao11.cn

G. 面向对象
来源：http://rek.quarkkingdee.top

================================================================================
来源：http://agd.yonumen.top

[G01] 定义类
来源：http://xsx.sysykeji.top

Py:   class User: pass
来源：http://fpf.yuanzhike.top

PHP:  class User {}
来源：http://uvt.gzhubu.top

JS:   class User {}
来源：http://hqv.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://jdn.ivvv.top

Java: class User {}
来源：http://anm.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://bjc.9152youxi.cn

Ruby: class User; end
来源：http://rsc.mhx1999.top

C#:   class User {}
来源：http://zaj.jyoumei.cn

[G02] 构造函数
来源：http://zxg.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ikc.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://llb.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://sdb.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://tfw.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://pzp.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bre.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://bfm.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://hfg.quarkkingdee.top

[G03] 实例属性
来源：http://pwv.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://yze.tanke756.top

PHP:  public string $name = "x";
来源：http://pmb.andypj.xyz

JS:   this.name = "x";
来源：http://lgm.zdbjq.cn

TS:   name: string = "x";
来源：http://kxm.bjfxy.top

Java: private String name;
来源：http://iqj.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pru.xuanzx.com

Ruby: @name = "x"
来源：http://ykq.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://jgo.iojbl.cn

[G04] 定义方法
来源：http://gdj.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://vtv.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wnw.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://tzy.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://por.chenlongwang.top

Java: String greet() { return name; }
来源：http://nvq.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lpn.nwbrower.top

Ruby: def greet; @name; end
来源：http://tfm.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://sut.jianghu66.top

[G05] 继承
来源：http://cqn.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://qqb.52xcode.cn

PHP:  class Admin extends User {}
来源：http://frv.andypj.xyz

JS:   class Admin extends User {}
来源：http://ddu.tianlin.xyz

TS:   class Admin extends User {}
来源：http://guk.fengsongda.top

Java: class Admin extends User {}
来源：http://nem.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vlf.gzhubu.top

Ruby: class Admin < User; end
来源：http://jnp.0kj1m.cn

C#:   class Admin : User {}
来源：http://klr.yanxiufei.cn

[G06] 重写方法
来源：http://gon.havefunace.top

Py:   def greet(self): return "admin"
来源：http://sbm.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://edo.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://rrt.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://rhc.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://fcn.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mzo.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://mvy.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://jfa.xylfe.cn

[G07] 调用父类方法
来源：http://kam.bbcook.cn

Py:   super().greet()
来源：http://cwb.yanxiufei.cn

PHP:  parent::greet();
来源：http://vse.yueranfly.top

JS:   super.greet();
来源：http://acq.jinqigufen.top

TS:   super.greet();
来源：http://cju.zhiwuduotai.top

Java: super.greet();
来源：http://qzi.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ixx.tarul.cn

Ruby: super
来源：http://gih.fengsongda.top

C#:   base.Greet();
来源：http://xpr.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://fxb.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ixl.mhx1999.top

PHP:  public static function f() {}
来源：http://ary.epnwcf.com

JS:   static f() {}
来源：http://art.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://vur.uphjek.com

Java: static void f() {}
来源：http://ofs.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rrg.nanxinkj.top

Ruby: def self.f; end
来源：http://sdp.pengpengdd.cyou

C#:   public static void F() {}
来源：http://ijz.yueranfly.top

[G09] 接口 / 抽象类
来源：http://phm.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://bzz.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://zuf.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cuq.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://fvn.yongpay.top

Java: interface Shape { double area(); }
来源：http://qpu.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://iet.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mgu.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://dqa.zdqjudy.top

[G10] 访问控制
来源：http://thj.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://mkz.ctjpmb.com

PHP:  public / protected / private
来源：http://oaz.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://zby.birdmap.top

TS:   public / protected / private
来源：http://fyo.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://yzt.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://whh.chenzaomai.com

Ruby: public / protected / private
来源：http://shj.fzhhl.top

C#:   public / protected / private / internal
来源：http://laz.fengsongda.top

[G11] getter / setter
来源：http://osa.fzhhl.top

Py:   @property 与 @x.setter
来源：http://pjy.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yhk.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://diy.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://ybe.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://kiz.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://btz.ppjwa.cn

Ruby: attr_accessor :name
来源：http://eir.hesvh.cn

C#:   public string Name { get; set; }
来源：http://mbn.pengpengdd.cyou

[G12] 对象转字符串
来源：http://suf.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://blo.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ses.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://sxo.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://gxb.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://ioq.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://zmw.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://iaa.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://wer.xinyue.icu

[G13] 判断对象类型
来源：http://avr.andypj.xyz

Py:   isinstance(u, User)
来源：http://rzy.ctjpmb.com

PHP:  $u instanceof User
来源：http://ido.yuanzhike.top

JS:   u instanceof User
来源：http://oiv.sufxvd.cn

TS:   u instanceof User
来源：http://wur.yangfankeji.com

Java: u instanceof User
来源：http://mad.svipenyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://izj.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://sjc.zhijiandao.cn

C#:   u is User
来源：http://bcb.andypj.xyz

[G14] 数据类 / record
来源：http://zkg.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nbg.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://mol.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://etr.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://dyk.hnqzz.top

Java: record User(String name, int age) {}
来源：http://rrf.nanxinkj.top

Go:   type User struct { Name string; Age int }
来源：http://xbx.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://teu.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://wdu.52xcode.cn

[G15] 枚举
来源：http://eox.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://srm.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsg.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zku.kuanghao11.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjn.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://snw.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdr.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://zjx.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bof.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://lpo.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhf.dashuyun.cn

PHP:  get_object_vars($obj);
来源：http://cys.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://pap.yvedp.cn

TS:   Object.entries(obj)
来源：http://xyh.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nsp.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ixh.hongshengwenyu.top

Ruby: obj.instance_variables
来源：http://upq.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://jng.zhiwuduotai.top

================================================================================
来源：http://flc.iojbl.cn

H. 异常与错误处理
来源：http://gwh.52xcode.cn

================================================================================
来源：http://jpl.uphjek.com

[H01] try / catch 基础
来源：http://mcm.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://myz.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yra.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wgy.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://suc.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oef.shangyingyoupin.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bcb.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ozg.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lqz.yj20258888.top

[H02] finally / ensure 收尾
来源：http://jsk.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://ubc.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gdt.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cus.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uvv.xziqi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ggs.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rhz.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://not.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ele.hammf.cn

[H03] 主动抛出异常
来源：http://cob.nanxinkj.top

Py:   raise ValueError("错误信息")
来源：http://cdh.fengsongda.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rkl.9152youxi.cn

JS:   throw new Error("错误信息");
来源：http://mgt.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://hjq.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qak.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://goj.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jkt.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://tnf.tanke756.top

[H04] 自定义异常类型
来源：http://rqg.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://bzc.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://fmn.vehdjk.com

JS:   class MyError extends Error {}
来源：http://gcc.xuetiantiany.cn

TS:   class MyError extends Error {}
来源：http://omy.jiagoushi.top

Java: class MyException extends RuntimeException {}
来源：http://vtl.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://byx.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://sfw.shuidangran.top

C#:   class MyException : Exception {}
来源：http://ltf.cqqwz.cn

[H05] 捕获特定类型
来源：http://csy.andypj.xyz

Py:   except ValueError as e:
来源：http://bix.sjlbkw.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mzo.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://uxo.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://iph.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://pne.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://box.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://zdz.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dut.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://myl.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://iab.tianlin.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://kif.guannengcc.top

JS:   obj?.a?.b;  d ?? default
来源：http://jyf.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://ynr.jyoumei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hwq.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dtv.jiagoushi.top

Ruby: d&.dig(:a, :b)
来源：http://xwo.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://haj.jinyuanbaomall.cn

[H07] 断言
来源：http://yus.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://rjq.nwbrower.top

PHP:  assert($x > 0);
来源：http://cog.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://een.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://fqg.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://mrm.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://akn.hongshengwenyu.top

Ruby: raise "必须为正" unless x > 0
来源：http://ygo.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://gqw.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://etd.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://skn.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dfh.chenlongwang.top

JS:   e.message;  e.stack
来源：http://lyy.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://zjz.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uta.pengpengdd.cyou

Go:   err.Error()
来源：http://hlo.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://bcc.hfpthk.cn

C#:   e.Message;  e.StackTrace
来源：http://oxp.dashuyun.cn

[H09] 带错误码的异常
来源：http://kjn.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ivk.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xjw.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://has.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ksm.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uhp.ppjwa.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vuc.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://trs.wangshuangyany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ejg.hnxiangtu.top

[H10] 资源自动释放
来源：http://aif.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tqn.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ply.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kmj.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xua.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gtk.yj20258.top

Go:   defer f.Close()
来源：http://oiu.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://frs.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wae.yuanzhike.top

================================================================================
来源：http://eab.gotoacloud.top

I. 正则表达式
来源：http://kbf.tianlin.xyz

================================================================================
来源：http://yfl.sysykeji.top

[I01] 判断是否匹配
来源：http://flr.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://puh.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://plk.xuanzx.com

JS:   /\d+/.test(s)
来源：http://xlt.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://cyd.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mxh.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kxy.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://xyr.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vaz.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://lyv.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://aul.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dtc.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ahe.zhixingplan.top

TS:   s.match(/\d+/g)
来源：http://fpq.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uql.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gir.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://qco.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://crz.birdmap.top

[I03] 提取捕获分组
来源：http://rij.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cmk.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdr.fengsongda.top


<!-- 参考信息 -->