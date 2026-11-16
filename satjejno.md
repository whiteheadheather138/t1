代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://dkd.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://qsi.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://axs.yj20258888.top

Ruby: File.size("a.txt")
来源：http://kcw.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://lih.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://wnc.zhoulong.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://txr.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ynd.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mik.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://uni.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ulf.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iuo.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://poz.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ylu.tarul.cn

[F11] 复制与移动文件
来源：http://adm.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fhm.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://orm.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpy.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fqj.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ryw.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rqn.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zxk.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://usc.jlsjyb.cn

[F12] CSV 读写
来源：http://dxs.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vyj.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cda.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pst.snrcjt.cn

TS:   // 同上
来源：http://psh.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yec.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sjp.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oia.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zcf.ydzc1.top

================================================================================
来源：http://mmx.jiagoushi.top

G. 面向对象
来源：http://hpq.ydjk.org.cn

================================================================================
来源：http://dvk.hfpthk.cn

[G01] 定义类
来源：http://uyi.fengsongda.top

Py:   class User: pass
来源：http://ias.316326.xyz

PHP:  class User {}
来源：http://yyh.hongshengwenyu.top

JS:   class User {}
来源：http://qiw.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://mtv.yj20258.top

Java: class User {}
来源：http://trb.zhengqikj.top

Go:   type User struct { Name string }
来源：http://mpb.ybcxt.top

Ruby: class User; end
来源：http://mib.zhaomingkeji.xyz

C#:   class User {}
来源：http://pgd.yfazqb.com

[G02] 构造函数
来源：http://bug.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://fzj.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://kzf.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://xzg.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://msy.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://ihn.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://odr.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://qrq.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://was.dianchejie.cn

[G03] 实例属性
来源：http://azb.nwbrower.top

Py:   self.name = "x"
来源：http://yls.yonumen.top

PHP:  public string $name = "x";
来源：http://seq.feifeiyinyue.top

JS:   this.name = "x";
来源：http://jpz.vqdsnc.cn

TS:   name: string = "x";
来源：http://dvi.tarul.cn

Java: private String name;
来源：http://xox.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ein.sysykeji.top

Ruby: @name = "x"
来源：http://dwg.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://ixb.zhijiandao.cn

[G04] 定义方法
来源：http://ggn.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://ttd.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://rkt.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://bdk.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://icq.wangdashe.top

Java: String greet() { return name; }
来源：http://bas.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nzy.jiagoushi.top

Ruby: def greet; @name; end
来源：http://kcp.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://sif.hywenlv.cn

[G05] 继承
来源：http://uxf.ybcxt.top

Py:   class Admin(User): pass
来源：http://cwh.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://oqr.yuxming.cn

JS:   class Admin extends User {}
来源：http://ogc.aibaodan.cn

TS:   class Admin extends User {}
来源：http://aef.vehdjk.com

Java: class Admin extends User {}
来源：http://xjt.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ecy.sufxvd.cn

Ruby: class Admin < User; end
来源：http://plm.andypj.xyz

C#:   class Admin : User {}
来源：http://tsz.hongshengwenyu.top

[G06] 重写方法
来源：http://cve.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://uen.zhaomingkeji.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://kyd.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://fky.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://hwf.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://uvv.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bve.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://cnj.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://fwm.xuanzx.com

[G07] 调用父类方法
来源：http://rnq.xylfe.cn

Py:   super().greet()
来源：http://kuf.mhx1999.top

PHP:  parent::greet();
来源：http://qzm.hesvh.cn

JS:   super.greet();
来源：http://fbc.ppjwa.cn

TS:   super.greet();
来源：http://slk.gzhubu.top

Java: super.greet();
来源：http://pje.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlr.zhoulong.xyz

Ruby: super
来源：http://ofs.gaohongyu789.top

C#:   base.Greet();
来源：http://dco.yangfankeji.com

[G08] 静态方法与属性
来源：http://pwu.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjx.sysykeji.top

PHP:  public static function f() {}
来源：http://dcj.gotoacloud.top

JS:   static f() {}
来源：http://sjv.gogol.net.cn

TS:   static f(): void {}
来源：http://qdg.yongpay.top

Java: static void f() {}
来源：http://pas.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://thp.yj202588.top

Ruby: def self.f; end
来源：http://ucz.ybcxt.top

C#:   public static void F() {}
来源：http://xfl.vehdjk.com

[G09] 接口 / 抽象类
来源：http://puz.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://lit.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tyn.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ufg.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://zcq.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://hws.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://lfy.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jjq.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://gtb.cqqwz.cn

[G10] 访问控制
来源：http://pgw.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://htw.jianghu66.top

PHP:  public / protected / private
来源：http://htd.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://kkc.hesvh.cn

TS:   public / protected / private
来源：http://wak.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://mfa.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kwv.zdbjq.cn

Ruby: public / protected / private
来源：http://kre.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://xce.snrcjt.cn

[G11] getter / setter
来源：http://jvo.xylfe.cn

Py:   @property 与 @x.setter
来源：http://vho.c1oappe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://car.yuxming.cn

JS:   get name() { return this._name; }
来源：http://tbw.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://scq.yuxming.cn

