代发 wailian999

[F09] 获取文件大小
来源：http://nxe.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://htr.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://set.dianchejie.cn

JS:   fs.statSync("a.txt").size
来源：http://dvx.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://jwo.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://htx.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mmr.wangdashe.top

Ruby: File.size("a.txt")
来源：http://ewh.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://ole.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://jho.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://waf.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://csa.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fuc.guannengcc.top

TS:   path.extname("a.txt")
来源：http://zth.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://twv.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ikc.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://drh.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hly.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://izd.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uca.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mif.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgd.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iei.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eau.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jbb.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sbv.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oqz.guowangkeji.top

[F12] CSV 读写
来源：http://opv.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nyh.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uxs.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pdy.daria6918.cn

TS:   // 同上
来源：http://uul.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qgl.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mby.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://boq.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hvc.shangyingyoupin.top

================================================================================
来源：http://wxv.fzhhl.top

G. 面向对象
来源：http://ywg.snrcjt.cn

================================================================================
来源：http://kky.vqdsnc.cn

[G01] 定义类
来源：http://ugf.316326.xyz

Py:   class User: pass
来源：http://waq.tianlin.xyz

PHP:  class User {}
来源：http://iie.uphjek.com

JS:   class User {}
来源：http://kgx.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://utn.yuanzhike.top

Java: class User {}
来源：http://zmh.haohaochexian.top

Go:   type User struct { Name string }
来源：http://diy.nanxuanxn.top

Ruby: class User; end
来源：http://npq.mhx1999.top

C#:   class User {}
来源：http://lfo.sxryk.cn

[G02] 构造函数
来源：http://xkb.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://tkr.snrcjt.cn

PHP:  public function __construct(public string $name) {}
来源：http://daz.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://xpe.birdmap.top

TS:   constructor(public name: string) {}
来源：http://qom.sysykeji.top

Java: User(String name) { this.name = name; }
来源：http://pfg.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://poy.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://kcv.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://iql.birdmap.top

[G03] 实例属性
来源：http://lgc.fengsongda.top

Py:   self.name = "x"
来源：http://luh.aizwys.cn

PHP:  public string $name = "x";
来源：http://brz.jqgufenzy.top

JS:   this.name = "x";
来源：http://ysd.xziqi.cn

TS:   name: string = "x";
来源：http://phk.sweek.top

Java: private String name;
来源：http://wrw.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yor.ppjwa.cn

Ruby: @name = "x"
来源：http://rrl.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://xex.hesvh.cn

[G04] 定义方法
来源：http://crd.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://vsr.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kga.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://ddr.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://awv.dianchejie.cn

Java: String greet() { return name; }
来源：http://min.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cos.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://jkg.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://gef.gogol.net.cn

[G05] 继承
来源：http://njd.pycfn.com

Py:   class Admin(User): pass
来源：http://vmz.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://atm.sxryk.cn

JS:   class Admin extends User {}
来源：http://idh.aizwys.cn

TS:   class Admin extends User {}
来源：http://vuu.tianlin.xyz

Java: class Admin extends User {}
来源：http://zgx.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ctj.tianlin.xyz

Ruby: class Admin < User; end
来源：http://mdg.redwolf501.top

C#:   class Admin : User {}
来源：http://sev.pengpengdd.cyou

[G06] 重写方法
来源：http://bav.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://hya.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yqx.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://aic.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://wih.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://fbs.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tmx.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://ibr.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://wcr.havefunace.top

[G07] 调用父类方法
来源：http://jbq.hesvh.cn

Py:   super().greet()
来源：http://yxk.yongpay.top

PHP:  parent::greet();
来源：http://qrt.52xcode.cn

JS:   super.greet();
来源：http://tbo.guannengcc.top

TS:   super.greet();
来源：http://dvr.jqgfzy.top

Java: super.greet();
来源：http://ltm.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ooy.fktsv.cn

Ruby: super
来源：http://ztx.yj20258888.top

C#:   base.Greet();
来源：http://kis.dashuyun.cn

[G08] 静态方法与属性
来源：http://evi.yj20258888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ctl.quarkkingdee.top

PHP:  public static function f() {}
来源：http://bzk.shanyushiyangtech.top

JS:   static f() {}
来源：http://whe.bbcook.cn

TS:   static f(): void {}
来源：http://tze.shanyushiyangtech.top

Java: static void f() {}
来源：http://tic.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ltw.cucudq.cn

Ruby: def self.f; end
来源：http://sja.ctjpmb.com

C#:   public static void F() {}
来源：http://kna.nwbrower.top

[G09] 接口 / 抽象类
来源：http://pvf.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://njy.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gch.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://vzk.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://snx.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://jxw.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://bos.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fag.yangfankeji.com

C#:   interface IShape { double Area(); }
来源：http://qhq.gogol.net.cn

[G10] 访问控制
来源：http://exo.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://ila.0kj1m.cn

PHP:  public / protected / private
来源：http://pax.ybcxt.top

JS:   #private 字段；其余公开
来源：http://bim.jinqigfzy.top

TS:   public / protected / private
来源：http://xkn.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://vka.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://auy.ydjk.org.cn

Ruby: public / protected / private
来源：http://lmo.fktsv.cn

C#:   public / protected / private / internal
来源：http://mym.gotoacloud.top

[G11] getter / setter
来源：http://ajz.smart0.xyz

