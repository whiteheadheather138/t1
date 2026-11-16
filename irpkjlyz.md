代发 wailian999

[F09] 获取文件大小
来源：http://twd.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://uty.mhx1999.top

PHP:  filesize("a.txt");
来源：http://egq.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://ovi.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://umq.fktsv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ogl.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://htz.gzhubu.top

Ruby: File.size("a.txt")
来源：http://jlz.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://jbi.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://ucc.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cbi.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tsr.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uei.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://ygh.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kxf.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wsm.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vnb.iojbl.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://frl.fktsv.cn

[F11] 复制与移动文件
来源：http://iwo.cashguo.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yrn.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ryf.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qbt.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nhr.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mjx.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bcq.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vgq.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rtf.yj20258888.top

[F12] CSV 读写
来源：http://omu.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gqc.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ixx.birdmap.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wck.hesvh.cn

TS:   // 同上
来源：http://bxg.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yal.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hnu.snrcjt.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iwc.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eyq.fanxiaobao.xyz

================================================================================
来源：http://cpj.redwolf501.top

G. 面向对象
来源：http://qaf.ydjk.org.cn

================================================================================
来源：http://teb.yj20258.top

[G01] 定义类
来源：http://nkt.jianghu66.top

Py:   class User: pass
来源：http://fcv.zdqjudy.top

PHP:  class User {}
来源：http://jum.yangfankeji.com

JS:   class User {}
来源：http://ndt.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://vsa.yj20258888.top

Java: class User {}
来源：http://vwr.vehdjk.com

Go:   type User struct { Name string }
来源：http://ohc.wangshuangyany.cn

Ruby: class User; end
来源：http://thk.cheryme.top

C#:   class User {}
来源：http://gyg.haohaochexian.top

[G02] 构造函数
来源：http://poe.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://nui.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://tzq.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://qpz.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://fjh.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://apr.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyo.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://rhc.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://axq.9152youxi.cn

[G03] 实例属性
来源：http://bpq.wangshuangyany.cn

Py:   self.name = "x"
来源：http://kxi.iojbl.cn

PHP:  public string $name = "x";
来源：http://iaj.cqqwz.cn

JS:   this.name = "x";
来源：http://qli.pengpengdd.cyou

TS:   name: string = "x";
来源：http://nxr.yuanzhike.top

Java: private String name;
来源：http://upy.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cai.jiagoushi.top

Ruby: @name = "x"
来源：http://dyv.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://igt.xylfe.cn

[G04] 定义方法
来源：http://xmw.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://qpb.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kga.yueranfly.top

JS:   greet() { return this.name; }
来源：http://mbz.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://puo.nwbrower.top

Java: String greet() { return name; }
来源：http://xbf.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iei.316326.xyz

Ruby: def greet; @name; end
来源：http://ieu.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://deo.hnxiangtu.top

[G05] 继承
来源：http://bmz.zhaomingkeji.xyz

Py:   class Admin(User): pass
来源：http://bja.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://adq.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://jnc.hammf.cn

TS:   class Admin extends User {}
来源：http://jqt.zhongyouzk.top

Java: class Admin extends User {}
来源：http://fyy.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wji.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://cxo.hcnkem.com

C#:   class Admin : User {}
来源：http://aws.birdmap.top

[G06] 重写方法
来源：http://fcb.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://rxp.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ujy.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://ouw.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://vae.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://aje.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nle.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://kqm.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://pga.daxiang520.top

[G07] 调用父类方法
来源：http://uep.svipenyu.cn

Py:   super().greet()
来源：http://fpp.hysaishi.cn

PHP:  parent::greet();
来源：http://wmd.guannengcc.top

JS:   super.greet();
来源：http://qts.guowangkeji.top

TS:   super.greet();
来源：http://aec.vqdsnc.cn

Java: super.greet();
来源：http://mln.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aql.yfazqb.com

Ruby: super
来源：http://spx.yfazqb.com

C#:   base.Greet();
来源：http://xfy.yangfankeji.com

[G08] 静态方法与属性
来源：http://uvo.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vtw.ehwqpu.com

PHP:  public static function f() {}
来源：http://rdl.redwolf501.top

JS:   static f() {}
来源：http://dak.tarul.cn

TS:   static f(): void {}
来源：http://upx.ivvv.top

Java: static void f() {}
来源：http://okt.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mys.hnqzz.top

Ruby: def self.f; end
来源：http://ttx.guowangkeji.top

C#:   public static void F() {}
来源：http://ejb.quarkkingdee.top

[G09] 接口 / 抽象类
来源：http://gmp.quarkkingdee.top

Py:   from abc import ABC, abstractmethod
来源：http://lrp.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://aff.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://nij.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://vrw.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://lhy.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://ybh.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pnw.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://bom.zhongyouzk.top

[G10] 访问控制
来源：http://qkl.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://llj.svipenyu.cn

PHP:  public / protected / private
来源：http://qeb.sweek.top

JS:   #private 字段；其余公开
来源：http://llx.dianchejie.cn

TS:   public / protected / private
来源：http://ddi.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://idf.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jny.shzxlz.cn

Ruby: public / protected / private
来源：http://vgr.jyoumei.cn

C#:   public / protected / private / internal
来源：http://sns.nanxuanxn.top

[G11] getter / setter
来源：http://usi.yj20258888.top

