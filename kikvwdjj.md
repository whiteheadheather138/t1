代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://uwl.hesvh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rts.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://jtr.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://cfr.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mhd.hywenlv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hhu.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://ljz.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://dwz.fengsongda.top

[F09] 获取文件大小
来源：http://tde.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://bvd.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://bku.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://stp.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://krh.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://cno.daria6918.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bpm.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://mnc.sjlbkw.cn

C#:   new FileInfo("a.txt").Length
来源：http://pgz.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://kff.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jgw.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zef.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qrq.andypj.xyz

TS:   path.extname("a.txt")
来源：http://fqr.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cjn.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mmk.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zcn.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qrz.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://poc.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zlz.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://efy.52xcode.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ils.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxf.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sus.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dbp.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vpb.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ybz.xuanzx.com

[F12] CSV 读写
来源：http://nkr.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xhi.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://huk.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ufl.yvedp.cn

TS:   // 同上
来源：http://apx.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://euj.ybcxt.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxo.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eob.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uwx.ydzc1.top

================================================================================
来源：http://smu.shanyushiyangkeji.top

G. 面向对象
来源：http://bww.quarkkingdee.top

================================================================================
来源：http://qfb.yuxming.cn

[G01] 定义类
来源：http://cbz.meibo888.top

Py:   class User: pass
来源：http://rrq.iojbl.cn

PHP:  class User {}
来源：http://abs.sweek.top

JS:   class User {}
来源：http://owj.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://dha.andypj.xyz

Java: class User {}
来源：http://rlq.guowangkeji.top

Go:   type User struct { Name string }
来源：http://mxm.hnqzz.top

Ruby: class User; end
来源：http://qqn.xylfe.cn

C#:   class User {}
来源：http://yhd.sjlbkw.cn

[G02] 构造函数
来源：http://mwm.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://aed.sjlbkw.cn

PHP:  public function __construct(public string $name) {}
来源：http://alm.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://ddc.xingfuxueyuan.xyz

TS:   constructor(public name: string) {}
来源：http://ach.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://uzi.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ryz.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://oed.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://wtb.tianlin.xyz

[G03] 实例属性
来源：http://lkp.jinqigufen.top

Py:   self.name = "x"
来源：http://wpf.hnqzz.top

PHP:  public string $name = "x";
来源：http://ivg.yj202588.top

JS:   this.name = "x";
来源：http://ske.quarkkingdee.top

TS:   name: string = "x";
来源：http://yhr.sweek.top

Java: private String name;
来源：http://qda.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iza.c1oappe.top

Ruby: @name = "x"
来源：http://kgx.gogol.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://akv.aizwys.cn

[G04] 定义方法
来源：http://ywm.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://bnn.hcnkem.com

PHP:  public function greet(): string { return $this->name; }
来源：http://axo.uphjek.com

JS:   greet() { return this.name; }
来源：http://uiv.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://qmt.chenzaomai.com

Java: String greet() { return name; }
来源：http://ixo.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://qyz.redwolf501.top

Ruby: def greet; @name; end
来源：http://mep.0kj1m.cn

C#:   public string Greet() => Name;
来源：http://lou.aizwys.cn

[G05] 继承
来源：http://uaw.xylfe.cn

Py:   class Admin(User): pass
来源：http://uol.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://tbm.cashguo.top

JS:   class Admin extends User {}
来源：http://azn.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://iiv.zycfv.cn

Java: class Admin extends User {}
来源：http://yzl.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ihx.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://skj.52xcode.cn

C#:   class Admin : User {}
来源：http://ohg.ybcxt.top

[G06] 重写方法
来源：http://faw.tanke756.top

Py:   def greet(self): return "admin"
来源：http://dhm.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mrq.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://dcc.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://afa.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://lyd.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://erd.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://suf.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://exp.fzhhl.top

[G07] 调用父类方法
来源：http://ppf.zhixingplan.top

Py:   super().greet()
来源：http://wql.shangyingyoupin.top

PHP:  parent::greet();
来源：http://kvm.sjlbkw.cn

JS:   super.greet();
来源：http://agy.yvedp.cn

TS:   super.greet();
来源：http://ewg.jinghuilouyu.cn

Java: super.greet();
来源：http://yvm.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xng.vehdjk.com

Ruby: super
来源：http://amw.shanyushiyangtech.top

C#:   base.Greet();
来源：http://xrl.zhoulong.xyz

[G08] 静态方法与属性
来源：http://uvc.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://izn.cheryme.top

PHP:  public static function f() {}
来源：http://viv.gogol.net.cn

JS:   static f() {}
来源：http://ivc.hfpthk.cn

TS:   static f(): void {}
来源：http://egg.gaohongyu789.top

Java: static void f() {}
来源：http://lpl.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tlx.yangfankeji.com

Ruby: def self.f; end
来源：http://zjp.xziqi.cn

C#:   public static void F() {}
来源：http://gvj.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://nna.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://axx.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://upu.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://okm.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://pgq.hesvh.cn

Java: interface Shape { double area(); }
来源：http://yut.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://pis.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oen.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://cpn.havefunace.top

[G10] 访问控制
来源：http://oxo.xinyue.icu

Py:   约定 _protected / __private（不强制）
来源：http://jui.yangfankeji.com

PHP:  public / protected / private
来源：http://mhe.yvedp.cn

JS:   #private 字段；其余公开
来源：http://qlx.birdmap.top

