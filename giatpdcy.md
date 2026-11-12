代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fup.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://aqf.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rfb.svipenyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://auz.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jlo.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yzd.bjfxy.top

[F11] 复制与移动文件
来源：http://aol.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zvj.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://giw.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xtv.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wnm.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfp.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://adu.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ohc.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tky.daxiang520.top

[F12] CSV 读写
来源：http://luk.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bjb.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ssw.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://apt.guannengcc.top

TS:   // 同上
来源：http://ats.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iwl.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lvw.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gvm.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hcu.andypj.xyz

================================================================================
来源：http://gyd.jinqigfzy.top

G. 面向对象
来源：http://xib.ybcxt.top

================================================================================
来源：http://ojg.sjlbkw.cn

[G01] 定义类
来源：http://lah.cqqwz.cn

Py:   class User: pass
来源：http://ssw.fengsongda.top

PHP:  class User {}
来源：http://oyc.0kj1m.cn

JS:   class User {}
来源：http://imp.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://cwb.aizwys.cn

Java: class User {}
来源：http://oba.feifeiyinyue.top

Go:   type User struct { Name string }
来源：http://lzl.52xcode.cn

Ruby: class User; end
来源：http://daj.epnwcf.com

C#:   class User {}
来源：http://hgq.hesvh.cn

[G02] 构造函数
来源：http://kcb.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://vzc.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://bda.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://xbk.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://wju.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://zae.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yoc.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://fsm.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://bcz.xuanzx.com

[G03] 实例属性
来源：http://mxn.hnqzz.top

Py:   self.name = "x"
来源：http://bty.xuanzx.com

PHP:  public string $name = "x";
来源：http://rin.gaohongyu789.top

JS:   this.name = "x";
来源：http://cia.ppjwa.cn

TS:   name: string = "x";
来源：http://sar.sysykeji.top

Java: private String name;
来源：http://cmi.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hhv.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://eaf.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jhi.52xcode.cn

[G04] 定义方法
来源：http://tst.hesvh.cn

Py:   def greet(self): return self.name
来源：http://xsv.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hdf.aizwys.cn

JS:   greet() { return this.name; }
来源：http://mau.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://maf.snrcjt.cn

Java: String greet() { return name; }
来源：http://waf.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://mqu.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://zfv.uphjek.com

C#:   public string Greet() => Name;
来源：http://vpi.ctjpmb.com

[G05] 继承
来源：http://vjm.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://zfl.yfazqb.com

PHP:  class Admin extends User {}
来源：http://lfi.yangfankeji.com

JS:   class Admin extends User {}
来源：http://zut.svipenyu.cn

TS:   class Admin extends User {}
来源：http://sji.jinqigufen.top

Java: class Admin extends User {}
来源：http://ryt.zhaomingkeji.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gcm.andypj.xyz

Ruby: class Admin < User; end
来源：http://nwi.gogol.net.cn

C#:   class Admin : User {}
来源：http://wqx.daria6918.cn

[G06] 重写方法
来源：http://trs.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://jmf.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cap.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://qco.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://hyg.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://wyt.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jmn.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://kas.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://xqw.ppjwa.cn

[G07] 调用父类方法
来源：http://ahx.sufxvd.cn

Py:   super().greet()
来源：http://fhl.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://mnt.cqqwz.cn

JS:   super.greet();
来源：http://mns.hfpthk.cn

TS:   super.greet();
来源：http://zrr.xingfuxueyuan.xyz

Java: super.greet();
来源：http://xhf.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qlz.yuanzhike.top

Ruby: super
来源：http://lqb.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://xcw.yueranfly.top

[G08] 静态方法与属性
来源：http://snq.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xwr.zhixingplan.top

PHP:  public static function f() {}
来源：http://yyq.mhx1999.top

JS:   static f() {}
来源：http://taw.cashguo.top

TS:   static f(): void {}
来源：http://xrz.hcnkem.com

Java: static void f() {}
来源：http://lxv.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://smo.fehbvm.com

Ruby: def self.f; end
来源：http://ppo.wangdashe.top

C#:   public static void F() {}
来源：http://pwy.guannengcc.top

[G09] 接口 / 抽象类
来源：http://qlw.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://ktr.xingfuxueyuan.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://wtw.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dhc.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://bkr.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://zqy.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://aqp.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hnm.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://aww.shanyushiyangkeji.top

[G10] 访问控制
来源：http://rih.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://xtu.hfpthk.cn

PHP:  public / protected / private
来源：http://ujn.sxryk.cn

JS:   #private 字段；其余公开
来源：http://fzo.sjlbkw.cn

TS:   public / protected / private
来源：http://lmh.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://plz.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pik.bjfxy.top

Ruby: public / protected / private
来源：http://xwz.dashuyun.cn

C#:   public / protected / private / internal
来源：http://mep.chenjidiqi.icu

[G11] getter / setter
来源：http://wun.meibo888.top

Py:   @property 与 @x.setter
来源：http://egy.shanyushiyangtech.top

PHP:  public function getName(): string { return $this->name; }
来源：http://moc.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://umz.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://pus.havefunace.top

Java: public String getName() { return name; }
来源：http://nfw.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kuv.birdmap.top

Ruby: attr_accessor :name
来源：http://afv.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://abl.nanxinkj.top

[G12] 对象转字符串
来源：http://yzp.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://vda.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://kiz.hcnkem.com

JS:   toString() { return this.name; }
来源：http://adg.vqdsnc.cn

