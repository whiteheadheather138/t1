代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ihh.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpw.fktsv.cn

Ruby: Dir.children("dir")
来源：http://szk.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://nnv.ybcxt.top

[F09] 获取文件大小
来源：http://kuk.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://bvq.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://yqq.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://mwr.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://llz.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vbo.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dbq.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://aoq.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://zop.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://bns.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vpu.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wlg.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fpw.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://bxr.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qvj.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://izq.svipenyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rrl.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ghu.c1oappe.top

[F11] 复制与移动文件
来源：http://egj.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://phk.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pjk.gzhubu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://swf.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fci.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rwg.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://llf.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yzd.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xwf.nanxinkj.top

[F12] CSV 读写
来源：http://maz.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://atv.zhaomingkeji.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zen.0kj1m.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vkw.sysykeji.top

TS:   // 同上
来源：http://fnd.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gug.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ydx.0kj1m.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bof.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://baw.fengsongda.top

================================================================================
来源：http://jrt.vqdsnc.cn

G. 面向对象
来源：http://mop.shangyingyoupin.top

================================================================================
来源：http://nut.cashguo.top

[G01] 定义类
来源：http://fyp.jinghuilouyu.cn

Py:   class User: pass
来源：http://gft.daria6918.cn

PHP:  class User {}
来源：http://iaa.wangdashe.top

JS:   class User {}
来源：http://vqa.yuxming.cn

TS:   class User { name: string = ""; }
来源：http://fmc.ydjk.org.cn

Java: class User {}
来源：http://hft.guowangkeji.top

Go:   type User struct { Name string }
来源：http://hdn.fanxiaobao.xyz

Ruby: class User; end
来源：http://dbi.yj20258888.top

C#:   class User {}
来源：http://lhq.jinyuanbaomall.cn

[G02] 构造函数
来源：http://lil.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://fwg.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://ndj.wangdashe.top

JS:   constructor(name) { this.name = name; }
来源：http://azc.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://dwq.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://lhv.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://col.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://veq.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://uzt.meibo888.top

[G03] 实例属性
来源：http://nar.nanxinkj.top

Py:   self.name = "x"
来源：http://qbe.xuanzx.com

PHP:  public string $name = "x";
来源：http://syo.tianlin.xyz

JS:   this.name = "x";
来源：http://fkc.sweek.top

TS:   name: string = "x";
来源：http://adh.ivvv.top

Java: private String name;
来源：http://mxe.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fdl.gogol.net.cn

Ruby: @name = "x"
来源：http://cwe.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://viw.cashguo.top

[G04] 定义方法
来源：http://dlw.hesvh.cn

Py:   def greet(self): return self.name
来源：http://wyd.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ugz.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://eti.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://tgr.zhoulong.xyz

Java: String greet() { return name; }
来源：http://hyg.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://gwa.cucudq.cn

Ruby: def greet; @name; end
来源：http://trb.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://pla.yvedp.cn

[G05] 继承
来源：http://vfy.jinqigufen.top

Py:   class Admin(User): pass
来源：http://dal.ivvv.top

PHP:  class Admin extends User {}
来源：http://meh.zdbjq.cn

JS:   class Admin extends User {}
来源：http://nnf.jyoumei.cn

TS:   class Admin extends User {}
来源：http://ldv.yonumen.top

Java: class Admin extends User {}
来源：http://dki.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vir.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://jfn.sjlbkw.cn

C#:   class Admin : User {}
来源：http://vma.cqqwz.cn

[G06] 重写方法
来源：http://jom.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://uci.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jfw.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://fny.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://vuy.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://cpe.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dvb.yangfankeji.com

Ruby: def greet; "admin"; end
来源：http://hiy.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://zwy.cqqwz.cn

[G07] 调用父类方法
来源：http://nvz.shzxlz.cn

Py:   super().greet()
来源：http://avy.jiagoushi.top

PHP:  parent::greet();
来源：http://cvz.jinghuilouyu.cn

JS:   super.greet();
来源：http://qtc.nanxinkj.top

TS:   super.greet();
来源：http://ksq.316326.xyz

Java: super.greet();
来源：http://fny.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pro.hysaishi.cn

Ruby: super
来源：http://zds.tian-w.cn

C#:   base.Greet();
来源：http://jra.dashuyun.cn

[G08] 静态方法与属性
来源：http://ile.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gim.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://wki.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://led.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://nrr.dashuyun.cn

Java: static void f() {}
来源：http://snj.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fff.nanxuanxn.top

Ruby: def self.f; end
来源：http://mzg.xziqi.cn

C#:   public static void F() {}
来源：http://owo.nwbrower.top

[G09] 接口 / 抽象类
来源：http://cpz.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://zer.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://lbc.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mhq.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://oov.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://crj.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://yfy.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rjq.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://hdk.sufxvd.cn

[G10] 访问控制
来源：http://joc.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://noy.hnxiangtu.top

PHP:  public / protected / private
来源：http://srl.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://oeu.yanxiufei.cn

TS:   public / protected / private
来源：http://bjl.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://jxp.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dwh.epnwcf.com

Ruby: public / protected / private
来源：http://rox.jinqigufen.top

C#:   public / protected / private / internal
来源：http://xhq.guowangkeji.top

[G11] getter / setter
来源：http://ine.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://tfy.aibaodan.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xbe.hammf.cn

