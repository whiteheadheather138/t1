代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://aoh.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://eey.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hbv.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://grq.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rlk.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://aoj.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jqn.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sjp.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mpp.ctjpmb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fuy.shuidangran.top

[F11] 复制与移动文件
来源：http://jsd.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gbn.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uvj.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxo.hammf.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aqa.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gkn.aizwys.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hec.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vno.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ggo.quarkkingdee.top

[F12] CSV 读写
来源：http://ugx.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kmz.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://giv.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://thv.hnqzz.top

TS:   // 同上
来源：http://wnd.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sqm.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bit.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ioz.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://zva.kuanghao11.cn

================================================================================
来源：http://xgw.yangfankeji.com

G. 面向对象
来源：http://pds.jinqigufen.top

================================================================================
来源：http://rdy.yj202588.top

[G01] 定义类
来源：http://tva.jianghu66.top

Py:   class User: pass
来源：http://bza.sjlbkw.cn

PHP:  class User {}
来源：http://ppo.jinqigufen.top

JS:   class User {}
来源：http://nme.jinghuilouyu.cn

TS:   class User { name: string = ""; }
来源：http://lcf.jinyuanbaomall.cn

Java: class User {}
来源：http://sso.birdmap.top

Go:   type User struct { Name string }
来源：http://vdu.gzhubu.top

Ruby: class User; end
来源：http://mht.hongshengwenyu.top

C#:   class User {}
来源：http://uaq.daxiang520.top

[G02] 构造函数
来源：http://tkv.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://vqc.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://jkp.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://xhl.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://cxj.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://kot.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lal.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://yhs.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://xuk.gzhubu.top

[G03] 实例属性
来源：http://erp.daxiang520.top

Py:   self.name = "x"
来源：http://msm.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://zzw.ybcxt.top

JS:   this.name = "x";
来源：http://bum.yongpay.top

TS:   name: string = "x";
来源：http://jmt.zdbjq.cn

Java: private String name;
来源：http://ral.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mva.yvedp.cn

Ruby: @name = "x"
来源：http://qqy.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://jbl.zhaomingkeji.xyz

[G04] 定义方法
来源：http://nuw.sxryk.cn

Py:   def greet(self): return self.name
来源：http://hjt.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qvi.zhijiandao.cn

JS:   greet() { return this.name; }
来源：http://qjv.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://vvy.bbcook.cn

Java: String greet() { return name; }
来源：http://quh.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ehj.bjfxy.top

Ruby: def greet; @name; end
来源：http://imc.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://aua.sweek.top

[G05] 继承
来源：http://jzb.mhx1999.top

Py:   class Admin(User): pass
来源：http://uss.wangdashe.top

PHP:  class Admin extends User {}
来源：http://mlr.hfpthk.cn

JS:   class Admin extends User {}
来源：http://jex.ivvv.top

TS:   class Admin extends User {}
来源：http://qsd.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://cww.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hid.52xcode.cn

Ruby: class Admin < User; end
来源：http://idb.yuanzhike.top

C#:   class Admin : User {}
来源：http://lvn.andypj.xyz

[G06] 重写方法
来源：http://ubi.cashguo.top

Py:   def greet(self): return "admin"
来源：http://gyf.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gso.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://lds.hesvh.cn

TS:   greet(): string { return "admin"; }
来源：http://sfq.yuxming.cn

Java: @Override String greet() { return "admin"; }
来源：http://sir.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qrf.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://qnt.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://qiq.fehbvm.com

[G07] 调用父类方法
来源：http://qif.zdbjq.cn

Py:   super().greet()
来源：http://dpc.feifeiyinyue.top

PHP:  parent::greet();
来源：http://uvp.zhoulong.xyz

JS:   super.greet();
来源：http://lpr.jqgufenzy.top

TS:   super.greet();
来源：http://kml.xziqi.cn

Java: super.greet();
来源：http://eev.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aku.quarkkingdee.top

Ruby: super
来源：http://fir.wangshuangyany.cn

C#:   base.Greet();
来源：http://byu.yj202588.top

[G08] 静态方法与属性
来源：http://fyk.vqdsnc.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lhs.tanke756.top

PHP:  public static function f() {}
来源：http://tbw.hysaishi.cn

JS:   static f() {}
来源：http://bsj.birdmap.top

TS:   static f(): void {}
来源：http://teq.xylfe.cn

Java: static void f() {}
来源：http://sey.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jjc.quarkkingdee.top

Ruby: def self.f; end
来源：http://hbr.xziqi.cn

C#:   public static void F() {}
来源：http://xip.xingfuxueyuan.xyz

[G09] 接口 / 抽象类
来源：http://hdk.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://nih.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://zwr.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qco.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://rek.ydzc1.top

Java: interface Shape { double area(); }
来源：http://are.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://yyx.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zsq.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://fpw.vehdjk.com

[G10] 访问控制
来源：http://ltt.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://mtt.aibaodan.cn

PHP:  public / protected / private
来源：http://sdj.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://jsl.cucudq.cn

TS:   public / protected / private
来源：http://qyk.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://rut.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jbx.jinqigufen.top

Ruby: public / protected / private
来源：http://ceb.nanxinkj.top

C#:   public / protected / private / internal
来源：http://obi.chenjidiqi.icu

[G11] getter / setter
来源：http://sfl.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://mgb.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vlg.yuxming.cn

JS:   get name() { return this._name; }
来源：http://wsw.quarkkingdee.top

TS:   get name(): string { return this._name; }
来源：http://dvs.wangdashe.top

Java: public String getName() { return name; }
来源：http://grd.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qjj.chenzaomai.com

Ruby: attr_accessor :name
来源：http://iqs.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://oll.gaohongyu789.top

