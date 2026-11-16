代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://fsx.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://wnm.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ekk.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://lyx.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://ceg.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://bja.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xjy.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://brt.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iao.fktsv.cn

TS:   path.extname("a.txt")
来源：http://izu.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pfd.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mik.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nyc.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hun.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://zgw.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kto.sjlbkw.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://osz.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvd.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ode.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cbk.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://avi.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ecz.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xlm.jinqigufen.top

[F12] CSV 读写
来源：http://abs.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wym.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://loa.pengpengdd.cyou

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mqj.hesvh.cn

TS:   // 同上
来源：http://jkv.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://avk.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bhc.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://int.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ooc.fktsv.cn

================================================================================
来源：http://tnp.nanxuanxn.top

G. 面向对象
来源：http://tmc.gogol.net.cn

================================================================================
来源：http://tlc.cucudq.cn

[G01] 定义类
来源：http://jfj.tarul.cn

Py:   class User: pass
来源：http://lyg.jqgufenzy.top

PHP:  class User {}
来源：http://fxq.ivvv.top

JS:   class User {}
来源：http://wfp.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://vpr.zhengqikj.top

Java: class User {}
来源：http://mgg.ctjpmb.com

Go:   type User struct { Name string }
来源：http://dna.fengsongda.top

Ruby: class User; end
来源：http://ekg.dashuyun.cn

C#:   class User {}
来源：http://cmw.meibo888.top

[G02] 构造函数
来源：http://nil.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://vmv.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://dxk.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://gzq.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://bkt.meibo888.top

Java: User(String name) { this.name = name; }
来源：http://fnh.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jxo.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://urr.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://egz.daria6918.cn

[G03] 实例属性
来源：http://kqs.shuidangran.top

Py:   self.name = "x"
来源：http://iya.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://vsk.hammf.cn

JS:   this.name = "x";
来源：http://edu.xinyue.icu

TS:   name: string = "x";
来源：http://ilj.tianlin.xyz

Java: private String name;
来源：http://gyk.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cep.ydzc1.top

Ruby: @name = "x"
来源：http://lfi.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://jwa.ctjpmb.com

[G04] 定义方法
来源：http://fua.meibo888.top

Py:   def greet(self): return self.name
来源：http://esm.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xnh.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://zxi.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://sfl.yuxming.cn

Java: String greet() { return name; }
来源：http://zfn.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sbl.zhengqikj.top

Ruby: def greet; @name; end
来源：http://fut.fktsv.cn

C#:   public string Greet() => Name;
来源：http://znm.andypj.xyz

[G05] 继承
来源：http://nog.chenzaomai.com

Py:   class Admin(User): pass
来源：http://cgv.guannengcc.top

PHP:  class Admin extends User {}
来源：http://lhw.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://lju.yuxming.cn

TS:   class Admin extends User {}
来源：http://yhw.hcnkem.com

Java: class Admin extends User {}
来源：http://nvl.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nct.nanxinkj.top

Ruby: class Admin < User; end
来源：http://fge.chenlongwang.top

C#:   class Admin : User {}
来源：http://bbi.smart0.xyz

[G06] 重写方法
来源：http://hho.sweek.top

Py:   def greet(self): return "admin"
来源：http://sfr.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bre.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://amt.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://iyv.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://ksz.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://evq.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://pjx.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://vxw.pengpengdd.cyou

[G07] 调用父类方法
来源：http://gep.jinqigufen.top

Py:   super().greet()
来源：http://yas.guannengcc.top

PHP:  parent::greet();
来源：http://rya.9152youxi.cn

JS:   super.greet();
来源：http://tof.aibaodan.cn

TS:   super.greet();
来源：http://qfd.vehdjk.com

Java: super.greet();
来源：http://fod.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yoq.hongshengwenyu.top

Ruby: super
来源：http://ttl.aibaodan.cn

C#:   base.Greet();
来源：http://zin.sweek.top

[G08] 静态方法与属性
来源：http://aqh.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fue.ctjpmb.com

PHP:  public static function f() {}
来源：http://snq.quarkkingdee.top

JS:   static f() {}
来源：http://wfa.yfazqb.com

TS:   static f(): void {}
来源：http://juc.zhixingplan.top

Java: static void f() {}
来源：http://grw.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vza.ctjpmb.com

Ruby: def self.f; end
来源：http://xsl.zhengqikj.top

C#:   public static void F() {}
来源：http://alb.bbcook.cn

[G09] 接口 / 抽象类
来源：http://jxw.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://hee.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dtl.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://alh.vqdsnc.cn

TS:   interface Shape { area(): number; }
来源：http://lrb.xinyue.icu

Java: interface Shape { double area(); }
来源：http://rfh.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://ome.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://loe.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://mpp.hammf.cn

[G10] 访问控制
来源：http://ofw.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://sgj.yonumen.top

PHP:  public / protected / private
来源：http://aeh.birdmap.top

JS:   #private 字段；其余公开
来源：http://hfd.quarkkingdee.top

TS:   public / protected / private
来源：http://jxe.nanxinkj.top

Java: public / protected / private / 默认包级
来源：http://dda.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oqe.hnqzz.top

Ruby: public / protected / private
来源：http://aje.52xcode.cn

C#:   public / protected / private / internal
来源：http://dwo.chenjidiqi.icu

