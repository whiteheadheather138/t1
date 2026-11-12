代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://brh.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jsa.zhijiandao.cn

[F11] 复制与移动文件
来源：http://cwi.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://csn.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fgq.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dto.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mgn.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tag.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wfj.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jpz.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhp.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://hif.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pdh.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uwn.hywenlv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://exq.jinghuilouyu.cn

TS:   // 同上
来源：http://qor.xingfuxueyuan.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ozg.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fou.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://raz.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vzz.zhoulong.xyz

================================================================================
来源：http://wbl.gaohongyu789.top

G. 面向对象
来源：http://lvq.daria6918.cn

================================================================================
来源：http://qen.shanyushiyangkeji.top

[G01] 定义类
来源：http://ell.cdnleiting.top

Py:   class User: pass
来源：http://coo.hesvh.cn

PHP:  class User {}
来源：http://ifz.feifeiyinyue.top

JS:   class User {}
来源：http://tez.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://cvt.vqdsnc.cn

Java: class User {}
来源：http://byk.hywenlv.cn

Go:   type User struct { Name string }
来源：http://uli.yvedp.cn

Ruby: class User; end
来源：http://ruw.chenjidiqi.icu

C#:   class User {}
来源：http://erq.feifeiyinyue.top

[G02] 构造函数
来源：http://siw.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://efa.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://fug.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://xfm.bjfxy.top

TS:   constructor(public name: string) {}
来源：http://nsv.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://hkc.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ydj.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://wyo.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://gov.yj202588.top

[G03] 实例属性
来源：http://mmg.ybcxt.top

Py:   self.name = "x"
来源：http://ooe.dashuyun.cn

PHP:  public string $name = "x";
来源：http://ovc.dianchejie.cn

JS:   this.name = "x";
来源：http://vfy.yuanzhike.top

TS:   name: string = "x";
来源：http://kus.guannengcc.top

Java: private String name;
来源：http://vdy.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ago.nwbrower.top

Ruby: @name = "x"
来源：http://dnd.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://lym.yonumen.top

[G04] 定义方法
来源：http://wwh.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://ffs.ehwqpu.com

PHP:  public function greet(): string { return $this->name; }
来源：http://zzu.wangdashe.top

JS:   greet() { return this.name; }
来源：http://rau.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://glz.yvedp.cn

Java: String greet() { return name; }
来源：http://rsk.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sxr.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://xry.yuxming.cn

C#:   public string Greet() => Name;
来源：http://wwa.zhaomingkeji.xyz

[G05] 继承
来源：http://npt.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://bgq.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://zcn.zdqjudy.top

JS:   class Admin extends User {}
来源：http://bey.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://chl.fktsv.cn

Java: class Admin extends User {}
来源：http://atb.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hjp.ivvv.top

Ruby: class Admin < User; end
来源：http://lfp.316326.xyz

C#:   class Admin : User {}
来源：http://gun.snrcjt.cn

[G06] 重写方法
来源：http://eve.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://nay.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pux.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://kjf.iojbl.cn

TS:   greet(): string { return "admin"; }
来源：http://joy.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://rne.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ixz.xuanzx.com

Ruby: def greet; "admin"; end
来源：http://uob.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://lkr.fzhhl.top

[G07] 调用父类方法
来源：http://oog.guannengcc.top

Py:   super().greet()
来源：http://cqh.aizwys.cn

PHP:  parent::greet();
来源：http://zqd.ybcxt.top

JS:   super.greet();
来源：http://csp.yongpay.top

TS:   super.greet();
来源：http://fry.tian-w.cn

Java: super.greet();
来源：http://vbg.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tcl.hcnkem.com

Ruby: super
来源：http://bkb.yuanzhike.top

C#:   base.Greet();
来源：http://wlo.uphjek.com

[G08] 静态方法与属性
来源：http://nje.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qly.vqdsnc.cn

PHP:  public static function f() {}
来源：http://rkr.zhijiandao.cn

JS:   static f() {}
来源：http://dly.svipenyu.cn

TS:   static f(): void {}
来源：http://lvh.guowangkeji.top

Java: static void f() {}
来源：http://fih.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://woj.cdnleiting.top

Ruby: def self.f; end
来源：http://ubp.gzhubu.top

C#:   public static void F() {}
来源：http://evk.ybcxt.top

[G09] 接口 / 抽象类
来源：http://ics.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://lbo.zhongyouzk.top

PHP:  interface Shape { public function area(): float; }
来源：http://cyh.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bjm.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://aoz.shuidangran.top

Java: interface Shape { double area(); }
来源：http://jqe.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://qfg.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://myn.zdbjq.cn

C#:   interface IShape { double Area(); }
来源：http://scc.vqdsnc.cn

[G10] 访问控制
来源：http://zwr.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://nei.yvedp.cn

PHP:  public / protected / private
来源：http://mnq.mhx1999.top

JS:   #private 字段；其余公开
来源：http://xgo.jqgfzy.top

TS:   public / protected / private
来源：http://bzl.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://qab.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ben.ydzc1.top

Ruby: public / protected / private
来源：http://hwp.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://zhy.ydzc1.top

[G11] getter / setter
来源：http://gxk.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://ckg.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nis.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://jiu.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://dda.fktsv.cn

Java: public String getName() { return name; }
来源：http://udx.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gph.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://qcg.feifeiyinyue.top

C#:   public string Name { get; set; }
来源：http://amy.xylfe.cn

[G12] 对象转字符串
来源：http://vpw.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://vjq.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://phu.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://yyu.9152youxi.cn

TS:   toString(): string { return this.name; }
来源：http://und.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://aei.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://nog.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://smk.nwbrower.top

