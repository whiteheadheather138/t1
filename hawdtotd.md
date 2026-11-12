代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hqi.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://tru.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nil.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://faq.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gkq.fktsv.cn

TS:   path.extname("a.txt")
来源：http://fjr.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qpo.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://srw.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnl.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gta.andypj.xyz

[F11] 复制与移动文件
来源：http://nij.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://woj.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fra.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qbs.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mri.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lwl.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cpy.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xqk.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxa.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://xnb.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ckv.quarkkingdee.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://icd.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ixp.chenzaomai.com

TS:   // 同上
来源：http://pam.jqgufenzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fug.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oyv.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vro.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://llk.zhixingplan.top

================================================================================
来源：http://rll.dianchejie.cn

G. 面向对象
来源：http://tuq.quarkkingdee.top

================================================================================
来源：http://mxy.zycfv.cn

[G01] 定义类
来源：http://ieh.vehdjk.com

Py:   class User: pass
来源：http://jla.tanke756.top

PHP:  class User {}
来源：http://wkt.cqqwz.cn

JS:   class User {}
来源：http://mxo.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://zis.kuanghao11.cn

Java: class User {}
来源：http://hcj.yvedp.cn

Go:   type User struct { Name string }
来源：http://euz.jianghu66.top

Ruby: class User; end
来源：http://uff.svipenyu.cn

C#:   class User {}
来源：http://eyj.hongshengwenyu.top

[G02] 构造函数
来源：http://iqm.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://gse.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://fug.wangshuangyany.cn

JS:   constructor(name) { this.name = name; }
来源：http://xga.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://bgr.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://zqt.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mat.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://olo.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://gby.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://jkm.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://pvq.pycfn.com

PHP:  public string $name = "x";
来源：http://crt.jqgufenzy.top

JS:   this.name = "x";
来源：http://rvc.gogol.net.cn

TS:   name: string = "x";
来源：http://xgw.guowangkeji.top

Java: private String name;
来源：http://ssn.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gqz.andypj.xyz

Ruby: @name = "x"
来源：http://dcy.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://nex.zhaomingkeji.xyz

[G04] 定义方法
来源：http://dzw.hesvh.cn

Py:   def greet(self): return self.name
来源：http://svk.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://src.c1oappe.top

JS:   greet() { return this.name; }
来源：http://mzp.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://djg.jianghu66.top

Java: String greet() { return name; }
来源：http://cag.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sbq.c1oappe.top

Ruby: def greet; @name; end
来源：http://wjm.yfazqb.com

C#:   public string Greet() => Name;
来源：http://fst.52xcode.cn

[G05] 继承
来源：http://vgh.vehdjk.com

Py:   class Admin(User): pass
来源：http://efq.xziqi.cn

PHP:  class Admin extends User {}
来源：http://vvh.chenzaomai.com

JS:   class Admin extends User {}
来源：http://gkp.daxiang520.top

TS:   class Admin extends User {}
来源：http://pam.fengsongda.top

Java: class Admin extends User {}
来源：http://tpi.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kav.ydjk.org.cn

Ruby: class Admin < User; end
来源：http://roa.9152youxi.cn

C#:   class Admin : User {}
来源：http://kcv.quarkkingdee.top

[G06] 重写方法
来源：http://lkr.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://ryl.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vjr.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://sed.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://pxy.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://auz.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cww.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://tvx.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://svf.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://qgt.iojbl.cn

Py:   super().greet()
来源：http://yay.shuidangran.top

PHP:  parent::greet();
来源：http://qyj.bjfxy.top

JS:   super.greet();
来源：http://ifb.zhiwuduotai.top

TS:   super.greet();
来源：http://uef.iojbl.cn

Java: super.greet();
来源：http://fia.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wqu.quarkkingdee.top

Ruby: super
来源：http://nwh.tanke756.top

C#:   base.Greet();
来源：http://nbb.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://jxz.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cyd.fengsongda.top

PHP:  public static function f() {}
来源：http://wik.uphjek.com

JS:   static f() {}
来源：http://dpr.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://gxj.haohaochexian.top

Java: static void f() {}
来源：http://vle.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://djk.yj202588.top

Ruby: def self.f; end
来源：http://qlm.yj20258888.top

C#:   public static void F() {}
来源：http://smt.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://dyx.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://qoq.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://ypo.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://fim.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://gfh.tanke756.top

Java: interface Shape { double area(); }
来源：http://vft.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://tkl.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vjs.yongpay.top

C#:   interface IShape { double Area(); }
来源：http://xlc.daxiang520.top

[G10] 访问控制
来源：http://msv.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://teo.gogol.net.cn

PHP:  public / protected / private
来源：http://irv.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://esx.zycfv.cn

TS:   public / protected / private
来源：http://gbv.cashguo.top

Java: public / protected / private / 默认包级
来源：http://wkt.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://msx.hnqzz.top

Ruby: public / protected / private
来源：http://hsp.bjfxy.top

C#:   public / protected / private / internal
来源：http://kdy.shzxlz.cn

[G11] getter / setter
来源：http://oqx.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://zct.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cpi.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://ghf.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://soi.yuanzhike.top

Java: public String getName() { return name; }
来源：http://dtx.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wxg.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://hlg.ydzc1.top

