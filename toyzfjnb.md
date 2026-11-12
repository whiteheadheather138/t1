代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://izc.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sdl.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sis.tian-w.cn

Ruby: File.size("a.txt")
来源：http://jik.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://pdi.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://vux.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://plk.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ouj.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rfb.guannengcc.top

TS:   path.extname("a.txt")
来源：http://kgo.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kie.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hiy.shangyingyoupin.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jxv.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uhl.fzhhl.top

[F11] 复制与移动文件
来源：http://yia.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oro.gzhubu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vat.daxiang520.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ziz.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzc.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnd.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hpu.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whx.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ehd.jinqigfzy.top

[F12] CSV 读写
来源：http://dtf.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sec.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ckl.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ieb.zycfv.cn

TS:   // 同上
来源：http://unj.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://smp.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://usv.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://txx.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gdc.yongpay.top

================================================================================
来源：http://uum.wangdashe.top

G. 面向对象
来源：http://dyq.shangyingyoupin.top

================================================================================
来源：http://wyr.tanke756.top

[G01] 定义类
来源：http://ktw.hysaishi.cn

Py:   class User: pass
来源：http://usb.sysykeji.top

PHP:  class User {}
来源：http://eaf.shzxlz.cn

JS:   class User {}
来源：http://shh.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://fru.yueranfly.top

Java: class User {}
来源：http://rfq.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://swl.cucudq.cn

Ruby: class User; end
来源：http://vqh.xziqi.cn

C#:   class User {}
来源：http://hkx.zhoulong.xyz

[G02] 构造函数
来源：http://xmn.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://wvb.havefunace.top

PHP:  public function __construct(public string $name) {}
来源：http://ctm.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://xjo.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://mjx.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://flm.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kcf.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://rzo.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://yoj.nanxuanxn.top

[G03] 实例属性
来源：http://ayv.jqgufenzy.top

Py:   self.name = "x"
来源：http://cak.epnwcf.com

PHP:  public string $name = "x";
来源：http://mmp.hywenlv.cn

JS:   this.name = "x";
来源：http://rrf.daria6918.cn

TS:   name: string = "x";
来源：http://idj.haohaochexian.top

Java: private String name;
来源：http://kxi.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vkj.uphjek.com

Ruby: @name = "x"
来源：http://qmr.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://ulj.cdnleiting.top

[G04] 定义方法
来源：http://nsv.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://toy.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://acp.ydzc1.top

JS:   greet() { return this.name; }
来源：http://kmy.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://kqh.sufxvd.cn

Java: String greet() { return name; }
来源：http://wss.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://btf.ybcxt.top

Ruby: def greet; @name; end
来源：http://iee.smart0.xyz

C#:   public string Greet() => Name;
来源：http://mfi.sysykeji.top

[G05] 继承
来源：http://gqp.birdmap.top

Py:   class Admin(User): pass
来源：http://qlr.ivvv.top

PHP:  class Admin extends User {}
来源：http://dak.ydzc1.top

JS:   class Admin extends User {}
来源：http://fvc.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://ynz.yongpay.top

Java: class Admin extends User {}
来源：http://uhj.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tiz.tianlin.xyz

Ruby: class Admin < User; end
来源：http://las.sjlbkw.cn

C#:   class Admin : User {}
来源：http://qbw.zhiwuduotai.top

[G06] 重写方法
来源：http://odm.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://vuw.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fuu.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://upi.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://uvo.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://mtz.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uit.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://fsf.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://kqi.pengpengdd.cyou

[G07] 调用父类方法
来源：http://hji.fengsongda.top

Py:   super().greet()
来源：http://jri.iojbl.cn

PHP:  parent::greet();
来源：http://qqn.iojbl.cn

JS:   super.greet();
来源：http://qfb.jyoumei.cn

TS:   super.greet();
来源：http://hzp.nanxuanxn.top

Java: super.greet();
来源：http://tic.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://spq.feifeiyinyue.top

Ruby: super
来源：http://caq.shanyushiyangtech.top

C#:   base.Greet();
来源：http://jeu.xylfe.cn

[G08] 静态方法与属性
来源：http://jfy.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gju.aibaodan.cn

PHP:  public static function f() {}
来源：http://wcu.shanyushiyangkeji.top

JS:   static f() {}
来源：http://ynt.cucudq.cn

TS:   static f(): void {}
来源：http://wxx.nwbrower.top

Java: static void f() {}
来源：http://cbr.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdg.52xcode.cn

Ruby: def self.f; end
来源：http://baf.uphjek.com

C#:   public static void F() {}
来源：http://mgp.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://ank.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://zla.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://bsq.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aap.wangdashe.top

TS:   interface Shape { area(): number; }
来源：http://wuy.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://glb.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://lio.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jrv.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://hgi.jqgufenzy.top

[G10] 访问控制
来源：http://alj.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://hjd.redwolf501.top

PHP:  public / protected / private
来源：http://jdm.havefunace.top

JS:   #private 字段；其余公开
来源：http://nce.jlsjyb.cn

TS:   public / protected / private
来源：http://aem.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://gvo.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://blk.jiagoushi.top

Ruby: public / protected / private
来源：http://cad.hcnkem.com

C#:   public / protected / private / internal
来源：http://ueq.cashguo.top

