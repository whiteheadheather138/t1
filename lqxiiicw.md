代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vlw.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://won.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://twc.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://aza.xuanzx.com

[F09] 获取文件大小
来源：http://ooq.birdmap.top

Py:   os.path.getsize("a.txt")
来源：http://sla.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://gep.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://szu.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://mpw.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://ttg.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gwn.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://fqn.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://lea.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://dqk.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://our.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dsq.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://idr.mhx1999.top

TS:   path.extname("a.txt")
来源：http://mpc.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ibe.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xvg.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wzg.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rhq.hysaishi.cn

[F11] 复制与移动文件
来源：http://kur.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jxt.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://skk.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sft.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ojb.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pde.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xap.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dzi.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xqg.hongshengwenyu.top

[F12] CSV 读写
来源：http://oor.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kpg.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ehg.sxryk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nnt.gotoacloud.top

TS:   // 同上
来源：http://plk.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dgn.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ykb.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://erg.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xgs.quarkkingdee.top

================================================================================
来源：http://iqw.vqdsnc.cn

G. 面向对象
来源：http://xky.fanxiaobao.xyz

================================================================================
来源：http://dth.hnqzz.top

[G01] 定义类
来源：http://txv.zhengqikj.top

Py:   class User: pass
来源：http://mog.yj202588.top

PHP:  class User {}
来源：http://bcx.gotoacloud.top

JS:   class User {}
来源：http://urz.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://tmv.jiagoushi.top

Java: class User {}
来源：http://nye.andypj.xyz

Go:   type User struct { Name string }
来源：http://zyx.wangdashe.top

Ruby: class User; end
来源：http://age.epnwcf.com

C#:   class User {}
来源：http://ovz.daxiang520.top

[G02] 构造函数
来源：http://owx.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://aiv.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://cbk.mhx1999.top

JS:   constructor(name) { this.name = name; }
来源：http://ful.uphjek.com

TS:   constructor(public name: string) {}
来源：http://bzf.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://iow.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lkl.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://kdz.zdbjq.cn

C#:   public User(string name) { Name = name; }
来源：http://jvh.hongshengwenyu.top

[G03] 实例属性
来源：http://vdj.chenlongwang.top

Py:   self.name = "x"
来源：http://wjs.redwolf501.top

PHP:  public string $name = "x";
来源：http://iyl.havefunace.top

JS:   this.name = "x";
来源：http://qrf.chenlongwang.top

TS:   name: string = "x";
来源：http://ter.hfpthk.cn

Java: private String name;
来源：http://suc.dashuyun.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tnq.kuanghao11.cn

Ruby: @name = "x"
来源：http://jpj.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://uqd.shuidangran.top

[G04] 定义方法
来源：http://qrf.meibo888.top

Py:   def greet(self): return self.name
来源：http://osx.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gzy.bjfxy.top

JS:   greet() { return this.name; }
来源：http://nbc.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://lmm.guowangkeji.top

Java: String greet() { return name; }
来源：http://tfw.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fkd.gotoacloud.top

Ruby: def greet; @name; end
来源：http://qwj.xinyue.icu

C#:   public string Greet() => Name;
来源：http://lpp.xuanzx.com

[G05] 继承
来源：http://jml.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://kxj.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://iwa.chenzaomai.com

JS:   class Admin extends User {}
来源：http://zfg.daria6918.cn

TS:   class Admin extends User {}
来源：http://izg.birdmap.top

Java: class Admin extends User {}
来源：http://jld.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://svd.yj20258.top

Ruby: class Admin < User; end
来源：http://qzr.kuanghao11.cn

C#:   class Admin : User {}
来源：http://kcx.hammf.cn

[G06] 重写方法
来源：http://fdy.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://imv.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ebb.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://kws.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://vpc.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ble.xziqi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jnm.epnwcf.com

Ruby: def greet; "admin"; end
来源：http://xgs.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://uuu.jiagoushi.top

[G07] 调用父类方法
来源：http://uhs.nanxinkj.top

Py:   super().greet()
来源：http://ebt.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://uka.hysaishi.cn

JS:   super.greet();
来源：http://hvb.yuxming.cn

TS:   super.greet();
来源：http://evj.cdnleiting.top

Java: super.greet();
来源：http://zkk.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jnx.birdmap.top

Ruby: super
来源：http://uin.0kj1m.cn

C#:   base.Greet();
来源：http://hwv.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://vbp.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gmf.c1oappe.top

PHP:  public static function f() {}
来源：http://nrc.316326.xyz

JS:   static f() {}
来源：http://rvh.pengpengdd.cyou

TS:   static f(): void {}
来源：http://inr.hnxiangtu.top

Java: static void f() {}
来源：http://inv.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xsm.nanxuanxn.top

Ruby: def self.f; end
来源：http://rxb.wangdashe.top

C#:   public static void F() {}
来源：http://exk.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://tzf.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://ixb.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://xtq.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lpg.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://oxe.yj20258888.top

Java: interface Shape { double area(); }
来源：http://vtl.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://pwe.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jfb.0kj1m.cn

C#:   interface IShape { double Area(); }
来源：http://caw.xinyue.icu

[G10] 访问控制
来源：http://yap.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://uxr.yuanzhike.top

PHP:  public / protected / private
来源：http://qio.andypj.xyz

