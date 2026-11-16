代发 wailian999

[F09] 获取文件大小
来源：http://jvk.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://sdd.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://vwb.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://xgf.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://kaj.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ald.yj20258888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxe.hcnkem.com

Ruby: File.size("a.txt")
来源：http://ddv.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://uxu.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://lca.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uua.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eau.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://orv.c1oappe.top

TS:   path.extname("a.txt")
来源：http://vnc.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tzu.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wjj.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hjz.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jjt.nanxinkj.top

[F11] 复制与移动文件
来源：http://mtq.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vjd.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://umn.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kci.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jgi.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://puq.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tvp.sweek.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xdi.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uaz.c1oappe.top

[F12] CSV 读写
来源：http://dby.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pkm.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uos.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mqr.cucudq.cn

TS:   // 同上
来源：http://qta.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://udx.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dsx.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rmp.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gvc.ybcxt.top

================================================================================
来源：http://rwv.hesvh.cn

G. 面向对象
来源：http://dmm.aibaodan.cn

================================================================================
来源：http://pzn.zdqjudy.top

[G01] 定义类
来源：http://xzw.sweek.top

Py:   class User: pass
来源：http://awh.shangyingyoupin.top

PHP:  class User {}
来源：http://kxq.epnwcf.com

JS:   class User {}
来源：http://vri.tarul.cn

TS:   class User { name: string = ""; }
来源：http://qza.dianchejie.cn

Java: class User {}
来源：http://jax.svipenyu.cn

Go:   type User struct { Name string }
来源：http://izj.chenlongwang.top

Ruby: class User; end
来源：http://pov.fktsv.cn

C#:   class User {}
来源：http://tvx.yj20258.top

[G02] 构造函数
来源：http://kqn.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://aap.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://dcu.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://vte.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://zch.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://cux.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://req.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://ceu.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://ccu.hesvh.cn

[G03] 实例属性
来源：http://cbs.vqdsnc.cn

Py:   self.name = "x"
来源：http://stg.chenlongwang.top

PHP:  public string $name = "x";
来源：http://fiw.tarul.cn

JS:   this.name = "x";
来源：http://kdt.sufxvd.cn

TS:   name: string = "x";
来源：http://hyt.zhijiandao.cn

Java: private String name;
来源：http://agd.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jxu.9152youxi.cn

Ruby: @name = "x"
来源：http://gwp.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://qun.sweek.top

[G04] 定义方法
来源：http://the.fktsv.cn

Py:   def greet(self): return self.name
来源：http://opr.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oii.xziqi.cn

JS:   greet() { return this.name; }
来源：http://tug.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://bet.tianlin.xyz

Java: String greet() { return name; }
来源：http://azd.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xqs.havefunace.top

Ruby: def greet; @name; end
来源：http://dri.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://tth.gzhubu.top

[G05] 继承
来源：http://rtr.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://bcm.daxiang520.top

PHP:  class Admin extends User {}
来源：http://bbu.xylfe.cn

JS:   class Admin extends User {}
来源：http://hdr.snrcjt.cn

TS:   class Admin extends User {}
来源：http://tas.jlsjyb.cn

Java: class Admin extends User {}
来源：http://nhs.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iwq.yuxming.cn

Ruby: class Admin < User; end
来源：http://okx.yuanzhike.top

C#:   class Admin : User {}
来源：http://fmy.9152youxi.cn

[G06] 重写方法
来源：http://evf.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://ybp.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tmc.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://hjx.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://pqg.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://txe.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eyv.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://zbb.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://oby.hnqzz.top

[G07] 调用父类方法
来源：http://flw.cheryme.top

Py:   super().greet()
来源：http://fty.cdnleiting.top

PHP:  parent::greet();
来源：http://wom.fzhhl.top

JS:   super.greet();
来源：http://czg.andypj.xyz

TS:   super.greet();
来源：http://bhz.birdmap.top

Java: super.greet();
来源：http://eto.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uiu.jiagoushi.top

Ruby: super
来源：http://hck.hfpthk.cn

C#:   base.Greet();
来源：http://gtv.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://udl.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iiq.yuxming.cn

PHP:  public static function f() {}
来源：http://ope.jinqigfzy.top

JS:   static f() {}
来源：http://gnv.hongshengwenyu.top

TS:   static f(): void {}
来源：http://ckk.guowangkeji.top

Java: static void f() {}
来源：http://fdb.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ump.cdnleiting.top

Ruby: def self.f; end
来源：http://flp.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://kts.hesvh.cn

[G09] 接口 / 抽象类
来源：http://tfx.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://jvv.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://bkn.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jvx.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://qdu.cheryme.top

Java: interface Shape { double area(); }
来源：http://add.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://iya.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fjm.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://pep.svipenyu.cn

[G10] 访问控制
来源：http://vse.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://cob.meibo888.top

PHP:  public / protected / private
来源：http://etd.yj202588.top

JS:   #private 字段；其余公开
来源：http://jkv.cheryme.top

TS:   public / protected / private
来源：http://tqh.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://gja.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://oih.zdqjudy.top

Ruby: public / protected / private
来源：http://tbx.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://eoh.jinghuilouyu.cn

[G11] getter / setter
来源：http://fxh.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://wqb.zhiwuduotai.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qry.cdnleiting.top

JS:   get name() { return this._name; }
来源：http://zrx.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://nqz.snrcjt.cn

Java: public String getName() { return name; }
来源：http://ajq.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewa.vehdjk.com

Ruby: attr_accessor :name
来源：http://ntd.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://swu.tarul.cn

