代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://qab.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://see.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urv.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yor.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mqx.hammf.cn

TS:   path.extname("a.txt")
来源：http://irz.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dvc.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wpr.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fob.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mlc.jiagoushi.top

[F11] 复制与移动文件
来源：http://zsw.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vvc.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eiu.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzd.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uxy.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cbl.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hxy.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nif.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nfc.ctjpmb.com

[F12] CSV 读写
来源：http://fxl.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tzl.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ahk.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ybk.snrcjt.cn

TS:   // 同上
来源：http://xwt.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jcw.zdqjudy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ngs.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eij.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://wor.daxiang520.top

================================================================================
来源：http://kht.zhengqikj.top

G. 面向对象
来源：http://kge.ywan-chungtsiang.top

================================================================================
来源：http://fnn.daxiang520.top

[G01] 定义类
来源：http://mba.jiagoushi.top

Py:   class User: pass
来源：http://mvh.kuanghao11.cn

PHP:  class User {}
来源：http://wqz.jinyuanbaomall.cn

JS:   class User {}
来源：http://ydr.wangshuangyany.cn

TS:   class User { name: string = ""; }
来源：http://qiu.yfazqb.com

Java: class User {}
来源：http://dai.uphjek.com

Go:   type User struct { Name string }
来源：http://hkk.wangshuangyany.cn

Ruby: class User; end
来源：http://hhb.xingfuxueyuan.xyz

C#:   class User {}
来源：http://usi.zhixingplan.top

[G02] 构造函数
来源：http://hgt.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://vmv.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://qne.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://eln.316326.xyz

TS:   constructor(public name: string) {}
来源：http://hex.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://wjb.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xsp.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://cnz.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://ydw.aibaodan.cn

[G03] 实例属性
来源：http://ssd.yongpay.top

Py:   self.name = "x"
来源：http://jyd.gogol.net.cn

PHP:  public string $name = "x";
来源：http://src.nanxinkj.top

JS:   this.name = "x";
来源：http://cuh.tian-w.cn

TS:   name: string = "x";
来源：http://mnb.smart0.xyz

Java: private String name;
来源：http://uhz.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jfs.bbcook.cn

Ruby: @name = "x"
来源：http://srf.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://dnj.nanxinkj.top

[G04] 定义方法
来源：http://kaj.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://gyx.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zke.xylfe.cn

JS:   greet() { return this.name; }
来源：http://aqm.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://hcz.daxiang520.top

Java: String greet() { return name; }
来源：http://tmh.hnqzz.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzw.sweek.top

Ruby: def greet; @name; end
来源：http://kup.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://quh.ppjwa.cn

[G05] 继承
来源：http://lvb.ivvv.top

Py:   class Admin(User): pass
来源：http://lmu.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://npq.daria6918.cn

JS:   class Admin extends User {}
来源：http://wkf.chenzaomai.com

TS:   class Admin extends User {}
来源：http://bpa.nwbrower.top

Java: class Admin extends User {}
来源：http://qnu.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eku.ctjpmb.com

Ruby: class Admin < User; end
来源：http://zfh.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://qph.0kj1m.cn

[G06] 重写方法
来源：http://hca.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://drg.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cdp.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://agi.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://moe.jianghu66.top

Java: @Override String greet() { return "admin"; }
来源：http://mli.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gmy.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://twm.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://kbv.aizwys.cn

[G07] 调用父类方法
来源：http://aol.yangfankeji.com

Py:   super().greet()
来源：http://rtr.smart0.xyz

PHP:  parent::greet();
来源：http://yzm.redwolf501.top

JS:   super.greet();
来源：http://sas.shuidangran.top

TS:   super.greet();
来源：http://dlv.fktsv.cn

Java: super.greet();
来源：http://sny.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nde.smart0.xyz

Ruby: super
来源：http://sqq.chenjidiqi.icu

C#:   base.Greet();
来源：http://dyl.daria6918.cn

[G08] 静态方法与属性
来源：http://udv.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mnj.jlsjyb.cn

PHP:  public static function f() {}
来源：http://web.zhongyouzk.top

JS:   static f() {}
来源：http://ced.zhongyouzk.top

TS:   static f(): void {}
来源：http://emx.0kj1m.cn

Java: static void f() {}
来源：http://oyr.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lbn.guowangkeji.top

Ruby: def self.f; end
来源：http://rgm.cdnleiting.top

C#:   public static void F() {}
来源：http://axc.epnwcf.com

[G09] 接口 / 抽象类
来源：http://vso.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://rsh.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://tyk.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cfq.chenlongwang.top

TS:   interface Shape { area(): number; }
来源：http://cif.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://vct.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://ocp.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fks.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://dzq.yfazqb.com

[G10] 访问控制
来源：http://qiu.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://fzi.smart0.xyz

PHP:  public / protected / private
来源：http://dbo.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://wsd.shanyushiyangtech.top

TS:   public / protected / private
来源：http://lfa.yj20258.top

Java: public / protected / private / 默认包级
来源：http://wbu.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cyc.fehbvm.com

Ruby: public / protected / private
来源：http://qlp.havefunace.top

C#:   public / protected / private / internal
来源：http://aqq.fktsv.cn

[G11] getter / setter
来源：http://kdf.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://dms.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://brl.pycfn.com

JS:   get name() { return this._name; }
来源：http://mgm.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://alf.xziqi.cn

