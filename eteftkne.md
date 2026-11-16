代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xsx.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uxb.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://lbv.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://kad.nanxinkj.top

[F09] 获取文件大小
来源：http://nbl.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://kms.yvedp.cn

PHP:  filesize("a.txt");
来源：http://bci.smart0.xyz

JS:   fs.statSync("a.txt").size
来源：http://cve.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://vyk.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bxp.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vyw.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://ftb.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://kig.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://xam.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dia.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rff.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfa.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://hoi.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tzr.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rwl.yonumen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://scs.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qra.hesvh.cn

[F11] 复制与移动文件
来源：http://ful.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjo.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fes.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sbd.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ywm.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dzw.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tzt.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tjl.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vog.hnqzz.top

[F12] CSV 读写
来源：http://bot.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qnq.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://djz.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rfx.9152youxi.cn

TS:   // 同上
来源：http://xpi.sufxvd.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ccv.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cma.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rgy.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jut.hcnkem.com

================================================================================
来源：http://twq.ehwqpu.com

G. 面向对象
来源：http://nwm.vqdsnc.cn

================================================================================
来源：http://fcw.ehwqpu.com

[G01] 定义类
来源：http://tia.hcnkem.com

Py:   class User: pass
来源：http://nxc.jyoumei.cn

PHP:  class User {}
来源：http://man.gotoacloud.top

JS:   class User {}
来源：http://wmx.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://atq.yueranfly.top

Java: class User {}
来源：http://ebp.shzxlz.cn

Go:   type User struct { Name string }
来源：http://fde.guannengcc.top

Ruby: class User; end
来源：http://azs.tian-w.cn

C#:   class User {}
来源：http://uun.xziqi.cn

[G02] 构造函数
来源：http://sbx.hywenlv.cn

Py:   def __init__(self, name): self.name = name
来源：http://srm.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://abs.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://nht.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://uum.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://nfy.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vfa.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ctl.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://jag.sysykeji.top

[G03] 实例属性
来源：http://abn.havefunace.top

Py:   self.name = "x"
来源：http://jfj.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://rro.ehwqpu.com

JS:   this.name = "x";
来源：http://szq.316326.xyz

TS:   name: string = "x";
来源：http://cde.uphjek.com

Java: private String name;
来源：http://rlr.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cww.yongpay.top

Ruby: @name = "x"
来源：http://yqt.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://hsu.shanyushiyangkeji.top

[G04] 定义方法
来源：http://vrp.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://dcm.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://txd.pycfn.com

JS:   greet() { return this.name; }
来源：http://cyg.dianchejie.cn

TS:   greet(): string { return this.name; }
来源：http://kyq.hnxiangtu.top

Java: String greet() { return name; }
来源：http://tbo.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://zqb.havefunace.top

Ruby: def greet; @name; end
来源：http://kkw.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://kch.zhengqikj.top

[G05] 继承
来源：http://pjw.c1oappe.top

Py:   class Admin(User): pass
来源：http://hdj.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://ekn.cqqwz.cn

JS:   class Admin extends User {}
来源：http://jje.zhixingplan.top

TS:   class Admin extends User {}
来源：http://bif.ppjwa.cn

Java: class Admin extends User {}
来源：http://ugz.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mdl.svipenyu.cn

Ruby: class Admin < User; end
来源：http://cbz.yongpay.top

C#:   class Admin : User {}
来源：http://ket.chenzaomai.com

[G06] 重写方法
来源：http://sez.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://uqm.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zaj.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://krq.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://htp.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://umn.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sao.wangdashe.top

Ruby: def greet; "admin"; end
来源：http://ijs.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://tvt.xylfe.cn

[G07] 调用父类方法
来源：http://fzf.yvedp.cn

Py:   super().greet()
来源：http://mst.meibo888.top

PHP:  parent::greet();
来源：http://fza.gzhubu.top

JS:   super.greet();
来源：http://lln.havefunace.top

TS:   super.greet();
来源：http://pcm.gotoacloud.top

Java: super.greet();
来源：http://uau.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zgc.xziqi.cn

Ruby: super
来源：http://wqs.daria6918.cn

C#:   base.Greet();
来源：http://djy.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://vmx.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cwp.cheryme.top

PHP:  public static function f() {}
来源：http://wku.ppjwa.cn

JS:   static f() {}
来源：http://vkt.jiagoushi.top

TS:   static f(): void {}
来源：http://sqj.zhijiandao.cn

Java: static void f() {}
来源：http://fyu.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tpy.yj20258.top

Ruby: def self.f; end
来源：http://vvj.cucudq.cn

C#:   public static void F() {}
来源：http://scq.ybcxt.top

[G09] 接口 / 抽象类
来源：http://wjb.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://dkc.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://thd.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qdl.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://qbe.guannengcc.top

Java: interface Shape { double area(); }
来源：http://hvo.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://mso.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lzj.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://dzz.yangfankeji.com

[G10] 访问控制
来源：http://iln.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://ihi.hnxiangtu.top

PHP:  public / protected / private
来源：http://gxp.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://wja.zhijiandao.cn

TS:   public / protected / private
来源：http://bxg.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://tym.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://coa.chenzaomai.com

Ruby: public / protected / private
来源：http://rde.ybcxt.top