JS:   #private 字段；其余公开
来源：http://bgn.pycfn.com

TS:   public / protected / private
来源：http://hcv.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://dtc.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mwy.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://rzj.hywenlv.cn

C#:   public / protected / private / internal
来源：http://cmt.yueranfly.top

[G11] getter / setter
来源：http://zzq.ydzc1.top

Py:   @property 与 @x.setter
来源：http://luj.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://emd.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://cvn.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://sxa.nwbrower.top

Java: public String getName() { return name; }
来源：http://ies.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tjn.hywenlv.cn

Ruby: attr_accessor :name
来源：http://jwu.tanke756.top

C#:   public string Name { get; set; }
来源：http://juz.havefunace.top

[G12] 对象转字符串
来源：http://hoo.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://nkw.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wxb.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://yqc.fktsv.cn

TS:   toString(): string { return this.name; }
来源：http://usd.bjfxy.top

Java: @Override public String toString() { return name; }
来源：http://zev.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://ngs.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://ozk.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://vdb.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://qgr.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://uob.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://kyq.yangfankeji.com

JS:   u instanceof User
来源：http://iqd.tian-w.cn

TS:   u instanceof User
来源：http://ahm.nwbrower.top

Java: u instanceof User
来源：http://nkg.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qvy.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://ihd.zycfv.cn

C#:   u is User
来源：http://mki.ctjpmb.com

[G14] 数据类 / record
来源：http://sff.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ugs.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://zkk.daria6918.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lbx.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://jym.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://trg.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://qfw.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cog.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://tps.ydzc1.top

[G15] 枚举
来源：http://cki.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://whj.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xpd.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gju.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sea.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://lwp.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gmb.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://dmu.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wkt.tarul.cn

[G16] 对象转数组 / 字典
来源：http://uwg.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vvq.birdmap.top

PHP:  get_object_vars($obj);
来源：http://irz.guowangkeji.top

JS:   Object.entries(obj)
来源：http://xoj.sxryk.cn

TS:   Object.entries(obj)
来源：http://zfr.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://poz.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pys.hfpthk.cn

Ruby: obj.instance_variables
来源：http://zhv.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://bte.haohaochexian.top

================================================================================
来源：http://dmj.hysaishi.cn

H. 异常与错误处理
来源：http://sjc.gotoacloud.top

================================================================================
来源：http://miw.0kj1m.cn

[H01] try / catch 基础
来源：http://lrz.fehbvm.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bov.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rrz.epnwcf.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dmk.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ewd.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://orp.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hwh.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgc.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vzc.tian-w.cn

[H02] finally / ensure 收尾
来源：http://tkg.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kkn.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mrx.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qhv.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tom.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iig.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xbj.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://gdm.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pov.hywenlv.cn

[H03] 主动抛出异常
来源：http://wks.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://qal.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbk.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://cih.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://njq.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bbu.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ssl.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ipc.ivvv.top

C#:   throw new ArgumentException("错误信息");
来源：http://bat.birdmap.top

[H04] 自定义异常类型
来源：http://hlk.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://ttg.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://tul.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://srz.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://ief.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://byr.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wuz.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://pfa.ydzc1.top

C#:   class MyException : Exception {}
来源：http://mgc.sxryk.cn

[H05] 捕获特定类型
来源：http://ifm.0kj1m.cn

Py:   except ValueError as e:
来源：http://qag.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sou.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://lsm.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://wtu.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://dff.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dwo.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://gyk.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cie.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://lrv.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://qai.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://jkx.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://arz.guowangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://ipb.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sxe.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nls.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://tgq.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://ikt.shzxlz.cn

[H07] 断言
来源：http://kfh.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://osg.52xcode.cn

PHP:  assert($x > 0);
来源：http://mln.daria6918.cn

JS:   console.assert(x > 0);
来源：http://qrl.jianghu66.top

TS:   console.assert(x > 0);
来源：http://sip.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://jok.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://caa.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://cbg.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://jem.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://ilm.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://zzh.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fqg.jianghu66.top

JS:   e.message;  e.stack
来源：http://bzx.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oes.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://alb.aizwys.cn

Go:   err.Error()
来源：http://bca.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://idt.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://ceu.yj20258888.top

[H09] 带错误码的异常
来源：http://bjr.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ebj.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pgd.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xml.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://exj.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jcs.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cyq.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://qdv.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ddv.hammf.cn

[H10] 资源自动释放
来源：http://dwx.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lcr.jinqigufen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://owd.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qqn.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zpe.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xcd.yanxiufei.cn

Go:   defer f.Close()
来源：http://ubj.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wel.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gig.gaohongyu789.top

================================================================================
来源：http://wfk.iojbl.cn

I. 正则表达式
来源：http://rmt.yongpay.top

================================================================================
来源：http://ksi.sxryk.cn

[I01] 判断是否匹配
来源：http://xzi.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vqd.redwolf501.top

PHP:  preg_match('/\d+/', $s);
来源：http://dns.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://kpo.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://dso.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ufv.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sjg.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://vok.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eaq.316326.xyz

[I02] 提取所有匹配
来源：http://fmh.xuetiantiany.cn

Py:   re.findall(r"\d+", s)
来源：http://eoy.ydjk.org.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jfz.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qhh.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://bjt.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rnm.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rwt.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://kwu.gogol.net.cn


<!-- 参考信息 -->