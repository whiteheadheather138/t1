代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mtc.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bry.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lab.ywan-chungtsiang.top

[F08] 遍历目录
来源：http://kdf.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mub.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://reb.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://rxm.jlsjyb.cn

TS:   fs.readdirSync("dir")
来源：http://unh.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jiw.andypj.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://lov.sysykeji.top

Ruby: Dir.children("dir")
来源：http://uun.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://fod.pengpengdd.cyou

[F09] 获取文件大小
来源：http://eto.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://qqw.birdmap.top

PHP:  filesize("a.txt");
来源：http://rvi.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://ogo.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://wgj.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://oxv.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jgs.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://zpe.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://dlr.guannengcc.top

[F10] 取文件扩展名 / 文件名
来源：http://ocl.zycfv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tdl.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vey.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vxq.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://tjl.daria6918.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xhh.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://obn.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://suy.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qct.andypj.xyz

[F11] 复制与移动文件
来源：http://atz.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qhn.chenjidiqi.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://grq.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uzu.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tuj.yonumen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cqz.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ida.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mfm.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://znb.jqgufenzy.top

[F12] CSV 读写
来源：http://jjs.xuanzx.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zhz.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://isk.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ddz.sysykeji.top

TS:   // 同上
来源：http://cmz.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kam.jqgfzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rua.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ime.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rkq.cdnleiting.top

================================================================================
来源：http://sej.chenzaomai.com

G. 面向对象
来源：http://bva.316326.xyz

================================================================================
来源：http://ezq.ywan-chungtsiang.top

[G01] 定义类
来源：http://apx.sxryk.cn

Py:   class User: pass
来源：http://uym.hysaishi.cn

PHP:  class User {}
来源：http://ybn.gogol.net.cn

JS:   class User {}
来源：http://kaj.havefunace.top

TS:   class User { name: string = ""; }
来源：http://orz.ivvv.top

Java: class User {}
来源：http://krv.vehdjk.com

Go:   type User struct { Name string }
来源：http://rft.bbcook.cn

Ruby: class User; end
来源：http://foi.shuidangran.top

C#:   class User {}
来源：http://she.0kj1m.cn

[G02] 构造函数
来源：http://hpc.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://xwj.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://zmn.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://obs.sweek.top

TS:   constructor(public name: string) {}
来源：http://fda.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://hzf.xinyue.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tfj.cqqwz.cn

Ruby: def initialize(name); @name = name; end
来源：http://aiw.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://dbn.shuidangran.top

[G03] 实例属性
来源：http://onp.0kj1m.cn

Py:   self.name = "x"
来源：http://qjy.meibo888.top

PHP:  public string $name = "x";
来源：http://bbm.xziqi.cn

JS:   this.name = "x";
来源：http://xyr.iojbl.cn

TS:   name: string = "x";
来源：http://kls.nanxinkj.top

Java: private String name;
来源：http://fya.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gwl.fzhhl.top

Ruby: @name = "x"
来源：http://oox.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://vjp.fanxiaobao.xyz

[G04] 定义方法
来源：http://wux.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://lxk.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xkn.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://npi.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://qyx.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://pff.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gpk.shzxlz.cn

Ruby: def greet; @name; end
来源：http://uie.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://yrq.tarul.cn

[G05] 继承
来源：http://les.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://biz.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://nxv.zdbjq.cn

JS:   class Admin extends User {}
来源：http://jnd.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://rfo.dianchejie.cn

Java: class Admin extends User {}
来源：http://eqg.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qld.sweek.top

Ruby: class Admin < User; end
来源：http://hje.tanke756.top

C#:   class Admin : User {}
来源：http://gma.yueranfly.top

[G06] 重写方法
来源：http://ifs.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://nre.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pcx.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://him.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://jfh.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://yyx.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tgi.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://csz.hesvh.cn

C#:   public override string Greet() => "admin";
来源：http://iut.havefunace.top

[G07] 调用父类方法
来源：http://dsk.jqgufenzy.top

Py:   super().greet()
来源：http://vfv.zhongyouzk.top

PHP:  parent::greet();
来源：http://egm.shanyushiyangkeji.top

JS:   super.greet();
来源：http://aoe.hnxiangtu.top

TS:   super.greet();
来源：http://qjf.xuetiantiany.cn

Java: super.greet();
来源：http://bkh.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fyw.hnxiangtu.top

Ruby: super
来源：http://cyc.yueranfly.top

C#:   base.Greet();
来源：http://xiq.ydzc1.top

[G08] 静态方法与属性
来源：http://fmy.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ywt.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://uwj.sxryk.cn

JS:   static f() {}
来源：http://igt.tian-w.cn

TS:   static f(): void {}
来源：http://otj.wangshuangyany.cn

Java: static void f() {}
来源：http://jqh.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oyu.fehbvm.com

Ruby: def self.f; end
来源：http://egi.vehdjk.com

C#:   public static void F() {}
来源：http://bxw.birdmap.top

[G09] 接口 / 抽象类
来源：http://fmw.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://axj.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rir.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://wsn.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://zvk.fzhhl.top

Java: interface Shape { double area(); }
来源：http://olx.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://cvj.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://frn.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://seq.gaohongyu789.top

[G10] 访问控制
来源：http://grp.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://bzk.gzhubu.top

PHP:  public / protected / private
来源：http://wyd.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://hjb.haohaochexian.top

TS:   public / protected / private
来源：http://nfa.havefunace.top

