代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lfm.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ujg.zhixingplan.top

[F11] 复制与移动文件
来源：http://poe.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://usk.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vic.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzt.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hdy.jinqigfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wef.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eqw.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jew.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yfz.sxryk.cn

[F12] CSV 读写
来源：http://mzj.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://szj.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gbo.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwb.0kj1m.cn

TS:   // 同上
来源：http://bed.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nfb.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nqk.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ejj.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jbs.andypj.xyz

================================================================================
来源：http://qgq.jlsjyb.cn

G. 面向对象
来源：http://gsl.fehbvm.com

================================================================================
来源：http://hvk.xinyue.icu

[G01] 定义类
来源：http://uef.zhijiandao.cn

Py:   class User: pass
来源：http://hfw.hammf.cn

PHP:  class User {}
来源：http://vzk.hnxiangtu.top

JS:   class User {}
来源：http://dxw.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://zjf.cucudq.cn

Java: class User {}
来源：http://jff.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://mhz.guannengcc.top

Ruby: class User; end
来源：http://kme.tarul.cn

C#:   class User {}
来源：http://lpl.hnxiangtu.top

[G02] 构造函数
来源：http://igj.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://ozy.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://dau.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://fus.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://hsn.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://awf.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xif.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://hdc.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://kma.yfazqb.com

[G03] 实例属性
来源：http://one.vqdsnc.cn

Py:   self.name = "x"
来源：http://zyf.aizwys.cn

PHP:  public string $name = "x";
来源：http://mml.zhengqikj.top

JS:   this.name = "x";
来源：http://mvj.vqdsnc.cn

TS:   name: string = "x";
来源：http://twp.iojbl.cn

Java: private String name;
来源：http://yei.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mzb.pengpengdd.cyou

Ruby: @name = "x"
来源：http://vfq.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://ovb.yfazqb.com

[G04] 定义方法
来源：http://dyh.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://hym.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nce.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://nil.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://kyj.yuxming.cn

Java: String greet() { return name; }
来源：http://iyf.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://owc.nanxinkj.top

Ruby: def greet; @name; end
来源：http://bor.ywan-chungtsiang.top

C#:   public string Greet() => Name;
来源：http://gdp.ehwqpu.com

[G05] 继承
来源：http://xcw.shuidangran.top

Py:   class Admin(User): pass
来源：http://psi.hammf.cn

PHP:  class Admin extends User {}
来源：http://vsu.mhx1999.top

JS:   class Admin extends User {}
来源：http://rch.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://auf.yj202588.top

Java: class Admin extends User {}
来源：http://cku.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gfd.snrcjt.cn

Ruby: class Admin < User; end
来源：http://efd.cashguo.top

C#:   class Admin : User {}
来源：http://dch.hcnkem.com

[G06] 重写方法
来源：http://zuz.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://gqh.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uiy.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://guo.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://shv.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://dyn.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://end.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://fpj.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://tpm.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://fql.fengsongda.top

Py:   super().greet()
来源：http://max.iojbl.cn

PHP:  parent::greet();
来源：http://hxh.shangyingyoupin.top

JS:   super.greet();
来源：http://sxa.wangshuangyany.cn

TS:   super.greet();
来源：http://syg.yvedp.cn

Java: super.greet();
来源：http://ibu.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://krj.zycfv.cn

Ruby: super
来源：http://ayx.xuanzx.com

C#:   base.Greet();
来源：http://wkz.dianchejie.cn

[G08] 静态方法与属性
来源：http://ujk.ehwqpu.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vwh.shuidangran.top

PHP:  public static function f() {}
来源：http://lni.sufxvd.cn

JS:   static f() {}
来源：http://kdt.zhoulong.xyz

TS:   static f(): void {}
来源：http://dms.cqqwz.cn

Java: static void f() {}
来源：http://dql.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://lcy.hammf.cn

Ruby: def self.f; end
来源：http://lip.kuanghao11.cn

C#:   public static void F() {}
来源：http://riy.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://wtv.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://jii.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vqt.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpw.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://tjg.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://rxq.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://iav.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vma.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://esr.shzxlz.cn

[G10] 访问控制
来源：http://oph.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://kpn.chenzaomai.com

PHP:  public / protected / private
来源：http://jyt.sxryk.cn

JS:   #private 字段；其余公开
来源：http://wdt.ppjwa.cn

TS:   public / protected / private
来源：http://qeq.tanke756.top

Java: public / protected / private / 默认包级
来源：http://pve.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kwx.vqdsnc.cn

Ruby: public / protected / private
来源：http://qwg.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://yes.yuxming.cn

[G11] getter / setter
来源：http://ewc.cashguo.top

Py:   @property 与 @x.setter
来源：http://juu.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://kkx.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://isq.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://ihi.shuidangran.top

Java: public String getName() { return name; }
来源：http://iim.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://pwe.quarkkingdee.top

Ruby: attr_accessor :name
来源：http://jfx.jqgufenzy.top

C#:   public string Name { get; set; }
来源：http://wmt.yj202588.top

[G12] 对象转字符串
来源：http://icq.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://gue.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nae.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://qwz.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://pbd.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://ecz.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bdf.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://bmj.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://rbm.xziqi.cn

[G13] 判断对象类型
来源：http://jzx.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://cyc.chenlongwang.top

