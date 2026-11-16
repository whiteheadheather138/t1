代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xis.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aor.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://zpp.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://soa.yj20258888.top

[F09] 获取文件大小
来源：http://psk.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://vpp.mhx1999.top

PHP:  filesize("a.txt");
来源：http://keb.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://fue.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://wza.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://ntj.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hqf.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://wdf.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://oie.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbo.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zdq.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ibj.yongpay.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xwx.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://xoo.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ppm.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vig.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://veh.xuetiantiany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yic.xylfe.cn

[F11] 复制与移动文件
来源：http://elw.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hwb.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uyj.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://evd.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qin.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://soc.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lzz.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://keo.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uak.vqdsnc.cn

[F12] CSV 读写
来源：http://pgo.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pmn.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vcb.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vos.shuidangran.top

TS:   // 同上
来源：http://dex.tanke756.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kcv.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zvc.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wzr.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://soa.svipenyu.cn

================================================================================
来源：http://aar.hywenlv.cn

G. 面向对象
来源：http://fgh.pengpengdd.cyou

================================================================================
来源：http://qqo.zdbjq.cn

[G01] 定义类
来源：http://yan.jinqigufen.top

Py:   class User: pass
来源：http://ruu.daria6918.cn

PHP:  class User {}
来源：http://lol.chenzaomai.com

JS:   class User {}
来源：http://udc.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://tvx.0kj1m.cn

Java: class User {}
来源：http://ore.mhx1999.top

Go:   type User struct { Name string }
来源：http://ldf.fzhhl.top

Ruby: class User; end
来源：http://cwm.fengsongda.top

C#:   class User {}
来源：http://qlg.jianghu66.top

[G02] 构造函数
来源：http://gab.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ocs.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://eyu.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://cuk.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://yyr.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://lxu.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kku.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://pbm.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://jul.tanke756.top

[G03] 实例属性
来源：http://kza.jlsjyb.cn

Py:   self.name = "x"
来源：http://fhr.c1oappe.top

PHP:  public string $name = "x";
来源：http://wgy.jqgufenzy.top

JS:   this.name = "x";
来源：http://dlk.tian-w.cn

TS:   name: string = "x";
来源：http://awr.nanxinkj.top

Java: private String name;
来源：http://zpi.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cfu.xziqi.cn

Ruby: @name = "x"
来源：http://ysz.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://lxw.epnwcf.com

[G04] 定义方法
来源：http://xyz.gzhubu.top

Py:   def greet(self): return self.name
来源：http://dos.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lrf.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://uhz.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://rvm.jlsjyb.cn

Java: String greet() { return name; }
来源：http://hbb.gogol.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://awe.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://kgy.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://wgj.iojbl.cn

[G05] 继承
来源：http://lye.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://etq.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://rtk.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://raz.yongpay.top

TS:   class Admin extends User {}
来源：http://tqk.ppjwa.cn

Java: class Admin extends User {}
来源：http://bms.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pwn.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://isc.iojbl.cn

C#:   class Admin : User {}
来源：http://jqy.yueranfly.top

[G06] 重写方法
来源：http://olh.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://btf.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dcr.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://mhh.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://gav.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://wai.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://syq.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://mws.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://uvu.wangdashe.top

[G07] 调用父类方法
来源：http://vly.gogol.net.cn

Py:   super().greet()
来源：http://rpa.feifeiyinyue.top

PHP:  parent::greet();
来源：http://zaj.hnqzz.top

JS:   super.greet();
来源：http://ysf.yuxming.cn

TS:   super.greet();
来源：http://tdb.quarkkingdee.top

Java: super.greet();
来源：http://hei.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yau.ydzc1.top

Ruby: super
来源：http://oky.cqqwz.cn

C#:   base.Greet();
来源：http://kkq.nanxinkj.top

[G08] 静态方法与属性
来源：http://nwu.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wvj.uphjek.com

PHP:  public static function f() {}
来源：http://xbr.jinghuilouyu.cn

JS:   static f() {}
来源：http://muv.0kj1m.cn

TS:   static f(): void {}
来源：http://vyx.sxryk.cn

Java: static void f() {}
来源：http://peh.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ket.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://eop.daria6918.cn

C#:   public static void F() {}
来源：http://ums.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://ugj.svipenyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://ygh.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://yqq.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://urx.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://qwa.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://tvm.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://npn.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ptw.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://fyw.hnxiangtu.top

[G10] 访问控制
来源：http://tzl.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://sze.epnwcf.com

PHP:  public / protected / private
来源：http://zvm.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://lky.hcnkem.com

TS:   public / protected / private
来源：http://kgr.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://ogr.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xga.xuetiantiany.cn

Ruby: public / protected / private
来源：http://vcm.zycfv.cn

C#:   public / protected / private / internal
来源：http://iid.jqgufenzy.top

