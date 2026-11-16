代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tye.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iee.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uxn.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dkq.gaohongyu789.top

================================================================================
来源：http://osa.9152youxi.cn

G. 面向对象
来源：http://dff.nanxuanxn.top

================================================================================
来源：http://hbh.tianlin.xyz

[G01] 定义类
来源：http://xuj.fengsongda.top

Py:   class User: pass
来源：http://fak.yuxming.cn

PHP:  class User {}
来源：http://rdf.hysaishi.cn

JS:   class User {}
来源：http://oce.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://ebb.redwolf501.top

Java: class User {}
来源：http://onj.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://zal.nwbrower.top

Ruby: class User; end
来源：http://zzb.nwbrower.top

C#:   class User {}
来源：http://geg.yj202588.top

[G02] 构造函数
来源：http://cby.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://zfw.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://zht.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://drz.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://rxy.haohaochexian.top

Java: User(String name) { this.name = name; }
来源：http://vtf.zdqjudy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iwg.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ggu.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://qnj.hnqzz.top

[G03] 实例属性
来源：http://qdh.cheryme.top

Py:   self.name = "x"
来源：http://vav.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://ugr.ydzc1.top

JS:   this.name = "x";
来源：http://xhe.ydjk.org.cn

TS:   name: string = "x";
来源：http://hle.bbcook.cn

Java: private String name;
来源：http://wwe.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://czn.quarkkingdee.top

Ruby: @name = "x"
来源：http://dpg.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://pry.daria6918.cn

[G04] 定义方法
来源：http://gnc.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://qag.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://omy.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://pll.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://yix.fehbvm.com

Java: String greet() { return name; }
来源：http://ukf.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hzh.aizwys.cn

Ruby: def greet; @name; end
来源：http://icu.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://qma.snrcjt.cn

[G05] 继承
来源：http://smm.xuanzx.com

Py:   class Admin(User): pass
来源：http://ieq.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://vnb.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://tmp.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://ays.cucudq.cn

Java: class Admin extends User {}
来源：http://kzl.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tbf.sysykeji.top

Ruby: class Admin < User; end
来源：http://zkx.guowangkeji.top

C#:   class Admin : User {}
来源：http://ttl.hnqzz.top

[G06] 重写方法
来源：http://svj.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://yrg.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dau.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://ggr.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://fio.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://xtv.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://szy.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://vsg.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://ryp.pengpengdd.cyou

[G07] 调用父类方法
来源：http://dtu.ctjpmb.com

Py:   super().greet()
来源：http://xpo.ydjk.org.cn

PHP:  parent::greet();
来源：http://aon.fktsv.cn

JS:   super.greet();
来源：http://dxn.zhaomingkeji.xyz

TS:   super.greet();
来源：http://pkj.gzhubu.top

Java: super.greet();
来源：http://ctv.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qch.jinqigfzy.top

Ruby: super
来源：http://kne.jlsjyb.cn

C#:   base.Greet();
来源：http://nia.ppjwa.cn

[G08] 静态方法与属性
来源：http://yut.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cwr.iojbl.cn

PHP:  public static function f() {}
来源：http://nmb.tanke756.top

JS:   static f() {}
来源：http://eoh.smart0.xyz

TS:   static f(): void {}
来源：http://qrg.fengsongda.top

Java: static void f() {}
来源：http://nvo.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zwa.ybcxt.top

Ruby: def self.f; end
来源：http://klh.yangfankeji.com

C#:   public static void F() {}
来源：http://ggc.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://uyp.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://mwz.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://mca.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://poj.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://nwu.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://kwo.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://fgp.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eps.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://smm.fengsongda.top

[G10] 访问控制
来源：http://jny.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://ytx.snrcjt.cn

PHP:  public / protected / private
来源：http://ydn.wangdashe.top

JS:   #private 字段；其余公开
来源：http://jjl.yanxiufei.cn

TS:   public / protected / private
来源：http://fgu.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://qbr.vehdjk.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://oap.yvedp.cn

Ruby: public / protected / private
来源：http://wgj.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://yvm.dianchejie.cn

[G11] getter / setter
来源：http://dha.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://giv.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zxi.xinyue.icu

JS:   get name() { return this._name; }
来源：http://qhp.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://gri.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://nht.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gwz.nanxinkj.top

Ruby: attr_accessor :name
来源：http://lvi.sysykeji.top

C#:   public string Name { get; set; }
来源：http://fwe.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://hwg.yongpay.top

Py:   def __str__(self): return self.name
来源：http://kvp.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bty.birdmap.top

JS:   toString() { return this.name; }
来源：http://mze.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://mjs.sweek.top

Java: @Override public String toString() { return name; }
来源：http://fjr.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://iji.yvedp.cn

Ruby: def to_s; @name; end
来源：http://ixu.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://gte.cucudq.cn

[G13] 判断对象类型
来源：http://ind.zhijiandao.cn

Py:   isinstance(u, User)
来源：http://zcg.jyoumei.cn

PHP:  $u instanceof User
来源：http://qdy.yueranfly.top

JS:   u instanceof User
来源：http://doj.zhoulong.xyz

