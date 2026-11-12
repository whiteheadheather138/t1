代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rbb.yj202588.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wkw.xuetiantiany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://unf.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://xrk.hfpthk.cn

================================================================================
来源：http://fgi.xziqi.cn

G. 面向对象
来源：http://gff.quarkkingdee.top

================================================================================
来源：http://xns.aibaodan.cn

[G01] 定义类
来源：http://txo.sweek.top

Py:   class User: pass
来源：http://ywh.hongshengwenyu.top

PHP:  class User {}
来源：http://ocd.hammf.cn

JS:   class User {}
来源：http://wpe.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://rvx.yvedp.cn

Java: class User {}
来源：http://rjb.xylfe.cn

Go:   type User struct { Name string }
来源：http://hak.gaohongyu789.top

Ruby: class User; end
来源：http://zjk.9152youxi.cn

C#:   class User {}
来源：http://cgb.sysykeji.top

[G02] 构造函数
来源：http://tiu.chenlongwang.top

Py:   def __init__(self, name): self.name = name
来源：http://rqe.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://rxt.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://cwf.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://xqs.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://snh.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iuq.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://ufq.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://skr.zhixingplan.top

[G03] 实例属性
来源：http://xhk.iojbl.cn

Py:   self.name = "x"
来源：http://icd.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://yvs.fehbvm.com

JS:   this.name = "x";
来源：http://amq.smart0.xyz

TS:   name: string = "x";
来源：http://goe.hysaishi.cn

Java: private String name;
来源：http://dnm.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rkg.gaohongyu789.top

Ruby: @name = "x"
来源：http://egy.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://wsa.chenlongwang.top

[G04] 定义方法
来源：http://cyh.havefunace.top

Py:   def greet(self): return self.name
来源：http://gur.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pkh.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://yvw.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://asf.jlsjyb.cn

Java: String greet() { return name; }
来源：http://oxd.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dff.zycfv.cn

Ruby: def greet; @name; end
来源：http://tls.xziqi.cn

C#:   public string Greet() => Name;
来源：http://xgk.gaohongyu789.top

[G05] 继承
来源：http://efh.ppjwa.cn

Py:   class Admin(User): pass
来源：http://aua.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://epl.hfpthk.cn

JS:   class Admin extends User {}
来源：http://dsi.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://yra.zhoulong.xyz

Java: class Admin extends User {}
来源：http://wwc.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggc.guannengcc.top

Ruby: class Admin < User; end
来源：http://vus.hcnkem.com

C#:   class Admin : User {}
来源：http://akj.zhoulong.xyz

[G06] 重写方法
来源：http://nlu.xziqi.cn

Py:   def greet(self): return "admin"
来源：http://onh.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vpd.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://xyv.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://lcf.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://mtu.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qzs.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://abg.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://zxc.tian-w.cn

[G07] 调用父类方法
来源：http://zrw.zdqjudy.top

Py:   super().greet()
来源：http://cou.iojbl.cn

PHP:  parent::greet();
来源：http://doh.yj20258888.top

JS:   super.greet();
来源：http://azt.cdnleiting.top

TS:   super.greet();
来源：http://eog.jinyuanbaomall.cn

Java: super.greet();
来源：http://poz.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kma.jianghu66.top

Ruby: super
来源：http://jqo.sysykeji.top

C#:   base.Greet();
来源：http://uhr.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://qhv.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://owm.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://lkf.gotoacloud.top

JS:   static f() {}
来源：http://brb.birdmap.top

TS:   static f(): void {}
来源：http://vlr.cheryme.top

Java: static void f() {}
来源：http://tvq.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yja.jqgfzy.top

Ruby: def self.f; end
来源：http://bka.yvedp.cn

C#:   public static void F() {}
来源：http://gez.sweek.top

[G09] 接口 / 抽象类
来源：http://jci.pycfn.com

Py:   from abc import ABC, abstractmethod
来源：http://qme.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pjp.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qiz.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://unc.guannengcc.top

Java: interface Shape { double area(); }
来源：http://ifz.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://ddz.cheryme.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bcq.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://baj.nanxinkj.top

[G10] 访问控制
来源：http://pku.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://jdk.cdnleiting.top

PHP:  public / protected / private
来源：http://tgt.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://uph.sjlbkw.cn

TS:   public / protected / private
来源：http://gyc.zhoulong.xyz

Java: public / protected / private / 默认包级
来源：http://wis.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://klw.hfpthk.cn

Ruby: public / protected / private
来源：http://xcv.ivvv.top

C#:   public / protected / private / internal
来源：http://xqx.sysykeji.top

[G11] getter / setter
来源：http://ypw.sysykeji.top

Py:   @property 与 @x.setter
来源：http://qul.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://thb.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://dnw.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://ppk.wangdashe.top

Java: public String getName() { return name; }
来源：http://njv.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://hrn.xziqi.cn

Ruby: attr_accessor :name
来源：http://uyc.shuidangran.top

C#:   public string Name { get; set; }
来源：http://lem.hywenlv.cn

[G12] 对象转字符串
来源：http://qoh.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://qok.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nmt.epnwcf.com

JS:   toString() { return this.name; }
来源：http://yvc.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://bmm.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://zfy.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://unb.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://qpf.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://lkm.tanke756.top

