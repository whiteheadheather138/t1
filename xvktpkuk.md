代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lje.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cfk.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ryh.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdf.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qjp.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://drw.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eun.zhongyouzk.top

[F12] CSV 读写
来源：http://ymp.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://doe.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bnd.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aik.ydzc1.top

TS:   // 同上
来源：http://oyx.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gtc.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://reb.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ifc.quarkkingdee.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tbp.0kj1m.cn

================================================================================
来源：http://poh.jqgfzy.top

G. 面向对象
来源：http://zne.haohaochexian.top

================================================================================
来源：http://pwh.birdmap.top

[G01] 定义类
来源：http://ayp.svipenyu.cn

Py:   class User: pass
来源：http://sox.iojbl.cn

PHP:  class User {}
来源：http://pba.gaohongyu789.top

JS:   class User {}
来源：http://nog.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://xhq.cdnleiting.top

Java: class User {}
来源：http://srn.birdmap.top

Go:   type User struct { Name string }
来源：http://gwu.gogol.net.cn

Ruby: class User; end
来源：http://fhb.52xcode.cn

C#:   class User {}
来源：http://wdk.zhixingplan.top

[G02] 构造函数
来源：http://vbn.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://xtc.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://evj.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://piz.yonumen.top

TS:   constructor(public name: string) {}
来源：http://xzc.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://iur.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://was.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://box.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://brx.zhiwuduotai.top

[G03] 实例属性
来源：http://mym.smart0.xyz

Py:   self.name = "x"
来源：http://xwp.52xcode.cn

PHP:  public string $name = "x";
来源：http://xkq.zycfv.cn

JS:   this.name = "x";
来源：http://ibg.daxiang520.top

TS:   name: string = "x";
来源：http://buj.tanke756.top

Java: private String name;
来源：http://aab.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rpw.hywenlv.cn

Ruby: @name = "x"
来源：http://hhf.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://nsu.ctjpmb.com

[G04] 定义方法
来源：http://cpp.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://dhr.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://opl.xuanzx.com

JS:   greet() { return this.name; }
来源：http://plr.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://aff.sysykeji.top

Java: String greet() { return name; }
来源：http://jen.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uza.haohaochexian.top

Ruby: def greet; @name; end
来源：http://ntx.c1oappe.top

C#:   public string Greet() => Name;
来源：http://mbp.sweek.top

[G05] 继承
来源：http://krx.fehbvm.com

Py:   class Admin(User): pass
来源：http://vdt.nwbrower.top

PHP:  class Admin extends User {}
来源：http://hlr.jqgufenzy.top

JS:   class Admin extends User {}
来源：http://zkj.yj202588.top

TS:   class Admin extends User {}
来源：http://sbl.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://rln.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zhm.hcnkem.com

Ruby: class Admin < User; end
来源：http://vle.jlsjyb.cn

C#:   class Admin : User {}
来源：http://hjo.wangshuangyany.cn

[G06] 重写方法
来源：http://oao.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://wzf.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mlz.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://div.hywenlv.cn

TS:   greet(): string { return "admin"; }
来源：http://org.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://byf.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://btj.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://cew.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://lpq.52xcode.cn

[G07] 调用父类方法
来源：http://cym.tanke756.top

Py:   super().greet()
来源：http://aou.wangdashe.top

PHP:  parent::greet();
来源：http://uyd.daria6918.cn

JS:   super.greet();
来源：http://ulw.zdqjudy.top

TS:   super.greet();
来源：http://xng.fktsv.cn

Java: super.greet();
来源：http://aqr.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cox.9152youxi.cn

Ruby: super
来源：http://lyb.zhixingplan.top

C#:   base.Greet();
来源：http://eyj.daxiang520.top

[G08] 静态方法与属性
来源：http://wft.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mvi.yangfankeji.com

PHP:  public static function f() {}
来源：http://pgy.chenjidiqi.icu

JS:   static f() {}
来源：http://enq.chenlongwang.top

TS:   static f(): void {}
来源：http://urx.hysaishi.cn

Java: static void f() {}
来源：http://cys.bbcook.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xlo.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://uoo.zdbjq.cn

C#:   public static void F() {}
来源：http://hqg.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://bbo.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://dcl.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://ngf.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rjh.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://awh.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://lsi.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://rnd.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yoy.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://tla.hesvh.cn

[G10] 访问控制
来源：http://hkq.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://aar.pengpengdd.cyou

PHP:  public / protected / private
来源：http://rqj.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://krs.zycfv.cn

TS:   public / protected / private
来源：http://foe.aibaodan.cn

Java: public / protected / private / 默认包级
来源：http://nup.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xcq.xingfuxueyuan.xyz

Ruby: public / protected / private
来源：http://nkm.ivvv.top

C#:   public / protected / private / internal
来源：http://hpr.nanxuanxn.top

[G11] getter / setter
来源：http://ibo.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://nej.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wpb.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://mvm.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://zjf.yongpay.top

Java: public String getName() { return name; }
来源：http://rry.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ycm.yanxiufei.cn

Ruby: attr_accessor :name
来源：http://dgf.birdmap.top

C#:   public string Name { get; set; }
来源：http://vaz.zhaomingkeji.xyz

[G12] 对象转字符串
来源：http://wcf.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://ztv.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zzd.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://ghf.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://eyn.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://svp.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://otv.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://lvx.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://vxn.zhoulong.xyz

[G13] 判断对象类型
来源：http://lik.mhx1999.top

