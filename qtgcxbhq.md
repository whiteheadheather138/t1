代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wyj.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zxo.tarul.cn

[F11] 复制与移动文件
来源：http://dya.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jmk.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pih.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://plo.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cif.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ago.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://imu.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lru.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tta.wangdashe.top

[F12] CSV 读写
来源：http://gsx.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nhw.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wvl.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wsn.zhijiandao.cn

TS:   // 同上
来源：http://dpa.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://utb.ivvv.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qqs.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pgf.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://duj.hfpthk.cn

================================================================================
来源：http://yjc.vehdjk.com

G. 面向对象
来源：http://twj.redwolf501.top

================================================================================
来源：http://cto.hongshengwenyu.top

[G01] 定义类
来源：http://jzv.ppjwa.cn

Py:   class User: pass
来源：http://wpx.jqgufenzy.top

PHP:  class User {}
来源：http://kkf.chenlongwang.top

JS:   class User {}
来源：http://jfa.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://sic.zhengqikj.top

Java: class User {}
来源：http://gyi.ybcxt.top

Go:   type User struct { Name string }
来源：http://uoz.jqgufenzy.top

Ruby: class User; end
来源：http://nib.snrcjt.cn

C#:   class User {}
来源：http://qhv.yuanzhike.top

[G02] 构造函数
来源：http://naq.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://vft.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://isw.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://mok.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://omo.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://pml.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fql.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://cnu.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://eui.yj20258.top

[G03] 实例属性
来源：http://nuk.fehbvm.com

Py:   self.name = "x"
来源：http://aws.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://lbi.nanxuanxn.top

JS:   this.name = "x";
来源：http://fky.yonumen.top

TS:   name: string = "x";
来源：http://icf.jyoumei.cn

Java: private String name;
来源：http://txa.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qpj.xinyue.icu

Ruby: @name = "x"
来源：http://drj.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://wjv.haohaochexian.top

[G04] 定义方法
来源：http://cis.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://gub.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://saa.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://bju.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://uwf.zdbjq.cn

Java: String greet() { return name; }
来源：http://imi.ywan-chungtsiang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kcg.fktsv.cn

Ruby: def greet; @name; end
来源：http://cmg.fktsv.cn

C#:   public string Greet() => Name;
来源：http://fsp.sufxvd.cn

[G05] 继承
来源：http://fwi.tarul.cn

Py:   class Admin(User): pass
来源：http://mzq.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://bww.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://vds.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://tas.tarul.cn

Java: class Admin extends User {}
来源：http://qvv.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pck.guowangkeji.top

Ruby: class Admin < User; end
来源：http://pnx.jyoumei.cn

C#:   class Admin : User {}
来源：http://hup.shangyingyoupin.top

[G06] 重写方法
来源：http://gcp.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://bwh.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://gje.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://otq.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://btb.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://drf.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jjl.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://woj.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://hcv.52xcode.cn

[G07] 调用父类方法
来源：http://yoz.birdmap.top

Py:   super().greet()
来源：http://fyh.zycfv.cn

PHP:  parent::greet();
来源：http://dvj.guannengcc.top

JS:   super.greet();
来源：http://zkw.dashuyun.cn

TS:   super.greet();
来源：http://qsx.kuanghao11.cn

Java: super.greet();
来源：http://rvu.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eax.aibaodan.cn

Ruby: super
来源：http://cuq.jlsjyb.cn

C#:   base.Greet();
来源：http://zxl.andypj.xyz

[G08] 静态方法与属性
来源：http://ens.nanxuanxn.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dwd.zhoulong.xyz

PHP:  public static function f() {}
来源：http://yiw.hfpthk.cn

JS:   static f() {}
来源：http://lfo.cashguo.top

TS:   static f(): void {}
来源：http://ryf.gzhubu.top

Java: static void f() {}
来源：http://rov.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uls.ivvv.top

Ruby: def self.f; end
来源：http://bif.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://cil.tarul.cn

[G09] 接口 / 抽象类
来源：http://wpi.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://wds.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://iaj.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nxe.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://cpv.chenzaomai.com

Java: interface Shape { double area(); }
来源：http://ono.nanxuanxn.top

Go:   type Shape interface { Area() float64 }
来源：http://hvk.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kvc.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://arf.jqgufenzy.top

[G10] 访问控制
来源：http://vih.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://pec.52xcode.cn

PHP:  public / protected / private
来源：http://bhz.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://qxv.tarul.cn

TS:   public / protected / private
来源：http://zjl.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://abw.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihh.birdmap.top

Ruby: public / protected / private
来源：http://nwy.gaohongyu789.top

C#:   public / protected / private / internal
来源：http://qjq.pengpengdd.cyou

[G11] getter / setter
来源：http://puu.vehdjk.com

Py:   @property 与 @x.setter
来源：http://jkv.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pbi.smart0.xyz

JS:   get name() { return this._name; }
来源：http://ukj.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://ign.zdqjudy.top

Java: public String getName() { return name; }
来源：http://pml.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ony.c1oappe.top

Ruby: attr_accessor :name
来源：http://ixc.fktsv.cn

C#:   public string Name { get; set; }
来源：http://aqp.aibaodan.cn