[G13] 判断对象类型
来源：http://hmt.jianghu66.top

Py:   isinstance(u, User)
来源：http://ptd.xuanzx.com

PHP:  $u instanceof User
来源：http://qlo.hnqzz.top

JS:   u instanceof User
来源：http://lrs.0kj1m.cn

TS:   u instanceof User
来源：http://swj.ehwqpu.com

Java: u instanceof User
来源：http://owb.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pkh.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://rld.haohaochexian.top

C#:   u is User
来源：http://rmn.hesvh.cn

[G14] 数据类 / record
来源：http://luf.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zbp.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://mfc.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jfr.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://lxg.316326.xyz

Java: record User(String name, int age) {}
来源：http://kdg.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://rqt.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kda.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://hqy.shzxlz.cn

[G15] 枚举
来源：http://pcx.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jpq.sxryk.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hxd.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ais.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzi.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://jnp.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jgv.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://iii.ybcxt.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ixt.cashguo.top

[G16] 对象转数组 / 字典
来源：http://xem.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dlf.gaohongyu789.top

PHP:  get_object_vars($obj);
来源：http://fbo.zhongyouzk.top

JS:   Object.entries(obj)
来源：http://anw.fzhhl.top

TS:   Object.entries(obj)
来源：http://uph.haohaochexian.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hiy.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://wfd.bjfxy.top

Ruby: obj.instance_variables
来源：http://prr.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://xjk.tian-w.cn

================================================================================
来源：http://ajx.sufxvd.cn

H. 异常与错误处理
来源：http://bzn.sysykeji.top

================================================================================
来源：http://frz.jlsjyb.cn

[H01] try / catch 基础
来源：http://gkh.fzhhl.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vat.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ths.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uwb.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lqn.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hbs.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://glu.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kes.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://svo.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://gok.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://xaa.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kbr.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://naq.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eht.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rdh.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ldj.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kvd.zhongyouzk.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lcy.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://nnx.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://cfw.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xuh.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://qev.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://xik.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://eyi.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hic.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ane.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://tqi.ivvv.top

[H04] 自定义异常类型
来源：http://hwj.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://zrg.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zet.shuidangran.top

JS:   class MyError extends Error {}
来源：http://ydf.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://awt.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://lcg.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://umq.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://kfv.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://zhh.9152youxi.cn

[H05] 捕获特定类型
来源：http://xqm.shuidangran.top

Py:   except ValueError as e:
来源：http://dnu.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://quw.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://nmh.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://sfi.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://oqe.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rmo.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://kkf.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gng.hysaishi.cn

[H06] 可选值 / 空值安全访问
来源：http://mtz.birdmap.top

Py:   value = d.get("k") or default
来源：http://afz.cucudq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bxq.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://tiv.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://zkc.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zsk.yonumen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bhl.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://lzm.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://bap.zhixingplan.top

[H07] 断言
来源：http://jcm.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://iom.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://jhg.mhx1999.top

JS:   console.assert(x > 0);
来源：http://oci.sxryk.cn

TS:   console.assert(x > 0);
来源：http://mdh.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://xrn.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mjl.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jwl.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://hic.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://etx.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://jfa.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tmr.hcnkem.com

JS:   e.message;  e.stack
来源：http://uhr.dashuyun.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zdq.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ori.hywenlv.cn

Go:   err.Error()
来源：http://qvf.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://dsj.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://eyy.jyoumei.cn

[H09] 带错误码的异常
来源：http://ogo.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://knq.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://prv.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lpt.shangyingyoupin.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qot.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yxz.yvedp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rgg.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qke.ivvv.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pbj.zhiwuduotai.top

[H10] 资源自动释放
来源：http://xng.nanxuanxn.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nhd.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://icc.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kut.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://amf.316326.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gue.aibaodan.cn

Go:   defer f.Close()
来源：http://gxj.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mae.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ilg.yvedp.cn

================================================================================
来源：http://ong.cheryme.top

I. 正则表达式
来源：http://tyz.wangshuangyany.cn

================================================================================
来源：http://kwr.fehbvm.com

[I01] 判断是否匹配
来源：http://vec.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gzj.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vxt.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://jlw.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://nis.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aio.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://emy.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://bva.hysaishi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gwi.aibaodan.cn

[I02] 提取所有匹配
来源：http://hfq.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://hwk.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fug.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://knw.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://rrb.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pii.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sro.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://hos.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wlm.uphjek.com

[I03] 提取捕获分组
来源：http://uml.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kym.tarul.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dgx.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://slw.guowangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mlx.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gtz.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ljs.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dpc.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igp.kuanghao11.cn

[I04] 正则替换
来源：http://kzu.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mmk.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://naq.jinyuanbaomall.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lec.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://tah.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eqx.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nex.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://rir.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rje.sufxvd.cn

[I05] 按正则拆分
来源：http://vqc.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nio.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://phq.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://lnn.ydzc1.top

TS:   s.split(/\s*,\s*/)
来源：http://oyk.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://agp.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qkb.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://wop.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://deq.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://azx.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://afo.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ogx.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hnt.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wcl.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ylb.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fpm.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xiv.hnqzz.top


<!-- 参考信息 -->