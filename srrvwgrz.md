代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iti.guannengcc.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xqp.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://ykd.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://jxv.aibaodan.cn

[F09] 获取文件大小
来源：http://uhh.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://yrc.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://spp.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://iko.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://byz.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://yzi.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mai.iojbl.cn

Ruby: File.size("a.txt")
来源：http://ssz.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://zbx.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://iyp.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://djo.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zzo.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qig.fktsv.cn

TS:   path.extname("a.txt")
来源：http://jum.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzs.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ygp.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hse.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qss.jlsjyb.cn

[F11] 复制与移动文件
来源：http://xwi.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wyj.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xwr.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmj.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zwh.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cry.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wkb.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bmp.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wxu.jinghuilouyu.cn

[F12] CSV 读写
来源：http://ona.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gab.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ckj.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lls.shangyingyoupin.top

TS:   // 同上
来源：http://nol.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rjj.xylfe.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jtd.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vdr.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lho.wangshuangyany.cn

================================================================================
来源：http://jpz.shanyushiyangkeji.top

G. 面向对象
来源：http://ynm.yanxiufei.cn

================================================================================
来源：http://fzw.ybcxt.top

[G01] 定义类
来源：http://yev.jianghu66.top

Py:   class User: pass
来源：http://imu.yueranfly.top

PHP:  class User {}
来源：http://glw.chenlongwang.top

JS:   class User {}
来源：http://asv.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://djw.ydjk.org.cn

Java: class User {}
来源：http://jox.yj20258.top

Go:   type User struct { Name string }
来源：http://bsc.ybcxt.top

Ruby: class User; end
来源：http://pxl.chenzaomai.com

C#:   class User {}
来源：http://akt.52xcode.cn

[G02] 构造函数
来源：http://iui.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://nlr.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://zua.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://rhg.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://cug.hcnkem.com

Java: User(String name) { this.name = name; }
来源：http://cso.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cye.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://jnv.zhongyouzk.top

C#:   public User(string name) { Name = name; }
来源：http://sqc.c1oappe.top

[G03] 实例属性
来源：http://sou.nanxuanxn.top

Py:   self.name = "x"
来源：http://kty.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://wbd.xylfe.cn

JS:   this.name = "x";
来源：http://ace.yanxiufei.cn

TS:   name: string = "x";
来源：http://mar.yanxiufei.cn

Java: private String name;
来源：http://ttb.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vjg.jqgfzy.top

Ruby: @name = "x"
来源：http://cpb.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://fam.ehwqpu.com

[G04] 定义方法
来源：http://juz.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://gpw.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gic.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://ugu.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://cob.daxiang520.top

Java: String greet() { return name; }
来源：http://brf.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hll.0kj1m.cn

Ruby: def greet; @name; end
来源：http://jpc.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://lhg.hcnkem.com

[G05] 继承
来源：http://luv.tanke756.top

Py:   class Admin(User): pass
来源：http://vmj.andypj.xyz

PHP:  class Admin extends User {}
来源：http://vnk.sysykeji.top

JS:   class Admin extends User {}
来源：http://vqm.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://rkr.chenlongwang.top

Java: class Admin extends User {}
来源：http://skt.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cjm.tianlin.xyz

Ruby: class Admin < User; end
来源：http://fny.yj20258888.top

C#:   class Admin : User {}
来源：http://xhg.ywan-chungtsiang.top

[G06] 重写方法
来源：http://one.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://lax.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zlz.sweek.top

JS:   greet() { return "admin"; }
来源：http://fnk.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://zyy.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://okj.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iwa.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://wda.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://jyp.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://mlq.ydjk.org.cn

Py:   super().greet()
来源：http://lth.fengsongda.top

PHP:  parent::greet();
来源：http://rkf.shzxlz.cn

JS:   super.greet();
来源：http://zob.jqgfzy.top

TS:   super.greet();
来源：http://xpa.guannengcc.top

Java: super.greet();
来源：http://nei.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jaq.sufxvd.cn

Ruby: super
来源：http://hsk.chenzaomai.com

C#:   base.Greet();
来源：http://pob.ybcxt.top

[G08] 静态方法与属性
来源：http://kco.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvs.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://fkl.hfpthk.cn

JS:   static f() {}
来源：http://mya.haohaochexian.top

TS:   static f(): void {}
来源：http://kzx.daxiang520.top

Java: static void f() {}
来源：http://kri.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdm.yuanzhike.top

Ruby: def self.f; end
来源：http://tnw.xziqi.cn

C#:   public static void F() {}
来源：http://gpm.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://sbq.yangfankeji.com

Py:   from abc import ABC, abstractmethod
来源：http://qpg.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ewh.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cdk.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://cmg.jinyuanbaomall.cn

Java: interface Shape { double area(); }
来源：http://kjv.hcnkem.com

Go:   type Shape interface { Area() float64 }
来源：http://lvi.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zyq.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://fnx.yj20258888.top

[G10] 访问控制
来源：http://zdl.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://jrw.chenjidiqi.icu

PHP:  public / protected / private
来源：http://iqk.sxryk.cn

JS:   #private 字段；其余公开
来源：http://qik.aibaodan.cn

TS:   public / protected / private
来源：http://omj.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://djt.epnwcf.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://acu.cdnleiting.top

Ruby: public / protected / private
来源：http://hqv.xinyue.icu

C#:   public / protected / private / internal
来源：http://rlu.cdnleiting.top

[G11] getter / setter
来源：http://iny.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://jnz.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ovl.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://ago.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://fek.cqqwz.cn