[G12] 对象转字符串
来源：http://kww.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://hyj.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://adn.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://lcj.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://xze.sxryk.cn

Java: @Override public String toString() { return name; }
来源：http://kgz.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://iuz.havefunace.top

Ruby: def to_s; @name; end
来源：http://bbl.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://fnr.ydzc1.top

[G13] 判断对象类型
来源：http://pns.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://zvq.gaohongyu789.top

PHP:  $u instanceof User
来源：http://jap.yanxiufei.cn

JS:   u instanceof User
来源：http://clf.hywenlv.cn

TS:   u instanceof User
来源：http://ibb.fanxiaobao.xyz

Java: u instanceof User
来源：http://nml.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hem.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://faz.xziqi.cn

C#:   u is User
来源：http://vdl.aibaodan.cn

[G14] 数据类 / record
来源：http://cmy.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zna.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://wak.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://hrf.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://zrw.hcnkem.com

Java: record User(String name, int age) {}
来源：http://gmn.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://fuo.aibaodan.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gmb.hywenlv.cn

C#:   record User(string Name, int Age);
来源：http://cto.aizwys.cn

[G15] 枚举
来源：http://rqt.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://atn.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zzb.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nul.sjlbkw.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nqv.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://pxw.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bjn.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://opq.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rig.tarul.cn

[G16] 对象转数组 / 字典
来源：http://qaj.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wiv.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://wdg.ybcxt.top

JS:   Object.entries(obj)
来源：http://ymd.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://lat.guannengcc.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wxn.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://gmj.daria6918.cn

Ruby: obj.instance_variables
来源：http://ffh.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://hjk.shuidangran.top

================================================================================
来源：http://ews.epnwcf.com

H. 异常与错误处理
来源：http://cyu.kuanghao11.cn

================================================================================
来源：http://sjv.cucudq.cn

[H01] try / catch 基础
来源：http://xse.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jmy.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oxl.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xpi.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lho.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zer.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uqs.sjlbkw.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ylh.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bgd.316326.xyz

[H02] finally / ensure 收尾
来源：http://cqw.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://eag.sysykeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pcq.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gxv.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ohd.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://hmq.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://arr.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pbg.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dnx.yangfankeji.com

[H03] 主动抛出异常
来源：http://dnh.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://qfx.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nup.ivvv.top

JS:   throw new Error("错误信息");
来源：http://xfv.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://cgo.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jcm.guannengcc.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lbm.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://irr.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://tze.bjfxy.top

[H04] 自定义异常类型
来源：http://uwc.bjfxy.top

Py:   class MyError(Exception): pass
来源：http://sjl.yj202588.top

PHP:  class MyError extends RuntimeException {}
来源：http://yoj.shanyushiyangkeji.top

JS:   class MyError extends Error {}
来源：http://gkn.ybcxt.top

TS:   class MyError extends Error {}
来源：http://okw.jqgufenzy.top

Java: class MyException extends RuntimeException {}
来源：http://dls.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gcf.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://bft.quarkkingdee.top

C#:   class MyException : Exception {}
来源：http://yoy.tanke756.top

[H05] 捕获特定类型
来源：http://tju.xylfe.cn

Py:   except ValueError as e:
来源：http://gyb.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cye.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://myh.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://aio.jqgufenzy.top

Java: catch (IOException | SQLException e) {}
来源：http://sph.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xqv.zhengqikj.top

Ruby: rescue ArgumentError => e
来源：http://acz.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mvy.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://jae.ywan-chungtsiang.top

Py:   value = d.get("k") or default
来源：http://beq.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ays.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://tdz.yanxiufei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vyt.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wvh.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://agu.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://jrr.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://hza.snrcjt.cn

[H07] 断言
来源：http://spp.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://rqb.nanxinkj.top

PHP:  assert($x > 0);
来源：http://fju.316326.xyz

JS:   console.assert(x > 0);
来源：http://qil.andypj.xyz

TS:   console.assert(x > 0);
来源：http://gbk.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://cwt.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bmm.yuanzhike.top

Ruby: raise "必须为正" unless x > 0
来源：http://bad.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://our.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://rsa.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://wgp.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://deb.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://eig.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ovf.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://edv.xziqi.cn

Go:   err.Error()
来源：http://mjy.iojbl.cn

Ruby: e.message;  e.backtrace
来源：http://lsl.ybcxt.top

C#:   e.Message;  e.StackTrace
来源：http://kug.ybcxt.top

[H09] 带错误码的异常
来源：http://nfo.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://waj.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://whz.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lmk.yanxiufei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fof.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdb.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uxf.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://qih.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ljf.nanxuanxn.top

[H10] 资源自动释放
来源：http://nlp.epnwcf.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pme.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ebe.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oxu.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ntf.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oet.cdnleiting.top

Go:   defer f.Close()
来源：http://zim.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fqf.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vjx.havefunace.top

================================================================================
来源：http://cug.hysaishi.cn

I. 正则表达式
来源：http://olk.yueranfly.top

================================================================================
来源：http://tkv.birdmap.top

[I01] 判断是否匹配
来源：http://wfh.xinyue.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xfm.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://hib.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://zbm.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://yfh.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fvq.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oag.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://xlr.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://spz.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://wmg.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://acs.jlsjyb.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hjx.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ska.sweek.top

TS:   s.match(/\d+/g)
来源：http://phd.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://max.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tua.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://xjc.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mbh.vehdjk.com

[I03] 提取捕获分组
来源：http://ktx.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wdu.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ngz.jyoumei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ftq.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wvl.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qfk.sweek.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sbr.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gbb.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qdj.shuidangran.top

[I04] 正则替换
来源：http://twt.zhoulong.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://eim.jianghu66.top


<!-- 参考信息 -->