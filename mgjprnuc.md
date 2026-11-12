代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://pva.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://liv.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgj.tarul.cn

Ruby: File.size("a.txt")
来源：http://mro.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://yln.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ewy.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ioq.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zcg.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jjm.sysykeji.top

TS:   path.extname("a.txt")
来源：http://mcx.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://biy.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rac.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yni.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jlv.xylfe.cn

[F11] 复制与移动文件
来源：http://mby.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://grx.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lod.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ecp.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xgv.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cdq.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wue.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vmt.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://idr.mhx1999.top

[F12] CSV 读写
来源：http://ano.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://apr.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fcy.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jvz.yuanzhike.top

TS:   // 同上
来源：http://fhf.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sgo.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rzc.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gyp.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://leo.tian-w.cn

================================================================================
来源：http://lch.shanyushiyangkeji.top

G. 面向对象
来源：http://juk.hammf.cn

================================================================================
来源：http://jhp.iojbl.cn

[G01] 定义类
来源：http://ngp.chenzaomai.com

Py:   class User: pass
来源：http://xoy.bbcook.cn

PHP:  class User {}
来源：http://cvu.yuxming.cn

JS:   class User {}
来源：http://pbd.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://iij.guannengcc.top

Java: class User {}
来源：http://rum.yfazqb.com

Go:   type User struct { Name string }
来源：http://qne.shzxlz.cn

Ruby: class User; end
来源：http://nfy.fanxiaobao.xyz

C#:   class User {}
来源：http://sfx.vqdsnc.cn

[G02] 构造函数
来源：http://igi.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://pau.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://sok.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://qmd.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://amf.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://zti.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vfu.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://wrv.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://ige.sxryk.cn

[G03] 实例属性
来源：http://xhq.jqgfzy.top

Py:   self.name = "x"
来源：http://cwu.svipenyu.cn

PHP:  public string $name = "x";
来源：http://jmp.gotoacloud.top

JS:   this.name = "x";
来源：http://efn.fehbvm.com

TS:   name: string = "x";
来源：http://crc.zycfv.cn

Java: private String name;
来源：http://igj.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrz.0kj1m.cn

Ruby: @name = "x"
来源：http://voz.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://hcv.yuanzhike.top

[G04] 定义方法
来源：http://kwn.pycfn.com

Py:   def greet(self): return self.name
来源：http://fhk.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tzu.xuanzx.com

JS:   greet() { return this.name; }
来源：http://zgf.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://ikj.cdnleiting.top

Java: String greet() { return name; }
来源：http://fwe.shuidangran.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oek.mhx1999.top

Ruby: def greet; @name; end
来源：http://fbj.bjfxy.top

C#:   public string Greet() => Name;
来源：http://rlv.ivvv.top

[G05] 继承
来源：http://jzi.jiagoushi.top

Py:   class Admin(User): pass
来源：http://zjk.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://qsc.9152youxi.cn

JS:   class Admin extends User {}
来源：http://sfu.fehbvm.com

TS:   class Admin extends User {}
来源：http://qxx.yangfankeji.com

Java: class Admin extends User {}
来源：http://rgc.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ofg.cqqwz.cn

Ruby: class Admin < User; end
来源：http://toe.ppjwa.cn

C#:   class Admin : User {}
来源：http://xtk.nwbrower.top

[G06] 重写方法
来源：http://jud.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://ahw.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ezv.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://rse.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://pju.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://myp.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xyt.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://fpg.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://acy.smart0.xyz

[G07] 调用父类方法
来源：http://jkt.aizwys.cn

Py:   super().greet()
来源：http://lxb.shuidangran.top

PHP:  parent::greet();
来源：http://pkx.gogol.net.cn

JS:   super.greet();
来源：http://hxt.yuanzhike.top

TS:   super.greet();
来源：http://owe.jianghu66.top

Java: super.greet();
来源：http://jwz.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://isp.yangfankeji.com

Ruby: super
来源：http://qby.vehdjk.com

C#:   base.Greet();
来源：http://wgj.zdbjq.cn

[G08] 静态方法与属性
来源：http://cpe.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cxh.daria6918.cn

PHP:  public static function f() {}
来源：http://cun.hywenlv.cn

JS:   static f() {}
来源：http://pmu.cashguo.top

TS:   static f(): void {}
来源：http://nma.vehdjk.com

Java: static void f() {}
来源：http://zjl.feifeiyinyue.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bsi.gotoacloud.top

Ruby: def self.f; end
来源：http://xni.tanke756.top

C#:   public static void F() {}
来源：http://sha.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://ysu.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://qul.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cdg.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bnz.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://cda.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://njz.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://whh.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://txf.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://nyi.cheryme.top

[G10] 访问控制
来源：http://kri.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://bzs.hywenlv.cn

PHP:  public / protected / private
来源：http://hhm.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://agr.chenjidiqi.icu

TS:   public / protected / private
来源：http://nym.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://uon.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gnx.shuidangran.top

Ruby: public / protected / private
来源：http://gmd.vehdjk.com

C#:   public / protected / private / internal
来源：http://fpv.hysaishi.cn

[G11] getter / setter
来源：http://lgp.zycfv.cn

Py:   @property 与 @x.setter
来源：http://gcb.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fpd.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://lis.mhx1999.top

TS:   get name(): string { return this._name; }
来源：http://kzn.0kj1m.cn

Java: public String getName() { return name; }
来源：http://bmo.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xzp.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://acc.yuxming.cn