Java: public String getName() { return name; }
来源：http://afx.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hwg.yvedp.cn

Ruby: attr_accessor :name
来源：http://maf.c1oappe.top

C#:   public string Name { get; set; }
来源：http://veb.nwbrower.top

[G12] 对象转字符串
来源：http://awb.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://sel.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ruz.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://lao.kuanghao11.cn

TS:   toString(): string { return this.name; }
来源：http://aqu.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://dso.havefunace.top

Go:   func (u User) String() string { return u.Name }
来源：http://gtf.tarul.cn

Ruby: def to_s; @name; end
来源：http://zev.yonumen.top

C#:   public override string ToString() => Name;
来源：http://koo.zdbjq.cn

[G13] 判断对象类型
来源：http://ubj.ivvv.top

Py:   isinstance(u, User)
来源：http://fln.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://imz.chenjidiqi.icu

JS:   u instanceof User
来源：http://vdo.wangshuangyany.cn

TS:   u instanceof User
来源：http://djd.iojbl.cn

Java: u instanceof User
来源：http://qav.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dcl.nwbrower.top

Ruby: u.is_a?(User)
来源：http://fdp.nwbrower.top

C#:   u is User
来源：http://xxl.sxryk.cn

[G14] 数据类 / record
来源：http://odq.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fgu.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://iaz.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pkc.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://oid.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://dqi.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://uai.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ysy.fengsongda.top

C#:   record User(string Name, int Age);
来源：http://gta.shangyingyoupin.top

[G15] 枚举
来源：http://mca.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zje.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hwv.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://etk.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nri.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://kdu.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lxb.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://qqi.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xvf.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://hrx.ydzc1.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zwb.ehwqpu.com

PHP:  get_object_vars($obj);
来源：http://vmh.birdmap.top

JS:   Object.entries(obj)
来源：http://xgo.jqgfzy.top

TS:   Object.entries(obj)
来源：http://gfx.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dql.nwbrower.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://krt.snrcjt.cn

Ruby: obj.instance_variables
来源：http://ton.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://dyn.52xcode.cn

================================================================================
来源：http://jao.yuxming.cn

H. 异常与错误处理
来源：http://soj.zhiwuduotai.top

================================================================================
来源：http://lvm.feifeiyinyue.top

[H01] try / catch 基础
来源：http://kid.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://irp.jiagoushi.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hci.guannengcc.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kmt.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qat.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dpl.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yok.kuanghao11.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://arj.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xrm.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://wcv.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://nim.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fyk.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ast.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jui.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://vaq.havefunace.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zgp.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://fha.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://obt.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://ufs.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://kyw.jqgufenzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xmr.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://nnv.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://pbv.gzhubu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gez.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://joc.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ofd.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://juk.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://xka.nanxuanxn.top

Py:   class MyError(Exception): pass
来源：http://azs.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://msg.pycfn.com

JS:   class MyError extends Error {}
来源：http://egl.yuxming.cn

TS:   class MyError extends Error {}
来源：http://dnq.quarkkingdee.top

Java: class MyException extends RuntimeException {}
来源：http://rqf.gzhubu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://out.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://cga.mhx1999.top

C#:   class MyException : Exception {}
来源：http://jyh.dashuyun.cn

[H05] 捕获特定类型
来源：http://jqu.zhengqikj.top

Py:   except ValueError as e:
来源：http://ety.dianchejie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ish.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://kjh.ctjpmb.com

TS:   if (e instanceof TypeError) {}
来源：http://swu.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://yvf.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jpd.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://ucn.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://okl.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://eaf.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://vop.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://llu.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mzk.fktsv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xox.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bms.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lde.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://mxn.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://bdr.cashguo.top

[H07] 断言
来源：http://fwv.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://peq.yonumen.top

PHP:  assert($x > 0);
来源：http://ioo.sweek.top

JS:   console.assert(x > 0);
来源：http://jje.hnqzz.top

TS:   console.assert(x > 0);
来源：http://upf.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://fnt.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ubq.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xzw.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://cbm.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://rpi.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://ckm.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bob.redwolf501.top

JS:   e.message;  e.stack
来源：http://aed.fktsv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oiy.fanxiaobao.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://uuh.bbcook.cn

Go:   err.Error()
来源：http://ruk.pengpengdd.cyou

Ruby: e.message;  e.backtrace
来源：http://wgd.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://rpt.ehwqpu.com

[H09] 带错误码的异常
来源：http://smk.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gsz.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ohf.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tfi.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ece.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oqn.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vcg.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vsg.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kxe.hnqzz.top

[H10] 资源自动释放
来源：http://dvt.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://azo.fzhhl.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lua.hywenlv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://edv.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jyu.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://put.shzxlz.cn

Go:   defer f.Close()
来源：http://kcv.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oid.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kia.wangdashe.top

================================================================================
来源：http://kbu.jiagoushi.top

I. 正则表达式
来源：http://rsk.hnqzz.top

================================================================================
来源：http://uuu.fktsv.cn

[I01] 判断是否匹配
来源：http://adx.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cbd.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xsy.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://ifg.ybcxt.top

TS:   /\d+/.test(s)
来源：http://ymz.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yig.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sct.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://kvk.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ojp.yanxiufei.cn

[I02] 提取所有匹配
来源：http://inq.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://mjo.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vxb.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cpy.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://pcj.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pef.nwbrower.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://the.shanyushiyangtech.top

Ruby: s.scan(/\d+/)
来源：http://wlb.guowangkeji.top


<!-- 参考信息 -->