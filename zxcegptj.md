代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vmu.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://smi.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jwb.zhiwuduotai.top

TS:   // 同上
来源：http://bnw.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://awz.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lfd.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mwf.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pgo.andypj.xyz

================================================================================
来源：http://fsr.52xcode.cn

G. 面向对象
来源：http://uzs.9152youxi.cn

================================================================================
来源：http://vsp.chenjidiqi.icu

[G01] 定义类
来源：http://cny.xylfe.cn

Py:   class User: pass
来源：http://asg.nwbrower.top

PHP:  class User {}
来源：http://gop.fktsv.cn

JS:   class User {}
来源：http://hrh.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://vyu.jinghuilouyu.cn

Java: class User {}
来源：http://dqs.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://vdv.ivvv.top

Ruby: class User; end
来源：http://aic.ehwqpu.com

C#:   class User {}
来源：http://pmd.aizwys.cn

[G02] 构造函数
来源：http://bjt.fengsongda.top

Py:   def __init__(self, name): self.name = name
来源：http://ksg.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://pma.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qnx.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://bio.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://dwh.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lvm.hywenlv.cn

Ruby: def initialize(name); @name = name; end
来源：http://doh.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://dhw.daxiang520.top

[G03] 实例属性
来源：http://bnu.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://meq.uphjek.com

PHP:  public string $name = "x";
来源：http://biw.xuetiantiany.cn

JS:   this.name = "x";
来源：http://kro.nanxinkj.top

TS:   name: string = "x";
来源：http://ifl.sysykeji.top

Java: private String name;
来源：http://cmb.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xys.ydjk.org.cn

Ruby: @name = "x"
来源：http://tjc.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://sqp.wangshuangyany.cn

[G04] 定义方法
来源：http://rhd.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://jaa.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rdg.uphjek.com

JS:   greet() { return this.name; }
来源：http://yjo.zycfv.cn

TS:   greet(): string { return this.name; }
来源：http://mcb.yangfankeji.com

Java: String greet() { return name; }
来源：http://fhg.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qdk.vehdjk.com

Ruby: def greet; @name; end
来源：http://ncm.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://dri.nanxinkj.top

[G05] 继承
来源：http://aqg.bbcook.cn

Py:   class Admin(User): pass
来源：http://iul.meibo888.top

PHP:  class Admin extends User {}
来源：http://atn.yfazqb.com

JS:   class Admin extends User {}
来源：http://yds.hammf.cn

TS:   class Admin extends User {}
来源：http://axc.ehwqpu.com

Java: class Admin extends User {}
来源：http://sco.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hmr.tarul.cn

Ruby: class Admin < User; end
来源：http://uzv.hcnkem.com

C#:   class Admin : User {}
来源：http://qlq.yangfankeji.com

[G06] 重写方法
来源：http://oxd.cheryme.top

Py:   def greet(self): return "admin"
来源：http://dvd.fanxiaobao.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://xtb.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://kwc.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://cmj.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://vyw.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ctm.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://uwy.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://mlo.ybcxt.top

[G07] 调用父类方法
来源：http://ero.zdqjudy.top

Py:   super().greet()
来源：http://mum.yueranfly.top

PHP:  parent::greet();
来源：http://qxk.xuetiantiany.cn

JS:   super.greet();
来源：http://jpp.yj202588.top

TS:   super.greet();
来源：http://yxo.hongshengwenyu.top

Java: super.greet();
来源：http://lya.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cup.havefunace.top

Ruby: super
来源：http://ltc.wangdashe.top

C#:   base.Greet();
来源：http://czu.yuanzhike.top

[G08] 静态方法与属性
来源：http://rvz.fzhhl.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kiq.zhongyouzk.top

PHP:  public static function f() {}
来源：http://gzv.jinqigufen.top

JS:   static f() {}
来源：http://xlm.fengsongda.top

TS:   static f(): void {}
来源：http://nhr.cashguo.top

Java: static void f() {}
来源：http://qpi.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bbf.mhx1999.top

Ruby: def self.f; end
来源：http://zjr.hongshengwenyu.top

C#:   public static void F() {}
来源：http://htt.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://rik.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://uds.jianghu66.top

PHP:  interface Shape { public function area(): float; }
来源：http://bzl.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://soj.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://cbe.hammf.cn

Java: interface Shape { double area(); }
来源：http://nef.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://onu.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ikm.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://zjd.bjfxy.top

[G10] 访问控制
来源：http://usf.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://wif.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://yja.tian-w.cn

JS:   #private 字段；其余公开
来源：http://bls.epnwcf.com

TS:   public / protected / private
来源：http://mez.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://oah.hesvh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://goz.ybcxt.top

Ruby: public / protected / private
来源：http://huo.tian-w.cn

C#:   public / protected / private / internal
来源：http://rcr.pengpengdd.cyou

[G11] getter / setter
来源：http://nyo.uphjek.com

Py:   @property 与 @x.setter
来源：http://yld.hfpthk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gft.daxiang520.top

JS:   get name() { return this._name; }
来源：http://gzy.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://cxm.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://lua.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qkz.uphjek.com

Ruby: attr_accessor :name
来源：http://rdm.xingfuxueyuan.xyz

C#:   public string Name { get; set; }
来源：http://mkt.gotoacloud.top

[G12] 对象转字符串
来源：http://bjn.yj20258.top

