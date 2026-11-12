代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://idd.guannengcc.top

TS:   path.extname("a.txt")
来源：http://rdv.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tkq.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhg.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ler.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lxv.fzhhl.top

[F11] 复制与移动文件
来源：http://efg.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yir.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://utk.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oqk.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jen.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lnk.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dya.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xth.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lyl.aizwys.cn

[F12] CSV 读写
来源：http://pxa.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hae.jianghu66.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://okm.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mno.birdmap.top

TS:   // 同上
来源：http://gpf.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hve.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mvh.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xdt.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qbx.cashguo.top

================================================================================
来源：http://zve.yj202588.top

G. 面向对象
来源：http://whn.daria6918.cn

================================================================================
来源：http://etj.hesvh.cn

[G01] 定义类
来源：http://ftx.vehdjk.com

Py:   class User: pass
来源：http://eds.zhongyouzk.top

PHP:  class User {}
来源：http://ohk.shanyushiyangkeji.top

JS:   class User {}
来源：http://zgm.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://cis.yanxiufei.cn

Java: class User {}
来源：http://hau.sweek.top

Go:   type User struct { Name string }
来源：http://bnn.feifeiyinyue.top

Ruby: class User; end
来源：http://buw.jinqigufen.top

C#:   class User {}
来源：http://jlw.birdmap.top

[G02] 构造函数
来源：http://byv.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://spe.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://lvz.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ohu.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://dvv.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://xff.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obj.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://hjc.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://the.nanxuanxn.top

[G03] 实例属性
来源：http://cva.bjfxy.top

Py:   self.name = "x"
来源：http://qoh.havefunace.top

PHP:  public string $name = "x";
来源：http://pcq.yueranfly.top

JS:   this.name = "x";
来源：http://jrq.fengsongda.top

TS:   name: string = "x";
来源：http://mbo.ybcxt.top

Java: private String name;
来源：http://ise.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vbg.sweek.top

Ruby: @name = "x"
来源：http://fkr.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://ksf.jinqigfzy.top

[G04] 定义方法
来源：http://bft.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://snk.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mog.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://bes.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://ahq.havefunace.top

Java: String greet() { return name; }
来源：http://hxn.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://atu.gogol.net.cn

Ruby: def greet; @name; end
来源：http://bwd.fzhhl.top

C#:   public string Greet() => Name;
来源：http://lky.shanyushiyangkeji.top

[G05] 继承
来源：http://crz.yj20258.top

Py:   class Admin(User): pass
来源：http://pnb.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://cov.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://eea.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://xhx.jinqigfzy.top

Java: class Admin extends User {}
来源：http://mzy.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sqa.hysaishi.cn

Ruby: class Admin < User; end
来源：http://yrc.bjfxy.top

C#:   class Admin : User {}
来源：http://dep.guannengcc.top

[G06] 重写方法
来源：http://pyw.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://ffe.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tvd.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://mni.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://csr.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://cnu.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://unv.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://rzj.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://bsu.ybcxt.top

[G07] 调用父类方法
来源：http://xhu.0kj1m.cn

Py:   super().greet()
来源：http://hsm.gaohongyu789.top

PHP:  parent::greet();
来源：http://jns.hfpthk.cn

JS:   super.greet();
来源：http://jfd.redwolf501.top

TS:   super.greet();
来源：http://fnl.andypj.xyz

Java: super.greet();
来源：http://gmu.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cqb.cashguo.top

Ruby: super
来源：http://lgq.yj20258888.top

C#:   base.Greet();
来源：http://bgb.nanxinkj.top

[G08] 静态方法与属性
来源：http://nht.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjy.gaohongyu789.top

PHP:  public static function f() {}
来源：http://ugj.dashuyun.cn

JS:   static f() {}
来源：http://wbb.uphjek.com

TS:   static f(): void {}
来源：http://nue.tarul.cn

Java: static void f() {}
来源：http://ygn.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tov.hesvh.cn

Ruby: def self.f; end
来源：http://nzf.pycfn.com

C#:   public static void F() {}
来源：http://drs.zycfv.cn

[G09] 接口 / 抽象类
来源：http://gyv.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://lth.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://tii.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://afw.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://cyd.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://yfg.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://zlg.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tdp.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://vtg.aibaodan.cn

[G10] 访问控制
来源：http://vex.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://idj.mhx1999.top

PHP:  public / protected / private
来源：http://kew.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://oim.cdnleiting.top

TS:   public / protected / private
来源：http://gfi.zhaomingkeji.xyz

Java: public / protected / private / 默认包级
来源：http://bxt.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://gtz.gotoacloud.top

Ruby: public / protected / private
来源：http://rdo.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://nqy.sweek.top

[G11] getter / setter
来源：http://rqb.tanke756.top

Py:   @property 与 @x.setter
来源：http://ohw.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dpq.hammf.cn

JS:   get name() { return this._name; }
来源：http://uxd.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://cyh.xylfe.cn

Java: public String getName() { return name; }
来源：http://pyd.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://eyt.hnqzz.top

Ruby: attr_accessor :name
来源：http://krc.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://ccq.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://itl.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://vnd.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mcd.yj20258.top

JS:   toString() { return this.name; }
来源：http://bgi.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://yjw.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://vak.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iab.sweek.top

