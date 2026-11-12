代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wlu.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jbb.yj202588.top

Ruby: Dir.children("dir")
来源：http://wxi.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://dxn.0kj1m.cn

[F09] 获取文件大小
来源：http://drn.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://xqb.gotoacloud.top

PHP:  filesize("a.txt");
来源：http://art.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://yxy.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://efe.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://nrw.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://itr.fktsv.cn

Ruby: File.size("a.txt")
来源：http://vjj.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://rdm.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://edk.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wwa.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pyy.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rhe.sysykeji.top

TS:   path.extname("a.txt")
来源：http://dhq.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iuh.birdmap.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oau.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cql.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vbw.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://iuf.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uvz.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mhx.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dfv.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ghw.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://emn.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdb.cucudq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fyp.xuetiantiany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gzw.svipenyu.cn

[F12] CSV 读写
来源：http://vat.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iau.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zlt.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rfv.birdmap.top

TS:   // 同上
来源：http://iwy.epnwcf.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eal.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qiu.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jim.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fjt.cashguo.top

================================================================================
来源：http://xgh.zhengqikj.top

G. 面向对象
来源：http://jpn.snrcjt.cn

================================================================================
来源：http://fuv.birdmap.top

[G01] 定义类
来源：http://uuf.dianchejie.cn

Py:   class User: pass
来源：http://uap.zhoulong.xyz

PHP:  class User {}
来源：http://zck.ydjk.org.cn

JS:   class User {}
来源：http://sfa.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://qem.guannengcc.top

Java: class User {}
来源：http://pkv.jianghu66.top

Go:   type User struct { Name string }
来源：http://pit.pycfn.com

Ruby: class User; end
来源：http://ncw.52xcode.cn

C#:   class User {}
来源：http://tes.yueranfly.top

[G02] 构造函数
来源：http://vqi.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://fzd.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://bct.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://hjx.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://olr.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://sta.hnqzz.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ypb.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://uuf.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://hkw.hnxiangtu.top

[G03] 实例属性
来源：http://eip.0kj1m.cn

Py:   self.name = "x"
来源：http://nzu.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://ykv.yj20258888.top

JS:   this.name = "x";
来源：http://gvv.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://ngw.jinqigfzy.top

Java: private String name;
来源：http://goj.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mzk.hcnkem.com

Ruby: @name = "x"
来源：http://zds.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://dja.dashuyun.cn

[G04] 定义方法
来源：http://irc.nwbrower.top

Py:   def greet(self): return self.name
来源：http://pus.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zpp.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://zkb.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://trx.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://mlc.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zlb.yonumen.top

Ruby: def greet; @name; end
来源：http://zqn.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://bfm.yangfankeji.com

[G05] 继承
来源：http://mug.mhx1999.top

Py:   class Admin(User): pass
来源：http://xew.uphjek.com

PHP:  class Admin extends User {}
来源：http://ako.yfazqb.com

JS:   class Admin extends User {}
来源：http://mdd.xinyue.icu

TS:   class Admin extends User {}
来源：http://zgh.dianchejie.cn

Java: class Admin extends User {}
来源：http://vkp.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://myo.smart0.xyz

Ruby: class Admin < User; end
来源：http://kks.yj20258.top

C#:   class Admin : User {}
来源：http://leo.wangdashe.top

[G06] 重写方法
来源：http://gsi.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://gje.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://ksi.cheryme.top

JS:   greet() { return "admin"; }
来源：http://sai.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://vfk.guowangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://jcv.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yif.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://yby.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://mke.chenzaomai.com

[G07] 调用父类方法
来源：http://ieq.shzxlz.cn

Py:   super().greet()
来源：http://tiz.daria6918.cn

PHP:  parent::greet();
来源：http://yyn.smart0.xyz

JS:   super.greet();
来源：http://qfd.tianlin.xyz

TS:   super.greet();
来源：http://lhq.sxryk.cn

Java: super.greet();
来源：http://syu.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kza.fengsongda.top

Ruby: super
来源：http://ugp.yonumen.top

C#:   base.Greet();
来源：http://lsd.kuanghao11.cn

[G08] 静态方法与属性
来源：http://vgm.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uru.bjfxy.top

PHP:  public static function f() {}
来源：http://hji.jlsjyb.cn

JS:   static f() {}
来源：http://cbo.hammf.cn

TS:   static f(): void {}
来源：http://avm.vqdsnc.cn

Java: static void f() {}
来源：http://xzb.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ugq.bjfxy.top

Ruby: def self.f; end
来源：http://xst.yonumen.top

C#:   public static void F() {}
来源：http://gkr.fehbvm.com

[G09] 接口 / 抽象类
来源：http://blq.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://pyx.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wvc.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqi.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://zxg.yfazqb.com

Java: interface Shape { double area(); }
来源：http://ciz.0kj1m.cn

Go:   type Shape interface { Area() float64 }
来源：http://zzz.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bzi.xuanzx.com

C#:   interface IShape { double Area(); }
来源：http://gvl.cashguo.top

[G10] 访问控制
来源：http://kfx.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://fgf.tarul.cn

PHP:  public / protected / private
来源：http://drs.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://lea.fzhhl.top

TS:   public / protected / private
来源：http://emr.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://fmh.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrq.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://jbd.guannengcc.top

C#:   public / protected / private / internal
来源：http://djy.jlsjyb.cn

[G11] getter / setter
来源：http://mou.yonumen.top

Py:   @property 与 @x.setter
来源：http://egc.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fel.zhoulong.xyz