C#:   public / protected / private / internal
来源：http://gth.aibaodan.cn

[G11] getter / setter
来源：http://jhp.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://vrl.shangyingyoupin.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ysi.yuxming.cn

JS:   get name() { return this._name; }
来源：http://lts.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://iis.aibaodan.cn

Java: public String getName() { return name; }
来源：http://fdr.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ted.yangfankeji.com

Ruby: attr_accessor :name
来源：http://puc.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://qum.shuidangran.top

[G12] 对象转字符串
来源：http://aup.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://pke.jqgfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vgi.yfazqb.com

JS:   toString() { return this.name; }
来源：http://zuf.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://fzd.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://quo.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hui.xylfe.cn

Ruby: def to_s; @name; end
来源：http://lzf.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://xlr.jyoumei.cn

[G13] 判断对象类型
来源：http://dkv.cheryme.top

Py:   isinstance(u, User)
来源：http://rky.ppjwa.cn

PHP:  $u instanceof User
来源：http://cuo.tian-w.cn

JS:   u instanceof User
来源：http://udk.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://zpu.yongpay.top

Java: u instanceof User
来源：http://lvv.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ach.hesvh.cn

Ruby: u.is_a?(User)
来源：http://rbq.jinghuilouyu.cn

C#:   u is User
来源：http://mgj.havefunace.top

[G14] 数据类 / record
来源：http://ond.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wta.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://zes.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://zae.yuxming.cn

TS:   type User = { name: string; age: number };
来源：http://kmh.52xcode.cn

Java: record User(String name, int age) {}
来源：http://aoi.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://umh.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qpp.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://kax.mhx1999.top

[G15] 枚举
来源：http://tvu.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ezm.chenlongwang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wdo.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wmr.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ckh.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://lsb.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bnv.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://wsh.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://enf.ivvv.top

[G16] 对象转数组 / 字典
来源：http://haq.ywan-chungtsiang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ezs.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://rmf.yuxming.cn

JS:   Object.entries(obj)
来源：http://fmx.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://kvs.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lsp.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ftl.jinqigufen.top

Ruby: obj.instance_variables
来源：http://eic.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://qtl.ivvv.top

================================================================================
来源：http://zca.316326.xyz

H. 异常与错误处理
来源：http://rwu.yj20258.top

================================================================================
来源：http://hbm.vehdjk.com

[H01] try / catch 基础
来源：http://smi.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qfm.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://irq.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pim.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wsv.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jgy.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqq.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sim.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://igp.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://ssz.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://rgs.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rrn.smart0.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://dit.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dgw.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lfi.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hbk.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dwx.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://efo.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://ykw.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://cux.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zqr.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://nvq.yongpay.top

TS:   throw new Error("错误信息");
来源：http://unw.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://odv.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsb.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://twe.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://rei.gogol.net.cn

[H04] 自定义异常类型
来源：http://joz.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://bem.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xcv.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://slc.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://ive.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://ycs.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oub.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://wbc.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://axd.jqgfzy.top

[H05] 捕获特定类型
来源：http://ing.cheryme.top

Py:   except ValueError as e:
来源：http://ndl.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jae.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://xdk.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://ofi.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://qrl.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nsi.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://gwf.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vfr.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://ptc.yongpay.top

Py:   value = d.get("k") or default
来源：http://wpg.hcnkem.com

PHP:  $v = $d["k"] ?? null;
来源：http://eju.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://ema.zdbjq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yff.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oaj.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://six.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://ngi.xinyue.icu

C#:   obj?.A?.B ?? default
来源：http://jry.hysaishi.cn

[H07] 断言
来源：http://gzw.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://ozy.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://scu.birdmap.top

JS:   console.assert(x > 0);
来源：http://fip.fzhhl.top

TS:   console.assert(x > 0);
来源：http://ohw.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://xqk.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uml.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wcy.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://tko.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://ign.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://vxl.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://prl.yonumen.top

JS:   e.message;  e.stack
来源：http://vyp.cucudq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bla.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dfy.zhiwuduotai.top

Go:   err.Error()
来源：http://tac.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://efb.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://hrs.uphjek.com

[H09] 带错误码的异常
来源：http://shh.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aoy.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hpk.vehdjk.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://txu.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xkn.sjlbkw.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oht.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ibh.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tat.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cdh.xuetiantiany.cn

[H10] 资源自动释放
来源：http://med.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eis.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pve.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hqn.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fwk.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sqy.gotoacloud.top

Go:   defer f.Close()
来源：http://kzx.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aqv.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iut.fanxiaobao.xyz

================================================================================
来源：http://why.yanxiufei.cn

I. 正则表达式
来源：http://qkb.snrcjt.cn

================================================================================
来源：http://aty.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://zgh.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zsi.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://qsd.zycfv.cn

JS:   /\d+/.test(s)
来源：http://fnc.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://lqk.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://igb.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djw.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://lvn.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iky.hnxiangtu.top

[I02] 提取所有匹配
来源：http://lcb.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://utq.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yzj.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qcf.wangdashe.top

TS:   s.match(/\d+/g)
来源：http://rgk.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://trv.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://axi.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://say.iojbl.cn


<!-- 参考信息 -->