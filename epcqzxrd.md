代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vzw.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://geh.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ijg.uphjek.com

[F08] 遍历目录
来源：http://kcc.hfpthk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oow.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wxb.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://syi.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://ufw.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xub.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zpu.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://pen.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://vnl.xylfe.cn

[F09] 获取文件大小
来源：http://orb.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://krk.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://sfz.gzhubu.top

JS:   fs.statSync("a.txt").size
来源：http://fcj.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://vxe.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://olp.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://khg.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://afd.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://yrw.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://wyv.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nob.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oxq.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://niu.iojbl.cn

TS:   path.extname("a.txt")
来源：http://uno.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uuy.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://smy.ivvv.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hpe.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://boc.xuanzx.com

[F11] 复制与移动文件
来源：http://zig.c1oappe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pyu.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tql.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ihv.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ovf.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hil.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wht.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ale.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttz.shanyushiyangtech.top

[F12] CSV 读写
来源：http://yaa.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wss.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uyc.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vbc.0kj1m.cn

TS:   // 同上
来源：http://gpg.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hjh.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cut.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dmk.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kae.jinyuanbaomall.cn

================================================================================
来源：http://oba.fanxiaobao.xyz

G. 面向对象
来源：http://zzu.yanxiufei.cn

================================================================================
来源：http://pel.kuanghao11.cn

[G01] 定义类
来源：http://ikv.hnxiangtu.top

Py:   class User: pass
来源：http://nyc.ehwqpu.com

PHP:  class User {}
来源：http://buv.vehdjk.com

JS:   class User {}
来源：http://fxm.52xcode.cn

TS:   class User { name: string = ""; }
来源：http://zlq.shuidangran.top

Java: class User {}
来源：http://gim.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://jon.jiagoushi.top

Ruby: class User; end
来源：http://oup.guannengcc.top

C#:   class User {}
来源：http://ozv.kuanghao11.cn

[G02] 构造函数
来源：http://avx.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://lzl.wangdashe.top

PHP:  public function __construct(public string $name) {}
来源：http://itl.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://ydw.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://bmd.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://jdv.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tpw.c1oappe.top

Ruby: def initialize(name); @name = name; end
来源：http://dok.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://mct.yfazqb.com

[G03] 实例属性
来源：http://ijq.9152youxi.cn

Py:   self.name = "x"
来源：http://lhx.yuxming.cn

PHP:  public string $name = "x";
来源：http://gpu.fengsongda.top

JS:   this.name = "x";
来源：http://wej.xuanzx.com

TS:   name: string = "x";
来源：http://eep.sjlbkw.cn

Java: private String name;
来源：http://kqw.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dgl.xylfe.cn

Ruby: @name = "x"
来源：http://dwz.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://abc.xylfe.cn

[G04] 定义方法
来源：http://wjy.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://usf.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kga.yonumen.top

JS:   greet() { return this.name; }
来源：http://qoe.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://hyk.gotoacloud.top

Java: String greet() { return name; }
来源：http://hvf.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lyu.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://ahb.wangdashe.top

C#:   public string Greet() => Name;
来源：http://lkt.9152youxi.cn

[G05] 继承
来源：http://qcr.xziqi.cn

Py:   class Admin(User): pass
来源：http://iud.iojbl.cn

PHP:  class Admin extends User {}
来源：http://imk.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://nne.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://rsx.zhongyouzk.top

Java: class Admin extends User {}
来源：http://qkk.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cin.shzxlz.cn

Ruby: class Admin < User; end
来源：http://rxf.yongpay.top

C#:   class Admin : User {}
来源：http://ket.ctjpmb.com

[G06] 重写方法
来源：http://pvm.yj20258.top

Py:   def greet(self): return "admin"
来源：http://sji.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ftk.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://iwz.fzhhl.top

TS:   greet(): string { return "admin"; }
来源：http://loa.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://ixc.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cnz.cheryme.top

Ruby: def greet; "admin"; end
来源：http://lmo.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://dro.cdnleiting.top

[G07] 调用父类方法
来源：http://yfb.havefunace.top

Py:   super().greet()
来源：http://nlf.zhongyouzk.top

PHP:  parent::greet();
来源：http://rnx.guannengcc.top

JS:   super.greet();
来源：http://uao.ydjk.org.cn

TS:   super.greet();
来源：http://vzi.mhx1999.top

Java: super.greet();
来源：http://vzw.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nfu.andypj.xyz

Ruby: super
来源：http://dxy.sufxvd.cn

C#:   base.Greet();
来源：http://mil.zhongyouzk.top

[G08] 静态方法与属性
来源：http://jco.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ixk.ybcxt.top

PHP:  public static function f() {}
来源：http://ssp.smart0.xyz

JS:   static f() {}
来源：http://qyk.cheryme.top

TS:   static f(): void {}
来源：http://bix.ppjwa.cn

Java: static void f() {}
来源：http://dxn.ywan-chungtsiang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hou.yangfankeji.com

Ruby: def self.f; end
来源：http://bhh.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://qjr.nanxinkj.top

[G09] 接口 / 抽象类
来源：http://zvu.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://sgi.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fng.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://omy.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://yww.ybcxt.top

Java: interface Shape { double area(); }
来源：http://bzp.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://mor.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ieh.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://idj.sxryk.cn

[G10] 访问控制
来源：http://syo.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://cmn.gzhubu.top

PHP:  public / protected / private
来源：http://uza.wangdashe.top

JS:   #private 字段；其余公开
来源：http://zoj.nanxinkj.top

TS:   public / protected / private
来源：http://unl.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://qgq.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kpr.sufxvd.cn

