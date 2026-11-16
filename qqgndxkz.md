代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lbi.shanyushiyangkeji.top

TS:   path.extname("a.txt")
来源：http://lza.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://stf.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zcc.jlsjyb.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://chd.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gxk.zdqjudy.top

[F11] 复制与移动文件
来源：http://tgu.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fok.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhd.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ify.ppjwa.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aor.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kzn.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmh.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bff.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybm.bjfxy.top

[F12] CSV 读写
来源：http://oou.aizwys.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sgx.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://snd.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ctb.zhoulong.xyz

TS:   // 同上
来源：http://hmz.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wpr.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wpm.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjm.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zcd.fzhhl.top

================================================================================
来源：http://scz.epnwcf.com

G. 面向对象
来源：http://hwp.meibo888.top

================================================================================
来源：http://vaw.ctjpmb.com

[G01] 定义类
来源：http://unq.zhixingplan.top

Py:   class User: pass
来源：http://eth.sjlbkw.cn

PHP:  class User {}
来源：http://jyc.gaohongyu789.top

JS:   class User {}
来源：http://bmj.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://zmn.bbcook.cn

Java: class User {}
来源：http://qhh.cucudq.cn

Go:   type User struct { Name string }
来源：http://xft.ybcxt.top

Ruby: class User; end
来源：http://xet.xuanzx.com

C#:   class User {}
来源：http://ftb.quarkkingdee.top

[G02] 构造函数
来源：http://tll.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://exp.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://vwz.chenjidiqi.icu

JS:   constructor(name) { this.name = name; }
来源：http://udl.yonumen.top

TS:   constructor(public name: string) {}
来源：http://aux.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://pik.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xyh.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://qay.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://bvo.cheryme.top

[G03] 实例属性
来源：http://lqj.jqgufenzy.top

Py:   self.name = "x"
来源：http://pjn.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://gqt.birdmap.top

JS:   this.name = "x";
来源：http://wyj.fehbvm.com

TS:   name: string = "x";
来源：http://vyx.hnqzz.top

Java: private String name;
来源：http://rzy.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xja.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://pzb.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://jkm.zhengqikj.top

[G04] 定义方法
来源：http://uoa.fzhhl.top

Py:   def greet(self): return self.name
来源：http://qtx.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cpa.hnqzz.top

JS:   greet() { return this.name; }
来源：http://kfg.zhixingplan.top

TS:   greet(): string { return this.name; }
来源：http://hre.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://mcm.tarul.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xym.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://ipu.birdmap.top

C#:   public string Greet() => Name;
来源：http://prp.yueranfly.top

[G05] 继承
来源：http://ouq.yj20258888.top

Py:   class Admin(User): pass
来源：http://vek.fzhhl.top

PHP:  class Admin extends User {}
来源：http://qwr.xinyue.icu

JS:   class Admin extends User {}
来源：http://kzg.aibaodan.cn

TS:   class Admin extends User {}
来源：http://xjp.vehdjk.com

Java: class Admin extends User {}
来源：http://pqi.hnxiangtu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oee.svipenyu.cn

Ruby: class Admin < User; end
来源：http://kte.fzhhl.top

C#:   class Admin : User {}
来源：http://opp.daria6918.cn

[G06] 重写方法
来源：http://ahw.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://szc.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://tpi.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://jro.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://nre.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://adz.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gcb.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://jah.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://ysg.jyoumei.cn

[G07] 调用父类方法
来源：http://suk.kuanghao11.cn

Py:   super().greet()
来源：http://ziu.jqgufenzy.top

PHP:  parent::greet();
来源：http://buh.cqqwz.cn

JS:   super.greet();
来源：http://fht.vehdjk.com

TS:   super.greet();
来源：http://aba.dianchejie.cn

Java: super.greet();
来源：http://dew.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vsd.jlsjyb.cn

Ruby: super
来源：http://fzj.sjlbkw.cn

C#:   base.Greet();
来源：http://xto.shzxlz.cn

[G08] 静态方法与属性
来源：http://nya.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eya.jinqigufen.top

PHP:  public static function f() {}
来源：http://btr.hnxiangtu.top

JS:   static f() {}
来源：http://rga.0kj1m.cn

TS:   static f(): void {}
来源：http://oec.yangfankeji.com

Java: static void f() {}
来源：http://xvb.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hkh.nanxuanxn.top

Ruby: def self.f; end
来源：http://uxo.svipenyu.cn

C#:   public static void F() {}
来源：http://sij.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://was.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://lhr.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://xcz.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://ikw.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://zcx.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://oci.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://fee.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blf.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://apg.zdqjudy.top

[G10] 访问控制
来源：http://pkb.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://hvt.uphjek.com

PHP:  public / protected / private
来源：http://tfw.fktsv.cn

JS:   #private 字段；其余公开
来源：http://ylv.shuidangran.top

TS:   public / protected / private
来源：http://esu.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://ahr.hnxiangtu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fqf.xinyue.icu

Ruby: public / protected / private
来源：http://ght.epnwcf.com

C#:   public / protected / private / internal
来源：http://ris.svipenyu.cn

[G11] getter / setter
来源：http://zfh.fzhhl.top

Py:   @property 与 @x.setter
来源：http://oni.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sup.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://irm.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://jox.hfpthk.cn

Java: public String getName() { return name; }
来源：http://npb.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xdv.jinqigufen.top

Ruby: attr_accessor :name
来源：http://cin.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://ryq.zdqjudy.top

[G12] 对象转字符串
来源：http://osl.shzxlz.cn

