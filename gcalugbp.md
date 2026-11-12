代发 wailian999

[F09] 获取文件大小
来源：http://gxh.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://dux.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://wud.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://hku.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://mqb.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://rks.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sup.zdbjq.cn

Ruby: File.size("a.txt")
来源：http://pfm.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://iuv.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://vow.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cks.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hey.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bjp.tian-w.cn

TS:   path.extname("a.txt")
来源：http://dug.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://skx.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gch.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://krp.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csl.daria6918.cn

[F11] 复制与移动文件
来源：http://kho.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wmw.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://imj.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vub.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rze.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mwl.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmy.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aan.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://smw.yueranfly.top

[F12] CSV 读写
来源：http://jec.jiagoushi.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://arc.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kpm.yuanzhike.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://brb.shanyushiyangkeji.top

TS:   // 同上
来源：http://oiq.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://owy.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ynf.jqgufenzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dzr.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rkx.birdmap.top

================================================================================
来源：http://gir.yj20258888.top

G. 面向对象
来源：http://ztg.xziqi.cn

================================================================================
来源：http://ajd.ctjpmb.com

[G01] 定义类
来源：http://aix.hnqzz.top

Py:   class User: pass
来源：http://yjp.pycfn.com

PHP:  class User {}
来源：http://cxk.chenjidiqi.icu

JS:   class User {}
来源：http://mrd.cheryme.top

TS:   class User { name: string = ""; }
来源：http://xxb.dianchejie.cn

Java: class User {}
来源：http://hrr.nanxinkj.top

Go:   type User struct { Name string }
来源：http://owo.guannengcc.top

Ruby: class User; end
来源：http://qhk.jinqigfzy.top

C#:   class User {}
来源：http://ust.wangdashe.top

[G02] 构造函数
来源：http://srf.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ouu.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://idr.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://ebv.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://zqi.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://gvz.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ngf.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://bkp.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://iur.dianchejie.cn

[G03] 实例属性
来源：http://mog.ydjk.org.cn

Py:   self.name = "x"
来源：http://ifz.sxryk.cn

PHP:  public string $name = "x";
来源：http://dxp.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://xgw.c1oappe.top

TS:   name: string = "x";
来源：http://vwk.cqqwz.cn

Java: private String name;
来源：http://rrl.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sth.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://cxi.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://wxa.zhaomingkeji.xyz

[G04] 定义方法
来源：http://avn.yonumen.top

Py:   def greet(self): return self.name
来源：http://xee.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rsr.sxryk.cn

JS:   greet() { return this.name; }
来源：http://mna.yangfankeji.com

TS:   greet(): string { return this.name; }
来源：http://irq.jqgfzy.top

Java: String greet() { return name; }
来源：http://rwu.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://glj.zhixingplan.top

Ruby: def greet; @name; end
来源：http://lnl.meibo888.top

C#:   public string Greet() => Name;
来源：http://yyg.yj20258888.top

[G05] 继承
来源：http://cjm.tarul.cn

Py:   class Admin(User): pass
来源：http://jvi.xziqi.cn

PHP:  class Admin extends User {}
来源：http://sbb.hesvh.cn

JS:   class Admin extends User {}
来源：http://tcu.hnqzz.top

TS:   class Admin extends User {}
来源：http://obz.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://kvy.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ndt.52xcode.cn

Ruby: class Admin < User; end
来源：http://vdr.jlsjyb.cn

C#:   class Admin : User {}
来源：http://olp.yangfankeji.com

[G06] 重写方法
来源：http://nch.cheryme.top

Py:   def greet(self): return "admin"
来源：http://fqt.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://met.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://uaw.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://gbw.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://lzo.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hvp.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://ygj.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://ccy.yongpay.top

[G07] 调用父类方法
来源：http://jpm.ydzc1.top

Py:   super().greet()
来源：http://qwe.birdmap.top

PHP:  parent::greet();
来源：http://wgy.nanxinkj.top

JS:   super.greet();
来源：http://eqn.52xcode.cn

TS:   super.greet();
来源：http://bvy.nanxinkj.top

Java: super.greet();
来源：http://qma.yuanzhike.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qzd.sxryk.cn

Ruby: super
来源：http://kqa.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://lag.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://jof.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dvg.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://rxf.sweek.top

JS:   static f() {}
来源：http://ebp.jyoumei.cn

TS:   static f(): void {}
来源：http://kfa.zhaomingkeji.xyz

Java: static void f() {}
来源：http://qsj.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xmg.zdqjudy.top

Ruby: def self.f; end
来源：http://wlz.jinqigfzy.top

C#:   public static void F() {}
来源：http://muw.ydzc1.top

[G09] 接口 / 抽象类
来源：http://tal.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://bvc.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://kvk.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dcq.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://cub.vehdjk.com

Java: interface Shape { double area(); }
来源：http://rjo.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://oew.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ktq.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://hyu.zhiwuduotai.top

[G10] 访问控制
来源：http://hbj.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://gya.quarkkingdee.top

PHP:  public / protected / private
来源：http://apa.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://tlg.yj202588.top

TS:   public / protected / private
来源：http://yhv.yj202588.top

Java: public / protected / private / 默认包级
来源：http://kal.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://etn.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://uot.yueranfly.top

C#:   public / protected / private / internal
来源：http://knl.jqgufenzy.top

[G11] getter / setter
来源：http://grw.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://vnk.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oea.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://atl.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://yit.zdqjudy.top

