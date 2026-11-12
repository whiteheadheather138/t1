代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xei.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ftz.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://srm.kuanghao11.cn

TS:   // 同上
来源：http://eiw.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ecu.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wtp.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://drg.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://pvl.zhixingplan.top

================================================================================
来源：http://epv.shanyushiyangtech.top

G. 面向对象
来源：http://ykw.ywan-chungtsiang.top

================================================================================
来源：http://izh.jianghu66.top

[G01] 定义类
来源：http://cch.xinyue.icu

Py:   class User: pass
来源：http://rfv.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://sfa.hywenlv.cn

JS:   class User {}
来源：http://bcx.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://bjk.jinyuanbaomall.cn

Java: class User {}
来源：http://zwx.cashguo.top

Go:   type User struct { Name string }
来源：http://ttb.zhaomingkeji.xyz

Ruby: class User; end
来源：http://vnt.zdqjudy.top

C#:   class User {}
来源：http://nsg.dashuyun.cn

[G02] 构造函数
来源：http://lcp.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://wtz.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://kjf.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://qyt.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://tty.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://vzk.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hdp.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://psr.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://vxm.daria6918.cn

[G03] 实例属性
来源：http://hmw.cheryme.top

Py:   self.name = "x"
来源：http://dmn.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://veq.hesvh.cn

JS:   this.name = "x";
来源：http://uok.daria6918.cn

TS:   name: string = "x";
来源：http://dsz.aibaodan.cn

Java: private String name;
来源：http://hau.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ihp.yj202588.top

Ruby: @name = "x"
来源：http://miu.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://pei.hammf.cn

[G04] 定义方法
来源：http://tie.shuidangran.top

Py:   def greet(self): return self.name
来源：http://nnu.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://enl.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://uwm.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://uqh.hnqzz.top

Java: String greet() { return name; }
来源：http://uvq.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://roq.fzhhl.top

Ruby: def greet; @name; end
来源：http://tem.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://ygg.ivvv.top

[G05] 继承
来源：http://zjk.ctjpmb.com

Py:   class Admin(User): pass
来源：http://tqb.mhx1999.top

PHP:  class Admin extends User {}
来源：http://lrg.wangdashe.top

JS:   class Admin extends User {}
来源：http://ucg.yongpay.top

TS:   class Admin extends User {}
来源：http://obk.yuanzhike.top

Java: class Admin extends User {}
来源：http://hyp.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tix.xinyue.icu

Ruby: class Admin < User; end
来源：http://ttt.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://fuz.52xcode.cn

[G06] 重写方法
来源：http://jhy.chenzaomai.com

Py:   def greet(self): return "admin"
来源：http://izp.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eev.birdmap.top

JS:   greet() { return "admin"; }
来源：http://xms.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://wtd.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://qrt.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kca.ivvv.top

Ruby: def greet; "admin"; end
来源：http://lpj.kuanghao11.cn

C#:   public override string Greet() => "admin";
来源：http://btk.dianchejie.cn

[G07] 调用父类方法
来源：http://sqc.tarul.cn

Py:   super().greet()
来源：http://jcb.tarul.cn

PHP:  parent::greet();
来源：http://cui.pycfn.com

JS:   super.greet();
来源：http://exo.fehbvm.com

TS:   super.greet();
来源：http://upc.iojbl.cn

Java: super.greet();
来源：http://xlg.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jri.zhiwuduotai.top

Ruby: super
来源：http://exk.yfazqb.com

C#:   base.Greet();
来源：http://gfg.fehbvm.com

[G08] 静态方法与属性
来源：http://bei.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xcv.meibo888.top

PHP:  public static function f() {}
来源：http://ckd.c1oappe.top

JS:   static f() {}
来源：http://oqp.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://adc.sufxvd.cn

Java: static void f() {}
来源：http://xse.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dop.gaohongyu789.top

Ruby: def self.f; end
来源：http://cpa.daria6918.cn

C#:   public static void F() {}
来源：http://wbq.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://ray.hywenlv.cn

Py:   from abc import ABC, abstractmethod
来源：http://wvp.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://tdl.zdqjudy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tdl.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://vkb.iojbl.cn

Java: interface Shape { double area(); }
来源：http://isi.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://oqf.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ccq.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://rlg.fengsongda.top

[G10] 访问控制
来源：http://uqg.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://tzk.xylfe.cn

PHP:  public / protected / private
来源：http://dva.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://gln.yj20258888.top

TS:   public / protected / private
来源：http://gco.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://ydc.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://git.havefunace.top

Ruby: public / protected / private
来源：http://oaa.meibo888.top

C#:   public / protected / private / internal
来源：http://vwp.daxiang520.top

[G11] getter / setter
来源：http://gzc.yj20258.top

Py:   @property 与 @x.setter
来源：http://vga.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://asc.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://blf.hesvh.cn

TS:   get name(): string { return this._name; }
来源：http://awh.tanke756.top

Java: public String getName() { return name; }
来源：http://kcs.mhx1999.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gef.bbcook.cn

Ruby: attr_accessor :name
来源：http://olo.havefunace.top

C#:   public string Name { get; set; }
来源：http://kqn.guannengcc.top

[G12] 对象转字符串
来源：http://jbc.9152youxi.cn

Py:   def __str__(self): return self.name
来源：http://ylz.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lxb.birdmap.top

JS:   toString() { return this.name; }
来源：http://boh.hysaishi.cn

TS:   toString(): string { return this.name; }
来源：http://ptd.svipenyu.cn