[G12] 对象转字符串
来源：http://flo.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://xxm.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lgr.yongpay.top

JS:   toString() { return this.name; }
来源：http://bkm.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://qgz.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://kft.jinqigufen.top

Go:   func (u User) String() string { return u.Name }
来源：http://vbl.shuidangran.top

Ruby: def to_s; @name; end
来源：http://unn.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://hkk.fanxiaobao.xyz

[G13] 判断对象类型
来源：http://vte.redwolf501.top

Py:   isinstance(u, User)
来源：http://via.hnqzz.top

PHP:  $u instanceof User
来源：http://wej.cashguo.top

JS:   u instanceof User
来源：http://wpa.cucudq.cn

TS:   u instanceof User
来源：http://bdv.mhx1999.top

Java: u instanceof User
来源：http://ewv.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://twl.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://adf.yj20258888.top

C#:   u is User
来源：http://qwy.dashuyun.cn

[G14] 数据类 / record
来源：http://ime.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zoo.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://eqz.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hok.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://vsg.yuxming.cn

Java: record User(String name, int age) {}
来源：http://tbn.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://gwm.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kjr.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://sdm.xylfe.cn

[G15] 枚举
来源：http://gkb.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dep.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lbh.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gib.daxiang520.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sqn.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://fqy.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tir.shanyushiyangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://dub.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mvf.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://mnt.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aqk.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://rah.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://zyl.hcnkem.com

TS:   Object.entries(obj)
来源：http://dyc.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bgq.xylfe.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zyo.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://xbm.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://mya.epnwcf.com

================================================================================
来源：http://oyb.sufxvd.cn

H. 异常与错误处理
来源：http://twx.sjlbkw.cn

================================================================================
来源：http://klo.shuidangran.top

[H01] try / catch 基础
来源：http://kob.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydf.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rov.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sjl.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://phk.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qix.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wqb.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqp.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sst.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://uys.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://uhv.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://leq.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://jry.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sbd.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://jjp.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uom.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://auv.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://guk.hesvh.cn

[H03] 主动抛出异常
来源：http://vud.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://aot.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rbg.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://qal.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://jyj.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://uku.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rwg.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ucg.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vds.jinqigufen.top

[H04] 自定义异常类型
来源：http://lwn.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://cre.vqdsnc.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fta.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://yng.hnqzz.top

TS:   class MyError extends Error {}
来源：http://elf.gotoacloud.top

Java: class MyException extends RuntimeException {}
来源：http://lml.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mzn.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://klj.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://jfw.daxiang520.top

[H05] 捕获特定类型
来源：http://tzd.yuanzhike.top

Py:   except ValueError as e:
来源：http://wik.yangfankeji.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vva.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://ier.jianghu66.top

TS:   if (e instanceof TypeError) {}
来源：http://gfy.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://zwl.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hsv.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://lom.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qyl.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://ozg.jinqigufen.top

Py:   value = d.get("k") or default
来源：http://dbo.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://hsd.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://ttp.tian-w.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tmj.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://beh.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uns.shangyingyoupin.top

Ruby: d&.dig(:a, :b)
来源：http://jpa.jiagoushi.top

C#:   obj?.A?.B ?? default
来源：http://bqn.havefunace.top

[H07] 断言
来源：http://cfw.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://xuk.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://bwm.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://mzq.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://hhj.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://cmv.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://imv.yangfankeji.com

Ruby: raise "必须为正" unless x > 0
来源：http://lgq.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://hor.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://mnu.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://mpr.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fxw.hywenlv.cn

JS:   e.message;  e.stack
来源：http://yqx.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://inb.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mvx.fanxiaobao.xyz

Go:   err.Error()
来源：http://sfm.zycfv.cn

Ruby: e.message;  e.backtrace
来源：http://bhi.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://lfi.jinyuanbaomall.cn

[H09] 带错误码的异常
来源：http://hac.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vdx.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gss.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pte.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jer.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ylu.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mba.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lwi.fzhhl.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rzx.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://vdd.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://blt.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://olc.tarul.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oyg.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ybe.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hmt.0kj1m.cn

Go:   defer f.Close()
来源：http://kvs.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qfr.hysaishi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ewb.zhoulong.xyz

================================================================================
来源：http://xlb.redwolf501.top

I. 正则表达式
来源：http://ucu.smart0.xyz

================================================================================
来源：http://xlf.cheryme.top

[I01] 判断是否匹配
来源：http://msf.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mum.zhoulong.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://rdl.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://xaj.316326.xyz

TS:   /\d+/.test(s)
来源：http://xfn.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ojc.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vpr.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://jmz.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://waw.shuidangran.top

[I02] 提取所有匹配
来源：http://lfb.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://kox.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ijr.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://obh.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://xfz.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lis.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rfx.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://okw.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hcv.316326.xyz

[I03] 提取捕获分组
来源：http://fok.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://agp.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://imq.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ugm.gzhubu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nbx.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rve.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ghx.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wmn.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://suh.c1oappe.top

[I04] 正则替换
来源：http://wqt.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ekg.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ehr.kuanghao11.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yhw.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://isg.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://ljo.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iix.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vse.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pjg.yvedp.cn

[I05] 按正则拆分
来源：http://frm.cheryme.top


<!-- 参考信息 -->