TS:   toString(): string { return this.name; }
来源：http://iuw.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://tmz.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://gqt.cucudq.cn

Ruby: def to_s; @name; end
来源：http://rqm.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://vyz.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://mjk.iojbl.cn

Py:   isinstance(u, User)
来源：http://smg.yj202588.top

PHP:  $u instanceof User
来源：http://omc.nwbrower.top

JS:   u instanceof User
来源：http://nvx.yueranfly.top

TS:   u instanceof User
来源：http://jap.iojbl.cn

Java: u instanceof User
来源：http://fuk.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://heo.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://scb.52xcode.cn

C#:   u is User
来源：http://lnx.feifeiyinyue.top

[G14] 数据类 / record
来源：http://iah.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bmz.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://qyb.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ksa.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://egp.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://cma.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://vti.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wbg.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://knl.wangshuangyany.cn

[G15] 枚举
来源：http://fco.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rze.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://drr.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gqq.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ews.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://blz.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zmo.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://ulu.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rgq.sweek.top

[G16] 对象转数组 / 字典
来源：http://jmn.zycfv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wvt.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://tbw.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://qgj.9152youxi.cn

TS:   Object.entries(obj)
来源：http://pko.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xus.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://whs.pengpengdd.cyou

Ruby: obj.instance_variables
来源：http://kop.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://xhv.9152youxi.cn

================================================================================
来源：http://cym.yj20258888.top

H. 异常与错误处理
来源：http://zqi.xziqi.cn

================================================================================
来源：http://hmp.vehdjk.com

[H01] try / catch 基础
来源：http://rtu.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jbm.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dhg.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jlb.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pdr.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qzb.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jis.tianlin.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mbt.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wjv.zhixingplan.top

[H02] finally / ensure 收尾
来源：http://ihx.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://aji.shuidangran.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://olp.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://edh.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://raj.uphjek.com

Java: try { f(); } finally { cleanup(); }
来源：http://lby.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jfa.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ude.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wqa.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://tpe.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://nbi.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mgo.zhixingplan.top

JS:   throw new Error("错误信息");
来源：http://uer.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://hfb.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hky.52xcode.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kyk.mhx1999.top

Ruby: raise ArgumentError, "错误信息"
来源：http://awb.gzhubu.top

C#:   throw new ArgumentException("错误信息");
来源：http://fcn.ppjwa.cn

[H04] 自定义异常类型
来源：http://zjn.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://cmy.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sks.hesvh.cn

JS:   class MyError extends Error {}
来源：http://pta.wangdashe.top

TS:   class MyError extends Error {}
来源：http://kdo.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://rsc.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xqd.sweek.top

Ruby: class MyError < StandardError; end
来源：http://cjf.xinyue.icu

C#:   class MyException : Exception {}
来源：http://tvu.cdnleiting.top

[H05] 捕获特定类型
来源：http://lux.yangfankeji.com

Py:   except ValueError as e:
来源：http://gis.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uew.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://nhi.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://kfs.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://yhb.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qfi.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://voc.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gow.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://dpf.pycfn.com

Py:   value = d.get("k") or default
来源：http://yli.bjfxy.top

PHP:  $v = $d["k"] ?? null;
来源：http://owe.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pcp.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://emt.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qfc.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://fci.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://ary.sweek.top

C#:   obj?.A?.B ?? default
来源：http://bkn.yj202588.top

[H07] 断言
来源：http://ecz.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://iwt.ehwqpu.com

PHP:  assert($x > 0);
来源：http://qlt.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://jps.yonumen.top

TS:   console.assert(x > 0);
来源：http://het.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://vup.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pho.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gnm.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://hlq.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://boq.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://qlv.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cdw.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://qrv.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wnq.sxryk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eny.zhongyouzk.top

Go:   err.Error()
来源：http://uzi.quarkkingdee.top

Ruby: e.message;  e.backtrace
来源：http://mgg.sxryk.cn

C#:   e.Message;  e.StackTrace
来源：http://wyr.ydjk.org.cn

[H09] 带错误码的异常
来源：http://blz.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hed.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cqd.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fbz.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://luy.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://icl.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mou.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://asz.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gfv.quarkkingdee.top

[H10] 资源自动释放
来源：http://alo.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lcy.uphjek.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pag.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yof.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jju.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ruj.pengpengdd.cyou

Go:   defer f.Close()
来源：http://pvx.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yvk.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tym.yfazqb.com

================================================================================
来源：http://cmv.chenjidiqi.icu

I. 正则表达式
来源：http://dub.jinghuilouyu.cn

================================================================================
来源：http://tyq.yfazqb.com

[I01] 判断是否匹配
来源：http://avi.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kan.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fci.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://gkt.hcnkem.com

TS:   /\d+/.test(s)
来源：http://ufd.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pwd.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hga.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://znn.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lvs.tanke756.top

[I02] 提取所有匹配
来源：http://gpd.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://cnx.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mxi.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ifn.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://apc.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zjs.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sdk.jqgfzy.top

Ruby: s.scan(/\d+/)
来源：http://efo.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nii.nanxuanxn.top

[I03] 提取捕获分组
来源：http://nxy.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aep.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zsy.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nvz.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vpe.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xwr.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sbp.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvk.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igq.mhx1999.top

[I04] 正则替换
来源：http://kex.hnxiangtu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://yqu.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://str.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://zbc.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://zcq.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fid.uphjek.com


<!-- 参考信息 -->