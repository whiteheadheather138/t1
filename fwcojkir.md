代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlf.sysykeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://chu.aibaodan.cn

[F11] 复制与移动文件
来源：http://fqk.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://csz.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ewc.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgk.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tsc.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jzi.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://scu.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yoo.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jqd.jianghu66.top

[F12] CSV 读写
来源：http://gwq.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qpk.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lvn.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egs.aizwys.cn

TS:   // 同上
来源：http://nlv.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rcl.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xvi.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://puc.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://zjh.tianlin.xyz

================================================================================
来源：http://wkf.shanyushiyangkeji.top

G. 面向对象
来源：http://jqd.shanyushiyangkeji.top

================================================================================
来源：http://rnr.smart0.xyz

[G01] 定义类
来源：http://qfg.aibaodan.cn

Py:   class User: pass
来源：http://shh.sxryk.cn

PHP:  class User {}
来源：http://ybs.daxiang520.top

JS:   class User {}
来源：http://pcq.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://zra.chenjidiqi.icu

Java: class User {}
来源：http://ygc.nwbrower.top

Go:   type User struct { Name string }
来源：http://njl.yonumen.top

Ruby: class User; end
来源：http://yrk.tianlin.xyz

C#:   class User {}
来源：http://oyi.quarkkingdee.top

[G02] 构造函数
来源：http://tlq.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://bmf.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://dmx.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://lny.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://bbg.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://nog.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://irg.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://jrt.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://ysc.havefunace.top

[G03] 实例属性
来源：http://sec.zhixingplan.top

Py:   self.name = "x"
来源：http://mbk.hysaishi.cn

PHP:  public string $name = "x";
来源：http://fvp.ydzc1.top

JS:   this.name = "x";
来源：http://xev.hesvh.cn

TS:   name: string = "x";
来源：http://gwt.zdbjq.cn

Java: private String name;
来源：http://gzs.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bcp.chenlongwang.top

Ruby: @name = "x"
来源：http://hsp.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://urt.hnxiangtu.top

[G04] 定义方法
来源：http://kmg.zycfv.cn

Py:   def greet(self): return self.name
来源：http://fla.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gwj.bbcook.cn

JS:   greet() { return this.name; }
来源：http://tmx.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://ugb.haohaochexian.top

Java: String greet() { return name; }
来源：http://vnu.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://das.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://lrj.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://pcv.hcnkem.com

[G05] 继承
来源：http://bco.xziqi.cn

Py:   class Admin(User): pass
来源：http://tfa.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://dje.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://xxn.hesvh.cn

TS:   class Admin extends User {}
来源：http://crx.quarkkingdee.top

Java: class Admin extends User {}
来源：http://vxk.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ody.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://zdm.zhongyouzk.top

C#:   class Admin : User {}
来源：http://kwp.nanxinkj.top

[G06] 重写方法
来源：http://icw.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://pxf.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wto.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://yzd.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://dma.hongshengwenyu.top

Java: @Override String greet() { return "admin"; }
来源：http://nky.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hlf.hammf.cn

Ruby: def greet; "admin"; end
来源：http://bud.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://nzd.cqqwz.cn

[G07] 调用父类方法
来源：http://rzm.fktsv.cn

Py:   super().greet()
来源：http://cvq.guannengcc.top

PHP:  parent::greet();
来源：http://vcg.mhx1999.top

JS:   super.greet();
来源：http://cgh.jlsjyb.cn

TS:   super.greet();
来源：http://eun.daxiang520.top

Java: super.greet();
来源：http://pvr.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pra.feifeiyinyue.top

Ruby: super
来源：http://zwg.gaohongyu789.top

C#:   base.Greet();
来源：http://vgw.ydjk.org.cn

[G08] 静态方法与属性
来源：http://ekh.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kjn.bjfxy.top

PHP:  public static function f() {}
来源：http://lry.0kj1m.cn

JS:   static f() {}
来源：http://zlm.redwolf501.top

TS:   static f(): void {}
来源：http://fsr.fzhhl.top

Java: static void f() {}
来源：http://tqh.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pvn.tanke756.top

Ruby: def self.f; end
来源：http://epu.yonumen.top

C#:   public static void F() {}
来源：http://zyp.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://mqq.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://rzc.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://tiy.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tdz.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://epv.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://zmm.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://vqk.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lyy.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://nff.svipenyu.cn

[G10] 访问控制
来源：http://ycp.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://nxr.fengsongda.top

PHP:  public / protected / private
来源：http://bla.yongpay.top

JS:   #private 字段；其余公开
来源：http://sgp.tarul.cn

TS:   public / protected / private
来源：http://epc.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://oqy.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://tyd.epnwcf.com

Ruby: public / protected / private
来源：http://paz.hfpthk.cn

C#:   public / protected / private / internal
来源：http://jhu.pengpengdd.cyou

[G11] getter / setter
来源：http://xvq.hesvh.cn

Py:   @property 与 @x.setter
来源：http://ssd.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nez.birdmap.top

JS:   get name() { return this._name; }
来源：http://onu.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://xzk.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://vud.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://shi.epnwcf.com

