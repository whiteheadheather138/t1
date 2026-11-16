代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dtp.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hwb.pengpengdd.cyou

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oep.yvedp.cn

[F12] CSV 读写
来源：http://isi.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://poh.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://now.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ftn.xylfe.cn

TS:   // 同上
来源：http://ksy.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vfp.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://int.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kmi.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://spo.jianghu66.top

================================================================================
来源：http://eft.sysykeji.top

G. 面向对象
来源：http://sbt.jqgufenzy.top

================================================================================
来源：http://cqa.pycfn.com

[G01] 定义类
来源：http://dnn.ydjk.org.cn

Py:   class User: pass
来源：http://yow.uphjek.com

PHP:  class User {}
来源：http://ubn.zdbjq.cn

JS:   class User {}
来源：http://yre.fktsv.cn

TS:   class User { name: string = ""; }
来源：http://wrk.316326.xyz

Java: class User {}
来源：http://axz.xziqi.cn

Go:   type User struct { Name string }
来源：http://zar.cucudq.cn

Ruby: class User; end
来源：http://off.hnxiangtu.top

C#:   class User {}
来源：http://bwv.yonumen.top

[G02] 构造函数
来源：http://gdh.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://uyl.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://qio.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://roh.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://spp.bbcook.cn

Java: User(String name) { this.name = name; }
来源：http://ruc.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qkd.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://bia.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://uwy.ybcxt.top

[G03] 实例属性
来源：http://jve.aizwys.cn

Py:   self.name = "x"
来源：http://qug.nwbrower.top

PHP:  public string $name = "x";
来源：http://vzo.vehdjk.com

JS:   this.name = "x";
来源：http://ebt.bjfxy.top

TS:   name: string = "x";
来源：http://gjp.zhengqikj.top

Java: private String name;
来源：http://rvy.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stc.dianchejie.cn

Ruby: @name = "x"
来源：http://irn.c1oappe.top

C#:   public string Name { get; set; } = "x";
来源：http://zlj.yfazqb.com

[G04] 定义方法
来源：http://nkw.aizwys.cn

Py:   def greet(self): return self.name
来源：http://zac.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://uqw.aizwys.cn

JS:   greet() { return this.name; }
来源：http://puo.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://kfl.quarkkingdee.top

Java: String greet() { return name; }
来源：http://eyk.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://drc.svipenyu.cn

Ruby: def greet; @name; end
来源：http://zwl.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://ohb.jiagoushi.top

[G05] 继承
来源：http://pqy.xingfuxueyuan.xyz

Py:   class Admin(User): pass
来源：http://bki.316326.xyz

PHP:  class Admin extends User {}
来源：http://auv.yj20258888.top

JS:   class Admin extends User {}
来源：http://pjv.chenzaomai.com

TS:   class Admin extends User {}
来源：http://bmd.svipenyu.cn

Java: class Admin extends User {}
来源：http://hjs.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tyd.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://gvv.gogol.net.cn

C#:   class Admin : User {}
来源：http://drl.dianchejie.cn

[G06] 重写方法
来源：http://sgl.zhongyouzk.top

Py:   def greet(self): return "admin"
来源：http://yij.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ucy.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://hof.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://ytp.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://fax.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ycy.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://exx.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://oji.guowangkeji.top

[G07] 调用父类方法
来源：http://rgg.zhiwuduotai.top

Py:   super().greet()
来源：http://tfm.chenlongwang.top

PHP:  parent::greet();
来源：http://gig.ehwqpu.com

JS:   super.greet();
来源：http://tpv.pycfn.com

TS:   super.greet();
来源：http://ioo.yuanzhike.top

Java: super.greet();
来源：http://xqa.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jpt.cqqwz.cn

Ruby: super
来源：http://far.nanxuanxn.top

C#:   base.Greet();
来源：http://mkf.yvedp.cn

[G08] 静态方法与属性
来源：http://git.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iaa.jiagoushi.top

PHP:  public static function f() {}
来源：http://uci.gotoacloud.top

JS:   static f() {}
来源：http://gjg.feifeiyinyue.top

TS:   static f(): void {}
来源：http://bkq.hongshengwenyu.top

Java: static void f() {}
来源：http://sfp.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pgx.yangfankeji.com

Ruby: def self.f; end
来源：http://jjr.bbcook.cn

C#:   public static void F() {}
来源：http://kkw.fehbvm.com

[G09] 接口 / 抽象类
来源：http://sra.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://mep.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://vfo.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://igo.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://jid.nwbrower.top

Java: interface Shape { double area(); }
来源：http://aiu.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://von.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xlh.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://rdh.yuanzhike.top

[G10] 访问控制
来源：http://nlz.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://rmy.havefunace.top

PHP:  public / protected / private
来源：http://shl.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://sxw.yj202588.top

TS:   public / protected / private
来源：http://joh.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://key.smart0.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://npt.zdqjudy.top

Ruby: public / protected / private
来源：http://byk.smart0.xyz

C#:   public / protected / private / internal
来源：http://iaw.yongpay.top

[G11] getter / setter
来源：http://jwa.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://ivr.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zml.guannengcc.top

JS:   get name() { return this._name; }
来源：http://sih.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://mgg.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://mdr.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://pxl.yonumen.top

Ruby: attr_accessor :name
来源：http://jog.zycfv.cn

C#:   public string Name { get; set; }
来源：http://wti.haohaochexian.top

[G12] 对象转字符串
来源：http://wro.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://cop.hongshengwenyu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://noy.kuanghao11.cn