Py:   isinstance(u, User)
来源：http://rju.nanxinkj.top

PHP:  $u instanceof User
来源：http://xlh.zhongyouzk.top

JS:   u instanceof User
来源：http://lvz.ybcxt.top

TS:   u instanceof User
来源：http://mhy.shanyushiyangkeji.top

Java: u instanceof User
来源：http://yuz.sweek.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wpn.cucudq.cn

Ruby: u.is_a?(User)
来源：http://ocj.snrcjt.cn

C#:   u is User
来源：http://quk.zdbjq.cn

[G14] 数据类 / record
来源：http://xxb.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bdl.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://upe.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kam.zhijiandao.cn

TS:   type User = { name: string; age: number };
来源：http://kpu.iojbl.cn

Java: record User(String name, int age) {}
来源：http://vvu.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://aci.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rmr.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://yvf.fanxiaobao.xyz

[G15] 枚举
来源：http://oky.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uxy.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://twf.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pqs.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jdr.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://jvm.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dxg.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://jcr.zhiwuduotai.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mlm.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://ejw.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jki.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://eqz.cqqwz.cn

JS:   Object.entries(obj)
来源：http://ckh.yuanzhike.top

TS:   Object.entries(obj)
来源：http://ewd.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hid.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lko.shzxlz.cn

Ruby: obj.instance_variables
来源：http://icc.ybcxt.top

C#:   // 用反射或 System.Text.Json
来源：http://bmu.andypj.xyz

================================================================================
来源：http://ucz.ydjk.org.cn

H. 异常与错误处理
来源：http://irg.aibaodan.cn

================================================================================
来源：http://zvo.cdnleiting.top

[H01] try / catch 基础
来源：http://mlq.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dxr.0kj1m.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ywy.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vis.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mqj.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bro.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zab.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://urw.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yyx.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://vid.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://kbl.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hnh.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qwy.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xxf.52xcode.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ary.chenzaomai.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://blr.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zbx.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ejx.hnqzz.top

[H03] 主动抛出异常
来源：http://wxx.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://jfu.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pvk.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://alc.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://xwa.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://kly.cucudq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hag.yfazqb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cwo.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kkv.fengsongda.top

[H04] 自定义异常类型
来源：http://tar.gaohongyu789.top

Py:   class MyError(Exception): pass
来源：http://uwu.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wgn.epnwcf.com

JS:   class MyError extends Error {}
来源：http://pnq.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://uqp.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://gdn.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ygn.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://xzf.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://stj.dianchejie.cn

[H05] 捕获特定类型
来源：http://aux.kuanghao11.cn

Py:   except ValueError as e:
来源：http://xsm.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wpr.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://gwn.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://xbo.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://krn.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jnd.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://tuk.zhongyouzk.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dun.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://out.tanke756.top

Py:   value = d.get("k") or default
来源：http://qsy.yj20258888.top

PHP:  $v = $d["k"] ?? null;
来源：http://aff.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://tku.sxryk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pgs.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vqm.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jnx.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://tps.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://btl.bjfxy.top

[H07] 断言
来源：http://gvl.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://fdn.chenlongwang.top

PHP:  assert($x > 0);
来源：http://pyj.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://zdk.jianghu66.top

TS:   console.assert(x > 0);
来源：http://yiq.sweek.top

Java: assert x > 0 : "必须为正";
来源：http://fkj.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bhc.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://fyi.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://mol.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://uop.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://dxg.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sez.ehwqpu.com

JS:   e.message;  e.stack
来源：http://urq.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tiu.ydjk.org.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gzw.guannengcc.top

Go:   err.Error()
来源：http://bav.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://rff.smart0.xyz

C#:   e.Message;  e.StackTrace
来源：http://cra.9152youxi.cn

[H09] 带错误码的异常
来源：http://egk.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tsp.daxiang520.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zpo.guannengcc.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hsk.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ogw.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tyu.pengpengdd.cyou

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ebb.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://lnn.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nam.shzxlz.cn

[H10] 资源自动释放
来源：http://fse.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xlm.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gqr.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xcc.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rzr.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nzm.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://jdh.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lzg.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mkb.fengsongda.top

================================================================================
来源：http://dgq.svipenyu.cn

I. 正则表达式
来源：http://vsz.hcnkem.com

================================================================================
来源：http://hte.zhixingplan.top

[I01] 判断是否匹配
来源：http://hat.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://auq.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://joo.aizwys.cn

JS:   /\d+/.test(s)
来源：http://pnz.fktsv.cn

TS:   /\d+/.test(s)
来源：http://lii.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://asz.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jfi.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://zpp.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qdz.guowangkeji.top

[I02] 提取所有匹配
来源：http://onh.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://wtp.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cvh.feifeiyinyue.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zib.havefunace.top

TS:   s.match(/\d+/g)
来源：http://spo.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://piz.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ahk.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://suk.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lke.pycfn.com

[I03] 提取捕获分组
来源：http://iqf.ydzc1.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yjs.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jrl.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cml.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gnj.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tqa.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wfd.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jsc.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pxj.c1oappe.top

[I04] 正则替换
来源：http://ukm.gaohongyu789.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qxr.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kgy.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://syu.tianlin.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://qtw.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://dpp.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nny.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ydj.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iza.shangyingyoupin.top

[I05] 按正则拆分
来源：http://lfz.hesvh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uqx.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ytw.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://eaf.xziqi.cn

TS:   s.split(/\s*,\s*/)
来源：http://nls.yueranfly.top


<!-- 参考信息 -->