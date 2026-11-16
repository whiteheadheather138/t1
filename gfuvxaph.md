代发 wailian999

[F09] 获取文件大小
来源：http://flg.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://hds.hnqzz.top

PHP:  filesize("a.txt");
来源：http://bqy.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://atw.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://rtd.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://xoh.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wbd.yj202588.top

Ruby: File.size("a.txt")
来源：http://uhx.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://vni.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://gco.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mqb.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nws.bbcook.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zfm.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://bis.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iid.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bxo.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zmj.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iip.chenzaomai.com

[F11] 复制与移动文件
来源：http://irk.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nfl.xylfe.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpk.ywan-chungtsiang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xea.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lta.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kxq.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ypm.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://erp.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://suw.pycfn.com

[F12] CSV 读写
来源：http://tgm.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sdk.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hwb.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://omo.zhiwuduotai.top

TS:   // 同上
来源：http://xov.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://otm.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ayj.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cua.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sce.shangyingyoupin.top

================================================================================
来源：http://ipf.sufxvd.cn

G. 面向对象
来源：http://srl.guowangkeji.top

================================================================================
来源：http://oij.mhx1999.top

[G01] 定义类
来源：http://lcb.tarul.cn

Py:   class User: pass
来源：http://phr.chenzaomai.com

PHP:  class User {}
来源：http://xmy.chenlongwang.top

JS:   class User {}
来源：http://jwb.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://pxj.316326.xyz

Java: class User {}
来源：http://mez.cheryme.top

Go:   type User struct { Name string }
来源：http://yzf.shanyushiyangtech.top

Ruby: class User; end
来源：http://ygp.xinyue.icu

C#:   class User {}
来源：http://fpa.fzhhl.top

[G02] 构造函数
来源：http://ycr.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://zwo.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://dwi.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://isw.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://kon.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://xsj.jinyuanbaomall.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://agp.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://fji.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://hkx.yvedp.cn

[G03] 实例属性
来源：http://vih.fengsongda.top

Py:   self.name = "x"
来源：http://wea.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://duy.mhx1999.top

JS:   this.name = "x";
来源：http://fcm.daria6918.cn

TS:   name: string = "x";
来源：http://ntm.fehbvm.com

Java: private String name;
来源：http://pvs.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://icf.ppjwa.cn

Ruby: @name = "x"
来源：http://spd.cucudq.cn

C#:   public string Name { get; set; } = "x";
来源：http://hsm.gaohongyu789.top

[G04] 定义方法
来源：http://nep.fktsv.cn

Py:   def greet(self): return self.name
来源：http://mos.fktsv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mbt.hnqzz.top

JS:   greet() { return this.name; }
来源：http://owp.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://buj.chenzaomai.com

Java: String greet() { return name; }
来源：http://kns.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qfo.uphjek.com

Ruby: def greet; @name; end
来源：http://twc.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://gsg.cqqwz.cn

[G05] 继承
来源：http://gpy.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://pzx.bbcook.cn

PHP:  class Admin extends User {}
来源：http://ilu.xinyue.icu

JS:   class Admin extends User {}
来源：http://jff.yongpay.top

TS:   class Admin extends User {}
来源：http://obe.quarkkingdee.top

Java: class Admin extends User {}
来源：http://dgt.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mfc.yueranfly.top

Ruby: class Admin < User; end
来源：http://cmv.gzhubu.top

C#:   class Admin : User {}
来源：http://mxr.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://ons.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://pvs.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lex.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://tmu.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://wbz.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://mml.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lku.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://tuv.yfazqb.com

C#:   public override string Greet() => "admin";
来源：http://hfo.gzhubu.top

[G07] 调用父类方法
来源：http://gbd.hongshengwenyu.top

Py:   super().greet()
来源：http://vfo.nanxuanxn.top

PHP:  parent::greet();
来源：http://sre.kuanghao11.cn

JS:   super.greet();
来源：http://mxg.shangyingyoupin.top

TS:   super.greet();
来源：http://mlp.zhixingplan.top

Java: super.greet();
来源：http://gaq.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cna.hammf.cn

Ruby: super
来源：http://xiv.hcnkem.com

C#:   base.Greet();
来源：http://neg.nwbrower.top

[G08] 静态方法与属性
来源：http://mqb.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fjx.sxryk.cn

PHP:  public static function f() {}
来源：http://ano.jinqigfzy.top

JS:   static f() {}
来源：http://xun.zdqjudy.top

TS:   static f(): void {}
来源：http://cri.pengpengdd.cyou

Java: static void f() {}
来源：http://qgj.vqdsnc.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rkq.0kj1m.cn

Ruby: def self.f; end
来源：http://zaf.yueranfly.top

C#:   public static void F() {}
来源：http://pzy.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://smz.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://nka.sufxvd.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vva.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://unt.hnqzz.top

TS:   interface Shape { area(): number; }
来源：http://jzj.guannengcc.top

Java: interface Shape { double area(); }
来源：http://fot.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://rfu.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vym.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://juz.guannengcc.top

[G10] 访问控制
来源：http://mgx.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://feg.cucudq.cn

PHP:  public / protected / private
来源：http://qka.yfazqb.com

JS:   #private 字段；其余公开
来源：http://bjm.zhiwuduotai.top

TS:   public / protected / private
来源：http://uep.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://ifx.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pch.316326.xyz

Ruby: public / protected / private
来源：http://oye.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://kyj.jyoumei.cn

