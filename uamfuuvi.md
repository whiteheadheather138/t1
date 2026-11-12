代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qoj.cucudq.cn

TS:   path.extname("a.txt")
来源：http://vom.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mke.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://coq.guowangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rop.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gtj.tarul.cn

[F11] 复制与移动文件
来源：http://dft.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://exr.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dbr.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nxu.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://glp.chenlongwang.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iwx.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lbu.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pii.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jzq.shzxlz.cn

[F12] CSV 读写
来源：http://nyn.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aat.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jie.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egd.gaohongyu789.top

TS:   // 同上
来源：http://tkw.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nio.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://apm.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oao.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://odx.fanxiaobao.xyz

================================================================================
来源：http://gtt.xingfuxueyuan.xyz

G. 面向对象
来源：http://ycl.jinqigufen.top

================================================================================
来源：http://lkz.gogol.net.cn

[G01] 定义类
来源：http://aab.shanyushiyangtech.top

Py:   class User: pass
来源：http://uaj.jqgufenzy.top

PHP:  class User {}
来源：http://ydg.52xcode.cn

JS:   class User {}
来源：http://iha.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://zqv.ybcxt.top

Java: class User {}
来源：http://mra.tian-w.cn

Go:   type User struct { Name string }
来源：http://ifk.havefunace.top

Ruby: class User; end
来源：http://mra.haohaochexian.top

C#:   class User {}
来源：http://dmz.sufxvd.cn

[G02] 构造函数
来源：http://dar.cashguo.top

Py:   def __init__(self, name): self.name = name
来源：http://zfy.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://gvc.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://yhl.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://wet.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://dyf.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ieh.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://hrs.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://roj.ydjk.org.cn

[G03] 实例属性
来源：http://gkb.nanxuanxn.top

Py:   self.name = "x"
来源：http://srj.nwbrower.top

PHP:  public string $name = "x";
来源：http://lzl.yvedp.cn

JS:   this.name = "x";
来源：http://kbj.jiagoushi.top

TS:   name: string = "x";
来源：http://ldw.9152youxi.cn

Java: private String name;
来源：http://kxq.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://toh.quarkkingdee.top

Ruby: @name = "x"
来源：http://nxd.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://aaz.snrcjt.cn

[G04] 定义方法
来源：http://ogx.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://mwt.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://naj.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://jhi.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://icp.gaohongyu789.top

Java: String greet() { return name; }
来源：http://zte.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://maj.hammf.cn

Ruby: def greet; @name; end
来源：http://fub.smart0.xyz

C#:   public string Greet() => Name;
来源：http://tfg.ivvv.top

[G05] 继承
来源：http://iad.epnwcf.com

Py:   class Admin(User): pass
来源：http://gjr.daxiang520.top

PHP:  class Admin extends User {}
来源：http://wze.guannengcc.top

JS:   class Admin extends User {}
来源：http://tua.xylfe.cn

TS:   class Admin extends User {}
来源：http://efz.zdqjudy.top

Java: class Admin extends User {}
来源：http://vpx.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bdb.smart0.xyz

Ruby: class Admin < User; end
来源：http://rbe.yanxiufei.cn

C#:   class Admin : User {}
来源：http://acx.dashuyun.cn

[G06] 重写方法
来源：http://qda.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://xtz.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://gsl.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://tzt.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://prj.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://hkz.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cxd.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://ign.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://jgv.ctjpmb.com

[G07] 调用父类方法
来源：http://dhy.sjlbkw.cn

Py:   super().greet()
来源：http://plr.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://xez.yvedp.cn

JS:   super.greet();
来源：http://rcl.kuanghao11.cn

TS:   super.greet();
来源：http://ist.fzhhl.top

Java: super.greet();
来源：http://tsz.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qbq.vehdjk.com

Ruby: super
来源：http://qcn.tarul.cn

C#:   base.Greet();
来源：http://jvw.hesvh.cn

[G08] 静态方法与属性
来源：http://slk.quarkkingdee.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qsa.fengsongda.top

PHP:  public static function f() {}
来源：http://zbc.hnxiangtu.top

JS:   static f() {}
来源：http://erm.yuanzhike.top

TS:   static f(): void {}
来源：http://jnf.jinqigfzy.top

Java: static void f() {}
来源：http://iqp.fzhhl.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bvh.vqdsnc.cn

Ruby: def self.f; end
来源：http://dnb.52xcode.cn

C#:   public static void F() {}
来源：http://kce.meibo888.top

[G09] 接口 / 抽象类
来源：http://icg.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://bqu.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://wnd.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lco.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://gwo.tarul.cn

Java: interface Shape { double area(); }
来源：http://vpv.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ecc.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aul.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://qfq.chenjidiqi.icu

[G10] 访问控制
来源：http://eca.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://pik.gogol.net.cn

PHP:  public / protected / private
来源：http://bjz.cucudq.cn

JS:   #private 字段；其余公开
来源：http://sli.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://dhy.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://mju.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hcs.zdbjq.cn

Ruby: public / protected / private
来源：http://sfx.yuanzhike.top

C#:   public / protected / private / internal
来源：http://vix.kuanghao11.cn

[G11] getter / setter
来源：http://zur.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://xws.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://cuz.wangshuangyany.cn

JS:   get name() { return this._name; }
来源：http://dfr.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://ppe.uphjek.com

Java: public String getName() { return name; }
来源：http://xdf.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xng.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://ugp.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://ssv.hongshengwenyu.top