Py:   def __str__(self): return self.name
来源：http://pzf.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xji.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://wnu.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://nel.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://shn.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sug.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://tgf.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://sve.zhongyouzk.top

[G13] 判断对象类型
来源：http://yfc.ehwqpu.com

Py:   isinstance(u, User)
来源：http://ldk.ydzc1.top

PHP:  $u instanceof User
来源：http://gyl.nanxinkj.top

JS:   u instanceof User
来源：http://qth.shuidangran.top

TS:   u instanceof User
来源：http://pho.jqgufenzy.top

Java: u instanceof User
来源：http://vzs.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ovt.zycfv.cn

Ruby: u.is_a?(User)
来源：http://vmr.tarul.cn

C#:   u is User
来源：http://vbn.yj20258888.top

[G14] 数据类 / record
来源：http://xed.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vun.jinyuanbaomall.cn

PHP:  // 用 readonly 属性模拟
来源：http://ety.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://duk.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://cxx.fanxiaobao.xyz

Java: record User(String name, int age) {}
来源：http://lak.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://xmj.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ivy.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://ril.redwolf501.top

[G15] 枚举
来源：http://udd.xziqi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qwf.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zuq.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rob.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vyi.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://pbw.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nff.hnxiangtu.top

Ruby: Color = %i[red green].freeze
来源：http://nag.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pja.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://tuf.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kkd.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://irj.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://tcu.wangdashe.top

TS:   Object.entries(obj)
来源：http://cwe.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nfd.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ivs.uphjek.com

Ruby: obj.instance_variables
来源：http://jth.meibo888.top

C#:   // 用反射或 System.Text.Json
来源：http://srv.ivvv.top

================================================================================
来源：http://wng.hnqzz.top

H. 异常与错误处理
来源：http://eqy.hfpthk.cn

================================================================================
来源：http://vse.redwolf501.top

[H01] try / catch 基础
来源：http://qes.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tze.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dik.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eox.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sjx.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://znv.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xgm.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ktb.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bjp.xinyue.icu

[H02] finally / ensure 收尾
来源：http://pho.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ity.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ckk.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aho.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tls.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://abt.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eiq.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gyh.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zat.sweek.top

[H03] 主动抛出异常
来源：http://qym.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://uls.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rdf.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://hfg.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://xoq.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://chg.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zmt.guowangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nik.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kkp.tarul.cn

[H04] 自定义异常类型
来源：http://yxe.tanke756.top

Py:   class MyError(Exception): pass
来源：http://rmv.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lxv.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://rfr.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://qum.haohaochexian.top

Java: class MyException extends RuntimeException {}
来源：http://cpn.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lap.yuanzhike.top

Ruby: class MyError < StandardError; end
来源：http://gbu.hammf.cn

C#:   class MyException : Exception {}
来源：http://qlf.zhoulong.xyz

[H05] 捕获特定类型
来源：http://lhp.sweek.top

Py:   except ValueError as e:
来源：http://xbo.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xul.dianchejie.cn

JS:   if (e instanceof TypeError) {}
来源：http://vgg.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://gvm.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://gtq.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xdt.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://hmy.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://efz.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://avp.ydzc1.top

Py:   value = d.get("k") or default
来源：http://ltk.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mou.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://lvh.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://aad.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jwy.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xqj.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://qlb.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://cad.jinyuanbaomall.cn

[H07] 断言
来源：http://law.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://tvj.jyoumei.cn

PHP:  assert($x > 0);
来源：http://cka.hnqzz.top

JS:   console.assert(x > 0);
来源：http://iea.guannengcc.top

TS:   console.assert(x > 0);
来源：http://wny.xziqi.cn

Java: assert x > 0 : "必须为正";
来源：http://isx.andypj.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gcw.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://jko.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://lzb.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://ezo.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://wxe.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hhv.jinqigufen.top

JS:   e.message;  e.stack
来源：http://fdy.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zee.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ytr.xylfe.cn

Go:   err.Error()
来源：http://cep.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://qkc.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://eod.chenzaomai.com

[H09] 带错误码的异常
来源：http://qsu.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ntm.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qlm.zdbjq.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ifo.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dcu.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://unt.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uiw.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oub.xylfe.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kah.nanxinkj.top

[H10] 资源自动释放
来源：http://ddq.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zno.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lnx.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://asd.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvu.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nyw.zhengqikj.top

Go:   defer f.Close()
来源：http://cnb.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oxf.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://itg.fehbvm.com

================================================================================
来源：http://rxd.tian-w.cn

I. 正则表达式
来源：http://zmb.zhaomingkeji.xyz

================================================================================
来源：http://ldr.shuidangran.top

[I01] 判断是否匹配
来源：http://eml.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zim.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://odl.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://qhu.yfazqb.com

TS:   /\d+/.test(s)
来源：http://ocl.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mop.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hjd.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://oua.nwbrower.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uia.gogol.net.cn

[I02] 提取所有匹配
来源：http://ava.zdbjq.cn

Py:   re.findall(r"\d+", s)
来源：http://hni.ywan-chungtsiang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pne.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qtg.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://jny.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://thz.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://phn.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://gcu.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xoj.aibaodan.cn

[I03] 提取捕获分组
来源：http://lbh.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zik.xuetiantiany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://feu.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nws.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qnc.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wuk.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ehb.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lcw.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zvi.jinyuanbaomall.cn

[I04] 正则替换
来源：http://vae.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fvx.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zth.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://kkq.yangfankeji.com

TS:   s.replace(/\d+/g, "#")
来源：http://hjw.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fdg.hesvh.cn


<!-- 参考信息 -->