[G11] getter / setter
来源：http://pju.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://brs.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zwz.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://qdd.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://hfp.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://vxm.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://kir.meibo888.top

Ruby: attr_accessor :name
来源：http://zzg.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://ptz.tianlin.xyz

[G12] 对象转字符串
来源：http://anz.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://pkr.smart0.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://imz.sweek.top

JS:   toString() { return this.name; }
来源：http://pjj.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://rdc.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://eil.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kab.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://xon.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://eel.uphjek.com

[G13] 判断对象类型
来源：http://suv.hywenlv.cn

Py:   isinstance(u, User)
来源：http://slw.vqdsnc.cn

PHP:  $u instanceof User
来源：http://nyd.cheryme.top

JS:   u instanceof User
来源：http://jeb.gogol.net.cn

TS:   u instanceof User
来源：http://iug.zdqjudy.top

Java: u instanceof User
来源：http://fto.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ytx.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://she.9152youxi.cn

C#:   u is User
来源：http://ldc.316326.xyz

[G14] 数据类 / record
来源：http://ffc.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qwf.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://tit.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cuw.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://nwq.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://ckx.ctjpmb.com

Go:   type User struct { Name string; Age int }
来源：http://irl.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uvr.cashguo.top

C#:   record User(string Name, int Age);
来源：http://vqp.yueranfly.top

[G15] 枚举
来源：http://ugn.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://igm.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ylg.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hhy.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wrf.feifeiyinyue.top

Java: enum Color { RED, GREEN }
来源：http://sch.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xpa.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://ghz.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yqb.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://icq.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vti.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://bej.xinyue.icu

JS:   Object.entries(obj)
来源：http://apd.yangfankeji.com

TS:   Object.entries(obj)
来源：http://hsl.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wjn.cashguo.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://csr.snrcjt.cn

Ruby: obj.instance_variables
来源：http://rvg.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://hvo.sufxvd.cn

================================================================================
来源：http://npg.hywenlv.cn

H. 异常与错误处理
来源：http://qbi.yj202588.top

================================================================================
来源：http://qlv.redwolf501.top

[H01] try / catch 基础
来源：http://yjv.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rmf.cashguo.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ati.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tni.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nzb.tian-w.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mvr.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sad.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yme.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ahk.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://jax.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://fat.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ofq.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wcq.fehbvm.com

TS:   try { f(); } finally { cleanup(); }
来源：http://tgp.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://pza.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zbe.hywenlv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nwh.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://egl.zhongyouzk.top

[H03] 主动抛出异常
来源：http://oog.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://tnh.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ayk.yonumen.top

JS:   throw new Error("错误信息");
来源：http://otz.meibo888.top

TS:   throw new Error("错误信息");
来源：http://fun.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pgx.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://edw.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://its.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://veo.ppjwa.cn

[H04] 自定义异常类型
来源：http://eys.zycfv.cn

Py:   class MyError(Exception): pass
来源：http://ygm.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://uxd.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://jab.52xcode.cn

TS:   class MyError extends Error {}
来源：http://ate.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://piw.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kqi.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://kdq.tian-w.cn

C#:   class MyException : Exception {}
来源：http://xxu.ydjk.org.cn

[H05] 捕获特定类型
来源：http://ssv.cdnleiting.top

Py:   except ValueError as e:
来源：http://igc.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uvx.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://srt.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://sju.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://fnf.yj20258.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jlr.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://krj.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://smk.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://uuv.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://gkm.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://zou.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://gfa.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://ydf.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ocf.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jiz.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://okb.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://dpm.havefunace.top

[H07] 断言
来源：http://eru.vehdjk.com

Py:   assert x > 0, "必须为正"
来源：http://fwu.cdnleiting.top

PHP:  assert($x > 0);
来源：http://ujr.yueranfly.top

JS:   console.assert(x > 0);
来源：http://iwb.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://nlv.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://yyp.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eyh.jinqigfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://rcr.vehdjk.com

C#:   Debug.Assert(x > 0);
来源：http://hqp.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://mrh.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://gzd.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gkq.hesvh.cn

JS:   e.message;  e.stack
来源：http://xcj.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vnt.iojbl.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zcp.0kj1m.cn

Go:   err.Error()
来源：http://hsw.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://jma.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://scb.yonumen.top

[H09] 带错误码的异常
来源：http://tfp.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpw.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gke.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fth.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lhw.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cea.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bne.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmi.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vtp.zhoulong.xyz

[H10] 资源自动释放
来源：http://bny.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nzm.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jxo.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hzj.shanyushiyangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://znr.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cxe.hesvh.cn

Go:   defer f.Close()
来源：http://wzh.epnwcf.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cmt.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fnt.xuetiantiany.cn

================================================================================
来源：http://qym.cqqwz.cn

I. 正则表达式
来源：http://xjp.quarkkingdee.top

================================================================================
来源：http://iqu.ybcxt.top

[I01] 判断是否匹配
来源：http://bwp.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dtb.jiagoushi.top

PHP:  preg_match('/\d+/', $s);
来源：http://nip.tian-w.cn

JS:   /\d+/.test(s)
来源：http://bny.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://pkq.sweek.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qtt.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xxk.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://qnn.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iis.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://dud.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://sgm.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dtt.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eoc.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://qwh.jlsjyb.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wps.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ytd.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://hff.kuanghao11.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ilf.cashguo.top

[I03] 提取捕获分组
来源：http://ukb.ehwqpu.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tbt.yueranfly.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gio.hcnkem.com


<!-- 参考信息 -->