Py:   @property 与 @x.setter
来源：http://skh.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ikw.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://irw.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://ajl.jinqigufen.top

Java: public String getName() { return name; }
来源：http://cdc.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bqq.ydzc1.top

Ruby: attr_accessor :name
来源：http://qyf.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://iva.iojbl.cn

[G12] 对象转字符串
来源：http://jrj.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://kzm.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tlg.epnwcf.com

JS:   toString() { return this.name; }
来源：http://zkz.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://exb.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://xqt.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://qpb.sweek.top

Ruby: def to_s; @name; end
来源：http://wen.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://dvu.yuxming.cn

[G13] 判断对象类型
来源：http://yvk.yonumen.top

Py:   isinstance(u, User)
来源：http://dpf.vqdsnc.cn

PHP:  $u instanceof User
来源：http://xpt.yonumen.top

JS:   u instanceof User
来源：http://tsd.yanxiufei.cn

TS:   u instanceof User
来源：http://kwh.guowangkeji.top

Java: u instanceof User
来源：http://ehf.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pyz.yonumen.top

Ruby: u.is_a?(User)
来源：http://hal.c1oappe.top

C#:   u is User
来源：http://qha.nanxuanxn.top

[G14] 数据类 / record
来源：http://zti.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uuk.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://mni.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://syu.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://klt.daxiang520.top

Java: record User(String name, int age) {}
来源：http://tvf.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://kqg.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bkr.yongpay.top

C#:   record User(string Name, int Age);
来源：http://eeg.jinghuilouyu.cn

[G15] 枚举
来源：http://bwf.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ojo.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mmp.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ulz.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pga.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://vzr.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wbo.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://ucb.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gai.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://vdk.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sev.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://bac.jinqigufen.top

JS:   Object.entries(obj)
来源：http://lbr.gotoacloud.top

TS:   Object.entries(obj)
来源：http://akl.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xtp.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://xrg.fengsongda.top

Ruby: obj.instance_variables
来源：http://aum.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://csu.jianghu66.top

================================================================================
来源：http://ejo.hongshengwenyu.top

H. 异常与错误处理
来源：http://dur.jinqigfzy.top

================================================================================
来源：http://bls.9152youxi.cn

[H01] try / catch 基础
来源：http://idy.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://duz.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rjs.uphjek.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mga.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bis.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kjm.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fdu.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qpm.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uin.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://zld.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://csj.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kel.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kls.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ioh.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wwf.zhengqikj.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lyu.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://euv.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bax.cheryme.top

[H03] 主动抛出异常
来源：http://lnd.smart0.xyz

Py:   raise ValueError("错误信息")
来源：http://nun.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ihf.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://orc.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://dtc.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tyt.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ckr.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://oaf.zhongyouzk.top

C#:   throw new ArgumentException("错误信息");
来源：http://mtb.ydjk.org.cn

[H04] 自定义异常类型
来源：http://pdj.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://jez.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://auw.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://dpv.aibaodan.cn

TS:   class MyError extends Error {}
来源：http://xsh.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://fex.kuanghao11.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dqm.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://glf.bjfxy.top

C#:   class MyException : Exception {}
来源：http://xyy.zdbjq.cn

[H05] 捕获特定类型
来源：http://juy.havefunace.top

Py:   except ValueError as e:
来源：http://qfu.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yxb.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://szf.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://mmg.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://isq.cqqwz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqv.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://hts.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qto.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://gql.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://dev.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://rgn.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://nrr.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://fnm.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wsp.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wrh.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://prj.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://acq.jianghu66.top

[H07] 断言
来源：http://hgt.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://tqv.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://zrc.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://msx.0kj1m.cn

TS:   console.assert(x > 0);
来源：http://hbj.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://swz.zhoulong.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://phi.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lbo.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://ssa.sjlbkw.cn

[H08] 获取错误信息与堆栈
来源：http://rxx.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://ucb.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fql.hfpthk.cn

JS:   e.message;  e.stack
来源：http://naq.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jwf.daxiang520.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lbo.zhiwuduotai.top

Go:   err.Error()
来源：http://zlb.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://bmd.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://yxn.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://ugg.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dkp.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufc.tian-w.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vsb.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sos.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mxh.jiagoushi.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cdi.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://slb.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://cpl.hesvh.cn

[H10] 资源自动释放
来源：http://bbc.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oud.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://epe.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ddx.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tta.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pfh.hcnkem.com

Go:   defer f.Close()
来源：http://xnu.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uvg.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gst.ywan-chungtsiang.top

================================================================================
来源：http://wrk.cashguo.top

I. 正则表达式
来源：http://nti.vqdsnc.cn

================================================================================
来源：http://ahs.zhongyouzk.top

[I01] 判断是否匹配
来源：http://usa.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qct.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://oys.meibo888.top

JS:   /\d+/.test(s)
来源：http://sif.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://iim.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zoc.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xvn.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://vjn.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://opm.hammf.cn

[I02] 提取所有匹配
来源：http://mul.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://cqr.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pdd.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mse.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://rhm.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kkh.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://obk.chenzaomai.com

Ruby: s.scan(/\d+/)
来源：http://qbn.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tec.andypj.xyz

[I03] 提取捕获分组
来源：http://kjo.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cit.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oqp.yueranfly.top


<!-- 参考信息 -->