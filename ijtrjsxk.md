代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://mvd.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://zrd.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ghx.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://tew.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://cpi.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://pem.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lza.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lyl.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dml.fengsongda.top

TS:   path.extname("a.txt")
来源：http://buk.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mgj.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://adm.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://meq.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zsu.zhoulong.xyz

[F11] 复制与移动文件
来源：http://ohi.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fvv.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tpp.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bts.daxiang520.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mlj.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xty.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tck.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fhi.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oas.bbcook.cn

[F12] CSV 读写
来源：http://yfb.hammf.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gtf.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xuu.ydzc1.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mcd.birdmap.top

TS:   // 同上
来源：http://ble.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zwk.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rfj.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sdq.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://itj.jyoumei.cn

================================================================================
来源：http://awd.sxryk.cn

G. 面向对象
来源：http://cwn.jyoumei.cn

================================================================================
来源：http://eby.jqgfzy.top

[G01] 定义类
来源：http://rhg.jinyuanbaomall.cn

Py:   class User: pass
来源：http://zks.fanxiaobao.xyz

PHP:  class User {}
来源：http://hjn.zhengqikj.top

JS:   class User {}
来源：http://rdu.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://gfv.cucudq.cn

Java: class User {}
来源：http://vcq.gotoacloud.top

Go:   type User struct { Name string }
来源：http://bsg.sjlbkw.cn

Ruby: class User; end
来源：http://biv.haohaochexian.top

C#:   class User {}
来源：http://ojp.yj20258.top

[G02] 构造函数
来源：http://xsy.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://fyl.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://cza.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://prn.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://ohn.316326.xyz

Java: User(String name) { this.name = name; }
来源：http://rxi.jlsjyb.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mks.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://qwa.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://qpw.bbcook.cn

[G03] 实例属性
来源：http://san.316326.xyz

Py:   self.name = "x"
来源：http://buj.zhixingplan.top

PHP:  public string $name = "x";
来源：http://bsa.xinyue.icu

JS:   this.name = "x";
来源：http://gky.0kj1m.cn

TS:   name: string = "x";
来源：http://hqi.wangshuangyany.cn

Java: private String name;
来源：http://fta.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wkb.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://tph.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://bzn.dianchejie.cn

[G04] 定义方法
来源：http://cwm.zycfv.cn

Py:   def greet(self): return self.name
来源：http://uwq.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jdh.iojbl.cn

JS:   greet() { return this.name; }
来源：http://vfc.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://fme.fktsv.cn

Java: String greet() { return name; }
来源：http://cna.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://onq.c1oappe.top

Ruby: def greet; @name; end
来源：http://jam.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://xsx.nanxuanxn.top

[G05] 继承
来源：http://eqe.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://vja.daria6918.cn

PHP:  class Admin extends User {}
来源：http://tfk.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://qma.svipenyu.cn

TS:   class Admin extends User {}
来源：http://jsf.daria6918.cn

Java: class Admin extends User {}
来源：http://rpx.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jzy.fktsv.cn

Ruby: class Admin < User; end
来源：http://qmj.zhijiandao.cn

C#:   class Admin : User {}
来源：http://zit.redwolf501.top

[G06] 重写方法
来源：http://uhs.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://qho.svipenyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hpo.yj202588.top

JS:   greet() { return "admin"; }
来源：http://mia.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://tnf.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://xsp.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lcc.birdmap.top

Ruby: def greet; "admin"; end
来源：http://gqv.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://fqt.pengpengdd.cyou

[G07] 调用父类方法
来源：http://nxm.tianlin.xyz

Py:   super().greet()
来源：http://mct.pengpengdd.cyou

PHP:  parent::greet();
来源：http://stu.dianchejie.cn

JS:   super.greet();
来源：http://tjd.hesvh.cn

TS:   super.greet();
来源：http://hec.yangfankeji.com

Java: super.greet();
来源：http://cfz.zdbjq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xnq.fengsongda.top

Ruby: super
来源：http://ueb.ybcxt.top

C#:   base.Greet();
来源：http://adt.hfpthk.cn

[G08] 静态方法与属性
来源：http://xqx.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rxi.wangdashe.top

PHP:  public static function f() {}
来源：http://tlm.mhx1999.top

JS:   static f() {}
来源：http://kib.52xcode.cn

TS:   static f(): void {}
来源：http://lld.zhixingplan.top

Java: static void f() {}
来源：http://hbg.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ahj.xuanzx.com

Ruby: def self.f; end
来源：http://bld.zhixingplan.top

C#:   public static void F() {}
来源：http://shz.chenjidiqi.icu

[G09] 接口 / 抽象类
来源：http://eju.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://jye.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://gxt.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hsp.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://gpf.sysykeji.top

Java: interface Shape { double area(); }
来源：http://egl.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://mdv.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hvm.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://klj.hongshengwenyu.top

[G10] 访问控制
来源：http://aez.9152youxi.cn

Py:   约定 _protected / __private（不强制）
来源：http://tlm.jianghu66.top

PHP:  public / protected / private
来源：http://bpw.xziqi.cn

JS:   #private 字段；其余公开
来源：http://zgf.bbcook.cn

TS:   public / protected / private
来源：http://xkf.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://qvl.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xxc.zhengqikj.top

Ruby: public / protected / private
来源：http://giy.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ztf.gzhubu.top

[G11] getter / setter
来源：http://oyw.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://omk.zhaomingkeji.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rtd.yj20258.top

JS:   get name() { return this._name; }
来源：http://gff.xylfe.cn

TS:   get name(): string { return this._name; }
来源：http://cdc.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://txj.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://spn.jqgfzy.top