TS:   u instanceof User
来源：http://xpn.tarul.cn

Java: u instanceof User
来源：http://qqf.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nvz.fktsv.cn

Ruby: u.is_a?(User)
来源：http://unb.sjlbkw.cn

C#:   u is User
来源：http://yco.hcnkem.com

[G14] 数据类 / record
来源：http://njv.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npq.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://vhy.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mgy.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://pik.cashguo.top

Java: record User(String name, int age) {}
来源：http://nuh.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://jdp.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://amr.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://hvf.mhx1999.top

[G15] 枚举
来源：http://ijv.jinqigufen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kxv.jlsjyb.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjq.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ysu.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cpm.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://qxa.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ssr.guannengcc.top

Ruby: Color = %i[red green].freeze
来源：http://aam.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vxy.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://fao.jinqigufen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jjx.meibo888.top

PHP:  get_object_vars($obj);
来源：http://vzk.yonumen.top

JS:   Object.entries(obj)
来源：http://gcd.cashguo.top

TS:   Object.entries(obj)
来源：http://asi.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aeg.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://inl.fengsongda.top

Ruby: obj.instance_variables
来源：http://hkm.daria6918.cn

C#:   // 用反射或 System.Text.Json
来源：http://hkc.fehbvm.com

================================================================================
来源：http://qyu.jqgfzy.top

H. 异常与错误处理
来源：http://qjr.yfazqb.com

================================================================================
来源：http://ghs.nanxuanxn.top

[H01] try / catch 基础
来源：http://vaf.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zjb.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cmp.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rpk.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://utv.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xrp.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gij.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vxf.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://doq.jinqigfzy.top

[H02] finally / ensure 收尾
来源：http://wzq.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://esv.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://ada.bjfxy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://olf.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://jze.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://ddv.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xfx.haohaochexian.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wsf.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wrl.kuanghao11.cn

[H03] 主动抛出异常
来源：http://thh.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://nss.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://otn.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://krc.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://lsr.yvedp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://afr.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://keh.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://euj.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://cvb.zdqjudy.top

[H04] 自定义异常类型
来源：http://uoo.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://vag.shanyushiyangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://dsq.aibaodan.cn

JS:   class MyError extends Error {}
来源：http://zey.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://ygg.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://hbk.hywenlv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kyo.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://kwb.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://nhu.316326.xyz

[H05] 捕获特定类型
来源：http://eru.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://zdy.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oxo.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://epd.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://pud.yuanzhike.top

Java: catch (IOException | SQLException e) {}
来源：http://cfp.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iim.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://kmf.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://clo.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://tav.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://oxb.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ufa.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://rxa.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hdm.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qeg.aibaodan.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ikb.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://ucg.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://hsc.zhixingplan.top

[H07] 断言
来源：http://pjv.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://dlc.cashguo.top

PHP:  assert($x > 0);
来源：http://kxl.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://ofk.gogol.net.cn

TS:   console.assert(x > 0);
来源：http://jaz.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://mky.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://llx.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ouw.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://lgi.xingfuxueyuan.xyz

[H08] 获取错误信息与堆栈
来源：http://tcg.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://dxy.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iyc.hywenlv.cn

JS:   e.message;  e.stack
来源：http://thf.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ivw.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rzh.c1oappe.top

Go:   err.Error()
来源：http://why.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://wyb.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://nmc.zhijiandao.cn

[H09] 带错误码的异常
来源：http://ldm.cqqwz.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rzw.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://bfj.cheryme.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qgk.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nkj.epnwcf.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uwk.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iin.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://aod.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tae.kuanghao11.cn

[H10] 资源自动释放
来源：http://fqt.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gep.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bgg.wangdashe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dlf.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pwo.ehwqpu.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xie.yanxiufei.cn

Go:   defer f.Close()
来源：http://ctb.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zcy.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qxm.aizwys.cn

================================================================================
来源：http://wzl.cucudq.cn

I. 正则表达式
来源：http://wfc.316326.xyz

================================================================================
来源：http://pip.daria6918.cn

[I01] 判断是否匹配
来源：http://iwr.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mkb.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://hbe.cheryme.top

JS:   /\d+/.test(s)
来源：http://mez.nwbrower.top

TS:   /\d+/.test(s)
来源：http://ikq.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://shx.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xss.gzhubu.top

Ruby: s.match?(/\d+/)
来源：http://biv.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kpn.kuanghao11.cn

[I02] 提取所有匹配
来源：http://vlr.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://pmf.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nyf.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwv.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://qpl.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvt.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vhb.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://jjh.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://buk.tian-w.cn

[I03] 提取捕获分组
来源：http://ymk.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nux.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwt.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xsh.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ogj.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fxa.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yyv.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rdu.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lix.yuanzhike.top

[I04] 正则替换
来源：http://oev.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sal.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qtb.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pga.gogol.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gsf.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://csx.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zkb.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://feb.feifeiyinyue.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gzp.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://naz.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jev.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mfi.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://lbw.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://kqb.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://wrm.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pdv.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://vmz.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nng.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yiw.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tii.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tnw.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smj.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rnr.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lyk.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xqm.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tkq.cqqwz.cn


<!-- 参考信息 -->