Ruby: attr_accessor :name
来源：http://jzh.c1oappe.top

C#:   public string Name { get; set; }
来源：http://ahv.zhijiandao.cn

[G12] 对象转字符串
来源：http://oke.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://cke.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xko.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://yii.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://har.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://vtl.yuxming.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gek.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://abt.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://dqg.yvedp.cn

[G13] 判断对象类型
来源：http://dpj.uphjek.com

Py:   isinstance(u, User)
来源：http://vgg.yj202588.top

PHP:  $u instanceof User
来源：http://wcu.jqgfzy.top

JS:   u instanceof User
来源：http://naj.yanxiufei.cn

TS:   u instanceof User
来源：http://wxh.cashguo.top

Java: u instanceof User
来源：http://rpt.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bsh.pengpengdd.cyou

Ruby: u.is_a?(User)
来源：http://bjg.daxiang520.top

C#:   u is User
来源：http://kux.9152youxi.cn

[G14] 数据类 / record
来源：http://cmm.zdqjudy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://agg.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://det.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://roz.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://npw.hcnkem.com

Java: record User(String name, int age) {}
来源：http://iys.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://nzb.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rjl.zhongyouzk.top

C#:   record User(string Name, int Age);
来源：http://uzl.vehdjk.com

[G15] 枚举
来源：http://dxg.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nxu.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hmf.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rgp.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://arv.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://zwm.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vxj.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://nsd.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cay.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://hmy.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dai.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://vuv.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://hpv.xziqi.cn

TS:   Object.entries(obj)
来源：http://ipi.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aub.ivvv.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hhv.cqqwz.cn

Ruby: obj.instance_variables
来源：http://pxs.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://ezz.52xcode.cn

================================================================================
来源：http://geo.52xcode.cn

H. 异常与错误处理
来源：http://rdv.hywenlv.cn

================================================================================
来源：http://gjq.yanxiufei.cn

[H01] try / catch 基础
来源：http://dte.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://asz.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zqy.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://req.hongshengwenyu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://clq.hongshengwenyu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vic.daxiang520.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pzt.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kaj.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dzz.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://wzn.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://rry.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ecx.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wfk.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://axg.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ilm.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cxu.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xdy.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rrt.jlsjyb.cn

[H03] 主动抛出异常
来源：http://okr.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://eoa.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zmm.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://rlw.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://tzq.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vfr.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hie.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lqn.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://gbx.tarul.cn

[H04] 自定义异常类型
来源：http://dow.fanxiaobao.xyz

Py:   class MyError(Exception): pass
来源：http://acc.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ffa.yj20258.top

JS:   class MyError extends Error {}
来源：http://zrq.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://dya.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://qdc.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rtb.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://pga.bjfxy.top

C#:   class MyException : Exception {}
来源：http://umu.xuanzx.com

[H05] 捕获特定类型
来源：http://giv.ppjwa.cn

Py:   except ValueError as e:
来源：http://yqq.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jbd.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://wff.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://hpq.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://jpa.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzn.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://hkg.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pjt.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://hyb.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://ntg.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lpn.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hwh.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ybj.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nat.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wwu.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://znr.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://vwn.c1oappe.top

[H07] 断言
来源：http://ubw.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://ypw.jqgfzy.top

PHP:  assert($x > 0);
来源：http://vyj.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://dum.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://umn.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://sxy.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bdt.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://bia.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://eqj.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://xbs.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://vsm.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bnr.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://feq.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nsk.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sdf.ctjpmb.com

Go:   err.Error()
来源：http://zjn.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://pvj.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://ply.sjlbkw.cn

[H09] 带错误码的异常
来源：http://gpp.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wsh.iojbl.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hfs.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://spv.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://byz.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pff.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://smb.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://xbk.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ing.fengsongda.top

[H10] 资源自动释放
来源：http://mbu.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://dnh.fktsv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oha.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qpd.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uis.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wlc.chenlongwang.top

Go:   defer f.Close()
来源：http://sjr.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tuf.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqu.jiagoushi.top

================================================================================
来源：http://jdh.fengsongda.top

I. 正则表达式
来源：http://eww.shangyingyoupin.top

================================================================================
来源：http://jyw.cdnleiting.top

[I01] 判断是否匹配
来源：http://uay.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cqu.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://ayj.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://umx.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://las.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbs.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mvd.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://iym.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ori.hywenlv.cn

[I02] 提取所有匹配
来源：http://rsv.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://oza.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yet.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xhc.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://ppi.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jty.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xob.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://ytx.vqdsnc.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jwn.shuidangran.top

[I03] 提取捕获分组
来源：http://sfw.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zvm.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vjo.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pxx.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tky.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://coa.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xau.yongpay.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gkq.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zoe.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://rbk.ydzc1.top

Py:   re.sub(r"\d+", "#", s)
来源：http://efi.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qor.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gte.zdqjudy.top

TS:   s.replace(/\d+/g, "#")
来源：http://krf.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://kko.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sry.yanxiufei.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bix.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bse.xinyue.icu

[I05] 按正则拆分
来源：http://nto.xuanzx.com


<!-- 参考信息 -->