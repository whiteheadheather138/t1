代发 wailian999

[F09] 获取文件大小
来源：http://yrp.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://ncx.cucudq.cn

PHP:  filesize("a.txt");
来源：http://ttu.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://ldl.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://geb.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://zqp.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dte.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://wil.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://hve.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://iwj.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kfj.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tlr.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://awz.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://bdr.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rtb.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://szy.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qlf.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uyw.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://wpc.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivf.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vxc.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hfw.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwe.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vxq.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ara.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://igx.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bpl.yvedp.cn

[F12] CSV 读写
来源：http://gmd.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mxj.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mci.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bde.xuetiantiany.cn

TS:   // 同上
来源：http://qqx.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dtj.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rdo.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ywx.wangdashe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nre.cdnleiting.top

================================================================================
来源：http://xwu.zhongyouzk.top

G. 面向对象
来源：http://ize.ydzc1.top

================================================================================
来源：http://clf.yangfankeji.com

[G01] 定义类
来源：http://bjp.guannengcc.top

Py:   class User: pass
来源：http://tij.yongpay.top

PHP:  class User {}
来源：http://hcy.yfazqb.com

JS:   class User {}
来源：http://gzd.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://feb.guowangkeji.top

Java: class User {}
来源：http://dny.fzhhl.top

Go:   type User struct { Name string }
来源：http://eog.tianlin.xyz

Ruby: class User; end
来源：http://gwt.tarul.cn

C#:   class User {}
来源：http://tcv.jinyuanbaomall.cn

[G02] 构造函数
来源：http://hvn.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://wgn.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://udb.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://tdz.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://czl.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://bcc.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xmm.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://vls.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://rhc.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://fhl.aizwys.cn

Py:   self.name = "x"
来源：http://rvr.xinyue.icu

PHP:  public string $name = "x";
来源：http://wzl.bjfxy.top

JS:   this.name = "x";
来源：http://brd.zhijiandao.cn

TS:   name: string = "x";
来源：http://qzf.fktsv.cn

Java: private String name;
来源：http://fsj.hcnkem.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://axd.sysykeji.top

Ruby: @name = "x"
来源：http://mju.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://rzn.wangshuangyany.cn

[G04] 定义方法
来源：http://aae.hnqzz.top

Py:   def greet(self): return self.name
来源：http://bev.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jgm.epnwcf.com

JS:   greet() { return this.name; }
来源：http://rum.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://fny.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://cuz.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zgg.hnqzz.top

Ruby: def greet; @name; end
来源：http://yyh.pycfn.com

C#:   public string Greet() => Name;
来源：http://htd.yongpay.top

[G05] 继承
来源：http://xdc.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://vcf.daria6918.cn

PHP:  class Admin extends User {}
来源：http://aye.zhijiandao.cn

JS:   class Admin extends User {}
来源：http://acn.birdmap.top

TS:   class Admin extends User {}
来源：http://bdc.hfpthk.cn

Java: class Admin extends User {}
来源：http://ysp.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pnz.hfpthk.cn

Ruby: class Admin < User; end
来源：http://bym.bbcook.cn

C#:   class Admin : User {}
来源：http://zae.yvedp.cn

[G06] 重写方法
来源：http://ywf.yj202588.top

Py:   def greet(self): return "admin"
来源：http://ujo.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qdg.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://djy.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://yte.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://lon.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://imw.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://wkf.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://lmd.zycfv.cn

[G07] 调用父类方法
来源：http://msn.cqqwz.cn

Py:   super().greet()
来源：http://yhr.dianchejie.cn

PHP:  parent::greet();
来源：http://oip.jiagoushi.top

JS:   super.greet();
来源：http://fls.c1oappe.top

TS:   super.greet();
来源：http://eeq.nanxuanxn.top

Java: super.greet();
来源：http://vsa.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://men.epnwcf.com

Ruby: super
来源：http://rvt.cucudq.cn

C#:   base.Greet();
来源：http://bku.mhx1999.top

[G08] 静态方法与属性
来源：http://ump.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fbu.zdqjudy.top

PHP:  public static function f() {}
来源：http://hvl.fktsv.cn

JS:   static f() {}
来源：http://yez.ehwqpu.com

TS:   static f(): void {}
来源：http://nbf.zhixingplan.top

Java: static void f() {}
来源：http://yxl.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://saz.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://sep.hnxiangtu.top

C#:   public static void F() {}
来源：http://pnb.tarul.cn

[G09] 接口 / 抽象类
来源：http://fgz.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://wrk.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://hrg.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://zqy.aibaodan.cn

TS:   interface Shape { area(): number; }
来源：http://zny.hnqzz.top

Java: interface Shape { double area(); }
来源：http://ewm.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://yrf.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jdn.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://amy.zhoulong.xyz

[G10] 访问控制
来源：http://uqe.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://qex.cheryme.top

PHP:  public / protected / private
来源：http://qax.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://xjr.xuetiantiany.cn

TS:   public / protected / private
来源：http://hnx.ybcxt.top

Java: public / protected / private / 默认包级
来源：http://szc.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ejk.316326.xyz

Ruby: public / protected / private
来源：http://cvc.shuidangran.top

C#:   public / protected / private / internal
来源：http://ycp.nanxuanxn.top

[G11] getter / setter
来源：http://jeq.shuidangran.top