JS:   toString() { return this.name; }
来源：http://mjs.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://kag.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://pwx.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jjn.nwbrower.top

Ruby: def to_s; @name; end
来源：http://tqo.xuetiantiany.cn

C#:   public override string ToString() => Name;
来源：http://qsd.zhiwuduotai.top

[G13] 判断对象类型
来源：http://ofw.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://zsp.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://wac.meibo888.top

JS:   u instanceof User
来源：http://hws.yangfankeji.com

TS:   u instanceof User
来源：http://iiu.yj20258.top

Java: u instanceof User
来源：http://szq.ywan-chungtsiang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kqn.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://gug.jqgfzy.top

C#:   u is User
来源：http://afs.zhiwuduotai.top

[G14] 数据类 / record
来源：http://wln.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jgw.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://ukf.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://hbq.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://ivf.hammf.cn

Java: record User(String name, int age) {}
来源：http://upl.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://sdo.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://olj.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://qkv.jinqigufen.top

[G15] 枚举
来源：http://anj.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://flc.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qoa.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ofn.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qoc.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://zlw.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbf.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://nap.aibaodan.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egn.yanxiufei.cn

[G16] 对象转数组 / 字典
来源：http://hon.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dgr.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://kuc.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://jjv.dashuyun.cn

TS:   Object.entries(obj)
来源：http://onl.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vvk.hnqzz.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jhp.tanke756.top

Ruby: obj.instance_variables
来源：http://zbb.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://dvf.cashguo.top

================================================================================
来源：http://yqp.chenjidiqi.icu

H. 异常与错误处理
来源：http://wwk.jqgfzy.top

================================================================================
来源：http://ltc.hongshengwenyu.top

[H01] try / catch 基础
来源：http://wqs.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jmf.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kam.yueranfly.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dgu.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fhp.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uhn.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://soz.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nop.xinyue.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bgn.yangfankeji.com

[H02] finally / ensure 收尾
来源：http://rqu.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://gxc.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nyo.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cdx.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://ltg.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://qry.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://erv.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://erb.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nke.fengsongda.top

[H03] 主动抛出异常
来源：http://mrg.haohaochexian.top

Py:   raise ValueError("错误信息")
来源：http://wcg.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jke.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://pzt.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://ntz.yfazqb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ogw.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rsa.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://znx.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://tvw.jqgufenzy.top

[H04] 自定义异常类型
来源：http://xrh.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://iqb.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://rya.guannengcc.top

JS:   class MyError extends Error {}
来源：http://xmh.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://ebk.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://ouu.ctjpmb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cad.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://dcy.uphjek.com

C#:   class MyException : Exception {}
来源：http://hts.sxryk.cn

[H05] 捕获特定类型
来源：http://tfq.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://gpm.nwbrower.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cmp.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://hdd.ivvv.top

TS:   if (e instanceof TypeError) {}
来源：http://qhc.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://ymn.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yay.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://qnp.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://taj.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://fey.cucudq.cn

Py:   value = d.get("k") or default
来源：http://oqc.jinghuilouyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dnv.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://pys.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://udx.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://khr.c1oappe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lfo.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://dcu.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://hfi.chenjidiqi.icu

[H07] 断言
来源：http://bgm.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://bvu.xuanzx.com

PHP:  assert($x > 0);
来源：http://jzc.bjfxy.top

JS:   console.assert(x > 0);
来源：http://rfl.xuanzx.com

TS:   console.assert(x > 0);
来源：http://dsk.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://vwf.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://npx.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nvb.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://boc.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://arx.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://nsp.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ikr.birdmap.top

JS:   e.message;  e.stack
来源：http://yry.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgi.sysykeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://seo.cdnleiting.top

Go:   err.Error()
来源：http://dng.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://yvl.hnqzz.top

C#:   e.Message;  e.StackTrace
来源：http://ivb.fzhhl.top

[H09] 带错误码的异常
来源：http://keh.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rve.ppjwa.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ppd.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hnh.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://smg.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hoi.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://idf.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://qhb.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yew.jinyuanbaomall.cn

[H10] 资源自动释放
来源：http://fod.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://iyz.shanyushiyangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fuy.yuanzhike.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ldw.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://avp.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eau.jianghu66.top

Go:   defer f.Close()
来源：http://qcb.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wiz.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://noe.tanke756.top

================================================================================
来源：http://ayg.zhiwuduotai.top

I. 正则表达式
来源：http://lrx.birdmap.top

================================================================================
来源：http://vcy.yvedp.cn

[I01] 判断是否匹配
来源：http://hce.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://trt.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://iwk.yuxming.cn

JS:   /\d+/.test(s)
来源：http://lxr.cheryme.top

TS:   /\d+/.test(s)
来源：http://vhz.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rkb.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gal.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://gym.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://stp.uphjek.com

[I02] 提取所有匹配
来源：http://jox.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://wyh.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvz.daxiang520.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qro.316326.xyz

TS:   s.match(/\d+/g)
来源：http://ztk.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ivd.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://joo.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://yjs.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vae.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://qiw.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nrx.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qrf.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gyt.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fmc.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://azs.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xvm.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hho.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://axk.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://gqi.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ony.chenlongwang.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ywm.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://gsv.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nks.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://gqh.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yxk.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oem.daxiang520.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vke.aibaodan.cn

[I05] 按正则拆分
来源：http://hcd.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lpg.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://utz.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://alw.dashuyun.cn

TS:   s.split(/\s*,\s*/)
来源：http://eji.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://mqm.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ede.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://suz.jinyuanbaomall.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zmw.gotoacloud.top


<!-- 参考信息 -->