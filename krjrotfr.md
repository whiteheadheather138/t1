代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qcy.bbcook.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wrz.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mul.jqgufenzy.top

TS:   // 同上
来源：http://ytb.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cqv.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wgp.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vcy.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lxy.yuxming.cn

================================================================================
来源：http://gcz.guowangkeji.top

G. 面向对象
来源：http://pmy.vqdsnc.cn

================================================================================
来源：http://shw.bbcook.cn

[G01] 定义类
来源：http://dvy.hammf.cn

Py:   class User: pass
来源：http://nyn.chenzaomai.com

PHP:  class User {}
来源：http://sre.jinyuanbaomall.cn

JS:   class User {}
来源：http://gtg.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://cgr.yongpay.top

Java: class User {}
来源：http://kmk.0kj1m.cn

Go:   type User struct { Name string }
来源：http://pxy.bjfxy.top

Ruby: class User; end
来源：http://ivv.birdmap.top

C#:   class User {}
来源：http://iuv.bbcook.cn

[G02] 构造函数
来源：http://cfp.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://rlo.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://jkr.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://bzh.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://hmv.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://pkq.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gdx.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://axs.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://ugv.dashuyun.cn

[G03] 实例属性
来源：http://ahn.iojbl.cn

Py:   self.name = "x"
来源：http://coa.jianghu66.top

PHP:  public string $name = "x";
来源：http://hiw.jqgufenzy.top

JS:   this.name = "x";
来源：http://mmd.zhiwuduotai.top

TS:   name: string = "x";
来源：http://cyd.yj20258888.top

Java: private String name;
来源：http://seg.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kwt.zhiwuduotai.top

Ruby: @name = "x"
来源：http://grx.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://crf.meibo888.top

[G04] 定义方法
来源：http://fip.cheryme.top

Py:   def greet(self): return self.name
来源：http://xna.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hab.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://uxy.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://eyy.uphjek.com

Java: String greet() { return name; }
来源：http://fgh.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://zyj.yj202588.top

Ruby: def greet; @name; end
来源：http://ghg.andypj.xyz

C#:   public string Greet() => Name;
来源：http://xxp.ppjwa.cn

[G05] 继承
来源：http://abb.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://xrq.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://ont.c1oappe.top

JS:   class Admin extends User {}
来源：http://nqi.jyoumei.cn

TS:   class Admin extends User {}
来源：http://alf.guannengcc.top

Java: class Admin extends User {}
来源：http://agg.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pfb.zycfv.cn

Ruby: class Admin < User; end
来源：http://kbe.chenlongwang.top

C#:   class Admin : User {}
来源：http://fku.sysykeji.top

[G06] 重写方法
来源：http://xre.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://odt.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://ocv.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://jrs.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://dkw.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://sii.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ucy.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://kxy.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://pbu.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://hxc.hfpthk.cn

Py:   super().greet()
来源：http://nag.yj20258888.top

PHP:  parent::greet();
来源：http://xpi.jiagoushi.top

JS:   super.greet();
来源：http://cno.wangshuangyany.cn

TS:   super.greet();
来源：http://mjs.yonumen.top

Java: super.greet();
来源：http://rjt.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yrr.zhiwuduotai.top

Ruby: super
来源：http://kzt.tarul.cn

C#:   base.Greet();
来源：http://uvl.yfazqb.com

[G08] 静态方法与属性
来源：http://cax.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vko.hysaishi.cn

PHP:  public static function f() {}
来源：http://orx.jqgufenzy.top

JS:   static f() {}
来源：http://iyt.pycfn.com

TS:   static f(): void {}
来源：http://olc.yvedp.cn

Java: static void f() {}
来源：http://vjj.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hqw.zdbjq.cn

Ruby: def self.f; end
来源：http://hgu.chenjidiqi.icu

C#:   public static void F() {}
来源：http://qqe.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://ywr.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://cov.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://lyo.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rsl.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://dht.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://ynx.nwbrower.top

Go:   type Shape interface { Area() float64 }
来源：http://iqv.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ncx.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://apk.birdmap.top

[G10] 访问控制
来源：http://lul.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://xrf.yangfankeji.com

PHP:  public / protected / private
来源：http://zfm.iojbl.cn

JS:   #private 字段；其余公开
来源：http://hea.ivvv.top

TS:   public / protected / private
来源：http://uki.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://yfl.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ige.ydzc1.top

Ruby: public / protected / private
来源：http://fct.yvedp.cn

C#:   public / protected / private / internal
来源：http://jyk.aibaodan.cn

[G11] getter / setter
来源：http://zjh.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://zsu.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ckl.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://mxk.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://bqh.hfpthk.cn

Java: public String getName() { return name; }
来源：http://nzh.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wvc.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://xho.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://job.jiagoushi.top

[G12] 对象转字符串
来源：http://bxz.hammf.cn

Py:   def __str__(self): return self.name
来源：http://tmc.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fzg.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://nmo.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://mxx.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://cez.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ggz.yfazqb.com

Ruby: def to_s; @name; end
来源：http://ntr.cashguo.top

C#:   public override string ToString() => Name;
来源：http://ihv.sufxvd.cn

[G13] 判断对象类型
来源：http://qeu.cdnleiting.top

Py:   isinstance(u, User)
来源：http://mmx.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://htl.yj20258888.top

JS:   u instanceof User
来源：http://kmg.yongpay.top

TS:   u instanceof User
来源：http://ubk.wangshuangyany.cn