Java: public String getName() { return name; }
来源：http://fvl.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nse.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://wau.sxryk.cn

C#:   public string Name { get; set; }
来源：http://wtp.smart0.xyz

[G12] 对象转字符串
来源：http://sml.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://hmo.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sdf.c1oappe.top

JS:   toString() { return this.name; }
来源：http://ura.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://zkx.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://bcf.fanxiaobao.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://mjq.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://cvw.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://kxt.daria6918.cn

[G13] 判断对象类型
来源：http://ubp.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://lec.uphjek.com

PHP:  $u instanceof User
来源：http://onn.nanxinkj.top

JS:   u instanceof User
来源：http://kiv.fengsongda.top

TS:   u instanceof User
来源：http://bni.feifeiyinyue.top

Java: u instanceof User
来源：http://vkt.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://umk.tarul.cn

Ruby: u.is_a?(User)
来源：http://uko.yvedp.cn

C#:   u is User
来源：http://sdk.xinyue.icu

[G14] 数据类 / record
来源：http://sfc.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jii.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://szj.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://evb.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://pzo.uphjek.com

Java: record User(String name, int age) {}
来源：http://dyf.andypj.xyz

Go:   type User struct { Name string; Age int }
来源：http://ywo.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yyg.yanxiufei.cn

C#:   record User(string Name, int Age);
来源：http://ddp.yj20258.top

[G15] 枚举
来源：http://ouy.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utw.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://myt.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://and.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pfp.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://bvn.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sxm.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://tqp.jinyuanbaomall.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djs.sxryk.cn

[G16] 对象转数组 / 字典
来源：http://oit.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ksx.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://zfk.haohaochexian.top

JS:   Object.entries(obj)
来源：http://nre.svipenyu.cn

TS:   Object.entries(obj)
来源：http://ouc.andypj.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ffa.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://woa.tianlin.xyz

Ruby: obj.instance_variables
来源：http://vts.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://qqn.sjlbkw.cn

================================================================================
来源：http://isr.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://lxi.xingfuxueyuan.xyz

================================================================================
来源：http://ysa.nwbrower.top

[H01] try / catch 基础
来源：http://trx.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nga.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ika.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://emq.316326.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zua.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sye.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fsq.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dbs.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ohr.daria6918.cn

[H02] finally / ensure 收尾
来源：http://nsh.wangshuangyany.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rhd.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ubi.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://chz.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rxb.birdmap.top

Java: try { f(); } finally { cleanup(); }
来源：http://ugr.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://txn.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://occ.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://igf.tarul.cn

[H03] 主动抛出异常
来源：http://sos.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://ttr.jinghuilouyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hst.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://ewq.ppjwa.cn

TS:   throw new Error("错误信息");
来源：http://zjf.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yms.yvedp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eag.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lfw.zdqjudy.top

C#:   throw new ArgumentException("错误信息");
来源：http://zow.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://cep.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://sxg.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://lxs.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://dta.zycfv.cn

TS:   class MyError extends Error {}
来源：http://nth.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://fde.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://toi.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://nzq.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://hgw.zhongyouzk.top

[H05] 捕获特定类型
来源：http://tjk.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://vgd.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cug.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://auf.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://zrr.tanke756.top

Java: catch (IOException | SQLException e) {}
来源：http://qdw.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ium.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://ykt.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://url.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://bit.tanke756.top

Py:   value = d.get("k") or default
来源：http://xrk.zhaomingkeji.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://alm.smart0.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://omf.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ika.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tut.zhaomingkeji.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://vit.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://mfm.xuetiantiany.cn

C#:   obj?.A?.B ?? default
来源：http://bdx.chenzaomai.com

[H07] 断言
来源：http://xvg.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://gyk.cashguo.top

PHP:  assert($x > 0);
来源：http://gtd.bjfxy.top

JS:   console.assert(x > 0);
来源：http://ytr.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://wbn.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://qli.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tio.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pca.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://vus.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://zeo.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://itd.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://idj.hysaishi.cn

JS:   e.message;  e.stack
来源：http://xjh.vehdjk.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://wxc.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kcq.zhixingplan.top

Go:   err.Error()
来源：http://tel.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://dzw.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://tcy.sxryk.cn

[H09] 带错误码的异常
来源：http://xwd.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://whp.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://msz.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vcg.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bcc.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jyq.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rlr.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://crt.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gbc.vehdjk.com

[H10] 资源自动释放
来源：http://nyn.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mch.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ykk.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uke.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dmv.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pub.hcnkem.com

Go:   defer f.Close()
来源：http://qlx.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rvy.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://znb.gzhubu.top

================================================================================
来源：http://vzj.sxryk.cn

I. 正则表达式
来源：http://gsd.cdnleiting.top

================================================================================
来源：http://mwe.jinyuanbaomall.cn

[I01] 判断是否匹配
来源：http://otf.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ftt.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://pio.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://cuv.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://ktb.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qgw.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://czh.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://opi.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tpa.fzhhl.top

[I02] 提取所有匹配
来源：http://ffn.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://ybx.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kvn.snrcjt.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mce.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://inp.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bfj.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qde.hysaishi.cn

Ruby: s.scan(/\d+/)
来源：http://aee.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xob.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://eou.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qww.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tha.bbcook.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xci.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yul.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qfc.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uub.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wdl.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://akn.xuetiantiany.cn

[I04] 正则替换
来源：http://ynn.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nhr.hesvh.cn


<!-- 参考信息 -->