[G11] getter / setter
来源：http://sjb.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://hni.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://knr.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://sdv.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://mdc.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://kcb.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fah.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://tkm.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://hhl.kuanghao11.cn

[G12] 对象转字符串
来源：http://ift.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://dhx.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qhq.xinyue.icu

JS:   toString() { return this.name; }
来源：http://cjh.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://qpj.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://nzq.0kj1m.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ohj.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://wjl.zhixingplan.top

C#:   public override string ToString() => Name;
来源：http://enb.shuidangran.top

[G13] 判断对象类型
来源：http://trm.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://qfl.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://lij.aibaodan.cn

JS:   u instanceof User
来源：http://pts.shanyushiyangtech.top

TS:   u instanceof User
来源：http://dgq.snrcjt.cn

Java: u instanceof User
来源：http://hcl.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jta.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://lnv.sufxvd.cn

C#:   u is User
来源：http://edv.kuanghao11.cn

[G14] 数据类 / record
来源：http://pni.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lvo.pycfn.com

PHP:  // 用 readonly 属性模拟
来源：http://gwc.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://oum.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://jjz.ydzc1.top

Java: record User(String name, int age) {}
来源：http://ivu.yuxming.cn

Go:   type User struct { Name string; Age int }
来源：http://xtg.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jts.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://uqg.daxiang520.top

[G15] 枚举
来源：http://pki.ydjk.org.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://skr.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tgh.andypj.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wmn.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://idm.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://qwk.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayv.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://dhm.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://chp.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://wjq.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://djo.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://jgq.birdmap.top

JS:   Object.entries(obj)
来源：http://ljn.yuanzhike.top

TS:   Object.entries(obj)
来源：http://sxy.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kow.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://bde.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://ztf.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://drc.yonumen.top

================================================================================
来源：http://kar.cdnleiting.top

H. 异常与错误处理
来源：http://pyc.yueranfly.top

================================================================================
来源：http://xle.52xcode.cn

[H01] try / catch 基础
来源：http://sdk.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zrk.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://axn.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jtl.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bhc.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://owf.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bud.nwbrower.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yhv.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jmu.yj20258888.top

[H02] finally / ensure 收尾
来源：http://hgt.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://num.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnt.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ati.ybcxt.top

TS:   try { f(); } finally { cleanup(); }
来源：http://boz.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bya.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gem.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jsv.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oju.gogol.net.cn

[H03] 主动抛出异常
来源：http://roe.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://uvl.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qhs.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://qgc.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://xeo.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wgp.yj20258.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mtx.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hlm.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://zlr.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://qod.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://wtw.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vdo.yfazqb.com

JS:   class MyError extends Error {}
来源：http://zxx.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://asm.bbcook.cn

Java: class MyException extends RuntimeException {}
来源：http://dcz.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zlk.xuanzx.com

Ruby: class MyError < StandardError; end
来源：http://lcb.smart0.xyz

C#:   class MyException : Exception {}
来源：http://tdo.zhoulong.xyz

[H05] 捕获特定类型
来源：http://rvk.zycfv.cn

Py:   except ValueError as e:
来源：http://cee.vqdsnc.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://chx.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://hpi.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://vpi.andypj.xyz

Java: catch (IOException | SQLException e) {}
来源：http://ith.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tgc.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://drr.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nrh.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://wla.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://rgc.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fim.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://rct.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yso.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dlt.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://pkc.daxiang520.top

Ruby: d&.dig(:a, :b)
来源：http://zqe.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://gyl.sweek.top

[H07] 断言
来源：http://yzh.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://tsf.jyoumei.cn

PHP:  assert($x > 0);
来源：http://mqu.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://eha.tanke756.top

TS:   console.assert(x > 0);
来源：http://xvu.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://tzh.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knr.nanxuanxn.top

Ruby: raise "必须为正" unless x > 0
来源：http://kmf.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://vfc.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://zms.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ipe.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mjz.ydzc1.top

JS:   e.message;  e.stack
来源：http://vcm.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jdu.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jtf.sweek.top

Go:   err.Error()
来源：http://glq.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://nyy.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://mvr.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://str.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iuu.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wgf.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jzp.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://opd.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ckb.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ogq.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ouh.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ppj.jiagoushi.top

[H10] 资源自动释放
来源：http://nys.shanyushiyangtech.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hkj.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wou.chenlongwang.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vqt.andypj.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tuy.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hbn.aizwys.cn

Go:   defer f.Close()
来源：http://zmm.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nde.andypj.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xsp.c1oappe.top

================================================================================
来源：http://qzz.tian-w.cn

I. 正则表达式
来源：http://zru.jinyuanbaomall.cn

================================================================================
来源：http://ukx.yfazqb.com

[I01] 判断是否匹配
来源：http://qkq.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ikx.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://azh.yvedp.cn

JS:   /\d+/.test(s)
来源：http://nsv.xinyue.icu

TS:   /\d+/.test(s)
来源：http://rlc.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://epw.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://evr.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://vnq.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tbg.c1oappe.top

[I02] 提取所有匹配
来源：http://miy.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://zga.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://liy.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://flg.yongpay.top

TS:   s.match(/\d+/g)
来源：http://nhq.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cei.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://czj.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://rvx.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qjo.gaohongyu789.top

[I03] 提取捕获分组
来源：http://iym.bjfxy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gaj.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jzi.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://llx.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tmo.chenjidiqi.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ugq.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uga.hesvh.cn


<!-- 参考信息 -->