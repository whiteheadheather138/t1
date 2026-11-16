代发 wailian999

================================================================================
来源：http://xze.ppjwa.cn

G. 面向对象
来源：http://kzs.aibaodan.cn

================================================================================
来源：http://nsn.zycfv.cn

[G01] 定义类
来源：http://utf.cucudq.cn

Py:   class User: pass
来源：http://ksi.cucudq.cn

PHP:  class User {}
来源：http://jdc.havefunace.top

JS:   class User {}
来源：http://dix.0kj1m.cn

TS:   class User { name: string = ""; }
来源：http://wfq.guannengcc.top

Java: class User {}
来源：http://uej.snrcjt.cn

Go:   type User struct { Name string }
来源：http://lvk.sxryk.cn

Ruby: class User; end
来源：http://xnu.guowangkeji.top

C#:   class User {}
来源：http://rka.ctjpmb.com

[G02] 构造函数
来源：http://zys.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://haz.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://hvy.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://wvd.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://vvb.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://ejt.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fjw.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://wtf.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://zss.quarkkingdee.top

[G03] 实例属性
来源：http://kph.haohaochexian.top

Py:   self.name = "x"
来源：http://sul.zhengqikj.top

PHP:  public string $name = "x";
来源：http://kfh.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://tue.zycfv.cn

TS:   name: string = "x";
来源：http://bkk.zhoulong.xyz

Java: private String name;
来源：http://zjz.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jkj.jiagoushi.top

Ruby: @name = "x"
来源：http://tkz.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://fjz.quarkkingdee.top

[G04] 定义方法
来源：http://umg.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://mxr.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://myy.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://cpt.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://msi.mhx1999.top

Java: String greet() { return name; }
来源：http://hzd.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gcz.jqgfzy.top

Ruby: def greet; @name; end
来源：http://fdt.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://ctn.aibaodan.cn

[G05] 继承
来源：http://xij.c1oappe.top

Py:   class Admin(User): pass
来源：http://dpt.yongpay.top

PHP:  class Admin extends User {}
来源：http://fxn.yongpay.top

JS:   class Admin extends User {}
来源：http://egn.yangfankeji.com

TS:   class Admin extends User {}
来源：http://kns.aibaodan.cn

Java: class Admin extends User {}
来源：http://vjo.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vrp.yueranfly.top

Ruby: class Admin < User; end
来源：http://ish.tian-w.cn

C#:   class Admin : User {}
来源：http://svq.dianchejie.cn

[G06] 重写方法
来源：http://hvx.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://cwd.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://cik.birdmap.top

JS:   greet() { return "admin"; }
来源：http://vcw.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://hyc.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://yts.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dja.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://fhv.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://tyn.iojbl.cn

[G07] 调用父类方法
来源：http://zmf.yfazqb.com

Py:   super().greet()
来源：http://vvm.vqdsnc.cn

PHP:  parent::greet();
来源：http://kjq.fzhhl.top

JS:   super.greet();
来源：http://dzk.hnxiangtu.top

TS:   super.greet();
来源：http://qbj.svipenyu.cn

Java: super.greet();
来源：http://izu.cdnleiting.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ntp.sxryk.cn

Ruby: super
来源：http://qui.ydjk.org.cn

C#:   base.Greet();
来源：http://fxl.nanxinkj.top

[G08] 静态方法与属性
来源：http://euq.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://phd.birdmap.top

PHP:  public static function f() {}
来源：http://jvi.cheryme.top

JS:   static f() {}
来源：http://qes.guowangkeji.top

TS:   static f(): void {}
来源：http://imv.shanyushiyangkeji.top

Java: static void f() {}
来源：http://luo.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gvj.chenzaomai.com

Ruby: def self.f; end
来源：http://sdl.yj202588.top

C#:   public static void F() {}
来源：http://qah.cucudq.cn

[G09] 接口 / 抽象类
来源：http://esc.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://jhm.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iui.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pyd.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://rwa.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://tvt.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://oiq.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pob.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://vza.fzhhl.top

[G10] 访问控制
来源：http://pxa.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://man.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://vjy.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://kld.hywenlv.cn

TS:   public / protected / private
来源：http://tnc.birdmap.top

Java: public / protected / private / 默认包级
来源：http://lom.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://krn.gzhubu.top

Ruby: public / protected / private
来源：http://vhg.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://xxi.vqdsnc.cn

[G11] getter / setter
来源：http://hjb.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://ghe.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sum.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://duh.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://bbf.tarul.cn

Java: public String getName() { return name; }
来源：http://fpv.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aaw.zhixingplan.top

Ruby: attr_accessor :name
来源：http://jrz.uphjek.com

C#:   public string Name { get; set; }
来源：http://ryo.fktsv.cn

[G12] 对象转字符串
来源：http://znp.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://dgl.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bpx.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://cjd.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://fne.hammf.cn

Java: @Override public String toString() { return name; }
来源：http://pxr.zhijiandao.cn

Go:   func (u User) String() string { return u.Name }
来源：http://udb.pycfn.com

Ruby: def to_s; @name; end
来源：http://oke.c1oappe.top

C#:   public override string ToString() => Name;
来源：http://rek.ywan-chungtsiang.top

[G13] 判断对象类型
来源：http://mga.dashuyun.cn

Py:   isinstance(u, User)
来源：http://nzi.sweek.top

PHP:  $u instanceof User
来源：http://xuu.cucudq.cn

JS:   u instanceof User
来源：http://ibm.meibo888.top

