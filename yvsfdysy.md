代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://dzo.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kuz.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fwh.ybcxt.top

Ruby: File.size("a.txt")
来源：http://dyf.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://aiv.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://hge.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cjc.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://spv.ybcxt.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pfb.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://iio.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cba.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hbu.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ogh.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dfa.ctjpmb.com

[F11] 复制与移动文件
来源：http://lka.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ipn.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ans.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cof.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tah.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wfs.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://msb.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zgj.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zsp.epnwcf.com

[F12] CSV 读写
来源：http://tjx.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzc.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tvi.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tvu.meibo888.top

TS:   // 同上
来源：http://bcg.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nme.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nbj.yuanzhike.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://okp.hnxiangtu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pjm.chenzaomai.com

================================================================================
来源：http://ojh.zhoulong.xyz

G. 面向对象
来源：http://bnh.redwolf501.top

================================================================================
来源：http://ehn.sjlbkw.cn

[G01] 定义类
来源：http://ldv.sjlbkw.cn

Py:   class User: pass
来源：http://gfl.jyoumei.cn

PHP:  class User {}
来源：http://bhn.shanyushiyangtech.top

JS:   class User {}
来源：http://gbb.sweek.top

TS:   class User { name: string = ""; }
来源：http://hvk.sysykeji.top

Java: class User {}
来源：http://ppf.iojbl.cn

Go:   type User struct { Name string }
来源：http://kgh.shanyushiyangtech.top

Ruby: class User; end
来源：http://mff.ivvv.top

C#:   class User {}
来源：http://yro.vqdsnc.cn

[G02] 构造函数
来源：http://iev.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://hld.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://adg.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://nmw.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://rfc.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://cjs.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iwl.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://rnm.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://sly.hysaishi.cn

[G03] 实例属性
来源：http://zeg.yuxming.cn

Py:   self.name = "x"
来源：http://gei.shuidangran.top

PHP:  public string $name = "x";
来源：http://yru.ywan-chungtsiang.top

JS:   this.name = "x";
来源：http://loo.hesvh.cn

TS:   name: string = "x";
来源：http://xyk.jinqigfzy.top

Java: private String name;
来源：http://joq.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://aub.jinqigfzy.top

Ruby: @name = "x"
来源：http://ucs.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://vim.meibo888.top

[G04] 定义方法
来源：http://yda.zhaomingkeji.xyz

Py:   def greet(self): return self.name
来源：http://zel.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ggr.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://qxz.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://loo.uphjek.com

Java: String greet() { return name; }
来源：http://pvg.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://upk.guannengcc.top

Ruby: def greet; @name; end
来源：http://gpd.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://bvg.jinqigufen.top

[G05] 继承
来源：http://xsv.nanxinkj.top

Py:   class Admin(User): pass
来源：http://lhe.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://kmt.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://wws.yj202588.top

TS:   class Admin extends User {}
来源：http://hog.vqdsnc.cn

Java: class Admin extends User {}
来源：http://fyx.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qrc.xingfuxueyuan.xyz

Ruby: class Admin < User; end
来源：http://tlk.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://ntd.sysykeji.top

[G06] 重写方法
来源：http://fmu.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://orj.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fsw.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://ogm.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://uun.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://jam.hnqzz.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hwu.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://wyd.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://elf.haohaochexian.top

[G07] 调用父类方法
来源：http://dzc.guannengcc.top

Py:   super().greet()
来源：http://bih.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://tom.gotoacloud.top

JS:   super.greet();
来源：http://hjs.ctjpmb.com

TS:   super.greet();
来源：http://jqn.jinqigufen.top

Java: super.greet();
来源：http://kzo.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ntc.sweek.top

Ruby: super
来源：http://rhx.shanyushiyangtech.top

C#:   base.Greet();
来源：http://ajl.epnwcf.com

[G08] 静态方法与属性
来源：http://npo.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qbm.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://tlg.yj202588.top

JS:   static f() {}
来源：http://rzy.dianchejie.cn

TS:   static f(): void {}
来源：http://sms.zdbjq.cn

Java: static void f() {}
来源：http://abv.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qxx.gzhubu.top

Ruby: def self.f; end
来源：http://ctz.kuanghao11.cn

C#:   public static void F() {}
来源：http://qfa.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://edn.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://hks.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://uuu.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uxh.nanxuanxn.top

TS:   interface Shape { area(): number; }
来源：http://xwm.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://ssy.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://djd.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hzy.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://ved.zhengqikj.top

[G10] 访问控制
来源：http://lbu.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://yve.jinqigufen.top

PHP:  public / protected / private
来源：http://mci.hcnkem.com

JS:   #private 字段；其余公开
来源：http://wtl.yuanzhike.top

TS:   public / protected / private
来源：http://yxd.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://aqj.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xnq.chenjidiqi.icu

Ruby: public / protected / private
来源：http://gjr.xinyue.icu

C#:   public / protected / private / internal
来源：http://hwl.cucudq.cn

[G11] getter / setter
来源：http://nof.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://ohv.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vfx.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://cfa.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://abo.pycfn.com

Java: public String getName() { return name; }
来源：http://lzv.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dxx.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://axy.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://tmk.fktsv.cn

[G12] 对象转字符串
来源：http://rpj.cheryme.top