C#:   public string Name { get; set; }
来源：http://dao.xinyue.icu

[G12] 对象转字符串
来源：http://ief.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://rme.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tom.xuanzx.com

JS:   toString() { return this.name; }
来源：http://jxg.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://syr.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://tjs.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://srm.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://jkd.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://eds.tarul.cn

[G13] 判断对象类型
来源：http://rtl.yvedp.cn

Py:   isinstance(u, User)
来源：http://giz.kuanghao11.cn

PHP:  $u instanceof User
来源：http://pgo.hnxiangtu.top

JS:   u instanceof User
来源：http://zxz.redwolf501.top

TS:   u instanceof User
来源：http://wvi.gogol.net.cn

Java: u instanceof User
来源：http://nya.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://yot.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://rwv.shuidangran.top

C#:   u is User
来源：http://enc.gogol.net.cn

[G14] 数据类 / record
来源：http://tfg.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vsq.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://qan.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://szt.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://ekw.shuidangran.top

Java: record User(String name, int age) {}
来源：http://bua.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://iil.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kju.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://yha.snrcjt.cn

[G15] 枚举
来源：http://fir.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yto.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://nuc.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ajc.zhaomingkeji.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hnj.guannengcc.top

Java: enum Color { RED, GREEN }
来源：http://isn.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cbf.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://neg.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ums.sweek.top

[G16] 对象转数组 / 字典
来源：http://ldq.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ctw.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://rxv.jinghuilouyu.cn

JS:   Object.entries(obj)
来源：http://snw.zhixingplan.top

TS:   Object.entries(obj)
来源：http://uiu.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ebr.iojbl.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zae.zycfv.cn

Ruby: obj.instance_variables
来源：http://wid.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://nzf.andypj.xyz

================================================================================
来源：http://faa.fehbvm.com

H. 异常与错误处理
来源：http://rzn.xingfuxueyuan.xyz

================================================================================
来源：http://hyy.yj20258888.top

[H01] try / catch 基础
来源：http://hrf.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vsh.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://skc.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eiv.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wuk.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rzg.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xah.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wwt.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dgq.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://ezu.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://wpq.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://brb.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dzo.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tub.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://now.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oky.aizwys.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rgm.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://axn.chenlongwang.top

[H03] 主动抛出异常
来源：http://qoz.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://pwj.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://syv.havefunace.top

JS:   throw new Error("错误信息");
来源：http://xxc.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://yla.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ppe.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gde.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://djo.yangfankeji.com

C#:   throw new ArgumentException("错误信息");
来源：http://mua.yfazqb.com

[H04] 自定义异常类型
来源：http://kmm.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://ipm.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://qez.nwbrower.top

JS:   class MyError extends Error {}
来源：http://zpd.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://ngp.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://yej.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rfg.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://mks.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://ben.jinqigfzy.top

[H05] 捕获特定类型
来源：http://pwy.yueranfly.top

Py:   except ValueError as e:
来源：http://kol.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xca.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://biw.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://aem.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://aou.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxq.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://gxa.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qvt.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://bvl.mhx1999.top

Py:   value = d.get("k") or default
来源：http://kwv.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fkv.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eps.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://eqr.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tsr.chenjidiqi.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://jwz.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://hhq.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://clh.c1oappe.top

[H07] 断言
来源：http://fxb.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://xgu.nanxinkj.top

PHP:  assert($x > 0);
来源：http://rlj.bjfxy.top

JS:   console.assert(x > 0);
来源：http://jvk.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://irg.ctjpmb.com

Java: assert x > 0 : "必须为正";
来源：http://kqr.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fta.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://shi.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://ash.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://ivw.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://ots.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cdp.gotoacloud.top

JS:   e.message;  e.stack
来源：http://ben.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bng.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pyf.316326.xyz

Go:   err.Error()
来源：http://qlr.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://mui.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://ova.tarul.cn

[H09] 带错误码的异常
来源：http://zmr.gogol.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frs.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://npd.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jwt.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://clu.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rex.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oyw.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://xio.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qnr.tian-w.cn

[H10] 资源自动释放
来源：http://eje.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xjx.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lhi.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ijb.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hex.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bbu.pengpengdd.cyou

Go:   defer f.Close()
来源：http://lml.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://stt.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jkj.pengpengdd.cyou

================================================================================
来源：http://zyy.tianlin.xyz

I. 正则表达式
来源：http://lui.jqgfzy.top

================================================================================
来源：http://cza.fehbvm.com

[I01] 判断是否匹配
来源：http://mzw.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ddf.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tbf.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://qbr.sysykeji.top

TS:   /\d+/.test(s)
来源：http://srx.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ipj.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kog.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://ezh.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qse.havefunace.top

[I02] 提取所有匹配
来源：http://foh.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://vtx.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ndh.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wds.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://poi.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vwo.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lxd.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://gkg.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nac.smart0.xyz

[I03] 提取捕获分组
来源：http://ejh.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://icd.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rfw.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://edh.yuxming.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://upx.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ben.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ueu.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esb.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kol.wangdashe.top

[I04] 正则替换
来源：http://wsw.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dhf.tianlin.xyz


<!-- 参考信息 -->