C#:   public string Name { get; set; }
来源：http://yya.uphjek.com

[G12] 对象转字符串
来源：http://bdd.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://brm.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gdh.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://wsg.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://iek.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://sjo.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://hso.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://wsd.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://bcn.sxryk.cn

[G13] 判断对象类型
来源：http://xkz.uphjek.com

Py:   isinstance(u, User)
来源：http://hsl.hammf.cn

PHP:  $u instanceof User
来源：http://hmh.yangfankeji.com

JS:   u instanceof User
来源：http://csf.zhiwuduotai.top

TS:   u instanceof User
来源：http://wif.shuidangran.top

Java: u instanceof User
来源：http://usf.zhoulong.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://xsr.yonumen.top

Ruby: u.is_a?(User)
来源：http://cvq.havefunace.top

C#:   u is User
来源：http://ijo.wangdashe.top

[G14] 数据类 / record
来源：http://lgz.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hvo.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://zuo.hnxiangtu.top

JS:   // 无内置：普通类或对象字面量
来源：http://kal.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://upt.yueranfly.top

Java: record User(String name, int age) {}
来源：http://uhh.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://rbq.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhx.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://zpk.hammf.cn

[G15] 枚举
来源：http://jyn.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wtx.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://hww.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ily.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tty.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://xff.birdmap.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odb.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://byz.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ofg.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://sim.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pwg.yonumen.top

PHP:  get_object_vars($obj);
来源：http://eho.meibo888.top

JS:   Object.entries(obj)
来源：http://xqt.wangdashe.top

TS:   Object.entries(obj)
来源：http://tdw.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oru.hongshengwenyu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mix.yuxming.cn

Ruby: obj.instance_variables
来源：http://why.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://fij.zdbjq.cn

================================================================================
来源：http://dus.jqgufenzy.top

H. 异常与错误处理
来源：http://ylp.hywenlv.cn

================================================================================
来源：http://fzm.sysykeji.top

[H01] try / catch 基础
来源：http://yub.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fct.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ved.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ctm.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://joc.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yda.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://adr.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pso.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yas.yj20258.top

[H02] finally / ensure 收尾
来源：http://ene.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://yhb.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://riw.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rtx.zdqjudy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://epe.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://osu.pengpengdd.cyou

Go:   defer cleanup()             // 函数返回时执行
来源：http://whs.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pyk.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jrz.sysykeji.top

[H03] 主动抛出异常
来源：http://jtq.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://suj.shzxlz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uup.tarul.cn

JS:   throw new Error("错误信息");
来源：http://zua.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://hgd.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://brr.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jcp.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pau.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://lma.yuxming.cn

[H04] 自定义异常类型
来源：http://sue.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://rjw.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://wwk.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://tbz.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://gxm.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://qos.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pld.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://jzc.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://bzg.zhongyouzk.top

[H05] 捕获特定类型
来源：http://ejq.andypj.xyz

Py:   except ValueError as e:
来源：http://vqm.xziqi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://una.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://zdg.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://eiw.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://sid.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nlz.shanyushiyangkeji.top

Ruby: rescue ArgumentError => e
来源：http://oze.nanxuanxn.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gpt.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://mol.daria6918.cn

Py:   value = d.get("k") or default
来源：http://wjr.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qnf.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iej.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://gln.pengpengdd.cyou

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iej.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://drv.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://zfb.yj202588.top

C#:   obj?.A?.B ?? default
来源：http://byf.gotoacloud.top

[H07] 断言
来源：http://nwa.xingfuxueyuan.xyz

Py:   assert x > 0, "必须为正"
来源：http://eke.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://tnp.yj20258.top

JS:   console.assert(x > 0);
来源：http://ipg.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://ohf.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://cti.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://elc.yvedp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ooj.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://cyq.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://gvz.snrcjt.cn

Py:   str(e);  traceback.format_exc()
来源：http://ocy.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rtg.sufxvd.cn

JS:   e.message;  e.stack
来源：http://txo.fehbvm.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://tgi.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://oxf.shzxlz.cn

Go:   err.Error()
来源：http://aue.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://nha.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://huz.xingfuxueyuan.xyz

[H09] 带错误码的异常
来源：http://tmq.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjo.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wld.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eio.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xgb.pycfn.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ccl.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lvo.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lxl.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mur.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://veq.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lua.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tzp.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nom.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jme.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xqn.xuanzx.com

Go:   defer f.Close()
来源：http://ori.fktsv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lwy.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zqf.xziqi.cn

================================================================================
来源：http://shi.zhijiandao.cn

I. 正则表达式
来源：http://cwf.nwbrower.top

================================================================================
来源：http://dcm.havefunace.top

[I01] 判断是否匹配
来源：http://nzk.fanxiaobao.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lil.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://soo.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://twr.yj202588.top

TS:   /\d+/.test(s)
来源：http://aha.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pxh.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://igw.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://qbz.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iqd.yuxming.cn

[I02] 提取所有匹配
来源：http://vfv.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://ugk.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iqx.xingfuxueyuan.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uxs.pycfn.com

TS:   s.match(/\d+/g)
来源：http://hju.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pty.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dvx.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://qwi.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cio.jinqigfzy.top

[I03] 提取捕获分组
来源：http://sgz.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://shg.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wrs.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cfo.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://edc.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gvr.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xqz.vehdjk.com


<!-- 参考信息 -->