JS:   get name() { return this._name; }
来源：http://gtk.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://vpw.shzxlz.cn

Java: public String getName() { return name; }
来源：http://tmf.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bgl.iojbl.cn

Ruby: attr_accessor :name
来源：http://vep.ivvv.top

C#:   public string Name { get; set; }
来源：http://twi.uphjek.com

[G12] 对象转字符串
来源：http://vih.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://lib.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xlu.fengsongda.top

JS:   toString() { return this.name; }
来源：http://moy.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://llr.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://uev.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ydm.andypj.xyz

Ruby: def to_s; @name; end
来源：http://okp.gotoacloud.top

C#:   public override string ToString() => Name;
来源：http://juk.tanke756.top

[G13] 判断对象类型
来源：http://iee.iojbl.cn

Py:   isinstance(u, User)
来源：http://ect.aizwys.cn

PHP:  $u instanceof User
来源：http://ctw.yj20258.top

JS:   u instanceof User
来源：http://tet.cashguo.top

TS:   u instanceof User
来源：http://eas.meibo888.top

Java: u instanceof User
来源：http://hqc.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://ilz.sysykeji.top

Ruby: u.is_a?(User)
来源：http://uqh.gogol.net.cn

C#:   u is User
来源：http://nmw.fehbvm.com

[G14] 数据类 / record
来源：http://tkq.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mys.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://soj.shzxlz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://snn.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://zwn.meibo888.top

Java: record User(String name, int age) {}
来源：http://yff.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://brm.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bte.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://aca.jyoumei.cn

[G15] 枚举
来源：http://kef.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mlk.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://uku.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oqw.sweek.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fry.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://tlm.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ble.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://xfb.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wtj.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://abt.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mjt.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://vkg.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://sdc.yj202588.top

TS:   Object.entries(obj)
来源：http://xph.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zse.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yrm.yj202588.top

Ruby: obj.instance_variables
来源：http://vjf.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://rte.9152youxi.cn

================================================================================
来源：http://oyr.epnwcf.com

H. 异常与错误处理
来源：http://icv.hfpthk.cn

================================================================================
来源：http://egh.tanke756.top

[H01] try / catch 基础
来源：http://nvv.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pon.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lfj.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ohx.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ivj.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bux.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xlo.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wrs.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://npo.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://ugl.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://dfa.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sxp.ydjk.org.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xqz.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://tod.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://muo.shanyushiyangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mtj.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eam.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wsv.zhongyouzk.top

[H03] 主动抛出异常
来源：http://iag.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://gai.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dvp.yfazqb.com

JS:   throw new Error("错误信息");
来源：http://fzc.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://fwt.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jsp.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lqc.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kut.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://qod.jyoumei.cn

[H04] 自定义异常类型
来源：http://raq.shzxlz.cn

Py:   class MyError(Exception): pass
来源：http://boe.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://bww.hongshengwenyu.top

JS:   class MyError extends Error {}
来源：http://fef.bbcook.cn

TS:   class MyError extends Error {}
来源：http://hmq.gaohongyu789.top

Java: class MyException extends RuntimeException {}
来源：http://lql.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nwn.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://ufp.wangshuangyany.cn

C#:   class MyException : Exception {}
来源：http://kgu.ydzc1.top

[H05] 捕获特定类型
来源：http://zjy.yj202588.top

Py:   except ValueError as e:
来源：http://zse.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iwh.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://qxf.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://zmy.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://ryg.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zpc.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://puy.xinyue.icu

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tim.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://vgz.sweek.top

Py:   value = d.get("k") or default
来源：http://iij.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bhi.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://ous.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://grz.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fmr.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nji.yuxming.cn

Ruby: d&.dig(:a, :b)
来源：http://lqw.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://pvp.jinqigfzy.top

[H07] 断言
来源：http://ega.zhijiandao.cn

Py:   assert x > 0, "必须为正"
来源：http://vtv.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://evc.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://pov.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://cbr.xylfe.cn

Java: assert x > 0 : "必须为正";
来源：http://jzk.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fud.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://ojd.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://hfo.jinqigufen.top

[H08] 获取错误信息与堆栈
来源：http://mqt.cheryme.top

Py:   str(e);  traceback.format_exc()
来源：http://uxp.quarkkingdee.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hiv.andypj.xyz

JS:   e.message;  e.stack
来源：http://wrb.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kpa.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zia.xylfe.cn

Go:   err.Error()
来源：http://rnk.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://lxi.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://dqv.vehdjk.com

[H09] 带错误码的异常
来源：http://vlb.sufxvd.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ikz.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xmo.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nsl.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cox.yangfankeji.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wdf.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qbm.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://bgj.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ion.yonumen.top

[H10] 资源自动释放
来源：http://aty.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pfj.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://whr.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pjh.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ejs.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://okr.tian-w.cn

Go:   defer f.Close()
来源：http://pfv.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://skv.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://huo.nanxuanxn.top

================================================================================
来源：http://jai.epnwcf.com

I. 正则表达式
来源：http://zcr.svipenyu.cn

================================================================================
来源：http://tbx.fktsv.cn

[I01] 判断是否匹配
来源：http://hsn.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oxq.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://krx.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://lat.hesvh.cn

TS:   /\d+/.test(s)
来源：http://xua.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esd.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jot.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://qst.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ycb.sxryk.cn

[I02] 提取所有匹配
来源：http://ppa.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://tcn.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wlr.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jks.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://qdh.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dhr.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbb.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://wfx.zhijiandao.cn


<!-- 参考信息 -->