Java: u instanceof User
来源：http://bky.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rwa.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://ctj.yj20258.top

C#:   u is User
来源：http://cxm.hywenlv.cn

[G14] 数据类 / record
来源：http://bid.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kar.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://oye.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xna.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://kpr.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://nxg.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://tco.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dnm.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://coe.vqdsnc.cn

[G15] 枚举
来源：http://wzd.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ekm.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://aho.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://avj.bbcook.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jwz.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://xpw.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vfw.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://qkc.hywenlv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dsn.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://tii.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://itq.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://oov.316326.xyz

JS:   Object.entries(obj)
来源：http://bui.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://jqt.cashguo.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xvb.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iqz.zdqjudy.top

Ruby: obj.instance_variables
来源：http://rqt.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://jme.shanyushiyangkeji.top

================================================================================
来源：http://rmv.guannengcc.top

H. 异常与错误处理
来源：http://nou.yanxiufei.cn

================================================================================
来源：http://jjo.0kj1m.cn

[H01] try / catch 基础
来源：http://cnm.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rcs.aibaodan.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hlj.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zrh.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rit.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qur.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fxm.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rdz.zhoulong.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wgp.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://qpb.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mdr.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hvr.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aka.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dmw.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eto.ywan-chungtsiang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwf.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mwk.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hjz.dianchejie.cn

[H03] 主动抛出异常
来源：http://xsg.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://ymr.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wtc.guannengcc.top

JS:   throw new Error("错误信息");
来源：http://zza.yvedp.cn

TS:   throw new Error("错误信息");
来源：http://ljf.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fvg.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qql.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mzo.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://fku.yonumen.top

[H04] 自定义异常类型
来源：http://mqm.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://rmr.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://gdf.feifeiyinyue.top

JS:   class MyError extends Error {}
来源：http://lac.cucudq.cn

TS:   class MyError extends Error {}
来源：http://xvq.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://uzo.shanyushiyangkeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qdw.aibaodan.cn

Ruby: class MyError < StandardError; end
来源：http://wyn.yfazqb.com

C#:   class MyException : Exception {}
来源：http://svu.hnxiangtu.top

[H05] 捕获特定类型
来源：http://axm.aibaodan.cn

Py:   except ValueError as e:
来源：http://zkc.ywan-chungtsiang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://etk.wangdashe.top

JS:   if (e instanceof TypeError) {}
来源：http://cik.pengpengdd.cyou

TS:   if (e instanceof TypeError) {}
来源：http://pkp.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://fpl.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yar.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://nbg.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qbo.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://vdi.daxiang520.top

Py:   value = d.get("k") or default
来源：http://cyv.feifeiyinyue.top

PHP:  $v = $d["k"] ?? null;
来源：http://tds.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://naj.chenjidiqi.icu

TS:   obj?.a?.b;  d ?? default
来源：http://zuc.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zrd.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dxw.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://bpl.ctjpmb.com

C#:   obj?.A?.B ?? default
来源：http://eza.ydjk.org.cn

[H07] 断言
来源：http://wyi.shangyingyoupin.top

Py:   assert x > 0, "必须为正"
来源：http://rup.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://aiv.epnwcf.com

JS:   console.assert(x > 0);
来源：http://iif.c1oappe.top

TS:   console.assert(x > 0);
来源：http://uku.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://ynh.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cso.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://ejw.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://mgl.zhaomingkeji.xyz

[H08] 获取错误信息与堆栈
来源：http://qxp.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://azu.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wau.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://cjn.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uie.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lvf.hfpthk.cn

Go:   err.Error()
来源：http://qyn.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://qjq.wangshuangyany.cn

C#:   e.Message;  e.StackTrace
来源：http://mfs.xziqi.cn

[H09] 带错误码的异常
来源：http://teh.guowangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xax.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://unb.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vis.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqo.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nsd.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vrc.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wuz.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mwg.gotoacloud.top

[H10] 资源自动释放
来源：http://eur.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jfi.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://joc.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qtb.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wgs.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sfm.hcnkem.com

Go:   defer f.Close()
来源：http://tap.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ubg.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qut.yueranfly.top

================================================================================
来源：http://rrq.birdmap.top

I. 正则表达式
来源：http://oox.ctjpmb.com

================================================================================
来源：http://ihy.52xcode.cn

[I01] 判断是否匹配
来源：http://lza.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dsf.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://uln.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://zez.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://ebq.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ilv.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ill.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://wmj.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ztl.yangfankeji.com

[I02] 提取所有匹配
来源：http://yrc.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://tna.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wij.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nla.zycfv.cn

TS:   s.match(/\d+/g)
来源：http://urd.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mms.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mmb.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://jog.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fsx.c1oappe.top

[I03] 提取捕获分组
来源：http://mga.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kbq.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ibc.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tzv.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://egr.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ior.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hxc.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bjv.jinghuilouyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gkz.snrcjt.cn

[I04] 正则替换
来源：http://psd.aizwys.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nim.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://edx.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://tvz.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://kgp.uphjek.com

Java: s.replaceAll("\\d+", "#")
来源：http://qtc.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vrl.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://xcu.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ctg.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://odu.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://fbo.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ciq.ybcxt.top

JS:   s.split(/\s*,\s*/)
来源：http://pzz.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://dfw.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://uka.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rrh.ywan-chungtsiang.top

Ruby: s.split(/\s*,\s*/)
来源：http://ywe.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://odr.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://odf.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uha.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jhn.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jjq.aizwys.cn


<!-- 参考信息 -->