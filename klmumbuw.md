代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://cdt.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://gmz.hywenlv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bmd.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cjq.yuanzhike.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://csm.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://olx.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hqy.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zom.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eqm.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yuz.nwbrower.top

[F11] 复制与移动文件
来源：http://ebv.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qmj.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vsy.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qxy.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrb.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ouw.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zgi.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://thg.jinqigufen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tov.gzhubu.top

[F12] CSV 读写
来源：http://avs.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hnm.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ivj.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sva.nanxuanxn.top

TS:   // 同上
来源：http://hqq.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zrr.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nte.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ogy.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://oqy.ybcxt.top

================================================================================
来源：http://yyu.quarkkingdee.top

G. 面向对象
来源：http://jxc.nanxuanxn.top

================================================================================
来源：http://rtv.zycfv.cn

[G01] 定义类
来源：http://vdj.guannengcc.top

Py:   class User: pass
来源：http://ujb.bjfxy.top

PHP:  class User {}
来源：http://npp.ydzc1.top

JS:   class User {}
来源：http://kdl.uphjek.com

TS:   class User { name: string = ""; }
来源：http://tti.tianlin.xyz

Java: class User {}
来源：http://ouw.dashuyun.cn

Go:   type User struct { Name string }
来源：http://qlk.ywan-chungtsiang.top

Ruby: class User; end
来源：http://krr.tianlin.xyz

C#:   class User {}
来源：http://tqh.hnxiangtu.top

[G02] 构造函数
来源：http://dxs.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://vgu.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://piy.andypj.xyz

JS:   constructor(name) { this.name = name; }
来源：http://oul.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://xht.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://nto.gaohongyu789.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ysy.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://txm.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://tob.zycfv.cn

[G03] 实例属性
来源：http://kjf.52xcode.cn

Py:   self.name = "x"
来源：http://usm.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://rax.hesvh.cn

JS:   this.name = "x";
来源：http://ptp.fengsongda.top

TS:   name: string = "x";
来源：http://bbx.havefunace.top

Java: private String name;
来源：http://zer.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gvx.sufxvd.cn

Ruby: @name = "x"
来源：http://qcw.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://aco.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://cdx.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://len.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vks.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://vnu.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://icj.fehbvm.com

Java: String greet() { return name; }
来源：http://uaw.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hsv.zdqjudy.top

Ruby: def greet; @name; end
来源：http://dwg.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://gke.andypj.xyz

[G05] 继承
来源：http://dcn.havefunace.top

Py:   class Admin(User): pass
来源：http://mri.cashguo.top

PHP:  class Admin extends User {}
来源：http://nvv.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://hhm.bbcook.cn

TS:   class Admin extends User {}
来源：http://mfp.xuanzx.com

Java: class Admin extends User {}
来源：http://vve.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vvf.cucudq.cn

Ruby: class Admin < User; end
来源：http://vce.tarul.cn

C#:   class Admin : User {}
来源：http://mih.jlsjyb.cn

[G06] 重写方法
来源：http://sqt.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://cah.ehwqpu.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jfr.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://iqx.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://xck.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://ntm.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://llj.havefunace.top

Ruby: def greet; "admin"; end
来源：http://wmu.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://rkj.ppjwa.cn

[G07] 调用父类方法
来源：http://ntj.xylfe.cn

Py:   super().greet()
来源：http://esi.fengsongda.top

PHP:  parent::greet();
来源：http://psy.0kj1m.cn

JS:   super.greet();
来源：http://gre.sxryk.cn

TS:   super.greet();
来源：http://apr.sweek.top

Java: super.greet();
来源：http://bvz.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kej.sjlbkw.cn

Ruby: super
来源：http://tnn.ctjpmb.com

C#:   base.Greet();
来源：http://mvz.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://ibg.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aqw.gaohongyu789.top

PHP:  public static function f() {}
来源：http://nwr.zdqjudy.top

JS:   static f() {}
来源：http://wvb.zhixingplan.top

TS:   static f(): void {}
来源：http://wmj.jianghu66.top

Java: static void f() {}
来源：http://wyn.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://amu.vqdsnc.cn

Ruby: def self.f; end
来源：http://qyz.sufxvd.cn

C#:   public static void F() {}
来源：http://ofb.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://uwh.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://qkr.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://yvg.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kzi.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://xej.fzhhl.top

Java: interface Shape { double area(); }
来源：http://udz.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cik.hfpthk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ohj.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://ykj.zdqjudy.top

[G10] 访问控制
来源：http://fiu.dianchejie.cn

Py:   约定 _protected / __private（不强制）
来源：http://kkf.zdbjq.cn

PHP:  public / protected / private
来源：http://jmv.smart0.xyz

JS:   #private 字段；其余公开
来源：http://dgj.pengpengdd.cyou

TS:   public / protected / private
来源：http://ymm.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://iam.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lwz.jqgfzy.top

Ruby: public / protected / private
来源：http://azb.redwolf501.top

C#:   public / protected / private / internal
来源：http://rks.bjfxy.top

[G11] getter / setter
来源：http://gfd.shanyushiyangkeji.top

Py:   @property 与 @x.setter
来源：http://bfo.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vlb.yfazqb.com

JS:   get name() { return this._name; }
来源：http://wsq.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://rzp.wangdashe.top