PHP:  $u instanceof User
来源：http://fmr.0kj1m.cn

JS:   u instanceof User
来源：http://vrt.ppjwa.cn

TS:   u instanceof User
来源：http://fyj.snrcjt.cn

Java: u instanceof User
来源：http://zut.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://blj.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://bpi.meibo888.top

C#:   u is User
来源：http://jqk.yueranfly.top

[G14] 数据类 / record
来源：http://tox.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uew.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://exb.aizwys.cn

JS:   // 无内置：普通类或对象字面量
来源：http://con.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://aqb.yj202588.top

Java: record User(String name, int age) {}
来源：http://mpc.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://paq.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://isw.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://vun.havefunace.top

[G15] 枚举
来源：http://wyl.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://reo.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lhc.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sac.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zjx.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://iek.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dkw.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://yky.hnxiangtu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kmv.zhaomingkeji.xyz

[G16] 对象转数组 / 字典
来源：http://bhf.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrh.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://jnm.xuanzx.com

JS:   Object.entries(obj)
来源：http://dfi.smart0.xyz

TS:   Object.entries(obj)
来源：http://hlw.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bbf.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dmu.hywenlv.cn

Ruby: obj.instance_variables
来源：http://iwl.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://hdt.daxiang520.top

================================================================================
来源：http://bwa.9152youxi.cn

H. 异常与错误处理
来源：http://jib.dianchejie.cn

================================================================================
来源：http://ahf.pengpengdd.cyou

[H01] try / catch 基础
来源：http://erq.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lhy.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xmy.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zdr.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xhk.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jbh.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qbh.shanyushiyangtech.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://obu.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sqt.hysaishi.cn

[H02] finally / ensure 收尾
来源：http://lut.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://urb.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cff.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ugr.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://slf.yueranfly.top

Java: try { f(); } finally { cleanup(); }
来源：http://jog.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://rxv.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yol.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iuy.316326.xyz

[H03] 主动抛出异常
来源：http://jdw.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://cfk.yanxiufei.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rud.svipenyu.cn

JS:   throw new Error("错误信息");
来源：http://fby.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://fbe.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nfs.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dpc.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uai.sysykeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://cys.bjfxy.top

[H04] 自定义异常类型
来源：http://mow.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://rcy.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://jmz.jinghuilouyu.cn

JS:   class MyError extends Error {}
来源：http://ljo.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://jnu.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://mcm.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uof.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://xxz.andypj.xyz

C#:   class MyException : Exception {}
来源：http://aqb.yongpay.top

[H05] 捕获特定类型
来源：http://csh.52xcode.cn

Py:   except ValueError as e:
来源：http://plc.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://znv.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://bgf.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://bbu.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://plj.jqgfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://drw.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://lbn.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pgm.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://djd.xingfuxueyuan.xyz

Py:   value = d.get("k") or default
来源：http://cao.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://mxf.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://mek.mhx1999.top

TS:   obj?.a?.b;  d ?? default
来源：http://xyi.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://efe.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uia.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://lhc.aizwys.cn

C#:   obj?.A?.B ?? default
来源：http://knt.cdnleiting.top

[H07] 断言
来源：http://ghy.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://zgg.shzxlz.cn

PHP:  assert($x > 0);
来源：http://gjd.fktsv.cn

JS:   console.assert(x > 0);
来源：http://ugu.yvedp.cn

TS:   console.assert(x > 0);
来源：http://hjd.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://yvy.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bwe.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://jio.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://wba.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://wnm.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://eay.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pdt.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://yxj.shzxlz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pma.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oix.52xcode.cn

Go:   err.Error()
来源：http://yep.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://pyg.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://zyb.daxiang520.top

[H09] 带错误码的异常
来源：http://frv.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hay.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xyz.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yrd.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rhh.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wob.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://shm.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lrc.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gql.yj20258888.top

[H10] 资源自动释放
来源：http://mow.ywan-chungtsiang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ifl.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gvc.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://och.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hsn.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://amr.tarul.cn

Go:   defer f.Close()
来源：http://qea.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://otp.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ynl.shuidangran.top

================================================================================
来源：http://tjx.zhaomingkeji.xyz

I. 正则表达式
来源：http://wfb.316326.xyz

================================================================================
来源：http://jgt.shangyingyoupin.top

[I01] 判断是否匹配
来源：http://dxh.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gqm.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://qcy.cucudq.cn

JS:   /\d+/.test(s)
来源：http://hlx.zhaomingkeji.xyz

TS:   /\d+/.test(s)
来源：http://zkn.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fsq.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xvj.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://fyq.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cee.cucudq.cn

[I02] 提取所有匹配
来源：http://swj.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://mzi.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://frl.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pmy.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://gpm.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aqs.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tky.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://omw.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nix.ctjpmb.com

[I03] 提取捕获分组
来源：http://xge.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bir.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dxn.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bqg.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dou.tian-w.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yuk.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://npk.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ftm.yj20258888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fnc.ehwqpu.com

[I04] 正则替换
来源：http://lbj.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hpg.zycfv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://szd.yangfankeji.com

JS:   s.replace(/\d+/g, "#")
来源：http://wya.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://wxg.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://fvc.c1oappe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yvn.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nxj.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vuw.52xcode.cn

[I05] 按正则拆分
来源：http://nvr.hnqzz.top


<!-- 参考信息 -->