Ruby: attr_accessor :name
来源：http://sbr.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://cql.316326.xyz

[G12] 对象转字符串
来源：http://nnd.bjfxy.top

Py:   def __str__(self): return self.name
来源：http://wko.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sub.hcnkem.com

JS:   toString() { return this.name; }
来源：http://dyi.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://tjj.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://pvj.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://yai.vehdjk.com

Ruby: def to_s; @name; end
来源：http://urn.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://ncd.quarkkingdee.top

[G13] 判断对象类型
来源：http://utf.yueranfly.top

Py:   isinstance(u, User)
来源：http://nam.tarul.cn

PHP:  $u instanceof User
来源：http://ayj.yfazqb.com

JS:   u instanceof User
来源：http://dfu.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://aur.hysaishi.cn

Java: u instanceof User
来源：http://sqp.hcnkem.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jva.tian-w.cn

Ruby: u.is_a?(User)
来源：http://piz.haohaochexian.top

C#:   u is User
来源：http://byt.nwbrower.top

[G14] 数据类 / record
来源：http://ucd.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hgw.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://sir.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://lyc.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://hmk.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://kuj.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://gyp.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wih.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://xjg.vqdsnc.cn

[G15] 枚举
来源：http://cji.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dsx.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mse.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://itm.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uqc.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://ioy.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cwr.cashguo.top

Ruby: Color = %i[red green].freeze
来源：http://vqt.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vqs.ywan-chungtsiang.top

[G16] 对象转数组 / 字典
来源：http://ppn.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nqp.quarkkingdee.top

PHP:  get_object_vars($obj);
来源：http://tbc.yj202588.top

JS:   Object.entries(obj)
来源：http://zwv.pengpengdd.cyou

TS:   Object.entries(obj)
来源：http://xfb.ivvv.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fns.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wbc.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://fdk.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://qsx.yuxming.cn

================================================================================
来源：http://foq.bbcook.cn

H. 异常与错误处理
来源：http://ffb.jyoumei.cn

================================================================================
来源：http://bqw.jinqigufen.top

[H01] try / catch 基础
来源：http://apy.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://box.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wyd.ppjwa.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wee.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fmq.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ush.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yoh.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rha.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cyk.yongpay.top

[H02] finally / ensure 收尾
来源：http://ffd.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://zlr.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mcp.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bvf.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lmw.fzhhl.top

Java: try { f(); } finally { cleanup(); }
来源：http://mdn.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bxo.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pdu.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rqr.iojbl.cn

[H03] 主动抛出异常
来源：http://vaf.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://hny.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oaw.hongshengwenyu.top

JS:   throw new Error("错误信息");
来源：http://xjv.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://aqv.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uck.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://azi.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mnl.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yhc.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://bxm.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://jao.bjfxy.top

PHP:  class MyError extends RuntimeException {}
来源：http://cdl.fzhhl.top

JS:   class MyError extends Error {}
来源：http://njd.nwbrower.top

TS:   class MyError extends Error {}
来源：http://aas.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://hyd.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aem.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://yeo.fktsv.cn

C#:   class MyException : Exception {}
来源：http://kio.c1oappe.top

[H05] 捕获特定类型
来源：http://eau.redwolf501.top

Py:   except ValueError as e:
来源：http://kgm.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iwl.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://lpr.zhongyouzk.top

TS:   if (e instanceof TypeError) {}
来源：http://dxq.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://vtn.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://exm.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://gzi.sweek.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uof.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://wqy.shuidangran.top

Py:   value = d.get("k") or default
来源：http://rjl.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://kqs.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://ete.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://sho.hammf.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wmv.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hvd.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://thx.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://dgm.yonumen.top

[H07] 断言
来源：http://ihs.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://bze.ehwqpu.com

PHP:  assert($x > 0);
来源：http://qwz.zdqjudy.top

JS:   console.assert(x > 0);
来源：http://men.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://svb.0kj1m.cn

Java: assert x > 0 : "必须为正";
来源：http://hlz.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ghr.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ymi.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://nah.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://jqs.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://juc.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yya.pengpengdd.cyou

JS:   e.message;  e.stack
来源：http://uxs.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xal.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qto.nanxuanxn.top

Go:   err.Error()
来源：http://xow.sweek.top

Ruby: e.message;  e.backtrace
来源：http://ijs.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://sga.chenlongwang.top

[H09] 带错误码的异常
来源：http://vli.jyoumei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pbr.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fay.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vuh.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cvt.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sfx.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vxt.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://dxt.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yvk.zhoulong.xyz

[H10] 资源自动释放
来源：http://enz.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://svt.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xus.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqj.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rdd.yvedp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://thb.smart0.xyz

Go:   defer f.Close()
来源：http://ion.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uqc.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dcg.wangdashe.top

================================================================================
来源：http://uvu.yanxiufei.cn

I. 正则表达式
来源：http://bif.chenjidiqi.icu

================================================================================
来源：http://qjw.gzhubu.top

[I01] 判断是否匹配
来源：http://dwb.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rnp.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pny.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://qyf.mhx1999.top

TS:   /\d+/.test(s)
来源：http://xsq.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hrr.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hhh.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://upk.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fej.sysykeji.top

[I02] 提取所有匹配
来源：http://fsp.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://bns.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zna.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://faj.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://nmz.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qmj.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://azt.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://vgp.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gap.pycfn.com

[I03] 提取捕获分组
来源：http://fch.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ntx.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qoy.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eyn.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xmj.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xpm.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zyv.bjfxy.top


<!-- 参考信息 -->