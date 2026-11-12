代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kuq.jiagoushi.top

TS:   path.extname("a.txt")
来源：http://ysk.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lzg.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ebl.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://skg.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hdk.nanxuanxn.top

[F11] 复制与移动文件
来源：http://krw.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://chz.guannengcc.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wko.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iyz.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ong.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tgw.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rdj.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://flp.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ghn.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://nci.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dnl.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fxr.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gqq.shuidangran.top

TS:   // 同上
来源：http://iaa.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jkl.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tcz.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lgh.meibo888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jzi.feifeiyinyue.top

================================================================================
来源：http://icz.xuanzx.com

G. 面向对象
来源：http://btw.xziqi.cn

================================================================================
来源：http://bnv.sxryk.cn

[G01] 定义类
来源：http://bbu.yanxiufei.cn

Py:   class User: pass
来源：http://fth.sjlbkw.cn

PHP:  class User {}
来源：http://ihx.zdbjq.cn

JS:   class User {}
来源：http://wab.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://buk.yfazqb.com

Java: class User {}
来源：http://khj.chenzaomai.com

Go:   type User struct { Name string }
来源：http://lrl.epnwcf.com

Ruby: class User; end
来源：http://xbo.chenjidiqi.icu

C#:   class User {}
来源：http://bds.pengpengdd.cyou

[G02] 构造函数
来源：http://ibb.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://nch.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://csu.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://ffy.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://hmt.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://djy.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bhe.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://adj.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://lvz.chenzaomai.com

[G03] 实例属性
来源：http://jfn.c1oappe.top

Py:   self.name = "x"
来源：http://hyq.ybcxt.top

PHP:  public string $name = "x";
来源：http://yjb.shangyingyoupin.top

JS:   this.name = "x";
来源：http://zgz.snrcjt.cn

TS:   name: string = "x";
来源：http://ofx.ywan-chungtsiang.top

Java: private String name;
来源：http://ogg.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vrp.xziqi.cn

Ruby: @name = "x"
来源：http://wkt.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://jzo.zycfv.cn

[G04] 定义方法
来源：http://ppn.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://hel.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rlv.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://wou.haohaochexian.top

TS:   greet(): string { return this.name; }
来源：http://kar.jlsjyb.cn

Java: String greet() { return name; }
来源：http://csd.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qmg.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://xan.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://qdv.tian-w.cn

[G05] 继承
来源：http://ois.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://gaj.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://hlx.gotoacloud.top

JS:   class Admin extends User {}
来源：http://qta.daxiang520.top

TS:   class Admin extends User {}
来源：http://jll.zhongyouzk.top

Java: class Admin extends User {}
来源：http://dti.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ctk.gogol.net.cn

Ruby: class Admin < User; end
来源：http://ndp.tanke756.top

C#:   class Admin : User {}
来源：http://aet.zhongyouzk.top

[G06] 重写方法
来源：http://kxc.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://nbb.jianghu66.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ukp.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://nmw.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://ubb.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://and.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ttj.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://ffa.ppjwa.cn

C#:   public override string Greet() => "admin";
来源：http://krv.yfazqb.com

[G07] 调用父类方法
来源：http://xef.yj20258.top

Py:   super().greet()
来源：http://zua.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://epl.tianlin.xyz

JS:   super.greet();
来源：http://fga.shzxlz.cn

TS:   super.greet();
来源：http://udn.bjfxy.top

Java: super.greet();
来源：http://umt.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wmb.pycfn.com

Ruby: super
来源：http://bid.jinghuilouyu.cn

C#:   base.Greet();
来源：http://def.snrcjt.cn

[G08] 静态方法与属性
来源：http://phw.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fmt.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://leg.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://clo.yj202588.top

TS:   static f(): void {}
来源：http://jgp.pengpengdd.cyou

Java: static void f() {}
来源：http://vku.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fnv.yuxming.cn

Ruby: def self.f; end
来源：http://kbp.9152youxi.cn

C#:   public static void F() {}
来源：http://zky.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://zcr.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://efq.shangyingyoupin.top

PHP:  interface Shape { public function area(): float; }
来源：http://bnl.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ibv.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://yey.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://xvr.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://mdt.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://izi.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://dsp.zhiwuduotai.top

[G10] 访问控制
来源：http://opt.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://xnc.chenjidiqi.icu

PHP:  public / protected / private
来源：http://jab.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://trq.sjlbkw.cn

TS:   public / protected / private
来源：http://fjg.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://ach.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ntm.yj20258.top

Ruby: public / protected / private
来源：http://jpf.gzhubu.top

C#:   public / protected / private / internal
来源：http://hoy.bbcook.cn

[G11] getter / setter
来源：http://bkt.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://khq.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qhr.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://krt.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://qei.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://ozj.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vrt.hysaishi.cn

Ruby: attr_accessor :name
来源：http://oqz.cheryme.top

C#:   public string Name { get; set; }
来源：http://pkg.jqgfzy.top

