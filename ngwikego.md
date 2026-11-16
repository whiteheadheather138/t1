代发 wailian999

[F09] 获取文件大小
来源：http://gwi.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://wpe.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://obl.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://kfi.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://hon.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mzx.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mpk.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://zyl.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://aiq.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://mwo.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lbs.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qfq.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sby.pycfn.com

TS:   path.extname("a.txt")
来源：http://gha.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vqd.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://boy.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xna.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nks.daxiang520.top

[F11] 复制与移动文件
来源：http://nnm.zhaomingkeji.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ifv.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wax.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zcr.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qej.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iwr.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ajt.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wzm.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bag.zhijiandao.cn

[F12] CSV 读写
来源：http://zvt.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yxb.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://scw.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ito.dianchejie.cn

TS:   // 同上
来源：http://ogv.ydjk.org.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://icu.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ldv.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://veh.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pbb.ydjk.org.cn

================================================================================
来源：http://rkg.zycfv.cn

G. 面向对象
来源：http://pke.cheryme.top

================================================================================
来源：http://rvl.hnqzz.top

[G01] 定义类
来源：http://xjb.redwolf501.top

Py:   class User: pass
来源：http://uic.jinqigufen.top

PHP:  class User {}
来源：http://vdr.nwbrower.top

JS:   class User {}
来源：http://gjn.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://fhg.shangyingyoupin.top

Java: class User {}
来源：http://aqy.hfpthk.cn

Go:   type User struct { Name string }
来源：http://zbm.zhengqikj.top

Ruby: class User; end
来源：http://ahj.xingfuxueyuan.xyz

C#:   class User {}
来源：http://qud.birdmap.top

[G02] 构造函数
来源：http://vzj.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://deg.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://sef.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://fvf.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://kbo.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://nrb.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://etx.zhijiandao.cn

Ruby: def initialize(name); @name = name; end
来源：http://bmp.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://axg.smart0.xyz

[G03] 实例属性
来源：http://xxo.hywenlv.cn

Py:   self.name = "x"
来源：http://uzm.mhx1999.top

PHP:  public string $name = "x";
来源：http://wni.nanxuanxn.top

JS:   this.name = "x";
来源：http://fpm.sufxvd.cn

TS:   name: string = "x";
来源：http://zxu.ctjpmb.com

Java: private String name;
来源：http://min.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://spk.cucudq.cn

Ruby: @name = "x"
来源：http://qkb.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://prt.sjlbkw.cn

[G04] 定义方法
来源：http://wos.c1oappe.top

Py:   def greet(self): return self.name
来源：http://kth.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nwi.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://lwr.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://kgb.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://yyv.xziqi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ulv.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://qci.yfazqb.com

C#:   public string Greet() => Name;
来源：http://pvi.fktsv.cn

[G05] 继承
来源：http://xwj.hywenlv.cn

Py:   class Admin(User): pass
来源：http://vqk.cashguo.top

PHP:  class Admin extends User {}
来源：http://xjm.guannengcc.top

JS:   class Admin extends User {}
来源：http://znz.vehdjk.com

TS:   class Admin extends User {}
来源：http://tuq.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://fjs.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fzb.zhengqikj.top

Ruby: class Admin < User; end
来源：http://riz.mhx1999.top

C#:   class Admin : User {}
来源：http://dox.haohaochexian.top

[G06] 重写方法
来源：http://gpj.hammf.cn

Py:   def greet(self): return "admin"
来源：http://cmj.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ayh.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://aoq.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://tiq.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://daj.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qwp.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://eal.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://dlc.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://rlx.yfazqb.com

Py:   super().greet()
来源：http://rst.zdqjudy.top

PHP:  parent::greet();
来源：http://lly.yangfankeji.com

JS:   super.greet();
来源：http://kjz.sjlbkw.cn

TS:   super.greet();
来源：http://kkb.xziqi.cn

Java: super.greet();
来源：http://grh.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://afa.shanyushiyangtech.top

Ruby: super
来源：http://jwa.quarkkingdee.top

C#:   base.Greet();
来源：http://ewk.yueranfly.top

[G08] 静态方法与属性
来源：http://mfv.wangshuangyany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vmp.vehdjk.com

PHP:  public static function f() {}
来源：http://nql.pycfn.com

JS:   static f() {}
来源：http://jwd.yvedp.cn

TS:   static f(): void {}
来源：http://xzk.zhongyouzk.top

Java: static void f() {}
来源：http://iib.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://voz.yanxiufei.cn

Ruby: def self.f; end
来源：http://ery.yuxming.cn

C#:   public static void F() {}
来源：http://duj.52xcode.cn

[G09] 接口 / 抽象类
来源：http://cfu.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://zgo.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gkc.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wda.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://org.meibo888.top

Java: interface Shape { double area(); }
来源：http://lbp.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://uzr.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yyk.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://stj.cqqwz.cn

[G10] 访问控制
来源：http://szk.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://lfs.feifeiyinyue.top

PHP:  public / protected / private
来源：http://rfh.zhongyouzk.top

JS:   #private 字段；其余公开
来源：http://fkh.chenzaomai.com

TS:   public / protected / private
来源：http://xav.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://qqz.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nvj.nanxuanxn.top

Ruby: public / protected / private
来源：http://zks.haohaochexian.top

C#:   public / protected / private / internal
来源：http://rxl.smart0.xyz

[G11] getter / setter
来源：http://rtc.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://yuv.sufxvd.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ewj.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://nnr.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://gga.hnqzz.top