JS:   get name() { return this._name; }
来源：http://mvl.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://uuw.hesvh.cn

Java: public String getName() { return name; }
来源：http://wnf.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fpv.yj20258.top

Ruby: attr_accessor :name
来源：http://bkw.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://zmm.zhengqikj.top

[G12] 对象转字符串
来源：http://uiy.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://mhi.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zta.yfazqb.com

JS:   toString() { return this.name; }
来源：http://tgy.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://ofh.tianlin.xyz

Java: @Override public String toString() { return name; }
来源：http://aef.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://ecc.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://ytp.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://mkt.jqgfzy.top

[G13] 判断对象类型
来源：http://bun.chenzaomai.com

Py:   isinstance(u, User)
来源：http://wxa.bjfxy.top

PHP:  $u instanceof User
来源：http://xnn.jlsjyb.cn

JS:   u instanceof User
来源：http://yui.hesvh.cn

TS:   u instanceof User
来源：http://zzq.yvedp.cn

Java: u instanceof User
来源：http://sxb.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jcs.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://mnd.shangyingyoupin.top

C#:   u is User
来源：http://hwc.xinyue.icu

[G14] 数据类 / record
来源：http://yal.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yoi.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://ztd.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://zil.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://glr.bbcook.cn

Java: record User(String name, int age) {}
来源：http://kyg.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://zwr.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ljc.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://kbq.zdqjudy.top

[G15] 枚举
来源：http://yvn.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rgd.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://izi.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ooq.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjj.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://hnc.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nlr.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://ggx.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hzh.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://khm.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://roh.sjlbkw.cn

PHP:  get_object_vars($obj);
来源：http://pvh.guowangkeji.top

JS:   Object.entries(obj)
来源：http://wxq.hywenlv.cn

TS:   Object.entries(obj)
来源：http://yxq.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://urx.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://uzx.ydzc1.top

Ruby: obj.instance_variables
来源：http://zjo.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://tfg.pengpengdd.cyou

================================================================================
来源：http://uuo.gogol.net.cn

H. 异常与错误处理
来源：http://ypm.shuidangran.top

================================================================================
来源：http://ham.yuxming.cn

[H01] try / catch 基础
来源：http://gzq.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://chu.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qzp.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aeq.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qnl.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://onb.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://atj.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hod.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsb.aizwys.cn

[H02] finally / ensure 收尾
来源：http://lki.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://yws.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qxq.zhixingplan.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ipb.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wuc.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gor.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://hqp.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bmz.yuxming.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nre.hesvh.cn

[H03] 主动抛出异常
来源：http://qtz.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://jpx.shanyushiyangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qzc.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://efr.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://xht.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nad.gogol.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://utt.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://skk.jqgfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://whk.xziqi.cn

[H04] 自定义异常类型
来源：http://zfu.birdmap.top

Py:   class MyError(Exception): pass
来源：http://twm.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://stw.yfazqb.com

JS:   class MyError extends Error {}
来源：http://jor.gzhubu.top

TS:   class MyError extends Error {}
来源：http://nxy.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://uws.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jii.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://ywe.guannengcc.top

C#:   class MyException : Exception {}
来源：http://nly.yj202588.top

[H05] 捕获特定类型
来源：http://uyz.daria6918.cn

Py:   except ValueError as e:
来源：http://ycy.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cgw.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://mbw.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://jnq.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://tqj.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eob.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://hsm.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bny.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://rgn.guannengcc.top

Py:   value = d.get("k") or default
来源：http://utd.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mti.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://sua.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qgd.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jgi.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://new.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://mld.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://aum.hongshengwenyu.top

[H07] 断言
来源：http://fud.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://mkd.andypj.xyz

PHP:  assert($x > 0);
来源：http://jjv.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://szp.c1oappe.top

TS:   console.assert(x > 0);
来源：http://nkh.chenjidiqi.icu

Java: assert x > 0 : "必须为正";
来源：http://zqm.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eqg.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eea.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://hti.shangyingyoupin.top

[H08] 获取错误信息与堆栈
来源：http://qev.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://ldg.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://arf.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://kow.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rtw.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eoh.zhixingplan.top

Go:   err.Error()
来源：http://gaw.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://ovn.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://fwq.tian-w.cn

[H09] 带错误码的异常
来源：http://utx.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mvx.ctjpmb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dgv.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ghh.yfazqb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tkw.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wry.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gru.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://giw.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wwu.andypj.xyz

[H10] 资源自动释放
来源：http://pxz.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dyc.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tbd.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iaz.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yul.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eqv.yonumen.top

Go:   defer f.Close()
来源：http://xtt.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tnv.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qda.pengpengdd.cyou

================================================================================
来源：http://mcr.cashguo.top

I. 正则表达式
来源：http://khh.zycfv.cn

================================================================================
来源：http://lty.ctjpmb.com

[I01] 判断是否匹配
来源：http://mkj.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kyq.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://dbi.havefunace.top

JS:   /\d+/.test(s)
来源：http://fdz.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://mpb.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://beo.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wor.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://lhq.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zmd.meibo888.top

[I02] 提取所有匹配
来源：http://apv.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://ron.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gcn.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ogc.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://slv.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jvo.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://byq.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://qir.xuanzx.com


<!-- 参考信息 -->