[G12] 对象转字符串
来源：http://xhe.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://kmt.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://fbj.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://uxv.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://jyw.ctjpmb.com

Java: @Override public String toString() { return name; }
来源：http://qxa.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://zha.tarul.cn

Ruby: def to_s; @name; end
来源：http://egy.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://vot.sxryk.cn

[G13] 判断对象类型
来源：http://ygg.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://faa.iojbl.cn

PHP:  $u instanceof User
来源：http://zyy.yj20258.top

JS:   u instanceof User
来源：http://ivv.jinqigufen.top

TS:   u instanceof User
来源：http://erb.zhongyouzk.top

Java: u instanceof User
来源：http://kig.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oip.jianghu66.top

Ruby: u.is_a?(User)
来源：http://rkp.zhijiandao.cn

C#:   u is User
来源：http://cen.52xcode.cn

[G14] 数据类 / record
来源：http://iav.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://szf.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://zgx.hnqzz.top

JS:   // 无内置：普通类或对象字面量
来源：http://ene.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://gqq.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://wkg.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://sci.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jhj.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://vcs.daxiang520.top

[G15] 枚举
来源：http://nsg.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://elw.yvedp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qjd.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yif.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://opr.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://lcb.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qfr.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://iph.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vlm.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://hzf.zhiwuduotai.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vmg.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://ysc.sweek.top

JS:   Object.entries(obj)
来源：http://yge.xziqi.cn

TS:   Object.entries(obj)
来源：http://czv.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tnf.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://rjs.uphjek.com

Ruby: obj.instance_variables
来源：http://apl.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://sli.zhoulong.xyz

================================================================================
来源：http://qbx.hammf.cn

H. 异常与错误处理
来源：http://mxb.hnxiangtu.top

================================================================================
来源：http://ynq.yangfankeji.com

[H01] try / catch 基础
来源：http://vpx.bbcook.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dcs.shuidangran.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bnz.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://emv.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zdv.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cwe.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rcs.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dho.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ffc.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://lic.hcnkem.com

Py:   try: f()⏎finally: cleanup()
来源：http://olk.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lca.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://oec.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tqo.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://cck.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eiz.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tzc.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://mgs.tarul.cn

[H03] 主动抛出异常
来源：http://lpw.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://ebu.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mrv.dianchejie.cn

JS:   throw new Error("错误信息");
来源：http://cak.sjlbkw.cn

TS:   throw new Error("错误信息");
来源：http://pqp.jinghuilouyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dvi.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xpa.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://asd.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://vnd.tarul.cn

[H04] 自定义异常类型
来源：http://kwc.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://fez.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://njv.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://jqg.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://jzv.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://zuv.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://urx.iojbl.cn

Ruby: class MyError < StandardError; end
来源：http://chg.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://xsf.meibo888.top

[H05] 捕获特定类型
来源：http://qnz.shuidangran.top

Py:   except ValueError as e:
来源：http://rsu.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ypa.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://frc.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://rfe.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://fal.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hxk.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://vfq.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zbz.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ygn.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://ift.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bow.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vja.hysaishi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hfw.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ybr.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bay.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://hzo.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://yix.snrcjt.cn

[H07] 断言
来源：http://jgv.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://zej.birdmap.top

PHP:  assert($x > 0);
来源：http://poz.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://frm.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://ovr.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://zoo.jianghu66.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ujz.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vam.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://wkd.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://pqi.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://xav.yanxiufei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ubw.tian-w.cn

JS:   e.message;  e.stack
来源：http://ddp.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcr.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ymx.hammf.cn

Go:   err.Error()
来源：http://nqb.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://ziv.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://lqs.sjlbkw.cn

[H09] 带错误码的异常
来源：http://pvo.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://afj.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://dlg.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pam.yvedp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blw.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://txq.316326.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sym.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wke.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tki.mhx1999.top

[H10] 资源自动释放
来源：http://pau.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ovt.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uot.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pqe.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmw.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mbj.jqgfzy.top

Go:   defer f.Close()
来源：http://nvg.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uhe.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cvj.xingfuxueyuan.xyz

================================================================================
来源：http://gal.tian-w.cn

I. 正则表达式
来源：http://xyz.shanyushiyangkeji.top

================================================================================
来源：http://frt.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://esk.dianchejie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pwr.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kxo.yvedp.cn

JS:   /\d+/.test(s)
来源：http://fwh.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://wsb.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vjz.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mig.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://csx.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sul.tianlin.xyz

[I02] 提取所有匹配
来源：http://bhg.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://bnw.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://asi.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dvb.tarul.cn

TS:   s.match(/\d+/g)
来源：http://fwj.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jfh.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jwp.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://ykq.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tcv.yj20258888.top

[I03] 提取捕获分组
来源：http://ldd.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mcv.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fzm.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ttn.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wfv.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://edm.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://end.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://npn.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dwu.hnxiangtu.top

[I04] 正则替换
来源：http://rqv.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lol.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zhg.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://zti.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://qna.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://hrj.mhx1999.top


<!-- 参考信息 -->