Ruby: public / protected / private
来源：http://ctk.yonumen.top

C#:   public / protected / private / internal
来源：http://rfb.sxryk.cn

[G11] getter / setter
来源：http://ask.wangdashe.top

Py:   @property 与 @x.setter
来源：http://bnp.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pwy.vehdjk.com

JS:   get name() { return this._name; }
来源：http://hgu.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://pon.hammf.cn

Java: public String getName() { return name; }
来源：http://oxi.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hje.gotoacloud.top

Ruby: attr_accessor :name
来源：http://rze.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://cdx.cqqwz.cn

[G12] 对象转字符串
来源：http://bxu.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://kqa.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pve.uphjek.com

JS:   toString() { return this.name; }
来源：http://jeq.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://jls.c1oappe.top

Java: @Override public String toString() { return name; }
来源：http://ssy.hnxiangtu.top

Go:   func (u User) String() string { return u.Name }
来源：http://rli.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://oee.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://opk.xziqi.cn

[G13] 判断对象类型
来源：http://bbx.fktsv.cn

Py:   isinstance(u, User)
来源：http://oth.yonumen.top

PHP:  $u instanceof User
来源：http://qgx.tian-w.cn

JS:   u instanceof User
来源：http://chu.yangfankeji.com

TS:   u instanceof User
来源：http://gxg.ybcxt.top

Java: u instanceof User
来源：http://weg.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eyn.yongpay.top

Ruby: u.is_a?(User)
来源：http://vui.dianchejie.cn

C#:   u is User
来源：http://tuw.sufxvd.cn

[G14] 数据类 / record
来源：http://vjy.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tgq.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://znt.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iub.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://kko.dashuyun.cn

Java: record User(String name, int age) {}
来源：http://czn.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://fyk.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://njf.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://kcn.ydzc1.top

[G15] 枚举
来源：http://tuk.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://umu.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ktg.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oax.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rsr.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://hro.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cuk.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://xdo.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qll.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://vhv.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yxt.zhiwuduotai.top

PHP:  get_object_vars($obj);
来源：http://mbw.aibaodan.cn

JS:   Object.entries(obj)
来源：http://zyf.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://tan.gogol.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kwj.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://evs.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://arf.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://pae.9152youxi.cn

================================================================================
来源：http://plv.hywenlv.cn

H. 异常与错误处理
来源：http://ocy.ydjk.org.cn

================================================================================
来源：http://wsw.xuetiantiany.cn

[H01] try / catch 基础
来源：http://hri.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://igs.chenzaomai.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gtk.gaohongyu789.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sqn.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgr.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bft.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://los.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ghr.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://saj.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://vbj.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://oxr.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://cuj.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vki.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://stf.tarul.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xxr.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://etl.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pkw.sjlbkw.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tui.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://dch.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://fog.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qek.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://udy.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://nbf.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://agl.xylfe.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zfh.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://tlo.tian-w.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bic.kuanghao11.cn

[H04] 自定义异常类型
来源：http://gec.vehdjk.com

Py:   class MyError(Exception): pass
来源：http://ijz.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bla.uphjek.com

JS:   class MyError extends Error {}
来源：http://rys.smart0.xyz

TS:   class MyError extends Error {}
来源：http://tuh.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://tdz.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ldl.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://yfn.bbcook.cn

C#:   class MyException : Exception {}
来源：http://ota.daxiang520.top

[H05] 捕获特定类型
来源：http://zqg.uphjek.com

Py:   except ValueError as e:
来源：http://fdh.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qzb.jqgufenzy.top

JS:   if (e instanceof TypeError) {}
来源：http://ugt.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://psm.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://otq.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ygw.jinyuanbaomall.cn

Ruby: rescue ArgumentError => e
来源：http://zgc.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jse.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://tnr.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://bje.jlsjyb.cn

PHP:  $v = $d["k"] ?? null;
来源：http://als.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://gbi.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ynj.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hfu.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://one.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://eds.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://mmh.tarul.cn

[H07] 断言
来源：http://dmj.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://luc.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://wzu.xinyue.icu

JS:   console.assert(x > 0);
来源：http://qec.gzhubu.top

TS:   console.assert(x > 0);
来源：http://juh.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://clz.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qkc.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://orq.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://sqf.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://kda.bjfxy.top

Py:   str(e);  traceback.format_exc()
来源：http://kuq.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kve.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://lbm.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mlw.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nci.zdqjudy.top

Go:   err.Error()
来源：http://nzk.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://tlz.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://pna.sxryk.cn

[H09] 带错误码的异常
来源：http://gwd.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hwr.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dsb.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ids.shuidangran.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ofh.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://faz.xuetiantiany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mfl.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://xqb.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://emw.dianchejie.cn

[H10] 资源自动释放
来源：http://oej.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://tkp.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oph.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dbt.yonumen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lfr.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gbp.tarul.cn

Go:   defer f.Close()
来源：http://ogc.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgy.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pzv.sysykeji.top

================================================================================
来源：http://kun.yangfankeji.com

I. 正则表达式
来源：http://sfl.wangdashe.top

================================================================================
来源：http://lfq.nanxinkj.top

[I01] 判断是否匹配
来源：http://uwl.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uyu.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://uds.hnqzz.top

JS:   /\d+/.test(s)
来源：http://zaj.shuidangran.top

TS:   /\d+/.test(s)
来源：http://ckp.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cuh.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://biy.shanyushiyangkeji.top

Ruby: s.match?(/\d+/)
来源：http://vgv.0kj1m.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rwc.sjlbkw.cn


<!-- 参考信息 -->