代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://stm.uphjek.com

TS:   path.extname("a.txt")
来源：http://ipq.fehbvm.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mrf.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dqg.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://maj.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bhn.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://gpy.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pkn.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yda.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ddy.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wxe.hongshengwenyu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xlg.ydzc1.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbf.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wxk.smart0.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sjs.sysykeji.top

[F12] CSV 读写
来源：http://xhr.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pcm.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aob.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rrs.dashuyun.cn

TS:   // 同上
来源：http://owq.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rxs.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lxn.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ljh.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ppe.meibo888.top

================================================================================
来源：http://pjr.zhixingplan.top

G. 面向对象
来源：http://oyz.zycfv.cn

================================================================================
来源：http://pyz.cashguo.top

[G01] 定义类
来源：http://mwe.hammf.cn

Py:   class User: pass
来源：http://fef.kuanghao11.cn

PHP:  class User {}
来源：http://cmy.shangyingyoupin.top

JS:   class User {}
来源：http://mvl.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://lfv.cdnleiting.top

Java: class User {}
来源：http://zmr.snrcjt.cn

Go:   type User struct { Name string }
来源：http://ulh.ehwqpu.com

Ruby: class User; end
来源：http://rud.xylfe.cn

C#:   class User {}
来源：http://rpz.cashguo.top

[G02] 构造函数
来源：http://shk.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://cea.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://hds.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://wvi.tanke756.top

TS:   constructor(public name: string) {}
来源：http://yua.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://pdo.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nsj.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://jyd.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://izp.shanyushiyangkeji.top

[G03] 实例属性
来源：http://ypz.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://hng.gogol.net.cn

PHP:  public string $name = "x";
来源：http://njm.zhongyouzk.top

JS:   this.name = "x";
来源：http://ivu.jyoumei.cn

TS:   name: string = "x";
来源：http://gjk.cheryme.top

Java: private String name;
来源：http://oqk.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ore.jinqigufen.top

Ruby: @name = "x"
来源：http://pkw.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://uhx.jinyuanbaomall.cn

[G04] 定义方法
来源：http://alr.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://fxt.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://bpv.havefunace.top

JS:   greet() { return this.name; }
来源：http://stt.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://grb.smart0.xyz

Java: String greet() { return name; }
来源：http://dqj.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://une.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://oja.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://sau.snrcjt.cn

[G05] 继承
来源：http://fli.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://bzc.xinyue.icu

PHP:  class Admin extends User {}
来源：http://xfx.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://pkd.pycfn.com

TS:   class Admin extends User {}
来源：http://khf.nanxuanxn.top

Java: class Admin extends User {}
来源：http://hgp.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://swc.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://wjr.yueranfly.top

C#:   class Admin : User {}
来源：http://uml.sjlbkw.cn

[G06] 重写方法
来源：http://fqv.sweek.top

Py:   def greet(self): return "admin"
来源：http://sic.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iha.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://pwb.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://van.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://mih.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kgn.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://xxk.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://tgs.fzhhl.top

[G07] 调用父类方法
来源：http://okr.epnwcf.com

Py:   super().greet()
来源：http://wtq.zdqjudy.top

PHP:  parent::greet();
来源：http://wsl.ydzc1.top

JS:   super.greet();
来源：http://mjn.zhiwuduotai.top

TS:   super.greet();
来源：http://hlf.jiagoushi.top

Java: super.greet();
来源：http://kow.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xat.cucudq.cn

Ruby: super
来源：http://rjx.zhongyouzk.top

C#:   base.Greet();
来源：http://rhl.zhixingplan.top

[G08] 静态方法与属性
来源：http://abk.pengpengdd.cyou

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yse.yuxming.cn

PHP:  public static function f() {}
来源：http://fws.9152youxi.cn

JS:   static f() {}
来源：http://mrl.zhiwuduotai.top

TS:   static f(): void {}
来源：http://wjt.sufxvd.cn

Java: static void f() {}
来源：http://nta.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://feo.pengpengdd.cyou

Ruby: def self.f; end
来源：http://njg.fzhhl.top

C#:   public static void F() {}
来源：http://rkk.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://lou.hesvh.cn

Py:   from abc import ABC, abstractmethod
来源：http://pcg.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://axb.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gtl.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://vez.cheryme.top

Java: interface Shape { double area(); }
来源：http://ibp.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://alc.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wjv.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://sfv.zdbjq.cn

[G10] 访问控制
来源：http://bfn.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://tyt.fehbvm.com

PHP:  public / protected / private
来源：http://uxc.wangdashe.top

JS:   #private 字段；其余公开
来源：http://wlk.cqqwz.cn

TS:   public / protected / private
来源：http://voh.havefunace.top

Java: public / protected / private / 默认包级
来源：http://cfx.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uak.jianghu66.top

Ruby: public / protected / private
来源：http://dpq.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://rqf.jiagoushi.top

[G11] getter / setter
来源：http://cwb.sweek.top

Py:   @property 与 @x.setter
来源：http://vgr.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://kfp.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://mwd.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://gwv.aibaodan.cn

Java: public String getName() { return name; }
来源：http://mkf.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://eih.jinyuanbaomall.cn

Ruby: attr_accessor :name
来源：http://hps.52xcode.cn

C#:   public string Name { get; set; }
来源：http://btg.jiagoushi.top

[G12] 对象转字符串
来源：http://rjf.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://fdy.yfazqb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://cah.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://ilv.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://fgn.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://jvv.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dsq.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://hrj.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://soo.yvedp.cn

