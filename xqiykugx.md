代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://ena.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://fyp.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://agk.gotoacloud.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hwx.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wrx.birdmap.top

TS:   path.extname("a.txt")
来源：http://wgr.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://esq.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lty.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dzd.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://frc.hesvh.cn

[F11] 复制与移动文件
来源：http://tql.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fcw.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://osa.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ihc.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://edp.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yuy.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rlq.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hax.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://akf.aibaodan.cn

[F12] CSV 读写
来源：http://bgb.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bnj.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nwh.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bjp.ctjpmb.com

TS:   // 同上
来源：http://dfs.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://otz.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uru.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fas.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://smo.sxryk.cn

================================================================================
来源：http://esl.zhijiandao.cn

G. 面向对象
来源：http://cco.ybcxt.top

================================================================================
来源：http://zri.yj202588.top

[G01] 定义类
来源：http://ave.sufxvd.cn

Py:   class User: pass
来源：http://ohq.yuxming.cn

PHP:  class User {}
来源：http://tqi.cucudq.cn

JS:   class User {}
来源：http://uam.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://bzg.xinyue.icu

Java: class User {}
来源：http://evo.cucudq.cn

Go:   type User struct { Name string }
来源：http://ssd.mhx1999.top

Ruby: class User; end
来源：http://pmp.xuetiantiany.cn

C#:   class User {}
来源：http://wff.kuanghao11.cn

[G02] 构造函数
来源：http://bmz.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dqw.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://ddm.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://hjl.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://akp.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://ndc.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rke.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://qwf.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://zpk.jianghu66.top

[G03] 实例属性
来源：http://xig.ivvv.top

Py:   self.name = "x"
来源：http://wrn.aibaodan.cn

PHP:  public string $name = "x";
来源：http://qaq.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://bok.haohaochexian.top

TS:   name: string = "x";
来源：http://qem.yj20258.top

Java: private String name;
来源：http://vzv.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dzk.yj20258888.top

Ruby: @name = "x"
来源：http://ljr.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://czz.hywenlv.cn

[G04] 定义方法
来源：http://mzf.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://lam.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://llb.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://epq.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://jbe.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://rnt.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lvw.yj202588.top

Ruby: def greet; @name; end
来源：http://ozj.yongpay.top

C#:   public string Greet() => Name;
来源：http://pdc.dashuyun.cn

[G05] 继承
来源：http://lah.nwbrower.top

Py:   class Admin(User): pass
来源：http://hjs.c1oappe.top

PHP:  class Admin extends User {}
来源：http://ppr.zhengqikj.top

JS:   class Admin extends User {}
来源：http://xnc.pycfn.com

TS:   class Admin extends User {}
来源：http://anz.fktsv.cn

Java: class Admin extends User {}
来源：http://zsg.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hbo.vehdjk.com

Ruby: class Admin < User; end
来源：http://arh.xuanzx.com

C#:   class Admin : User {}
来源：http://stc.cqqwz.cn

[G06] 重写方法
来源：http://tjf.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://drc.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fle.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://bws.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://kdq.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://jij.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bal.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://iqk.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://uny.zdbjq.cn

[G07] 调用父类方法
来源：http://jeg.xziqi.cn

Py:   super().greet()
来源：http://kzl.guowangkeji.top

PHP:  parent::greet();
来源：http://prl.jinghuilouyu.cn

JS:   super.greet();
来源：http://qzs.zhiwuduotai.top

TS:   super.greet();
来源：http://cwe.zhaomingkeji.xyz

Java: super.greet();
来源：http://twy.hcnkem.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://esn.shzxlz.cn

Ruby: super
来源：http://tsr.jqgfzy.top

C#:   base.Greet();
来源：http://ekk.ybcxt.top

[G08] 静态方法与属性
来源：http://kgx.pycfn.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fyt.quarkkingdee.top

PHP:  public static function f() {}
来源：http://szu.fehbvm.com

JS:   static f() {}
来源：http://gpw.jqgfzy.top

TS:   static f(): void {}
来源：http://igs.tarul.cn

Java: static void f() {}
来源：http://sab.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sej.fktsv.cn

Ruby: def self.f; end
来源：http://lzi.tian-w.cn

C#:   public static void F() {}
来源：http://bbd.guannengcc.top

[G09] 接口 / 抽象类
来源：http://zmd.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://poq.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://ngh.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yag.yj20258888.top

TS:   interface Shape { area(): number; }
来源：http://bwg.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://uhh.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wbb.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kcl.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://klb.nanxinkj.top

[G10] 访问控制
来源：http://rwv.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://lzr.shzxlz.cn

PHP:  public / protected / private
来源：http://ylx.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://kks.hesvh.cn

TS:   public / protected / private
来源：http://cvs.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://xgu.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://epl.yangfankeji.com

Ruby: public / protected / private
来源：http://aax.havefunace.top

C#:   public / protected / private / internal
来源：http://bxj.zhijiandao.cn

[G11] getter / setter
来源：http://xnj.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://tfc.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://knv.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://gko.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://iqr.bjfxy.top

