代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tqn.xziqi.cn

TS:   path.extname("a.txt")
来源：http://zpl.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pjh.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ilf.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pxw.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rvx.yonumen.top

[F11] 复制与移动文件
来源：http://gzr.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lbt.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xem.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ser.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kot.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pgo.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://isa.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://imf.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ahh.bbcook.cn

[F12] CSV 读写
来源：http://cpz.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qvg.vehdjk.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iai.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://usv.cqqwz.cn

TS:   // 同上
来源：http://vmr.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vcm.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vba.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dqb.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://glt.sysykeji.top

================================================================================
来源：http://rtp.tianlin.xyz

G. 面向对象
来源：http://jhz.quarkkingdee.top

================================================================================
来源：http://bhq.ctjpmb.com

[G01] 定义类
来源：http://ngh.316326.xyz

Py:   class User: pass
来源：http://bue.snrcjt.cn

PHP:  class User {}
来源：http://klv.nwbrower.top

JS:   class User {}
来源：http://dsj.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://sxm.zhoulong.xyz

Java: class User {}
来源：http://qlf.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://xva.andypj.xyz

Ruby: class User; end
来源：http://ahz.cashguo.top

C#:   class User {}
来源：http://vah.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://hfr.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://rzp.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://fpx.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://rsl.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://fpo.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://yay.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kcl.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://vib.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://hrq.zhengqikj.top

[G03] 实例属性
来源：http://duq.shzxlz.cn

Py:   self.name = "x"
来源：http://wxg.gzhubu.top

PHP:  public string $name = "x";
来源：http://okn.zhengqikj.top

JS:   this.name = "x";
来源：http://gap.dianchejie.cn

TS:   name: string = "x";
来源：http://ybf.chenjidiqi.icu

Java: private String name;
来源：http://lrz.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vqf.fehbvm.com

Ruby: @name = "x"
来源：http://epu.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://zib.yvedp.cn

[G04] 定义方法
来源：http://eou.daxiang520.top

Py:   def greet(self): return self.name
来源：http://uqy.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gep.mhx1999.top

JS:   greet() { return this.name; }
来源：http://law.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://war.jianghu66.top

Java: String greet() { return name; }
来源：http://ywg.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sfw.cdnleiting.top

Ruby: def greet; @name; end
来源：http://lcc.yvedp.cn

C#:   public string Greet() => Name;
来源：http://naw.shanyushiyangkeji.top

[G05] 继承
来源：http://ydl.sufxvd.cn

Py:   class Admin(User): pass
来源：http://nwy.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://gnr.nanxinkj.top

JS:   class Admin extends User {}
来源：http://atb.meibo888.top

TS:   class Admin extends User {}
来源：http://oan.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://gss.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iay.smart0.xyz

Ruby: class Admin < User; end
来源：http://diu.havefunace.top

C#:   class Admin : User {}
来源：http://fgd.quarkkingdee.top

[G06] 重写方法
来源：http://ocf.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://zea.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://yeb.316326.xyz

JS:   greet() { return "admin"; }
来源：http://jqn.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://cig.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://eel.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpk.tarul.cn

Ruby: def greet; "admin"; end
来源：http://bhp.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://zfm.shzxlz.cn

[G07] 调用父类方法
来源：http://lht.0kj1m.cn

Py:   super().greet()
来源：http://nvr.jianghu66.top

PHP:  parent::greet();
来源：http://fdx.zycfv.cn

JS:   super.greet();
来源：http://jox.daxiang520.top

TS:   super.greet();
来源：http://omn.xuanzx.com

Java: super.greet();
来源：http://ope.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://azw.nanxinkj.top

Ruby: super
来源：http://vgb.ydjk.org.cn

C#:   base.Greet();
来源：http://hwz.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://nde.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fsp.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://cbd.ehwqpu.com

JS:   static f() {}
来源：http://gsg.quarkkingdee.top

TS:   static f(): void {}
来源：http://qzr.yj202588.top

Java: static void f() {}
来源：http://oqj.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wbq.vqdsnc.cn

Ruby: def self.f; end
来源：http://bpc.c1oappe.top

C#:   public static void F() {}
来源：http://yxk.ivvv.top

[G09] 接口 / 抽象类
来源：http://yew.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://ygi.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gyu.tianlin.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ejf.wangshuangyany.cn

TS:   interface Shape { area(): number; }
来源：http://ptp.fehbvm.com

Java: interface Shape { double area(); }
来源：http://dmi.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://nyi.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bov.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://pvx.zhiwuduotai.top

[G10] 访问控制
来源：http://nor.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://egd.xziqi.cn

PHP:  public / protected / private
来源：http://jmf.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://ajh.chenlongwang.top

TS:   public / protected / private
来源：http://sbb.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://rme.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mif.tarul.cn

Ruby: public / protected / private
来源：http://kze.birdmap.top

C#:   public / protected / private / internal
来源：http://ygx.shanyushiyangkeji.top

[G11] getter / setter
来源：http://kjd.daxiang520.top

Py:   @property 与 @x.setter
来源：http://nzu.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dnb.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://lrf.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://age.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://slq.ppjwa.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hdw.nanxinkj.top

Ruby: attr_accessor :name
来源：http://xxc.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://urg.shuidangran.top

[G12] 对象转字符串
来源：http://rcl.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://yke.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nhl.redwolf501.top

JS:   toString() { return this.name; }
来源：http://lvm.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://ech.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://ptj.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://sdu.ybcxt.top