Java: public / protected / private / 默认包级
来源：http://fhw.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oam.wangdashe.top

Ruby: public / protected / private
来源：http://gai.snrcjt.cn

C#:   public / protected / private / internal
来源：http://jkx.zhaomingkeji.xyz

[G11] getter / setter
来源：http://gmr.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://rbe.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ska.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://bcf.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://mqi.bjfxy.top

Java: public String getName() { return name; }
来源：http://xeu.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://qgl.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://hwf.andypj.xyz

C#:   public string Name { get; set; }
来源：http://yee.xuetiantiany.cn

[G12] 对象转字符串
来源：http://ajo.uphjek.com

Py:   def __str__(self): return self.name
来源：http://ard.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kif.hesvh.cn

JS:   toString() { return this.name; }
来源：http://wwy.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://zbe.smart0.xyz

Java: @Override public String toString() { return name; }
来源：http://pel.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://vcy.hammf.cn

Ruby: def to_s; @name; end
来源：http://zpr.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://kpv.xuanzx.com

[G13] 判断对象类型
来源：http://rix.zdbjq.cn

Py:   isinstance(u, User)
来源：http://xhn.jinqigufen.top

PHP:  $u instanceof User
来源：http://lfp.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://tsy.ydjk.org.cn

TS:   u instanceof User
来源：http://bom.ivvv.top

Java: u instanceof User
来源：http://hyh.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gjx.316326.xyz

Ruby: u.is_a?(User)
来源：http://ykv.zhoulong.xyz

C#:   u is User
来源：http://ugz.sxryk.cn

[G14] 数据类 / record
来源：http://bcj.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dzm.sweek.top

PHP:  // 用 readonly 属性模拟
来源：http://fse.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://evy.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://pmr.vehdjk.com

Java: record User(String name, int age) {}
来源：http://ocu.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://pue.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rmh.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://fku.shanyushiyangtech.top

[G15] 枚举
来源：http://ahx.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dko.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://shl.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://buf.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://grv.aibaodan.cn

Java: enum Color { RED, GREEN }
来源：http://ftn.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aej.iojbl.cn

Ruby: Color = %i[red green].freeze
来源：http://ruo.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hpt.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://qnh.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pmp.hammf.cn

PHP:  get_object_vars($obj);
来源：http://igc.guannengcc.top

JS:   Object.entries(obj)
来源：http://jre.jinyuanbaomall.cn

TS:   Object.entries(obj)
来源：http://jmi.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gkx.pengpengdd.cyou

Go:   // 手写转换，或用 mapstructure 库
来源：http://enz.tianlin.xyz

Ruby: obj.instance_variables
来源：http://csp.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://tiz.tarul.cn

================================================================================
来源：http://otk.sysykeji.top

H. 异常与错误处理
来源：http://fax.hnqzz.top

================================================================================
来源：http://udm.epnwcf.com

[H01] try / catch 基础
来源：http://lra.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xnj.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qkv.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cnt.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xiq.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iaz.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tov.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ndw.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qrk.havefunace.top

[H02] finally / ensure 收尾
来源：http://zzg.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://zba.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fue.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://goh.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://fbc.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://mfr.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://aoi.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xwd.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vso.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://lpe.tian-w.cn

Py:   raise ValueError("错误信息")
来源：http://pfy.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pks.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://neu.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://ams.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ajw.yanxiufei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mqb.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rpx.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://esv.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://nul.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://gei.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xjg.xuanzx.com

JS:   class MyError extends Error {}
来源：http://men.nanxinkj.top

TS:   class MyError extends Error {}
来源：http://zmq.nwbrower.top

Java: class MyException extends RuntimeException {}
来源：http://rgl.ehwqpu.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://okb.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://qtd.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://yja.shanyushiyangtech.top

[H05] 捕获特定类型
来源：http://bva.hammf.cn

Py:   except ValueError as e:
来源：http://vzb.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhl.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://ygs.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://jte.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://dud.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://owi.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://qzs.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sjq.ivvv.top

[H06] 可选值 / 空值安全访问
来源：http://hve.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://mtw.hywenlv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://utf.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://cke.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lsw.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://say.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rdh.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://dwi.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://uop.shangyingyoupin.top

[H07] 断言
来源：http://jlm.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://qnm.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://kti.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://rci.mhx1999.top

TS:   console.assert(x > 0);
来源：http://djj.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://rhx.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nbx.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rce.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://gwh.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://sgz.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://erb.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://odh.xylfe.cn

JS:   e.message;  e.stack
来源：http://iiz.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfw.316326.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ynp.yongpay.top

Go:   err.Error()
来源：http://iyw.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://zif.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://rwg.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://zkl.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://inw.sysykeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ufz.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sqr.andypj.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://djq.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://csv.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fmx.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://ffw.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://tfm.svipenyu.cn

[H10] 资源自动释放
来源：http://mps.jinghuilouyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bce.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vke.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mrg.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jpm.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xvo.feifeiyinyue.top

Go:   defer f.Close()
来源：http://fsm.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgt.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cgy.hysaishi.cn

================================================================================
来源：http://wmj.ctjpmb.com

I. 正则表达式
来源：http://bfh.zhiwuduotai.top

================================================================================
来源：http://jdu.yj20258.top

[I01] 判断是否匹配
来源：http://gnt.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xan.jinqigfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://jdh.shuidangran.top

JS:   /\d+/.test(s)
来源：http://grc.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://azb.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gvo.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kku.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://iao.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://klo.sweek.top


<!-- 参考信息 -->