[G12] 对象转字符串
来源：http://mof.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://iux.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jer.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://kkc.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://qij.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://hny.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://jtq.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://uhf.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://gkg.ybcxt.top

[G13] 判断对象类型
来源：http://lip.zhixingplan.top

Py:   isinstance(u, User)
来源：http://gqw.fehbvm.com

PHP:  $u instanceof User
来源：http://xyn.hysaishi.cn

JS:   u instanceof User
来源：http://qkp.fzhhl.top

TS:   u instanceof User
来源：http://iri.guowangkeji.top

Java: u instanceof User
来源：http://jcv.hnxiangtu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://atk.c1oappe.top

Ruby: u.is_a?(User)
来源：http://hnb.yj202588.top

C#:   u is User
来源：http://acg.kuanghao11.cn

[G14] 数据类 / record
来源：http://wxa.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qxx.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://gqo.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://pih.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://bwl.tian-w.cn

Java: record User(String name, int age) {}
来源：http://aaz.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://bin.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vnk.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://cts.shuidangran.top

[G15] 枚举
来源：http://emx.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fgn.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rgh.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://led.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vjl.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://tpy.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mmy.wangdashe.top

Ruby: Color = %i[red green].freeze
来源：http://ffd.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lrj.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://jkx.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lfw.sweek.top

PHP:  get_object_vars($obj);
来源：http://pgs.jyoumei.cn

JS:   Object.entries(obj)
来源：http://oym.chenlongwang.top

TS:   Object.entries(obj)
来源：http://ysy.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qun.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lim.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://ubn.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://vsi.sufxvd.cn

================================================================================
来源：http://xdn.zdbjq.cn

H. 异常与错误处理
来源：http://wyd.fktsv.cn

================================================================================
来源：http://apn.yanxiufei.cn

[H01] try / catch 基础
来源：http://eba.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sjh.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rlw.ivvv.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fhj.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bgo.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ons.fehbvm.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oqc.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bfp.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://amw.cashguo.top

[H02] finally / ensure 收尾
来源：http://qwa.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xkn.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jfq.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://chp.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jrf.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jmb.52xcode.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lip.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yre.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://djx.uphjek.com

[H03] 主动抛出异常
来源：http://kyp.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://ulo.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qkk.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://lkn.wangdashe.top

TS:   throw new Error("错误信息");
来源：http://byf.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pzg.gaohongyu789.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gbo.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bps.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://gwg.yj202588.top

[H04] 自定义异常类型
来源：http://hhh.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://abn.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uqi.daxiang520.top

JS:   class MyError extends Error {}
来源：http://hhb.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://adq.c1oappe.top

Java: class MyException extends RuntimeException {}
来源：http://yru.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aek.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://irv.smart0.xyz

C#:   class MyException : Exception {}
来源：http://yep.pycfn.com

[H05] 捕获特定类型
来源：http://bbv.nwbrower.top

Py:   except ValueError as e:
来源：http://kgl.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owl.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://uxm.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://edy.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://mxr.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rxr.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://udm.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yis.hnxiangtu.top

[H06] 可选值 / 空值安全访问
来源：http://ire.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://ncl.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kxl.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eaq.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://rum.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eae.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dxr.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://dkz.cheryme.top

C#:   obj?.A?.B ?? default
来源：http://zed.jianghu66.top

[H07] 断言
来源：http://yva.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://jws.xylfe.cn

PHP:  assert($x > 0);
来源：http://rhm.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://mor.sxryk.cn

TS:   console.assert(x > 0);
来源：http://zjo.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://akk.vqdsnc.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zkv.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qbi.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://zqx.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://hhh.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://aup.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xdp.jlsjyb.cn

JS:   e.message;  e.stack
来源：http://ssx.chenzaomai.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qtx.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jyo.ppjwa.cn

Go:   err.Error()
来源：http://kjd.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://aed.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://xfx.9152youxi.cn

[H09] 带错误码的异常
来源：http://reg.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jzw.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cvs.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://waz.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tzd.quarkkingdee.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iip.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://avw.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://cdh.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pne.pycfn.com

[H10] 资源自动释放
来源：http://igq.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pfz.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qsw.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jxd.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gog.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wfj.sweek.top

Go:   defer f.Close()
来源：http://zre.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cab.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ipm.zhongyouzk.top

================================================================================
来源：http://wil.jinqigufen.top

I. 正则表达式
来源：http://lbn.nwbrower.top

================================================================================
来源：http://tep.shzxlz.cn

[I01] 判断是否匹配
来源：http://gtn.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jve.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pgl.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://bbg.fktsv.cn

TS:   /\d+/.test(s)
来源：http://rvb.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://usq.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://axo.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://bar.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://toe.fengsongda.top

[I02] 提取所有匹配
来源：http://qpu.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://clf.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dcl.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://khl.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://gxc.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xmm.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vec.jinyuanbaomall.cn

Ruby: s.scan(/\d+/)
来源：http://ogz.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pzt.hysaishi.cn

[I03] 提取捕获分组
来源：http://syy.gotoacloud.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pyg.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bhm.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://igl.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kmi.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gmg.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jse.ywan-chungtsiang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mjb.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mio.yfazqb.com

[I04] 正则替换
来源：http://qmr.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hlc.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://viu.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://lms.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://vrr.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://cdr.jiagoushi.top


<!-- 参考信息 -->