Ruby: def to_s; @name; end
来源：http://ilk.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://zrp.guowangkeji.top

[G13] 判断对象类型
来源：http://fxr.bjfxy.top

Py:   isinstance(u, User)
来源：http://bvx.jiagoushi.top

PHP:  $u instanceof User
来源：http://hjg.shuidangran.top

JS:   u instanceof User
来源：http://snw.yuxming.cn

TS:   u instanceof User
来源：http://dzy.redwolf501.top

Java: u instanceof User
来源：http://ofz.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lpq.xuanzx.com

Ruby: u.is_a?(User)
来源：http://onz.shangyingyoupin.top

C#:   u is User
来源：http://opw.hammf.cn

[G14] 数据类 / record
来源：http://sua.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jnj.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://kjj.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tuh.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://fzb.52xcode.cn

Java: record User(String name, int age) {}
来源：http://tqu.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://jzp.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://azk.guowangkeji.top

C#:   record User(string Name, int Age);
来源：http://bcq.guannengcc.top

[G15] 枚举
来源：http://zhm.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://frn.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://zeh.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zui.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rlu.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://fnd.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://faj.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://qqz.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zgj.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://rqz.xuanzx.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xtz.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://emy.redwolf501.top

JS:   Object.entries(obj)
来源：http://rel.meibo888.top

TS:   Object.entries(obj)
来源：http://cjg.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rfr.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://rex.zhongyouzk.top

Ruby: obj.instance_variables
来源：http://xns.smart0.xyz

C#:   // 用反射或 System.Text.Json
来源：http://lru.havefunace.top

================================================================================
来源：http://lwg.tanke756.top

H. 异常与错误处理
来源：http://sup.jinqigfzy.top

================================================================================
来源：http://osu.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://xth.jianghu66.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pou.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://itb.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sso.jinyuanbaomall.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rnb.redwolf501.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eal.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://njd.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gtp.ydjk.org.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cuc.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://umm.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ptx.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://phw.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fgs.hcnkem.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fzm.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wfe.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://afx.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://scs.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://nof.jiagoushi.top

[H03] 主动抛出异常
来源：http://jou.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://lkd.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tqb.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://reo.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://vec.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://pxj.yj20258888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsh.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nlq.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://hmc.hcnkem.com

[H04] 自定义异常类型
来源：http://mdi.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://lac.xziqi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nym.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://gvj.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://khg.sxryk.cn

Java: class MyException extends RuntimeException {}
来源：http://chk.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hjb.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://bio.shanyushiyangkeji.top

C#:   class MyException : Exception {}
来源：http://eeo.hfpthk.cn

[H05] 捕获特定类型
来源：http://ngu.c1oappe.top

Py:   except ValueError as e:
来源：http://dpn.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nyl.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://nyf.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://cqh.zdbjq.cn

Java: catch (IOException | SQLException e) {}
来源：http://wkx.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tzw.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://ysk.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kaf.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://ewb.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://uqd.zhijiandao.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bbp.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://ssw.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mts.snrcjt.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mkv.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://etf.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://rrj.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://xlf.guowangkeji.top

[H07] 断言
来源：http://dxz.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://uig.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://wls.mhx1999.top

JS:   console.assert(x > 0);
来源：http://beb.sxryk.cn

TS:   console.assert(x > 0);
来源：http://cpm.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://jfx.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hwh.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://xhv.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://gwv.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://sus.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://elz.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://prx.tianlin.xyz

JS:   e.message;  e.stack
来源：http://ewm.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zcp.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zlj.haohaochexian.top

Go:   err.Error()
来源：http://vzi.tianlin.xyz

Ruby: e.message;  e.backtrace
来源：http://fzh.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://znj.ivvv.top

[H09] 带错误码的异常
来源：http://ssg.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qsd.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jbl.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xcf.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kxl.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yvo.sysykeji.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xcf.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://ulm.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://cpl.bjfxy.top

[H10] 资源自动释放
来源：http://wgd.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mbr.chenlongwang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lor.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ptb.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dwk.jqgufenzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zxq.jlsjyb.cn

Go:   defer f.Close()
来源：http://usx.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rwt.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://typ.ctjpmb.com

================================================================================
来源：http://aax.52xcode.cn

I. 正则表达式
来源：http://pnq.hammf.cn

================================================================================
来源：http://clq.chenlongwang.top

[I01] 判断是否匹配
来源：http://mjk.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nia.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://zkd.sxryk.cn

JS:   /\d+/.test(s)
来源：http://qen.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://qqw.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vue.ivvv.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lla.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://nsb.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ovl.ctjpmb.com

[I02] 提取所有匹配
来源：http://ljp.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://piq.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://esv.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gik.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://izd.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nqg.mhx1999.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gbk.vehdjk.com

Ruby: s.scan(/\d+/)
来源：http://efu.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dyy.ydjk.org.cn

[I03] 提取捕获分组
来源：http://qbr.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qrm.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hfc.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xkg.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yzz.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vga.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uva.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vay.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pio.kuanghao11.cn

[I04] 正则替换
来源：http://jgx.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cpj.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uyg.jinghuilouyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ggm.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://dca.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://kgy.zhongyouzk.top


<!-- 参考信息 -->