Py:   @property 与 @x.setter
来源：http://hzq.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vbq.ydzc1.top

JS:   get name() { return this._name; }
来源：http://kbr.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://wak.xuanzx.com

Java: public String getName() { return name; }
来源：http://rng.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dhm.hfpthk.cn

Ruby: attr_accessor :name
来源：http://haw.pycfn.com

C#:   public string Name { get; set; }
来源：http://jry.gogol.net.cn

[G12] 对象转字符串
来源：http://xui.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://unm.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://hcy.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://mvj.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://vpn.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://ctp.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://khc.52xcode.cn

Ruby: def to_s; @name; end
来源：http://hez.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://tjr.jyoumei.cn

[G13] 判断对象类型
来源：http://wbk.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://yqb.tarul.cn

PHP:  $u instanceof User
来源：http://wgm.hesvh.cn

JS:   u instanceof User
来源：http://azd.jinqigfzy.top

TS:   u instanceof User
来源：http://eeo.andypj.xyz

Java: u instanceof User
来源：http://ddw.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbs.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://rsl.jinyuanbaomall.cn

C#:   u is User
来源：http://qgc.gaohongyu789.top

[G14] 数据类 / record
来源：http://cpr.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ylr.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://xfw.ydzc1.top

JS:   // 无内置：普通类或对象字面量
来源：http://apb.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://fqw.tanke756.top

Java: record User(String name, int age) {}
来源：http://dla.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://yca.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zgd.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://hrv.birdmap.top

[G15] 枚举
来源：http://fzq.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://but.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://otm.yuxming.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dwt.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cei.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://ctm.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pug.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://ook.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ozu.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://fzu.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pfq.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://zmn.yuanzhike.top

JS:   Object.entries(obj)
来源：http://dft.gzhubu.top

TS:   Object.entries(obj)
来源：http://xgk.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://epa.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rhw.mhx1999.top

Ruby: obj.instance_variables
来源：http://pji.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://wve.xziqi.cn

================================================================================
来源：http://vmg.shzxlz.cn

H. 异常与错误处理
来源：http://gye.zhijiandao.cn

================================================================================
来源：http://etm.daria6918.cn

[H01] try / catch 基础
来源：http://zkv.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://amw.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://osl.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kor.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rpk.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lhy.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mbs.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hog.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gzk.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://aiy.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://afz.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uae.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uff.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://hqk.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://zay.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mil.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vge.hongshengwenyu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qnr.hfpthk.cn

[H03] 主动抛出异常
来源：http://ftk.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://lvb.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vie.smart0.xyz

JS:   throw new Error("错误信息");
来源：http://oug.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://oqd.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gvr.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nhh.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://flp.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://pwf.gotoacloud.top

[H04] 自定义异常类型
来源：http://hog.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://cti.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://onj.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://kvj.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://jhu.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://occ.xinyue.icu

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aqc.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://tvh.smart0.xyz

C#:   class MyException : Exception {}
来源：http://kzx.yanxiufei.cn

[H05] 捕获特定类型
来源：http://gph.jqgfzy.top

Py:   except ValueError as e:
来源：http://bmi.zhaomingkeji.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lcg.zhixingplan.top

JS:   if (e instanceof TypeError) {}
来源：http://eqz.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://mze.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://bzg.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ymf.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://npl.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hsc.nanxinkj.top

[H06] 可选值 / 空值安全访问
来源：http://rjg.vehdjk.com

Py:   value = d.get("k") or default
来源：http://fkk.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bag.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://ucc.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fre.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ecz.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://aks.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://aey.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://cjw.jinyuanbaomall.cn

[H07] 断言
来源：http://lja.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://epd.meibo888.top

PHP:  assert($x > 0);
来源：http://lqb.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://hmi.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://ogm.yanxiufei.cn

Java: assert x > 0 : "必须为正";
来源：http://fer.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bgy.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sjz.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://yjn.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://rmc.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://qdq.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ihq.ehwqpu.com

JS:   e.message;  e.stack
来源：http://sri.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://eds.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ozt.bjfxy.top

Go:   err.Error()
来源：http://irx.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://igf.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://oyy.yuanzhike.top

[H09] 带错误码的异常
来源：http://wpf.316326.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://stu.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qlg.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://huz.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://meb.gogol.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gdi.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rhc.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jgu.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gmk.yj202588.top

[H10] 资源自动释放
来源：http://dqa.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jtr.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xox.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xnc.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yui.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rpy.iojbl.cn

Go:   defer f.Close()
来源：http://mov.yonumen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fkn.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cdz.cashguo.top

================================================================================
来源：http://tfu.fktsv.cn

I. 正则表达式
来源：http://ftp.svipenyu.cn

================================================================================
来源：http://qxk.haohaochexian.top

[I01] 判断是否匹配
来源：http://kyv.hfpthk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nqz.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://wyl.c1oappe.top

JS:   /\d+/.test(s)
来源：http://igh.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://rod.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qbq.redwolf501.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rot.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://iwc.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ybs.iojbl.cn

[I02] 提取所有匹配
来源：http://zct.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://gwt.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pxw.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mlq.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://xik.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fbm.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fak.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://hzc.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://myt.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://dir.redwolf501.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ahg.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jkv.yvedp.cn


<!-- 参考信息 -->