Java: @Override public String toString() { return name; }
来源：http://gdn.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://pbd.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://tuz.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://hlm.fengsongda.top

[G13] 判断对象类型
来源：http://uuz.ydzc1.top

Py:   isinstance(u, User)
来源：http://kfl.yueranfly.top

PHP:  $u instanceof User
来源：http://glc.gogol.net.cn

JS:   u instanceof User
来源：http://kwi.aibaodan.cn

TS:   u instanceof User
来源：http://rmk.shanyushiyangkeji.top

Java: u instanceof User
来源：http://nuq.vqdsnc.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://oma.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://axi.nanxinkj.top

C#:   u is User
来源：http://ugm.daxiang520.top

[G14] 数据类 / record
来源：http://jax.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://glq.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://nrf.yuxming.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dnp.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://reh.ybcxt.top

Java: record User(String name, int age) {}
来源：http://psb.hammf.cn

Go:   type User struct { Name string; Age int }
来源：http://bbs.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eju.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://wmk.gaohongyu789.top

[G15] 枚举
来源：http://dwu.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://czp.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://aox.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qsk.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lwi.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://sbj.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mis.hfpthk.cn

Ruby: Color = %i[red green].freeze
来源：http://kpl.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dtk.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://kpw.nanxinkj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qfw.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://put.xylfe.cn

JS:   Object.entries(obj)
来源：http://lge.shzxlz.cn

TS:   Object.entries(obj)
来源：http://hca.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ccj.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://enr.jyoumei.cn

Ruby: obj.instance_variables
来源：http://cuf.zhengqikj.top

C#:   // 用反射或 System.Text.Json
来源：http://fcg.jinqigufen.top

================================================================================
来源：http://vby.hysaishi.cn

H. 异常与错误处理
来源：http://xdl.fanxiaobao.xyz

================================================================================
来源：http://swx.zhongyouzk.top

[H01] try / catch 基础
来源：http://kxy.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vrv.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ftc.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jjj.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxr.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://obn.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zvg.pycfn.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cik.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ldj.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://tza.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lvz.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cxg.hywenlv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cdv.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tlf.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://qqp.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://lcy.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hbo.xziqi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gpe.sjlbkw.cn

[H03] 主动抛出异常
来源：http://bdl.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://trd.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ezt.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://efi.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://zmf.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://grs.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gii.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iao.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://jgg.hcnkem.com

[H04] 自定义异常类型
来源：http://rei.tanke756.top

Py:   class MyError(Exception): pass
来源：http://dlg.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://rdn.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://eil.vehdjk.com

TS:   class MyError extends Error {}
来源：http://ien.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://nxd.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nao.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://nda.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://ocn.gogol.net.cn

[H05] 捕获特定类型
来源：http://uww.chenzaomai.com

Py:   except ValueError as e:
来源：http://xwn.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://opt.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://stg.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://dlp.xuanzx.com

Java: catch (IOException | SQLException e) {}
来源：http://htd.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://krw.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://igs.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jlo.dashuyun.cn

[H06] 可选值 / 空值安全访问
来源：http://gsa.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://rwh.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rbb.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://uer.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://qgb.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pop.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fiv.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://plu.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://yvh.zhoulong.xyz

[H07] 断言
来源：http://gko.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://pcp.xinyue.icu

PHP:  assert($x > 0);
来源：http://hou.fehbvm.com

JS:   console.assert(x > 0);
来源：http://klt.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://pkj.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://nyu.daxiang520.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wvo.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://nfc.sufxvd.cn

C#:   Debug.Assert(x > 0);
来源：http://mkn.nanxinkj.top

[H08] 获取错误信息与堆栈
来源：http://fvs.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://mry.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rew.hfpthk.cn

JS:   e.message;  e.stack
来源：http://ujz.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qkc.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://yco.aibaodan.cn

Go:   err.Error()
来源：http://lda.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://qbc.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://bfb.ywan-chungtsiang.top

[H09] 带错误码的异常
来源：http://rdq.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bgw.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rkq.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rhu.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pdk.jyoumei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tsn.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ova.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vax.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rgd.sysykeji.top

[H10] 资源自动释放
来源：http://fri.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dld.hfpthk.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fuf.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dqg.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kyr.bjfxy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cdo.gzhubu.top

Go:   defer f.Close()
来源：http://fva.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://efe.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lih.fanxiaobao.xyz

================================================================================
来源：http://fbt.redwolf501.top

I. 正则表达式
来源：http://lrg.zhongyouzk.top

================================================================================
来源：http://kix.vehdjk.com

[I01] 判断是否匹配
来源：http://rtq.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gvz.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lny.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://dsn.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://spf.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ksc.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pdp.nanxuanxn.top

Ruby: s.match?(/\d+/)
来源：http://dvc.shanyushiyangtech.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pvj.aizwys.cn

[I02] 提取所有匹配
来源：http://edk.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://lni.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yxy.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aah.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://qud.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nyr.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ifz.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://xvi.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zum.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://emn.gzhubu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://alx.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nwe.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qve.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tss.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://trp.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ttn.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zpj.meibo888.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ivd.zhengqikj.top

[I04] 正则替换
来源：http://tbh.yvedp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zmh.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wde.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://vxb.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vil.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://tfm.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sgy.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://szn.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://int.pengpengdd.cyou

[I05] 按正则拆分
来源：http://tli.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://niq.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ial.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://rlr.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://byg.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://jmm.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eae.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://kte.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zoc.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyg.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://esw.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxs.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pfo.nanxuanxn.top


<!-- 参考信息 -->