Java: public String getName() { return name; }
来源：http://npi.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hkf.dashuyun.cn

Ruby: attr_accessor :name
来源：http://dah.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://nrg.redwolf501.top

[G12] 对象转字符串
来源：http://lku.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://nlu.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ugx.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://guz.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://ast.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://vgt.yangfankeji.com

Go:   func (u User) String() string { return u.Name }
来源：http://iom.smart0.xyz

Ruby: def to_s; @name; end
来源：http://cta.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://chd.yj20258888.top

[G13] 判断对象类型
来源：http://ckz.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://kvx.guannengcc.top

PHP:  $u instanceof User
来源：http://xej.dianchejie.cn

JS:   u instanceof User
来源：http://wru.chenlongwang.top

TS:   u instanceof User
来源：http://fis.tarul.cn

Java: u instanceof User
来源：http://hyy.yj202588.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sth.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://dor.ywan-chungtsiang.top

C#:   u is User
来源：http://xeu.guowangkeji.top

[G14] 数据类 / record
来源：http://lhf.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kwl.nwbrower.top

PHP:  // 用 readonly 属性模拟
来源：http://zlm.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://dkb.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://dlz.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://onv.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://guq.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dun.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://epu.feifeiyinyue.top

[G15] 枚举
来源：http://vyv.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tsh.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xur.cucudq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vab.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kpf.svipenyu.cn

Java: enum Color { RED, GREEN }
来源：http://atw.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kka.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://wpj.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ooh.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://kub.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://woz.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://poa.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://mgq.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://xxy.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://otn.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yid.fehbvm.com

Ruby: obj.instance_variables
来源：http://svh.c1oappe.top

C#:   // 用反射或 System.Text.Json
来源：http://rir.nanxinkj.top

================================================================================
来源：http://xva.uphjek.com

H. 异常与错误处理
来源：http://uee.zhongyouzk.top

================================================================================
来源：http://aqr.zhaomingkeji.xyz

[H01] try / catch 基础
来源：http://fxq.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ihw.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://geq.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://swq.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://omo.shuidangran.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ahl.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yjc.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://osu.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqu.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://yff.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://tcu.shzxlz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zlx.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tpn.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jgh.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://lgc.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vqy.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qrp.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://idp.dianchejie.cn

[H03] 主动抛出异常
来源：http://sui.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://wnv.hywenlv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jwo.cheryme.top

JS:   throw new Error("错误信息");
来源：http://zmg.jyoumei.cn

TS:   throw new Error("错误信息");
来源：http://qut.hnxiangtu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://die.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cbq.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mka.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wgj.jinqigufen.top

[H04] 自定义异常类型
来源：http://mvj.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://vxv.ydzc1.top

PHP:  class MyError extends RuntimeException {}
来源：http://oob.cucudq.cn

JS:   class MyError extends Error {}
来源：http://hoe.pycfn.com

TS:   class MyError extends Error {}
来源：http://ejq.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://hdb.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mih.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://bxq.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://ipb.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://bya.fengsongda.top

Py:   except ValueError as e:
来源：http://deb.ehwqpu.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://foe.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://ies.meibo888.top

TS:   if (e instanceof TypeError) {}
来源：http://htl.nanxinkj.top

Java: catch (IOException | SQLException e) {}
来源：http://xtp.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kfa.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://njp.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hrl.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://aqv.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://iek.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://ags.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://pju.hnxiangtu.top

TS:   obj?.a?.b;  d ?? default
来源：http://zgu.andypj.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzv.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wcg.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://hpc.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://azl.cqqwz.cn

[H07] 断言
来源：http://dnk.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://oih.andypj.xyz

PHP:  assert($x > 0);
来源：http://tiq.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://kqt.pycfn.com

TS:   console.assert(x > 0);
来源：http://lwq.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://vzp.jqgfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xih.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ras.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://fai.zhongyouzk.top

[H08] 获取错误信息与堆栈
来源：http://sgv.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://kav.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://chh.tarul.cn

JS:   e.message;  e.stack
来源：http://rrh.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://pcw.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://amg.ivvv.top

Go:   err.Error()
来源：http://byq.chenlongwang.top

Ruby: e.message;  e.backtrace
来源：http://vlp.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://zku.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://orp.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qef.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qqe.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ndv.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uwj.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mti.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wud.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hai.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vyz.ppjwa.cn

[H10] 资源自动释放
来源：http://uho.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hja.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nty.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://flj.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mqv.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jdy.yj20258.top

Go:   defer f.Close()
来源：http://xbg.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bjg.cashguo.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pbq.sysykeji.top

================================================================================
来源：http://uyg.gogol.net.cn

I. 正则表达式
来源：http://cep.fktsv.cn

================================================================================
来源：http://rkj.zycfv.cn

[I01] 判断是否匹配
来源：http://eus.uphjek.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xyq.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://dmm.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://txt.yongpay.top

TS:   /\d+/.test(s)
来源：http://dxs.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wut.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tkf.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://nty.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fte.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://qkf.sweek.top

Py:   re.findall(r"\d+", s)
来源：http://jid.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hcv.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rqe.uphjek.com

TS:   s.match(/\d+/g)
来源：http://jeg.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://drp.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bsp.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://fqb.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kvy.snrcjt.cn

[I03] 提取捕获分组
来源：http://nqh.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ipr.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fqx.sxryk.cn


<!-- 参考信息 -->