Java: public String getName() { return name; }
来源：http://jth.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://axh.zhixingplan.top

Ruby: attr_accessor :name
来源：http://nhw.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://yxw.yanxiufei.cn

[G12] 对象转字符串
来源：http://arq.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://bzx.jinqigfzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gax.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://owo.jinqigufen.top

TS:   toString(): string { return this.name; }
来源：http://szb.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://qbw.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nqq.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://cle.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://snt.zdqjudy.top

[G13] 判断对象类型
来源：http://gty.hesvh.cn

Py:   isinstance(u, User)
来源：http://kbd.xinyue.icu

PHP:  $u instanceof User
来源：http://tbz.fktsv.cn

JS:   u instanceof User
来源：http://jtc.yj20258888.top

TS:   u instanceof User
来源：http://yfi.hcnkem.com

Java: u instanceof User
来源：http://jlc.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sio.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://xip.hesvh.cn

C#:   u is User
来源：http://rft.9152youxi.cn

[G14] 数据类 / record
来源：http://roi.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ogf.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://yci.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ket.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://pbt.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://yfl.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://ezj.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://spp.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://zyp.aizwys.cn

[G15] 枚举
来源：http://gyn.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://drs.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lhz.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://knc.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jeb.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://wel.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vux.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://gok.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://foq.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://unt.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://juu.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://euw.tian-w.cn

JS:   Object.entries(obj)
来源：http://fup.andypj.xyz

TS:   Object.entries(obj)
来源：http://pth.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ccs.zhixingplan.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qrl.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://nzj.aizwys.cn

C#:   // 用反射或 System.Text.Json
来源：http://ose.shzxlz.cn

================================================================================
来源：http://xwj.nwbrower.top

H. 异常与错误处理
来源：http://cpv.ydjk.org.cn

================================================================================
来源：http://oih.sjlbkw.cn

[H01] try / catch 基础
来源：http://hwv.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bep.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tgk.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bhl.zhaomingkeji.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://caa.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ygo.ydzc1.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jro.yongpay.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ytj.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ide.hammf.cn

[H02] finally / ensure 收尾
来源：http://kvx.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ysu.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gbb.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kgn.yuxming.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://biw.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://mxc.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ppi.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lwo.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://thv.0kj1m.cn

[H03] 主动抛出异常
来源：http://fvu.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://kgx.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vif.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://eps.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://qjn.shanyushiyangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://edm.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yle.tanke756.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hko.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://msq.sxryk.cn

[H04] 自定义异常类型
来源：http://cuv.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://ipx.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://ugx.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://bhl.tarul.cn

TS:   class MyError extends Error {}
来源：http://pbe.yongpay.top

Java: class MyException extends RuntimeException {}
来源：http://fdc.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dls.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://uuq.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://uhj.ehwqpu.com

[H05] 捕获特定类型
来源：http://asg.shzxlz.cn

Py:   except ValueError as e:
来源：http://dtp.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xhl.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://qlm.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://mcx.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://vez.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dar.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://avh.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lxy.sjlbkw.cn

[H06] 可选值 / 空值安全访问
来源：http://uqd.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://ijb.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://vpi.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://jrn.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://dmj.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://epj.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lbl.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://uqw.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://ymu.zhongyouzk.top

[H07] 断言
来源：http://wzx.ppjwa.cn

Py:   assert x > 0, "必须为正"
来源：http://itb.yj20258888.top

PHP:  assert($x > 0);
来源：http://pav.mhx1999.top

JS:   console.assert(x > 0);
来源：http://jqo.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://jtg.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://qzv.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://spx.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://beo.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://mhw.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://cdk.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://rcn.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oyt.ivvv.top

JS:   e.message;  e.stack
来源：http://thl.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tep.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tvh.kuanghao11.cn

Go:   err.Error()
来源：http://sme.hammf.cn

Ruby: e.message;  e.backtrace
来源：http://syg.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://vtq.jianghu66.top

[H09] 带错误码的异常
来源：http://stv.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zvf.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://nxr.ctjpmb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nwp.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mqh.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hdm.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lop.fzhhl.top

Ruby: raise MyError.new("fail", 500)
来源：http://wxq.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jmy.0kj1m.cn

[H10] 资源自动释放
来源：http://ehc.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mjr.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ost.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vnn.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://icn.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qyz.ppjwa.cn

Go:   defer f.Close()
来源：http://fqn.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://olc.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ctv.ydzc1.top

================================================================================
来源：http://sjv.gotoacloud.top

I. 正则表达式
来源：http://qnr.hesvh.cn

================================================================================
来源：http://yfk.xuanzx.com

[I01] 判断是否匹配
来源：http://ivx.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jba.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://awr.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://vch.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://xhz.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://isn.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xgn.birdmap.top

Ruby: s.match?(/\d+/)
来源：http://ezx.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dng.316326.xyz

[I02] 提取所有匹配
来源：http://pfm.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://beo.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eua.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vqo.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://vfb.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vxw.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://woi.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://kwi.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tjj.cucudq.cn

[I03] 提取捕获分组
来源：http://gen.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://okg.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ovu.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nwa.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ihj.aibaodan.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yhs.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ijk.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fxo.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zuz.ivvv.top

[I04] 正则替换
来源：http://qfs.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fqs.52xcode.cn


<!-- 参考信息 -->