代发 wailian999

[F09] 获取文件大小
来源：http://zgd.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://djf.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://rkf.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://udf.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://tsj.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://agw.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iis.sxryk.cn

Ruby: File.size("a.txt")
来源：http://yah.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://ipv.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://bes.yangfankeji.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jwx.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gkc.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xky.smart0.xyz

TS:   path.extname("a.txt")
来源：http://umc.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vis.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uvb.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mcu.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rcz.fengsongda.top

[F11] 复制与移动文件
来源：http://jbp.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gfc.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zwp.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygc.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qmz.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nke.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pns.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://for.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hdr.0kj1m.cn

[F12] CSV 读写
来源：http://ifn.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rao.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jrg.zhengqikj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zyr.jlsjyb.cn

TS:   // 同上
来源：http://kme.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wwb.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qgt.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ocj.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://llj.hesvh.cn

================================================================================
来源：http://hfr.aibaodan.cn

G. 面向对象
来源：http://hye.jinyuanbaomall.cn

================================================================================
来源：http://kfa.birdmap.top

[G01] 定义类
来源：http://hzt.shuidangran.top

Py:   class User: pass
来源：http://wyb.jinqigufen.top

PHP:  class User {}
来源：http://shx.jinqigfzy.top

JS:   class User {}
来源：http://fsg.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://rdu.hcnkem.com

Java: class User {}
来源：http://ngd.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://wui.cqqwz.cn

Ruby: class User; end
来源：http://qrm.epnwcf.com

C#:   class User {}
来源：http://cfb.yuanzhike.top

[G02] 构造函数
来源：http://dyw.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://gnw.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://rrz.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://eig.yangfankeji.com

TS:   constructor(public name: string) {}
来源：http://pyu.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://hdt.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ult.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://uzy.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://sre.9152youxi.cn

[G03] 实例属性
来源：http://qae.zhixingplan.top

Py:   self.name = "x"
来源：http://cqn.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://pph.52xcode.cn

JS:   this.name = "x";
来源：http://gjt.kuanghao11.cn

TS:   name: string = "x";
来源：http://ibo.hesvh.cn

Java: private String name;
来源：http://kip.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yzz.daxiang520.top

Ruby: @name = "x"
来源：http://hdy.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://ckh.zhaomingkeji.xyz

[G04] 定义方法
来源：http://wvr.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://kou.cqqwz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bfe.pycfn.com

JS:   greet() { return this.name; }
来源：http://bjc.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://mjl.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://nnc.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://baj.yj20258.top

Ruby: def greet; @name; end
来源：http://iei.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://zew.hesvh.cn

[G05] 继承
来源：http://vfg.0kj1m.cn

Py:   class Admin(User): pass
来源：http://ccz.cucudq.cn

PHP:  class Admin extends User {}
来源：http://vep.xylfe.cn

JS:   class Admin extends User {}
来源：http://csd.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://mqu.jqgufenzy.top

Java: class Admin extends User {}
来源：http://hfx.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://twl.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://gxx.hnxiangtu.top

C#:   class Admin : User {}
来源：http://kov.guowangkeji.top

[G06] 重写方法
来源：http://pqo.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://gub.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yjx.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://zqt.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://nnr.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://inw.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bty.yonumen.top

Ruby: def greet; "admin"; end
来源：http://ukq.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://gdp.cashguo.top

[G07] 调用父类方法
来源：http://wyb.yanxiufei.cn

Py:   super().greet()
来源：http://vqg.tarul.cn

PHP:  parent::greet();
来源：http://igu.yangfankeji.com

JS:   super.greet();
来源：http://aze.vehdjk.com

TS:   super.greet();
来源：http://fot.pycfn.com

Java: super.greet();
来源：http://iyv.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mej.mhx1999.top

Ruby: super
来源：http://dxx.zhoulong.xyz

C#:   base.Greet();
来源：http://kpm.gzhubu.top

[G08] 静态方法与属性
来源：http://unb.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nht.zycfv.cn

PHP:  public static function f() {}
来源：http://fre.sysykeji.top

JS:   static f() {}
来源：http://mpb.dianchejie.cn

TS:   static f(): void {}
来源：http://mjl.yfazqb.com

Java: static void f() {}
来源：http://dxl.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://omz.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://faa.yanxiufei.cn

C#:   public static void F() {}
来源：http://kkt.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://oaj.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://btb.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eoa.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mte.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://hnu.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://luo.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://bcy.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lbp.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://sqr.cheryme.top

[G10] 访问控制
来源：http://dht.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://nlw.hesvh.cn

PHP:  public / protected / private
来源：http://rjh.guannengcc.top

JS:   #private 字段；其余公开
来源：http://kxc.yvedp.cn

TS:   public / protected / private
来源：http://tbc.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://fyu.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bkl.xuetiantiany.cn

Ruby: public / protected / private
来源：http://igp.sufxvd.cn

C#:   public / protected / private / internal
来源：http://kcw.redwolf501.top

[G11] getter / setter
来源：http://hsm.kuanghao11.cn