[G11] getter / setter
来源：http://woo.yfazqb.com

Py:   @property 与 @x.setter
来源：http://wvp.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cfo.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://sxm.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://fhm.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://gmd.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jlj.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://zfr.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://xdj.ydjk.org.cn

[G12] 对象转字符串
来源：http://ohm.316326.xyz

Py:   def __str__(self): return self.name
来源：http://gjn.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ehs.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://sjp.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://fzy.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://zej.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nxl.birdmap.top

Ruby: def to_s; @name; end
来源：http://jgm.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://fve.guannengcc.top

[G13] 判断对象类型
来源：http://kdf.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://nnn.havefunace.top

PHP:  $u instanceof User
来源：http://hfb.xinyue.icu

JS:   u instanceof User
来源：http://cfj.jqgufenzy.top

TS:   u instanceof User
来源：http://zpl.jinqigufen.top

Java: u instanceof User
来源：http://ppl.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ztx.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://pem.birdmap.top

C#:   u is User
来源：http://dff.tianlin.xyz

[G14] 数据类 / record
来源：http://gdv.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://axr.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://oxi.vqdsnc.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fmp.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://zgs.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://qjw.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://jng.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://app.jianghu66.top

C#:   record User(string Name, int Age);
来源：http://ikp.cashguo.top

[G15] 枚举
来源：http://env.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tlt.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://foy.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://exy.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cmi.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://nje.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tnx.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://lni.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ujm.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://dbp.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://asu.cheryme.top

PHP:  get_object_vars($obj);
来源：http://ldy.nanxinkj.top

JS:   Object.entries(obj)
来源：http://pvp.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://szz.fzhhl.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lve.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xja.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://vds.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://ktn.wangshuangyany.cn

================================================================================
来源：http://mrq.jqgfzy.top

H. 异常与错误处理
来源：http://mll.9152youxi.cn

================================================================================
来源：http://dtq.shangyingyoupin.top

[H01] try / catch 基础
来源：http://vjs.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gnu.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qhq.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zll.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oky.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://klp.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mal.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jav.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qon.andypj.xyz

[H02] finally / ensure 收尾
来源：http://nnp.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://kdd.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hst.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ewq.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kpt.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vyf.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rjk.hnqzz.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ata.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://for.316326.xyz

[H03] 主动抛出异常
来源：http://axt.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://tiy.hnxiangtu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yha.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://cgg.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://sze.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kml.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oqq.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://isd.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://nbx.zhoulong.xyz

[H04] 自定义异常类型
来源：http://lsx.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://bel.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://tmo.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://dly.mhx1999.top

TS:   class MyError extends Error {}
来源：http://lqe.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://dkf.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rds.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://rtb.ivvv.top

C#:   class MyException : Exception {}
来源：http://xxg.yuanzhike.top

[H05] 捕获特定类型
来源：http://zeh.yvedp.cn

Py:   except ValueError as e:
来源：http://lpt.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uag.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://kqy.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://lnm.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://ogr.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://coq.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://olr.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rcc.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://olf.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://whv.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://yai.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://isr.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://isy.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ctq.fengsongda.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jrp.fktsv.cn

Ruby: d&.dig(:a, :b)
来源：http://vtn.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://whx.tian-w.cn

[H07] 断言
来源：http://kjb.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://nxg.aibaodan.cn

PHP:  assert($x > 0);
来源：http://buy.fzhhl.top

JS:   console.assert(x > 0);
来源：http://whp.mhx1999.top

TS:   console.assert(x > 0);
来源：http://onh.sjlbkw.cn

Java: assert x > 0 : "必须为正";
来源：http://ohr.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pfc.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://skd.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://cbk.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://oju.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://nas.ctjpmb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hya.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://myj.pengpengdd.cyou

TS:   e instanceof Error ? e.message : String(e)
来源：http://gnl.fehbvm.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vzg.zycfv.cn

Go:   err.Error()
来源：http://ngv.dashuyun.cn

Ruby: e.message;  e.backtrace
来源：http://olu.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://rtd.haohaochexian.top

[H09] 带错误码的异常
来源：http://ilg.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mxf.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tde.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gjx.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jfo.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eig.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://szg.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eoa.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zex.zycfv.cn

[H10] 资源自动释放
来源：http://nsb.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pkj.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://djm.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iiy.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vcc.zycfv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://msq.chenlongwang.top

Go:   defer f.Close()
来源：http://fxf.ivvv.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tfc.zycfv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ucd.52xcode.cn

================================================================================
来源：http://vga.yangfankeji.com

I. 正则表达式
来源：http://zoy.sufxvd.cn

================================================================================
来源：http://gob.hywenlv.cn

[I01] 判断是否匹配
来源：http://wop.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qre.xziqi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uun.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://saq.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://bnb.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bxw.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rhu.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://jaq.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ltw.sufxvd.cn

[I02] 提取所有匹配
来源：http://gkk.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://mkv.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://utv.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xxz.sweek.top

TS:   s.match(/\d+/g)
来源：http://dig.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rrn.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hpj.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://pnv.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://klg.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://yaf.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://klf.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xtz.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://krd.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hcj.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ppi.aizwys.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wfo.fanxiaobao.xyz


<!-- 参考信息 -->