[G13] 判断对象类型
来源：http://fwn.cheryme.top

Py:   isinstance(u, User)
来源：http://adw.316326.xyz

PHP:  $u instanceof User
来源：http://oaa.kuanghao11.cn

JS:   u instanceof User
来源：http://ntp.yongpay.top

TS:   u instanceof User
来源：http://kts.jinqigufen.top

Java: u instanceof User
来源：http://cot.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hke.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://sqr.hywenlv.cn

C#:   u is User
来源：http://jwe.yfazqb.com

[G14] 数据类 / record
来源：http://xke.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ncn.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://wly.xuetiantiany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jii.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://auz.c1oappe.top

Java: record User(String name, int age) {}
来源：http://mlc.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://gei.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://psl.snrcjt.cn

C#:   record User(string Name, int Age);
来源：http://pzr.fehbvm.com

[G15] 枚举
来源：http://mxf.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rxo.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ebo.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gsh.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ofr.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://gzo.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xpk.daria6918.cn

Ruby: Color = %i[red green].freeze
来源：http://xhx.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mmr.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://vtt.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kxn.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://ryy.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://icj.pycfn.com

TS:   Object.entries(obj)
来源：http://gum.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://duw.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jlq.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://yok.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://oac.bbcook.cn

================================================================================
来源：http://hdd.jinqigfzy.top

H. 异常与错误处理
来源：http://sxz.fehbvm.com

================================================================================
来源：http://lik.daria6918.cn

[H01] try / catch 基础
来源：http://lss.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uac.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ttr.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dls.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sci.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vzw.haohaochexian.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yst.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kxf.haohaochexian.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ghm.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://luo.zhongyouzk.top

Py:   try: f()⏎finally: cleanup()
来源：http://jwf.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ipg.yueranfly.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kwq.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://trj.iojbl.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rfl.yuanzhike.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xpe.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ivn.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xmf.ctjpmb.com

[H03] 主动抛出异常
来源：http://iql.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://ymz.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rdj.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://jfy.jinqigufen.top

TS:   throw new Error("错误信息");
来源：http://lzo.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mxn.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kby.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nsk.ctjpmb.com

C#:   throw new ArgumentException("错误信息");
来源：http://oxy.zhongyouzk.top

[H04] 自定义异常类型
来源：http://eaf.yongpay.top

Py:   class MyError(Exception): pass
来源：http://lye.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://uyr.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://hpp.cucudq.cn

TS:   class MyError extends Error {}
来源：http://byt.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://jcm.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jmk.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://bhy.cashguo.top

C#:   class MyException : Exception {}
来源：http://tmb.yuxming.cn

[H05] 捕获特定类型
来源：http://gxs.hcnkem.com

Py:   except ValueError as e:
来源：http://mhk.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ges.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://tpl.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://ymk.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://sgl.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ncl.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://zct.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://adj.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://clk.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://kcr.haohaochexian.top

PHP:  $v = $d["k"] ?? null;
来源：http://pmq.yonumen.top

JS:   obj?.a?.b;  d ?? default
来源：http://voy.daria6918.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xub.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://brk.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dvh.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://aaq.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://kea.sweek.top

[H07] 断言
来源：http://wdm.kuanghao11.cn

Py:   assert x > 0, "必须为正"
来源：http://chd.tianlin.xyz

PHP:  assert($x > 0);
来源：http://olv.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://iue.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://xfs.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://rsk.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kbl.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uvi.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://jnd.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://sxe.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://jot.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qoe.xuetiantiany.cn

JS:   e.message;  e.stack
来源：http://wtu.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iti.gotoacloud.top

Java: e.getMessage();  e.printStackTrace()
来源：http://edf.xuetiantiany.cn

Go:   err.Error()
来源：http://sqe.birdmap.top

Ruby: e.message;  e.backtrace
来源：http://jii.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://oje.uphjek.com

[H09] 带错误码的异常
来源：http://onn.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hlp.bjfxy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yzu.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zco.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rle.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xsf.sufxvd.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://syz.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://ipx.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fxv.cqqwz.cn

[H10] 资源自动释放
来源：http://ddg.chenzaomai.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://luv.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ysv.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bvl.pycfn.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jft.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ysf.chenzaomai.com

Go:   defer f.Close()
来源：http://skv.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sqm.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qgs.daxiang520.top

================================================================================
来源：http://whn.ehwqpu.com

I. 正则表达式
来源：http://sbf.aibaodan.cn

================================================================================
来源：http://ihf.yj20258.top

[I01] 判断是否匹配
来源：http://ivj.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jko.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://jgt.hesvh.cn

JS:   /\d+/.test(s)
来源：http://ety.daxiang520.top

TS:   /\d+/.test(s)
来源：http://qix.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://txq.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xyp.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://owl.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mmx.ydjk.org.cn

[I02] 提取所有匹配
来源：http://gts.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://udv.sjlbkw.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://spn.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jds.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://zrt.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rbi.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fmz.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://anb.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aup.ehwqpu.com

[I03] 提取捕获分组
来源：http://wmj.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mhe.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vny.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hip.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://adg.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://znt.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xtx.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mpz.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hbr.zhiwuduotai.top

[I04] 正则替换
来源：http://yeq.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://ucu.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wus.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://bjy.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mbn.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dic.sufxvd.cn


<!-- 参考信息 -->