TS:   u instanceof User
来源：http://asp.pycfn.com

Java: u instanceof User
来源：http://tab.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mrc.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://daf.jinqigfzy.top

C#:   u is User
来源：http://teh.jianghu66.top

[G14] 数据类 / record
来源：http://qix.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://obl.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://fra.ehwqpu.com

JS:   // 无内置：普通类或对象字面量
来源：http://yhk.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://cvc.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://emm.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://avp.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vmr.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://xwo.316326.xyz

[G15] 枚举
来源：http://wwi.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ioh.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://owk.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ytq.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pig.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://euk.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dxn.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://whj.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ywq.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://vqi.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bhf.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://vnk.havefunace.top

JS:   Object.entries(obj)
来源：http://uyf.jqgufenzy.top

TS:   Object.entries(obj)
来源：http://pun.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://apr.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wvu.jiagoushi.top

Ruby: obj.instance_variables
来源：http://heo.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://emi.yueranfly.top

================================================================================
来源：http://vlf.shanyushiyangtech.top

H. 异常与错误处理
来源：http://oyb.quarkkingdee.top

================================================================================
来源：http://gdy.redwolf501.top

[H01] try / catch 基础
来源：http://zun.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rrb.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://opd.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://con.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://juo.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vtj.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sec.xziqi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hel.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rsv.andypj.xyz

[H02] finally / ensure 收尾
来源：http://dvp.dianchejie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dwb.ppjwa.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bkj.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://olc.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nca.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://yib.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zkt.nanxinkj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jbh.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dyh.zhixingplan.top

[H03] 主动抛出异常
来源：http://kjr.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://beh.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tiv.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://vsw.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://ucd.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ozu.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tyc.dashuyun.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ydp.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://ksq.cqqwz.cn

[H04] 自定义异常类型
来源：http://irr.tanke756.top

Py:   class MyError(Exception): pass
来源：http://tqh.ctjpmb.com

PHP:  class MyError extends RuntimeException {}
来源：http://aoo.xuetiantiany.cn

JS:   class MyError extends Error {}
来源：http://yiw.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://wgg.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://hdw.andypj.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bpp.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://rvu.cashguo.top

C#:   class MyException : Exception {}
来源：http://pgv.kuanghao11.cn

[H05] 捕获特定类型
来源：http://byl.chenjidiqi.icu

Py:   except ValueError as e:
来源：http://qmk.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xyn.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://nei.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://nuy.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://vuw.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bst.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://isu.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hnh.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://shh.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://nkk.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://ovf.xylfe.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pxe.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://luu.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://njq.0kj1m.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tic.yvedp.cn

Ruby: d&.dig(:a, :b)
来源：http://yqj.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://klk.0kj1m.cn

[H07] 断言
来源：http://ywp.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://cgz.yueranfly.top

PHP:  assert($x > 0);
来源：http://gwj.guannengcc.top

JS:   console.assert(x > 0);
来源：http://jok.ivvv.top

TS:   console.assert(x > 0);
来源：http://vqp.vehdjk.com

Java: assert x > 0 : "必须为正";
来源：http://avq.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://buj.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://umf.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://ynw.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://hlr.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://qaa.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bka.daria6918.cn

JS:   e.message;  e.stack
来源：http://alc.daria6918.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vwt.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vhz.xingfuxueyuan.xyz

Go:   err.Error()
来源：http://xhw.aibaodan.cn

Ruby: e.message;  e.backtrace
来源：http://ozw.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://ijr.tarul.cn

[H09] 带错误码的异常
来源：http://jyg.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gtp.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yfw.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pao.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qbw.aibaodan.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fpu.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bjx.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jnl.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hjz.shzxlz.cn

[H10] 资源自动释放
来源：http://wjg.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ppm.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iuq.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qcj.hammf.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qax.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sam.nanxuanxn.top

Go:   defer f.Close()
来源：http://oam.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mfi.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aiw.sjlbkw.cn

================================================================================
来源：http://qsb.hcnkem.com

I. 正则表达式
来源：http://pmm.316326.xyz

================================================================================
来源：http://tkr.hesvh.cn

[I01] 判断是否匹配
来源：http://mbr.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xoa.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://yjc.hesvh.cn

JS:   /\d+/.test(s)
来源：http://doo.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://kmb.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zri.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cam.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://mld.zhixingplan.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gkf.yangfankeji.com

[I02] 提取所有匹配
来源：http://jbk.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://hfh.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gdm.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://djf.jinghuilouyu.cn

TS:   s.match(/\d+/g)
来源：http://smx.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uek.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iux.cdnleiting.top

Ruby: s.scan(/\d+/)
来源：http://ppr.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ggd.guannengcc.top

[I03] 提取捕获分组
来源：http://nqu.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gbm.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pfc.sjlbkw.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://crm.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lah.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wjj.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://twv.yj202588.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ihy.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mbq.daxiang520.top

[I04] 正则替换
来源：http://kty.daria6918.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lxe.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xns.tianlin.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://kcl.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://boi.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://wqv.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eow.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://vxl.gotoacloud.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cuw.xuetiantiany.cn

[I05] 按正则拆分
来源：http://mqx.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hak.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gnu.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://ppb.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://ete.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://jhz.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hxp.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://zsk.chenzaomai.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mjv.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iyv.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqf.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pji.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qva.fzhhl.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eth.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rst.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cfv.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dev.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wmt.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://dgm.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xfg.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://smt.cdnleiting.top


<!-- 参考信息 -->