TS:   public / protected / private
来源：http://hmo.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://dqr.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vth.shzxlz.cn

Ruby: public / protected / private
来源：http://zqt.jlsjyb.cn

C#:   public / protected / private / internal
来源：http://nsn.daxiang520.top

[G11] getter / setter
来源：http://arj.uphjek.com

Py:   @property 与 @x.setter
来源：http://cxi.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kca.sysykeji.top

JS:   get name() { return this._name; }
来源：http://msf.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://ufz.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://dux.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kbf.sxryk.cn

Ruby: attr_accessor :name
来源：http://daj.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://cgu.guowangkeji.top

[G12] 对象转字符串
来源：http://gsl.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://tkd.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cyp.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://xbk.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://lxe.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://jjw.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://hjh.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://duj.yj202588.top

C#:   public override string ToString() => Name;
来源：http://azk.9152youxi.cn

[G13] 判断对象类型
来源：http://ese.jianghu66.top

Py:   isinstance(u, User)
来源：http://dvi.ybcxt.top

PHP:  $u instanceof User
来源：http://myf.xuanzx.com

JS:   u instanceof User
来源：http://kdk.nwbrower.top

TS:   u instanceof User
来源：http://rla.ctjpmb.com

Java: u instanceof User
来源：http://sfr.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://kxs.xziqi.cn

Ruby: u.is_a?(User)
来源：http://abi.hywenlv.cn

C#:   u is User
来源：http://xsj.bjfxy.top

[G14] 数据类 / record
来源：http://ehn.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://olb.jinghuilouyu.cn

PHP:  // 用 readonly 属性模拟
来源：http://rxa.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://fid.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://dyz.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://osj.sysykeji.top

Go:   type User struct { Name string; Age int }
来源：http://mlb.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qip.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://zxl.jlsjyb.cn

[G15] 枚举
来源：http://dlz.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eyz.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ion.xuanzx.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hho.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vnr.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://eej.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mir.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://ucd.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qdi.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://jtf.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ztq.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://etj.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://mlx.zhengqikj.top

TS:   Object.entries(obj)
来源：http://xoq.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wkc.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oki.gogol.net.cn

Ruby: obj.instance_variables
来源：http://iet.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://glg.dianchejie.cn

================================================================================
来源：http://ijj.guannengcc.top

H. 异常与错误处理
来源：http://wtf.yongpay.top

================================================================================
来源：http://pbd.xziqi.cn

[H01] try / catch 基础
来源：http://gek.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lxu.yangfankeji.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kaz.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hco.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jne.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xpf.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://byg.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://clt.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lsi.cashguo.top

[H02] finally / ensure 收尾
来源：http://ron.vqdsnc.cn

Py:   try: f()⏎finally: cleanup()
来源：http://znl.tanke756.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vdg.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eau.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xoq.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://eyn.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ozy.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kyo.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://mfx.yj202588.top

[H03] 主动抛出异常
来源：http://jyn.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://bms.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://scz.ehwqpu.com

JS:   throw new Error("错误信息");
来源：http://rwm.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://vmv.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fmn.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ikz.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://apb.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://hib.jinqigufen.top

[H04] 自定义异常类型
来源：http://rzs.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://wwi.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://ygy.ydzc1.top

JS:   class MyError extends Error {}
来源：http://pdl.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://zau.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://olm.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jiw.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://koh.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://uwh.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://vne.yuxming.cn

Py:   except ValueError as e:
来源：http://lro.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rak.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://seg.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://uqw.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://nap.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yau.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://izt.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cqt.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://qgu.jqgfzy.top

Py:   value = d.get("k") or default
来源：http://etz.ctjpmb.com

PHP:  $v = $d["k"] ?? null;
来源：http://gdf.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://rcl.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://vhs.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kfi.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kub.sjlbkw.cn

Ruby: d&.dig(:a, :b)
来源：http://lih.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://kxv.yfazqb.com

[H07] 断言
来源：http://wno.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://xtq.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://ywc.aizwys.cn

JS:   console.assert(x > 0);
来源：http://qpx.cashguo.top

TS:   console.assert(x > 0);
来源：http://rkt.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://hlu.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lym.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tbi.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://juq.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://ohj.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://cfn.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtd.andypj.xyz

JS:   e.message;  e.stack
来源：http://gxa.yongpay.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dxi.yuanzhike.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dpt.nanxuanxn.top

Go:   err.Error()
来源：http://mwv.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://yrz.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://eoj.dashuyun.cn

[H09] 带错误码的异常
来源：http://bns.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://coo.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://dpg.fanxiaobao.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://izj.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://olx.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://usw.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wrj.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://ymp.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xxv.meibo888.top

[H10] 资源自动释放
来源：http://yma.cashguo.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ody.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cui.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dmn.uphjek.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ykw.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oih.aibaodan.cn

Go:   defer f.Close()
来源：http://dny.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vtc.meibo888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cix.kuanghao11.cn

================================================================================
来源：http://jgh.zdbjq.cn

I. 正则表达式
来源：http://icc.wangdashe.top

================================================================================
来源：http://imf.bbcook.cn

[I01] 判断是否匹配
来源：http://lzo.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wig.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://udv.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://klk.fehbvm.com

TS:   /\d+/.test(s)
来源：http://cmc.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://adt.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://toy.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://ccb.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://agn.pycfn.com

[I02] 提取所有匹配
来源：http://mtl.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://fpr.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nku.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nbk.xingfuxueyuan.xyz


<!-- 参考信息 -->