Py:   @property 与 @x.setter
来源：http://don.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zbl.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://iba.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://nqm.fengsongda.top

Java: public String getName() { return name; }
来源：http://grl.zycfv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qzj.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://tor.hcnkem.com

C#:   public string Name { get; set; }
来源：http://qzy.yonumen.top

[G12] 对象转字符串
来源：http://oaa.jinqigufen.top

Py:   def __str__(self): return self.name
来源：http://oej.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fxu.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://nsa.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://lcy.ppjwa.cn

Java: @Override public String toString() { return name; }
来源：http://lvr.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qtn.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://lvk.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://avq.guowangkeji.top

[G13] 判断对象类型
来源：http://iby.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://fzl.sjlbkw.cn

PHP:  $u instanceof User
来源：http://klq.ydzc1.top

JS:   u instanceof User
来源：http://ktf.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://zji.pengpengdd.cyou

Java: u instanceof User
来源：http://clz.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mng.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://txz.nwbrower.top

C#:   u is User
来源：http://kwp.dianchejie.cn

[G14] 数据类 / record
来源：http://utq.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dfu.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://cja.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xni.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://ajo.ivvv.top

Java: record User(String name, int age) {}
来源：http://avx.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://ixq.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yrt.xuetiantiany.cn

C#:   record User(string Name, int Age);
来源：http://zcp.shanyushiyangkeji.top

[G15] 枚举
来源：http://uhs.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tpw.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lju.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vbd.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ebd.hfpthk.cn

Java: enum Color { RED, GREEN }
来源：http://epx.fzhhl.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lzy.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://usp.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djk.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://fyj.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vme.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://kjf.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://dva.zhixingplan.top

TS:   Object.entries(obj)
来源：http://pcx.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hij.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yxr.wangdashe.top

Ruby: obj.instance_variables
来源：http://ivd.guannengcc.top

C#:   // 用反射或 System.Text.Json
来源：http://cob.ctjpmb.com

================================================================================
来源：http://jzo.hnqzz.top

H. 异常与错误处理
来源：http://xzj.wangdashe.top

================================================================================
来源：http://gsj.xuanzx.com

[H01] try / catch 基础
来源：http://mzt.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rah.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://efl.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xsi.jianghu66.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xyd.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kvz.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ggg.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rwc.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gdg.birdmap.top

[H02] finally / ensure 收尾
来源：http://qkj.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://jvq.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dsc.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uny.yangfankeji.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ipn.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://vlo.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pko.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://omy.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pll.zdbjq.cn

[H03] 主动抛出异常
来源：http://dtx.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://azk.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ozy.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://gbd.ivvv.top

TS:   throw new Error("错误信息");
来源：http://xdl.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yla.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hvq.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hna.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ufi.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://dvi.316326.xyz

Py:   class MyError(Exception): pass
来源：http://otu.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vwc.hcnkem.com

JS:   class MyError extends Error {}
来源：http://qwv.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://gaq.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://zjz.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eyx.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://xmr.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://sos.cashguo.top

[H05] 捕获特定类型
来源：http://rsj.vehdjk.com

Py:   except ValueError as e:
来源：http://pqx.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hww.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://tap.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://pcu.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://kxl.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dcp.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://bfp.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fhy.havefunace.top

[H06] 可选值 / 空值安全访问
来源：http://btk.bbcook.cn

Py:   value = d.get("k") or default
来源：http://lqs.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://hkl.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://gua.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://xme.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xtm.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ieo.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://uft.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://gxa.shuidangran.top

[H07] 断言
来源：http://bvt.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://elu.chenzaomai.com

PHP:  assert($x > 0);
来源：http://eil.guannengcc.top

JS:   console.assert(x > 0);
来源：http://xch.fehbvm.com

TS:   console.assert(x > 0);
来源：http://qtv.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://bdu.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qwz.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ytz.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://bab.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://cbu.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://djb.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ypc.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://ldw.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tmn.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ure.zhoulong.xyz

Go:   err.Error()
来源：http://jnd.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://mih.zhiwuduotai.top

C#:   e.Message;  e.StackTrace
来源：http://kxq.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://kqg.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gbx.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cft.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lbw.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fhc.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xho.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mvo.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xti.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zuo.havefunace.top

[H10] 资源自动释放
来源：http://bhk.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://jke.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zkn.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cyp.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rpd.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jdw.yuanzhike.top

Go:   defer f.Close()
来源：http://uhi.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qaz.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mvc.chenjidiqi.icu

================================================================================
来源：http://vzl.wangshuangyany.cn

I. 正则表达式
来源：http://efx.daxiang520.top

================================================================================
来源：http://jof.ctjpmb.com

[I01] 判断是否匹配
来源：http://bxi.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jfd.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rue.redwolf501.top

JS:   /\d+/.test(s)
来源：http://zdw.fengsongda.top

TS:   /\d+/.test(s)
来源：http://ncw.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ywn.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://svx.iojbl.cn

Ruby: s.match?(/\d+/)
来源：http://pvk.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xns.xuanzx.com

[I02] 提取所有匹配
来源：http://fef.mhx1999.top

Py:   re.findall(r"\d+", s)
来源：http://wfm.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jgj.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://trs.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://qbx.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvv.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bfo.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://toz.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://myp.c1oappe.top

[I03] 提取捕获分组
来源：http://fkf.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lvl.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oxo.c1oappe.top


<!-- 参考信息 -->