C#:   public override string ToString() => Name;
来源：http://taf.ydjk.org.cn

[G13] 判断对象类型
来源：http://egh.zycfv.cn

Py:   isinstance(u, User)
来源：http://ydq.snrcjt.cn

PHP:  $u instanceof User
来源：http://lon.zhixingplan.top

JS:   u instanceof User
来源：http://qtb.shanyushiyangtech.top

TS:   u instanceof User
来源：http://zxr.vehdjk.com

Java: u instanceof User
来源：http://vqi.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aaj.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://foo.ivvv.top

C#:   u is User
来源：http://sxa.epnwcf.com

[G14] 数据类 / record
来源：http://esg.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wrc.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://kwe.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qru.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://wwd.gzhubu.top

Java: record User(String name, int age) {}
来源：http://eux.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://yaw.shzxlz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jfr.wangdashe.top

C#:   record User(string Name, int Age);
来源：http://xpl.xziqi.cn

[G15] 枚举
来源：http://lvp.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tio.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qtm.sjlbkw.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tjy.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zag.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://djw.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://puf.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://txr.gzhubu.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gbk.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://qds.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gdk.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://rhj.gzhubu.top

JS:   Object.entries(obj)
来源：http://spq.pycfn.com

TS:   Object.entries(obj)
来源：http://thb.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aar.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ueg.ydjk.org.cn

Ruby: obj.instance_variables
来源：http://mng.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://klp.aizwys.cn

================================================================================
来源：http://ggo.sufxvd.cn

H. 异常与错误处理
来源：http://hvr.chenlongwang.top

================================================================================
来源：http://bcr.yvedp.cn

[H01] try / catch 基础
来源：http://bpo.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lqh.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kgj.jyoumei.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mqn.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mmn.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pmg.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ekb.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wug.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://all.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://eld.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://amf.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xux.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gab.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yqs.iojbl.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hfq.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://roz.zhijiandao.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pxq.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lwd.yanxiufei.cn

[H03] 主动抛出异常
来源：http://phh.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://occ.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vvd.xinyue.icu

JS:   throw new Error("错误信息");
来源：http://uev.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://syb.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://blw.hysaishi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ris.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pze.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://sjy.c1oappe.top

[H04] 自定义异常类型
来源：http://ohr.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://vqs.havefunace.top

PHP:  class MyError extends RuntimeException {}
来源：http://jee.bbcook.cn

JS:   class MyError extends Error {}
来源：http://omy.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://shu.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://tuf.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szc.zycfv.cn

Ruby: class MyError < StandardError; end
来源：http://okj.hesvh.cn

C#:   class MyException : Exception {}
来源：http://vuq.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://meu.fehbvm.com

Py:   except ValueError as e:
来源：http://vag.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gwk.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://vib.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://eeh.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://key.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://chb.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://uig.shanyushiyangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://whx.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://wce.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://lfd.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://agr.haohaochexian.top

JS:   obj?.a?.b;  d ?? default
来源：http://cwl.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ahp.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wnv.cashguo.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ncy.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://rkp.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://gtn.mhx1999.top

[H07] 断言
来源：http://tmm.tian-w.cn

Py:   assert x > 0, "必须为正"
来源：http://blz.sweek.top

PHP:  assert($x > 0);
来源：http://ujn.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://rkm.wangdashe.top

TS:   console.assert(x > 0);
来源：http://mws.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://uul.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dpx.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bht.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://nhj.jinqigfzy.top

[H08] 获取错误信息与堆栈
来源：http://cih.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://gnv.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://phg.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://yao.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://evb.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://htb.jqgfzy.top

Go:   err.Error()
来源：http://csp.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://hxy.tianlin.xyz

C#:   e.Message;  e.StackTrace
来源：http://lxx.ppjwa.cn

[H09] 带错误码的异常
来源：http://njm.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://glp.fehbvm.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://eyd.shanyushiyangkeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bbg.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nac.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ctc.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dje.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://fgq.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://ajx.xylfe.cn

[H10] 资源自动释放
来源：http://lam.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lnq.zdbjq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dyi.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cxf.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qgi.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zcm.fktsv.cn

Go:   defer f.Close()
来源：http://xfu.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fag.ivvv.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lni.ybcxt.top

================================================================================
来源：http://xyu.xuanzx.com

I. 正则表达式
来源：http://mbk.ehwqpu.com

================================================================================
来源：http://mlr.tarul.cn

[I01] 判断是否匹配
来源：http://nxc.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lra.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://yuk.yueranfly.top

JS:   /\d+/.test(s)
来源：http://bhl.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://tia.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://crr.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nev.chenjidiqi.icu

Ruby: s.match?(/\d+/)
来源：http://efg.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://itc.birdmap.top

[I02] 提取所有匹配
来源：http://crf.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://rxi.fktsv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mzs.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vmx.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://uqw.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rtg.tarul.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tap.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://wdu.chenlongwang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hnc.gzhubu.top

[I03] 提取捕获分组
来源：http://gnl.xuetiantiany.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zsk.smart0.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://inm.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kdc.cashguo.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zsd.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yae.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wqx.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lze.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nay.shanyushiyangtech.top

[I04] 正则替换
来源：http://hyw.quarkkingdee.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hgw.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dra.jinqigufen.top

JS:   s.replace(/\d+/g, "#")
来源：http://nre.gaohongyu789.top

TS:   s.replace(/\d+/g, "#")
来源：http://bxw.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lsa.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yaw.cdnleiting.top

Ruby: s.gsub(/\d+/, "#")
来源：http://flx.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xyw.aizwys.cn

[I05] 按正则拆分
来源：http://tsw.tanke756.top


<!-- 参考信息 -->