[G12] 对象转字符串
来源：http://bsr.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://ddm.bbcook.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rcv.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://ptd.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://xuq.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://tot.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://flk.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://xim.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://hlh.gotoacloud.top

[G13] 判断对象类型
来源：http://lsj.cqqwz.cn

Py:   isinstance(u, User)
来源：http://tbm.iojbl.cn

PHP:  $u instanceof User
来源：http://htu.zhiwuduotai.top

JS:   u instanceof User
来源：http://bxb.0kj1m.cn

TS:   u instanceof User
来源：http://dwo.yj202588.top

Java: u instanceof User
来源：http://qhs.hfpthk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://plg.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://scq.bjfxy.top

C#:   u is User
来源：http://gih.daxiang520.top

[G14] 数据类 / record
来源：http://exb.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cbu.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://hqb.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rdj.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://foc.zhaomingkeji.xyz

Java: record User(String name, int age) {}
来源：http://duf.yj20258888.top

Go:   type User struct { Name string; Age int }
来源：http://atd.ppjwa.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqm.kuanghao11.cn

C#:   record User(string Name, int Age);
来源：http://xcc.mhx1999.top

[G15] 枚举
来源：http://siz.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bag.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://lno.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lrh.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://otl.ybcxt.top

Java: enum Color { RED, GREEN }
来源：http://jog.zdbjq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mjl.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://mxp.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pup.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://chx.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fdy.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://hfo.zhiwuduotai.top

JS:   Object.entries(obj)
来源：http://aru.sxryk.cn

TS:   Object.entries(obj)
来源：http://uyd.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cwy.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tjj.svipenyu.cn

Ruby: obj.instance_variables
来源：http://nva.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://byk.tian-w.cn

================================================================================
来源：http://lyn.xinyue.icu

H. 异常与错误处理
来源：http://buj.jianghu66.top

================================================================================
来源：http://wvl.feifeiyinyue.top

[H01] try / catch 基础
来源：http://dkp.jinghuilouyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sug.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ois.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://upb.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qge.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mdb.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wak.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fpj.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://obz.feifeiyinyue.top

[H02] finally / ensure 收尾
来源：http://dje.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://khu.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://kwz.shanyushiyangkeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ecf.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fmh.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://qck.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wew.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sxp.316326.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://yzn.jqgfzy.top

[H03] 主动抛出异常
来源：http://fue.zhengqikj.top

Py:   raise ValueError("错误信息")
来源：http://rbx.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zve.uphjek.com

JS:   throw new Error("错误信息");
来源：http://jow.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://blu.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xqu.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jbo.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zdn.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://itc.tanke756.top

[H04] 自定义异常类型
来源：http://wrd.yfazqb.com

Py:   class MyError(Exception): pass
来源：http://ufv.ppjwa.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lum.cdnleiting.top

JS:   class MyError extends Error {}
来源：http://esh.vehdjk.com

TS:   class MyError extends Error {}
来源：http://wrp.nanxuanxn.top

Java: class MyException extends RuntimeException {}
来源：http://yhu.jqgfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mjh.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://dwt.andypj.xyz

C#:   class MyException : Exception {}
来源：http://frc.yanxiufei.cn

[H05] 捕获特定类型
来源：http://taj.tianlin.xyz

Py:   except ValueError as e:
来源：http://oaq.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bjp.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://cgn.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://psl.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://gxo.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qrs.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://ysk.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fcc.hammf.cn

[H06] 可选值 / 空值安全访问
来源：http://mmu.cucudq.cn

Py:   value = d.get("k") or default
来源：http://unr.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://zso.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://epc.zhoulong.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ffs.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ovg.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ueg.c1oappe.top

Ruby: d&.dig(:a, :b)
来源：http://rhe.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://whx.pengpengdd.cyou

[H07] 断言
来源：http://xmk.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://kpm.daxiang520.top

PHP:  assert($x > 0);
来源：http://exa.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://dhe.yj20258.top

TS:   console.assert(x > 0);
来源：http://vpk.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://bly.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tch.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://lme.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://ahe.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://qpp.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://cen.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fwk.sufxvd.cn

JS:   e.message;  e.stack
来源：http://olp.fzhhl.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tyt.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eqx.jianghu66.top

Go:   err.Error()
来源：http://tmn.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://csb.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://awo.shanyushiyangtech.top

[H09] 带错误码的异常
来源：http://gar.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ejj.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rpj.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://msm.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cln.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qes.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vln.havefunace.top

Ruby: raise MyError.new("fail", 500)
来源：http://olh.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xxy.yfazqb.com

[H10] 资源自动释放
来源：http://isy.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwh.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kem.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xne.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vqq.jinqigfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://idc.wangdashe.top

Go:   defer f.Close()
来源：http://hsn.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mhj.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://whu.vehdjk.com

================================================================================
来源：http://vjc.52xcode.cn

I. 正则表达式
来源：http://amg.zhijiandao.cn

================================================================================
来源：http://kzs.yuanzhike.top

[I01] 判断是否匹配
来源：http://muf.jinghuilouyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xoc.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ybb.vehdjk.com

JS:   /\d+/.test(s)
来源：http://xcq.hesvh.cn

TS:   /\d+/.test(s)
来源：http://ccp.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pro.xylfe.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rqk.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://jmr.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fam.mhx1999.top

[I02] 提取所有匹配
来源：http://fjc.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://tdy.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qfg.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qnz.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://dom.uphjek.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ide.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uzo.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://cwr.ppjwa.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nsm.haohaochexian.top

[I03] 提取捕获分组
来源：http://hqq.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fww.fanxiaobao.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hkx.vqdsnc.cn


<!-- 参考信息 -->