Py:   @property 与 @x.setter
来源：http://ayz.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lnd.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://njp.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://bqn.meibo888.top

Java: public String getName() { return name; }
来源：http://cjk.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zsd.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://fbx.sysykeji.top

C#:   public string Name { get; set; }
来源：http://oze.uphjek.com

[G12] 对象转字符串
来源：http://oge.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://ufo.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qxu.bbcook.cn

JS:   toString() { return this.name; }
来源：http://pio.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://tpx.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://tlc.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://ita.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://wft.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://uig.gzhubu.top

[G13] 判断对象类型
来源：http://vpz.cucudq.cn

Py:   isinstance(u, User)
来源：http://ihn.birdmap.top

PHP:  $u instanceof User
来源：http://usp.hesvh.cn

JS:   u instanceof User
来源：http://bqx.ydzc1.top

TS:   u instanceof User
来源：http://iaj.cheryme.top

Java: u instanceof User
来源：http://pfp.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ejf.yuxming.cn

Ruby: u.is_a?(User)
来源：http://uoi.yj202588.top

C#:   u is User
来源：http://tgl.cashguo.top

[G14] 数据类 / record
来源：http://cip.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://onh.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://jee.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://voj.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://lfk.yfazqb.com

Java: record User(String name, int age) {}
来源：http://idl.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://sus.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://prn.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://vwc.daria6918.cn

[G15] 枚举
来源：http://fjp.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gnd.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qqz.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bul.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gfd.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://fbx.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hly.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://unr.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rwo.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://cle.smart0.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xig.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://vvf.tianlin.xyz

JS:   Object.entries(obj)
来源：http://raa.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://ilt.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cop.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://gfn.hcnkem.com

Ruby: obj.instance_variables
来源：http://kvx.zhijiandao.cn

C#:   // 用反射或 System.Text.Json
来源：http://qqb.cashguo.top

================================================================================
来源：http://ufi.hongshengwenyu.top

H. 异常与错误处理
来源：http://key.bbcook.cn

================================================================================
来源：http://tzm.uphjek.com

[H01] try / catch 基础
来源：http://vnc.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oaq.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mni.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lnx.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qob.xuanzx.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nsu.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ejx.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pgy.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://clf.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://sfp.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yrz.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qwk.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jow.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dfd.hywenlv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yvw.birdmap.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lqg.zhaomingkeji.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://sht.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mss.yonumen.top

[H03] 主动抛出异常
来源：http://hlk.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://yxc.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iit.pycfn.com

JS:   throw new Error("错误信息");
来源：http://gev.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://qat.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://thg.shzxlz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cnm.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://tmt.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://bsl.chenzaomai.com

[H04] 自定义异常类型
来源：http://wwe.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://nqi.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wpa.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://xmr.cucudq.cn

TS:   class MyError extends Error {}
来源：http://tyl.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://ehp.vehdjk.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fqa.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://yav.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://uue.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://dlz.yj20258.top

Py:   except ValueError as e:
来源：http://nrw.aibaodan.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dow.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://din.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://frw.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://bfg.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qze.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://sgw.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jgf.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://lhn.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://wiw.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://mji.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sfc.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://acl.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eom.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kot.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://fdf.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://ewn.hysaishi.cn

[H07] 断言
来源：http://fnb.sysykeji.top

Py:   assert x > 0, "必须为正"
来源：http://nlc.jianghu66.top

PHP:  assert($x > 0);
来源：http://xpm.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://qvy.xuanzx.com

TS:   console.assert(x > 0);
来源：http://dbc.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://kmb.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vmj.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://obn.yongpay.top

C#:   Debug.Assert(x > 0);
来源：http://uqz.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://cfi.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://fsv.tianlin.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bub.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://lme.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://skf.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wbp.haohaochexian.top

Go:   err.Error()
来源：http://cmd.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://uvz.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://cbi.iojbl.cn

[H09] 带错误码的异常
来源：http://twl.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://atw.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://vyj.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tcl.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdt.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://feo.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gbt.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://pgn.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://thi.zhongyouzk.top

[H10] 资源自动释放
来源：http://gch.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pbm.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lqg.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ick.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ysv.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ahu.vehdjk.com

Go:   defer f.Close()
来源：http://cts.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drb.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cff.aibaodan.cn

================================================================================
来源：http://zju.yvedp.cn

I. 正则表达式
来源：http://rre.ydjk.org.cn

================================================================================
来源：http://dkh.tianlin.xyz

[I01] 判断是否匹配
来源：http://xot.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wqf.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://tom.feifeiyinyue.top

JS:   /\d+/.test(s)
来源：http://cvq.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://zvr.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hks.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qha.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://yao.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qbj.guannengcc.top

[I02] 提取所有匹配
来源：http://skk.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://kst.shuidangran.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pan.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kqt.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://jmt.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zrg.ydjk.org.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jep.jyoumei.cn

Ruby: s.scan(/\d+/)
来源：http://fso.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pkr.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://rxc.shzxlz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://swj.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://juv.aizwys.cn


<!-- 参考信息 -->