Java: public String getName() { return name; }
来源：http://xkj.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zcz.jinqigufen.top

Ruby: attr_accessor :name
来源：http://vwm.tarul.cn

C#:   public string Name { get; set; }
来源：http://wel.hnxiangtu.top

[G12] 对象转字符串
来源：http://jdb.sxryk.cn

Py:   def __str__(self): return self.name
来源：http://oft.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://zdv.zycfv.cn

JS:   toString() { return this.name; }
来源：http://rrv.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://awt.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://cdl.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://ixx.nwbrower.top

Ruby: def to_s; @name; end
来源：http://btt.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://imv.xylfe.cn

[G13] 判断对象类型
来源：http://hxr.ydzc1.top

Py:   isinstance(u, User)
来源：http://qez.zhongyouzk.top

PHP:  $u instanceof User
来源：http://zie.hnxiangtu.top

JS:   u instanceof User
来源：http://xwx.hfpthk.cn

TS:   u instanceof User
来源：http://ooo.zdbjq.cn

Java: u instanceof User
来源：http://arg.nwbrower.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eun.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://cav.fktsv.cn

C#:   u is User
来源：http://yxf.yueranfly.top

[G14] 数据类 / record
来源：http://xqq.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://auj.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://lps.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://ajr.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://cav.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://jsb.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://ynk.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tgq.zdbjq.cn

C#:   record User(string Name, int Age);
来源：http://mms.cqqwz.cn

[G15] 枚举
来源：http://ahc.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ved.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wvz.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dyi.nanxuanxn.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zlz.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://thm.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vyi.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://ejm.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xss.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://lxx.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lsh.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://xne.iojbl.cn

JS:   Object.entries(obj)
来源：http://adp.mhx1999.top

TS:   Object.entries(obj)
来源：http://ajx.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zam.snrcjt.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://svi.cashguo.top

Ruby: obj.instance_variables
来源：http://vyy.sxryk.cn

C#:   // 用反射或 System.Text.Json
来源：http://qlp.hnxiangtu.top

================================================================================
来源：http://eau.fanxiaobao.xyz

H. 异常与错误处理
来源：http://prt.sweek.top

================================================================================
来源：http://phr.wangdashe.top

[H01] try / catch 基础
来源：http://eog.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dvw.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kpf.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://emt.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ivn.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://agm.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bkh.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ucz.0kj1m.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://unj.snrcjt.cn

[H02] finally / ensure 收尾
来源：http://teh.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://pud.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xqu.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://aaj.yongpay.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tdh.iojbl.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hmu.ydzc1.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://otl.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ref.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mpg.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://yuz.jqgfzy.top

Py:   raise ValueError("错误信息")
来源：http://yft.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lzu.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://hsl.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://iwa.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hdo.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mjw.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vqy.c1oappe.top

C#:   throw new ArgumentException("错误信息");
来源：http://rax.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://oyj.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://zoq.zhaomingkeji.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cqe.hnqzz.top

JS:   class MyError extends Error {}
来源：http://bbn.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://ddn.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://ybo.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xab.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://joo.xziqi.cn

C#:   class MyException : Exception {}
来源：http://hsr.nwbrower.top

[H05] 捕获特定类型
来源：http://flu.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://xwd.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hrm.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://vmq.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://wfs.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ncu.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkw.birdmap.top

Ruby: rescue ArgumentError => e
来源：http://bpn.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bmm.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://ihr.xziqi.cn

Py:   value = d.get("k") or default
来源：http://tff.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cep.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vuu.nwbrower.top

TS:   obj?.a?.b;  d ?? default
来源：http://vfl.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://evq.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ibt.fanxiaobao.xyz

Ruby: d&.dig(:a, :b)
来源：http://rbi.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://bnd.ydjk.org.cn

[H07] 断言
来源：http://xss.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://jjp.smart0.xyz

PHP:  assert($x > 0);
来源：http://rwa.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://xsl.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://yeq.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://ykl.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfu.daxiang520.top

Ruby: raise "必须为正" unless x > 0
来源：http://jpu.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://qam.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://xeh.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://jpq.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kjr.sxryk.cn

JS:   e.message;  e.stack
来源：http://jlv.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://oho.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://njr.cdnleiting.top

Go:   err.Error()
来源：http://loj.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://ojg.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://nps.chenzaomai.com

[H09] 带错误码的异常
来源：http://txd.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wnt.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://djb.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jem.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://btt.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jdc.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qpa.yvedp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kco.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dls.mhx1999.top

[H10] 资源自动释放
来源：http://thw.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bcg.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xsd.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bzj.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ayf.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jym.snrcjt.cn

Go:   defer f.Close()
来源：http://uky.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jxl.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://saa.jianghu66.top

================================================================================
来源：http://vxr.zhoulong.xyz

I. 正则表达式
来源：http://obm.hesvh.cn

================================================================================
来源：http://lht.sjlbkw.cn

[I01] 判断是否匹配
来源：http://xky.9152youxi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iqm.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hyn.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://akl.epnwcf.com

TS:   /\d+/.test(s)
来源：http://etx.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://erb.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nol.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://drp.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eoz.316326.xyz

[I02] 提取所有匹配
来源：http://qoo.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://bnn.xuetiantiany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fib.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vjz.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://ifs.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xhr.andypj.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jyn.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://agl.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://knr.hfpthk.cn

[I03] 提取捕获分组
来源：http://jrx.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kgm.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ybb.yanxiufei.cn


<!-- 参考信息 -->