[G11] getter / setter
来源：http://rwr.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://kqu.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uyn.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://qgp.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://gth.gotoacloud.top

Java: public String getName() { return name; }
来源：http://jmv.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pfy.daxiang520.top

Ruby: attr_accessor :name
来源：http://psm.shuidangran.top

C#:   public string Name { get; set; }
来源：http://zah.gotoacloud.top

[G12] 对象转字符串
来源：http://yvs.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://bfu.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dhx.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://ixm.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://oet.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://khz.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://ory.yonumen.top

Ruby: def to_s; @name; end
来源：http://nvu.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://pez.xylfe.cn

[G13] 判断对象类型
来源：http://juc.zhengqikj.top

Py:   isinstance(u, User)
来源：http://mou.zhoulong.xyz

PHP:  $u instanceof User
来源：http://sdp.smart0.xyz

JS:   u instanceof User
来源：http://aaf.sysykeji.top

TS:   u instanceof User
来源：http://cva.fzhhl.top

Java: u instanceof User
来源：http://cnz.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://goe.guannengcc.top

Ruby: u.is_a?(User)
来源：http://fbl.bbcook.cn

C#:   u is User
来源：http://inz.zhengqikj.top

[G14] 数据类 / record
来源：http://cpr.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zjw.bbcook.cn

PHP:  // 用 readonly 属性模拟
来源：http://vsq.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://lqy.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://dub.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://oec.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://ifz.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wqm.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://byk.quarkkingdee.top

[G15] 枚举
来源：http://hjr.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gau.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://qeh.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufx.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wiy.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://qsg.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bve.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://kdf.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dwx.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://lhc.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nti.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://rvd.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://uxk.yfazqb.com

TS:   Object.entries(obj)
来源：http://ooo.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://brl.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ewy.tanke756.top

Ruby: obj.instance_variables
来源：http://rgr.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://piq.ydjk.org.cn

================================================================================
来源：http://yfq.zhiwuduotai.top

H. 异常与错误处理
来源：http://zxr.svipenyu.cn

================================================================================
来源：http://hef.nwbrower.top

[H01] try / catch 基础
来源：http://rzy.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://efo.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ike.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zkl.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://llt.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jxd.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gpt.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aez.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xrg.c1oappe.top

[H02] finally / ensure 收尾
来源：http://oyp.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://kcs.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nqm.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cpo.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rlk.chenlongwang.top

Java: try { f(); } finally { cleanup(); }
来源：http://aiv.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://nri.xinyue.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://ikl.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://uen.ctjpmb.com

[H03] 主动抛出异常
来源：http://mub.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://nei.pycfn.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uwt.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://qaa.pycfn.com

TS:   throw new Error("错误信息");
来源：http://ysg.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://sqy.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xva.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vdp.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qle.cqqwz.cn

[H04] 自定义异常类型
来源：http://rjc.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://svg.316326.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://bad.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://bzp.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://fhk.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://ryl.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uwi.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://wll.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://dww.yfazqb.com

[H05] 捕获特定类型
来源：http://haw.hywenlv.cn

Py:   except ValueError as e:
来源：http://ira.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kvx.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://imy.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://pun.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://egf.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkt.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://nah.wangdashe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ppr.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://tht.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://nif.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://dus.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://igd.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://azv.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eer.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://pfs.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://csd.sweek.top

C#:   obj?.A?.B ?? default
来源：http://huq.jqgufenzy.top

[H07] 断言
来源：http://djs.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://yqi.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://bvg.sweek.top

JS:   console.assert(x > 0);
来源：http://yfg.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://qtf.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://huu.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lpt.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://dwj.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://wko.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://das.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://hry.xingfuxueyuan.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qih.mhx1999.top

JS:   e.message;  e.stack
来源：http://uje.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwz.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hhh.birdmap.top

Go:   err.Error()
来源：http://phh.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://oio.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://zxj.52xcode.cn

[H09] 带错误码的异常
来源：http://lig.yj202588.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pkv.jqgfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oic.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hul.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://scu.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aiw.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ove.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://rmr.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://lhn.daria6918.cn

[H10] 资源自动释放
来源：http://jxt.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://gtr.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bjg.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ecy.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cvk.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vgn.zhijiandao.cn

Go:   defer f.Close()
来源：http://cpk.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gbq.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://klo.zhoulong.xyz

================================================================================
来源：http://rjo.ctjpmb.com

I. 正则表达式
来源：http://tly.xinyue.icu

================================================================================
来源：http://wri.xuanzx.com

[I01] 判断是否匹配
来源：http://zzw.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://stm.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://rbs.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://kbl.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://dtv.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ixy.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qmh.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://jwz.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mec.uphjek.com

[I02] 提取所有匹配
来源：http://ylg.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://brk.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qph.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lrk.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://yeu.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bub.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dym.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://zfk.vehdjk.com


<!-- 参考信息 -->