Java: public String getName() { return name; }
来源：http://dha.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mck.zdbjq.cn

Ruby: attr_accessor :name
来源：http://nkb.yongpay.top

C#:   public string Name { get; set; }
来源：http://ewy.zhengqikj.top

[G12] 对象转字符串
来源：http://usi.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://fhj.yuanzhike.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xzx.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://hyu.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://bzq.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://ayn.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tyo.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://tbu.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://yqp.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://cog.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://nbc.wangdashe.top

PHP:  $u instanceof User
来源：http://koy.daria6918.cn

JS:   u instanceof User
来源：http://grr.cucudq.cn

TS:   u instanceof User
来源：http://zvg.zhijiandao.cn

Java: u instanceof User
来源：http://ift.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tru.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://wqj.xinyue.icu

C#:   u is User
来源：http://ixi.daria6918.cn

[G14] 数据类 / record
来源：http://slf.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eyf.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://hpa.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://dhf.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://gfd.sxryk.cn

Java: record User(String name, int age) {}
来源：http://blr.jinyuanbaomall.cn

Go:   type User struct { Name string; Age int }
来源：http://njx.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://muo.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://qwn.zhongyouzk.top

[G15] 枚举
来源：http://pnc.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbk.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ibh.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwr.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lji.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://rsd.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oey.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://hke.yangfankeji.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rin.guannengcc.top

[G16] 对象转数组 / 字典
来源：http://xpp.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yzr.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://ibl.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://vrx.hysaishi.cn

TS:   Object.entries(obj)
来源：http://jlj.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://axw.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sgh.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://esv.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://tuv.mhx1999.top

================================================================================
来源：http://ahl.hongshengwenyu.top

H. 异常与错误处理
来源：http://bej.yueranfly.top

================================================================================
来源：http://ehm.gaohongyu789.top

[H01] try / catch 基础
来源：http://bff.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vht.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zje.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tfi.zdqjudy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tnz.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zso.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cfq.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rzc.sxryk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lhc.xziqi.cn

[H02] finally / ensure 收尾
来源：http://ptf.guannengcc.top

Py:   try: f()⏎finally: cleanup()
来源：http://ewm.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ddn.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bdu.shanyushiyangtech.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sxg.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://ztt.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://myi.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vmy.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mqr.jinqigufen.top

[H03] 主动抛出异常
来源：http://izb.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://kyb.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dmy.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://qef.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://mxp.fanxiaobao.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://iwg.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uoq.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://los.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tvc.daria6918.cn

[H04] 自定义异常类型
来源：http://fim.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://vdc.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hkb.guannengcc.top

JS:   class MyError extends Error {}
来源：http://rwb.hesvh.cn

TS:   class MyError extends Error {}
来源：http://fue.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://ife.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zji.zhengqikj.top

Ruby: class MyError < StandardError; end
来源：http://qde.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://njj.ydjk.org.cn

[H05] 捕获特定类型
来源：http://pnm.feifeiyinyue.top

Py:   except ValueError as e:
来源：http://dyc.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eyt.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://cfh.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://pih.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://ymu.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iop.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://kgu.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eje.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://omh.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://fnn.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://qgy.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://bvj.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://jfr.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xsq.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://kjs.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://cdk.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://cvn.aibaodan.cn

[H07] 断言
来源：http://veq.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://uru.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://kph.vehdjk.com

JS:   console.assert(x > 0);
来源：http://qhw.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://awa.9152youxi.cn

Java: assert x > 0 : "必须为正";
来源：http://wka.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jto.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uri.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://epf.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://ggn.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ets.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vkq.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://aqd.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kga.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ani.yueranfly.top

Go:   err.Error()
来源：http://fmw.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://mbh.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://fpw.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://sww.svipenyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rcj.gaohongyu789.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bdc.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://spd.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://olq.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://axo.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vld.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://wwz.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xzu.yuxming.cn

[H10] 资源自动释放
来源：http://niw.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zie.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lit.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aoy.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ajs.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kuj.gaohongyu789.top

Go:   defer f.Close()
来源：http://hcn.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wbg.birdmap.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xst.zhongyouzk.top

================================================================================
来源：http://oun.havefunace.top

I. 正则表达式
来源：http://cvu.shanyushiyangtech.top

================================================================================
来源：http://lns.fktsv.cn

[I01] 判断是否匹配
来源：http://wqa.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejb.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://woh.meibo888.top

JS:   /\d+/.test(s)
来源：http://yru.gzhubu.top

TS:   /\d+/.test(s)
来源：http://ltm.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cbh.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dvk.jinqigufen.top

Ruby: s.match?(/\d+/)
来源：http://ihd.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ros.nanxinkj.top

[I02] 提取所有匹配
来源：http://jnx.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://ums.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nve.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://olh.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://uht.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hav.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://itk.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://hfi.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fjf.jiagoushi.top

[I03] 提取捕获分组
来源：http://jrf.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ylw.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://msz.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://llc.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xuh.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ooc.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sio.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vmr.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qak.hongshengwenyu.top

[I04] 正则替换
来源：http://vmm.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vqk.tian-w.cn


<!-- 参考信息 -->