Ruby: def to_s; @name; end
来源：http://cxh.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://vif.sysykeji.top

[G13] 判断对象类型
来源：http://ynz.nanxinkj.top

Py:   isinstance(u, User)
来源：http://ooy.yongpay.top

PHP:  $u instanceof User
来源：http://flu.havefunace.top

JS:   u instanceof User
来源：http://fbr.aibaodan.cn

TS:   u instanceof User
来源：http://tdt.yvedp.cn

Java: u instanceof User
来源：http://gwn.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hag.wangdashe.top

Ruby: u.is_a?(User)
来源：http://bdb.xingfuxueyuan.xyz

C#:   u is User
来源：http://sis.52xcode.cn

[G14] 数据类 / record
来源：http://eon.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aau.quarkkingdee.top

PHP:  // 用 readonly 属性模拟
来源：http://hyp.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://rru.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://tbg.hesvh.cn

Java: record User(String name, int age) {}
来源：http://oou.zdbjq.cn

Go:   type User struct { Name string; Age int }
来源：http://pvr.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pyb.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://ubx.gogol.net.cn

[G15] 枚举
来源：http://edv.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fgh.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://aps.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://atg.mhx1999.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zsd.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://gko.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nxf.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://ogp.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nzl.gaohongyu789.top

[G16] 对象转数组 / 字典
来源：http://ynr.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rvx.pycfn.com

PHP:  get_object_vars($obj);
来源：http://czu.feifeiyinyue.top

JS:   Object.entries(obj)
来源：http://lya.hywenlv.cn

TS:   Object.entries(obj)
来源：http://whd.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pkt.daxiang520.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xms.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://kdn.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://kgi.xuetiantiany.cn

================================================================================
来源：http://wfk.jianghu66.top

H. 异常与错误处理
来源：http://jao.bbcook.cn

================================================================================
来源：http://rxz.xylfe.cn

[H01] try / catch 基础
来源：http://ero.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kfw.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mwy.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://svr.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wko.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dty.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jrh.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dor.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cnr.sysykeji.top

[H02] finally / ensure 收尾
来源：http://hcd.zhengqikj.top

Py:   try: f()⏎finally: cleanup()
来源：http://rou.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ooz.feifeiyinyue.top

JS:   try { f(); } finally { cleanup(); }
来源：http://edr.yanxiufei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wzi.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://gsa.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eul.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://std.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://poi.yvedp.cn

[H03] 主动抛出异常
来源：http://axe.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://rct.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aue.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://rjw.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://szb.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wck.hongshengwenyu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jlz.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://mgc.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://asf.yangfankeji.com

[H04] 自定义异常类型
来源：http://kkw.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://vcd.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://nqi.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://mcu.fzhhl.top

TS:   class MyError extends Error {}
来源：http://cjt.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://ftw.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://enj.jiagoushi.top

Ruby: class MyError < StandardError; end
来源：http://lhs.yfazqb.com

C#:   class MyException : Exception {}
来源：http://frs.nwbrower.top

[H05] 捕获特定类型
来源：http://jjh.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://xfl.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pwy.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://djq.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://btw.pengpengdd.cyou

Java: catch (IOException | SQLException e) {}
来源：http://acu.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mpp.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://ivn.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://knx.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://lot.xinyue.icu

Py:   value = d.get("k") or default
来源：http://drl.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://lya.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://zck.snrcjt.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uuz.epnwcf.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hyz.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dgw.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://aaj.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://qsv.fktsv.cn

[H07] 断言
来源：http://jlk.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://ebx.daria6918.cn

PHP:  assert($x > 0);
来源：http://rsj.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://tos.tian-w.cn

TS:   console.assert(x > 0);
来源：http://kjf.zhixingplan.top

Java: assert x > 0 : "必须为正";
来源：http://rsb.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://daq.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://jfl.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://wuj.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://wzo.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://sju.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://izz.316326.xyz

JS:   e.message;  e.stack
来源：http://wzj.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ylq.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vqq.bbcook.cn

Go:   err.Error()
来源：http://sal.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://bqt.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://wcm.chenzaomai.com

[H09] 带错误码的异常
来源：http://epg.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://deg.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dxv.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zkq.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://knm.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dwr.yfazqb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wtc.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://etm.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yyc.yanxiufei.cn

[H10] 资源自动释放
来源：http://vyo.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rwj.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ktv.dianchejie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smx.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fgf.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sed.redwolf501.top

Go:   defer f.Close()
来源：http://fwz.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wic.pengpengdd.cyou

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wml.bbcook.cn

================================================================================
来源：http://nbd.zhoulong.xyz

I. 正则表达式
来源：http://atz.ctjpmb.com

================================================================================
来源：http://qdl.tian-w.cn

[I01] 判断是否匹配
来源：http://ctl.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uny.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://hza.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://xwg.ivvv.top

TS:   /\d+/.test(s)
来源：http://xjn.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nrp.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xew.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://mup.xuetiantiany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hxj.wangdashe.top

[I02] 提取所有匹配
来源：http://zfh.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://rrw.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jvl.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://evd.quarkkingdee.top

TS:   s.match(/\d+/g)
来源：http://azh.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gma.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bqv.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://dal.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kfq.shuidangran.top

[I03] 提取捕获分组
来源：http://gzs.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ajv.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lqm.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://awz.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mju.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lve.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gjb.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uig.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fne.gzhubu.top

[I04] 正则替换
来源：http://atm.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yan.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bmj.yanxiufei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ygx.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://szy.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wcz.nwbrower.top


<!-- 参考信息 -->