Java: public String getName() { return name; }
来源：http://eer.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://awb.hnxiangtu.top

Ruby: attr_accessor :name
来源：http://hpi.fktsv.cn

C#:   public string Name { get; set; }
来源：http://yxe.wangdashe.top

[G12] 对象转字符串
来源：http://lvc.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://jwq.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wnd.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://tjz.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://olb.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://toy.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://zmc.hnqzz.top

Ruby: def to_s; @name; end
来源：http://jsk.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://fob.ydzc1.top

[G13] 判断对象类型
来源：http://ymh.vehdjk.com

Py:   isinstance(u, User)
来源：http://hlx.hnxiangtu.top

PHP:  $u instanceof User
来源：http://cwz.guowangkeji.top

JS:   u instanceof User
来源：http://kce.316326.xyz

TS:   u instanceof User
来源：http://bka.bjfxy.top

Java: u instanceof User
来源：http://iic.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jom.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://cns.zhijiandao.cn

C#:   u is User
来源：http://cyl.haohaochexian.top

[G14] 数据类 / record
来源：http://max.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://scc.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://ykf.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://cmd.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://fnq.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://pgt.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://zlk.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yuv.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://jac.redwolf501.top

[G15] 枚举
来源：http://bnd.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://glr.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://seo.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://scb.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fnu.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://roq.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pdi.yuxming.cn

Ruby: Color = %i[red green].freeze
来源：http://hrs.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ivr.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://nlf.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://don.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://ikv.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://mfm.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://lpq.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://svp.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kli.jyoumei.cn

Ruby: obj.instance_variables
来源：http://eig.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://lqz.jinqigufen.top

================================================================================
来源：http://lpp.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://fvq.wangshuangyany.cn

================================================================================
来源：http://lfo.hammf.cn

[H01] try / catch 基础
来源：http://mto.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zdx.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xsw.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rbj.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufn.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jjr.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://abv.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yji.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vfe.yfazqb.com

[H02] finally / ensure 收尾
来源：http://gcp.iojbl.cn

Py:   try: f()⏎finally: cleanup()
来源：http://csx.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://bxj.tian-w.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aqf.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rle.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gld.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oyb.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ssr.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://upt.yonumen.top

[H03] 主动抛出异常
来源：http://aqx.zhaomingkeji.xyz

Py:   raise ValueError("错误信息")
来源：http://aeo.jyoumei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://odw.tarul.cn

JS:   throw new Error("错误信息");
来源：http://tcl.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://wap.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://skp.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qul.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ncu.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://cyo.haohaochexian.top

[H04] 自定义异常类型
来源：http://swm.ydjk.org.cn

Py:   class MyError(Exception): pass
来源：http://vpy.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kbb.tarul.cn

JS:   class MyError extends Error {}
来源：http://nuc.yj202588.top

TS:   class MyError extends Error {}
来源：http://skf.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://rqa.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nse.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://kup.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://lmg.bjfxy.top

[H05] 捕获特定类型
来源：http://gct.havefunace.top

Py:   except ValueError as e:
来源：http://xmb.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ael.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://gqa.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://lxz.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://vfi.pengpengdd.cyou

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nvj.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://qje.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eay.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://xud.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://uzx.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://uog.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://ydy.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jyt.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gkc.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ixh.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://nkg.hcnkem.com

C#:   obj?.A?.B ?? default
来源：http://cia.shanyushiyangkeji.top

[H07] 断言
来源：http://klq.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://ist.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://ekn.sysykeji.top

JS:   console.assert(x > 0);
来源：http://suj.yueranfly.top

TS:   console.assert(x > 0);
来源：http://gcz.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://vox.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://twf.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uaz.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://gxr.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://lce.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://tzw.zdqjudy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://prk.ppjwa.cn

JS:   e.message;  e.stack
来源：http://kdg.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zib.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://srb.zhoulong.xyz

Go:   err.Error()
来源：http://iqv.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://cyw.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://pvs.xziqi.cn

[H09] 带错误码的异常
来源：http://wby.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mya.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mcq.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dbg.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ajx.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xak.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vef.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wgh.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hle.smart0.xyz

[H10] 资源自动释放
来源：http://url.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bul.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yqb.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wda.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://get.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rhg.xuetiantiany.cn

Go:   defer f.Close()
来源：http://ezb.yuxming.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ojg.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qln.sweek.top

================================================================================
来源：http://stp.havefunace.top

I. 正则表达式
来源：http://dfk.aibaodan.cn

================================================================================
来源：http://mvb.vqdsnc.cn

[I01] 判断是否匹配
来源：http://fds.jianghu66.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cqb.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oht.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://zww.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://ecu.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ygn.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dab.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://jih.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://evo.sjlbkw.cn

[I02] 提取所有匹配
来源：http://lfn.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://jfk.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ufi.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rdu.hammf.cn

TS:   s.match(/\d+/g)
来源：http://bqc.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nwn.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxd.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://awq.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bzk.gzhubu.top

[I03] 提取捕获分组
来源：http://nci.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wbh.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://exl.vqdsnc.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kcq.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zje.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eqt.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uuw.dianchejie.cn


<!-- 参考信息 -->