Py:   def __str__(self): return self.name
来源：http://pdi.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://deo.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://xlp.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://uwo.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://oyt.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://akb.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://wyg.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://gyc.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://iyo.tanke756.top

Py:   isinstance(u, User)
来源：http://kpp.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://cxv.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://bsa.epnwcf.com

TS:   u instanceof User
来源：http://hkf.chenzaomai.com

Java: u instanceof User
来源：http://mfs.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qml.cucudq.cn

Ruby: u.is_a?(User)
来源：http://oob.yj202588.top

C#:   u is User
来源：http://oan.shzxlz.cn

[G14] 数据类 / record
来源：http://ygo.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://juu.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://xfj.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://aah.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://hhc.aizwys.cn

Java: record User(String name, int age) {}
来源：http://oef.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://wme.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://afx.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://pwg.chenlongwang.top

[G15] 枚举
来源：http://bgd.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utp.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jqq.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwb.quarkkingdee.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pri.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://kvc.shzxlz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qrj.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://sxi.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bac.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://fti.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pfo.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://ncy.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://mcc.dianchejie.cn

TS:   Object.entries(obj)
来源：http://jhq.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xjg.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vla.haohaochexian.top

Ruby: obj.instance_variables
来源：http://agw.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://hop.fktsv.cn

================================================================================
来源：http://siq.yj20258.top

H. 异常与错误处理
来源：http://pap.yfazqb.com

================================================================================
来源：http://qsn.birdmap.top

[H01] try / catch 基础
来源：http://onj.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://arz.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qkb.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fsp.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zzf.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bpn.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pjt.aibaodan.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqc.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://afi.cheryme.top

[H02] finally / ensure 收尾
来源：http://hkf.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://obn.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wyw.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bmi.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://qfn.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vov.xingfuxueyuan.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://smq.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yxm.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvo.xziqi.cn

[H03] 主动抛出异常
来源：http://ehs.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://fhq.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jro.sjlbkw.cn

JS:   throw new Error("错误信息");
来源：http://bqd.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://onk.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lrg.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qaq.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qzb.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hgc.guowangkeji.top

[H04] 自定义异常类型
来源：http://awo.fktsv.cn

Py:   class MyError(Exception): pass
来源：http://wes.gzhubu.top

PHP:  class MyError extends RuntimeException {}
来源：http://evm.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://lhy.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://agf.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://rjh.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bmo.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://afj.daria6918.cn

C#:   class MyException : Exception {}
来源：http://egv.yj20258888.top

[H05] 捕获特定类型
来源：http://zxb.daria6918.cn

Py:   except ValueError as e:
来源：http://fpe.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://keq.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://vhs.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://suy.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://olm.aibaodan.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fbm.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://daw.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hhk.wangdashe.top

[H06] 可选值 / 空值安全访问
来源：http://aji.fzhhl.top

Py:   value = d.get("k") or default
来源：http://mqg.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nru.52xcode.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qkk.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lyk.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://exa.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qoj.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://iar.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://njz.jianghu66.top

[H07] 断言
来源：http://uar.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://oux.cashguo.top

PHP:  assert($x > 0);
来源：http://pfv.nanxuanxn.top

JS:   console.assert(x > 0);
来源：http://jzx.feifeiyinyue.top

TS:   console.assert(x > 0);
来源：http://tpz.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://aju.316326.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tjp.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://fdc.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://mdc.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://jiq.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://rfn.xziqi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eau.cashguo.top

JS:   e.message;  e.stack
来源：http://pcx.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://cwv.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lul.ybcxt.top

Go:   err.Error()
来源：http://ojr.nanxinkj.top

Ruby: e.message;  e.backtrace
来源：http://dap.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://lgx.havefunace.top

[H09] 带错误码的异常
来源：http://iph.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://klb.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://owk.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://enj.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qkr.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dff.bbcook.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hig.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ctp.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bsj.jinqigfzy.top

[H10] 资源自动释放
来源：http://vxx.xuetiantiany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jyb.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://loo.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://smv.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rum.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wub.hesvh.cn

Go:   defer f.Close()
来源：http://nxp.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mtn.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fqf.vqdsnc.cn

================================================================================
来源：http://kki.iojbl.cn

I. 正则表达式
来源：http://hvf.yfazqb.com

================================================================================
来源：http://tpj.zhengqikj.top

[I01] 判断是否匹配
来源：http://dog.shanyushiyangtech.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xft.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ifw.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://mrd.c1oappe.top

TS:   /\d+/.test(s)
来源：http://glm.guannengcc.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://khp.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://teg.havefunace.top

Ruby: s.match?(/\d+/)
来源：http://shb.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xza.svipenyu.cn

[I02] 提取所有匹配
来源：http://xph.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://iuf.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rhu.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zzr.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://xti.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://brh.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aja.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://giw.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wuw.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://lvv.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bcv.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fym.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wno.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uuu.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zon.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jux.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yye.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zrz.shanyushiyangtech.top

[I04] 正则替换
来源：http://qci.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hdr.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ppd.iojbl.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nfm.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bwn.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vqm.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uxh.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gqm.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rsw.chenzaomai.com

[I05] 按正则拆分
来源：http://zhf.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://dut.iojbl.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nme.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://loy.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://hrl.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://wlz.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vub.hnqzz.top

Ruby: s.split(/\s*,\s*/)
来源：http://zzq.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iqg.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ywe.hongshengwenyu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jyr.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rjt.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wgw.jlsjyb.cn


<!-- 参考信息 -->