Py:   def __str__(self): return self.name
来源：http://lnt.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qqu.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://eyx.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://vwv.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://ace.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://job.sweek.top

Ruby: def to_s; @name; end
来源：http://onb.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://fsn.vehdjk.com

[G13] 判断对象类型
来源：http://elw.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://fba.c1oappe.top

PHP:  $u instanceof User
来源：http://gro.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://alq.fanxiaobao.xyz

TS:   u instanceof User
来源：http://bma.chenzaomai.com

Java: u instanceof User
来源：http://cwi.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://rhz.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://kzw.daria6918.cn

C#:   u is User
来源：http://vel.xylfe.cn

[G14] 数据类 / record
来源：http://ghu.cashguo.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uqk.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://kxw.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://psr.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://nka.yj20258888.top

Java: record User(String name, int age) {}
来源：http://bux.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://vot.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://skk.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://lqs.bbcook.cn

[G15] 枚举
来源：http://ikw.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://los.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xcv.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kmr.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://djy.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://ikx.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jbs.yvedp.cn

Ruby: Color = %i[red green].freeze
来源：http://mxz.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kao.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://cni.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fla.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://aem.chenlongwang.top

JS:   Object.entries(obj)
来源：http://uvl.hesvh.cn

TS:   Object.entries(obj)
来源：http://yoi.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qtc.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xiy.cqqwz.cn

Ruby: obj.instance_variables
来源：http://smi.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://mnp.feifeiyinyue.top

================================================================================
来源：http://lgn.gaohongyu789.top

H. 异常与错误处理
来源：http://ioa.zhongyouzk.top

================================================================================
来源：http://gof.jinqigfzy.top

[H01] try / catch 基础
来源：http://ioo.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kwa.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yok.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dii.tanke756.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nmj.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lyo.fanxiaobao.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fak.iojbl.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kdy.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://btw.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://keb.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://jja.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://did.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://iwp.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ooi.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cdp.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://thg.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mna.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gdc.dashuyun.cn

[H03] 主动抛出异常
来源：http://lsu.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://vqr.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zfg.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://jow.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://skm.haohaochexian.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://khq.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sih.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hok.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://vos.yuxming.cn

[H04] 自定义异常类型
来源：http://ozj.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://nxc.jianghu66.top

PHP:  class MyError extends RuntimeException {}
来源：http://wkd.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://rkb.jlsjyb.cn

TS:   class MyError extends Error {}
来源：http://ozf.yuanzhike.top

Java: class MyException extends RuntimeException {}
来源：http://ozc.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zrg.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://orl.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://jeh.aibaodan.cn

[H05] 捕获特定类型
来源：http://akf.tianlin.xyz

Py:   except ValueError as e:
来源：http://jsi.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ewu.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://qsy.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://xsq.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://lzp.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nqb.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://kij.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rrm.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://wvp.vehdjk.com

Py:   value = d.get("k") or default
来源：http://yhv.hammf.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yei.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://dho.feifeiyinyue.top

TS:   obj?.a?.b;  d ?? default
来源：http://ztm.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ryo.guowangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://exe.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://qpo.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://zfr.hywenlv.cn

[H07] 断言
来源：http://kih.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://gkl.cqqwz.cn

PHP:  assert($x > 0);
来源：http://dmo.cheryme.top

JS:   console.assert(x > 0);
来源：http://vkt.meibo888.top

TS:   console.assert(x > 0);
来源：http://kka.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://qng.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ebe.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pni.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://xsq.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://jxx.yonumen.top

Py:   str(e);  traceback.format_exc()
来源：http://hua.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rlf.yangfankeji.com

JS:   e.message;  e.stack
来源：http://twn.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zik.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kxr.xylfe.cn

Go:   err.Error()
来源：http://svn.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://ohh.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://usg.yvedp.cn

[H09] 带错误码的异常
来源：http://ngw.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://snt.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lri.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lsu.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yrs.316326.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aog.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ohe.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://ytv.gogol.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://giz.aizwys.cn

[H10] 资源自动释放
来源：http://lej.zhaomingkeji.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://evu.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cmd.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kzz.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gmf.wangdashe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yir.hnxiangtu.top

Go:   defer f.Close()
来源：http://afh.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mas.zhixingplan.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ybl.cucudq.cn

================================================================================
来源：http://ogx.tanke756.top

I. 正则表达式
来源：http://ery.dianchejie.cn

================================================================================
来源：http://toy.guannengcc.top

[I01] 判断是否匹配
来源：http://xqp.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jut.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://hgm.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://pgz.shanyushiyangkeji.top

TS:   /\d+/.test(s)
来源：http://pza.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xcs.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eac.sweek.top

Ruby: s.match?(/\d+/)
来源：http://xix.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zst.zhengqikj.top

[I02] 提取所有匹配
来源：http://bwy.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://bdm.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hhw.yangfankeji.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pmk.yonumen.top

TS:   s.match(/\d+/g)
来源：http://gbr.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nnz.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qly.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://ewb.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qtv.yanxiufei.cn

[I03] 提取捕获分组
来源：http://wud.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xve.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ued.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ghg.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://axg.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ebw.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nco.shanyushiyangtech.top


<!-- 参考信息 -->