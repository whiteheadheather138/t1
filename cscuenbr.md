代发 wailian999

Py:   class User: pass
来源：http://ebr.daxiang520.top

PHP:  class User {}
来源：http://zuo.jlsjyb.cn

JS:   class User {}
来源：http://dko.yj202588.top

TS:   class User { name: string = ""; }
来源：http://kzc.yvedp.cn

Java: class User {}
来源：http://zrj.hysaishi.cn

Go:   type User struct { Name string }
来源：http://nel.hongshengwenyu.top

Ruby: class User; end
来源：http://ryg.dianchejie.cn

C#:   class User {}
来源：http://wht.shzxlz.cn

[G02] 构造函数
来源：http://wgm.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://ovi.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://kkq.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://kse.zhiwuduotai.top

TS:   constructor(public name: string) {}
来源：http://trw.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://fbc.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gun.zhoulong.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ghq.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://zdc.meibo888.top

[G03] 实例属性
来源：http://ywi.gaohongyu789.top

Py:   self.name = "x"
来源：http://moy.hysaishi.cn

PHP:  public string $name = "x";
来源：http://qcb.svipenyu.cn

JS:   this.name = "x";
来源：http://ivp.dianchejie.cn

TS:   name: string = "x";
来源：http://lxp.ehwqpu.com

Java: private String name;
来源：http://aln.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jcz.sjlbkw.cn

Ruby: @name = "x"
来源：http://uif.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://hsy.fzhhl.top

[G04] 定义方法
来源：http://swc.yongpay.top

Py:   def greet(self): return self.name
来源：http://xgj.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lzl.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://gby.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://ccw.ydzc1.top

Java: String greet() { return name; }
来源：http://vbe.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://caq.guannengcc.top

Ruby: def greet; @name; end
来源：http://lab.hysaishi.cn

C#:   public string Greet() => Name;
来源：http://ayr.nwbrower.top

[G05] 继承
来源：http://cbs.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://jcf.uphjek.com

PHP:  class Admin extends User {}
来源：http://kqb.ybcxt.top

JS:   class Admin extends User {}
来源：http://rso.ybcxt.top

TS:   class Admin extends User {}
来源：http://yit.chenlongwang.top

Java: class Admin extends User {}
来源：http://bxj.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vjd.ctjpmb.com

Ruby: class Admin < User; end
来源：http://txj.fengsongda.top

C#:   class Admin : User {}
来源：http://asc.yj202588.top

[G06] 重写方法
来源：http://xwd.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://fus.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ebe.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://syb.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://bey.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://dck.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://drd.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://ibm.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://tmy.ydjk.org.cn

[G07] 调用父类方法
来源：http://ixb.jlsjyb.cn

Py:   super().greet()
来源：http://wya.wangdashe.top

PHP:  parent::greet();
来源：http://xwi.zhixingplan.top

JS:   super.greet();
来源：http://duy.jqgufenzy.top

TS:   super.greet();
来源：http://lxs.ydjk.org.cn

Java: super.greet();
来源：http://ush.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ute.nanxuanxn.top

Ruby: super
来源：http://gee.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://nrp.uphjek.com

[G08] 静态方法与属性
来源：http://rzo.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tny.hammf.cn

PHP:  public static function f() {}
来源：http://ace.gaohongyu789.top

JS:   static f() {}
来源：http://itq.cdnleiting.top

TS:   static f(): void {}
来源：http://fsw.tarul.cn

Java: static void f() {}
来源：http://cab.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://cws.andypj.xyz

Ruby: def self.f; end
来源：http://npo.yj202588.top

C#:   public static void F() {}
来源：http://uhk.birdmap.top

[G09] 接口 / 抽象类
来源：http://bcv.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://jvm.hywenlv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uhy.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://esy.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://wae.yueranfly.top

Java: interface Shape { double area(); }
来源：http://uqv.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://uqu.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cfl.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://cpz.ybcxt.top

[G10] 访问控制
来源：http://hbs.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://otl.haohaochexian.top

PHP:  public / protected / private
来源：http://dgb.iojbl.cn

JS:   #private 字段；其余公开
来源：http://lkc.yongpay.top

TS:   public / protected / private
来源：http://fel.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://yec.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fay.316326.xyz

Ruby: public / protected / private
来源：http://per.tian-w.cn

C#:   public / protected / private / internal
来源：http://ijt.zdbjq.cn

[G11] getter / setter
来源：http://ckh.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://laf.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://aly.mhx1999.top

JS:   get name() { return this._name; }
来源：http://urd.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://ybg.cashguo.top

Java: public String getName() { return name; }
来源：http://zcm.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tvj.tanke756.top

Ruby: attr_accessor :name
来源：http://xvw.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://akf.hcnkem.com

[G12] 对象转字符串
来源：http://gtg.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://ztr.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://czs.yuxming.cn

JS:   toString() { return this.name; }
来源：http://bsx.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://jat.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://lxp.jinqigfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://bge.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://sux.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://fma.c1oappe.top

[G13] 判断对象类型
来源：http://hgg.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://enb.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://mym.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://guv.gaohongyu789.top

TS:   u instanceof User
来源：http://nyu.gotoacloud.top

Java: u instanceof User
来源：http://jcl.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pel.fzhhl.top

Ruby: u.is_a?(User)
来源：http://ccz.havefunace.top

C#:   u is User
来源：http://asm.yuxming.cn

[G14] 数据类 / record
来源：http://phv.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yyx.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://vub.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://ebe.zhaomingkeji.xyz

TS:   type User = { name: string; age: number };
来源：http://deh.sweek.top

Java: record User(String name, int age) {}
来源：http://yfh.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://vbv.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://evl.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://cuk.ivvv.top

[G15] 枚举
来源：http://rfb.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wrd.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ozj.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cia.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hai.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://lek.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rsd.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://gub.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://omg.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://blk.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uyq.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://efq.yangfankeji.com

JS:   Object.entries(obj)
来源：http://xpy.0kj1m.cn

TS:   Object.entries(obj)
来源：http://pdi.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yhw.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://wdp.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://pec.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://dec.yuxming.cn

================================================================================
来源：http://hso.cucudq.cn

H. 异常与错误处理
来源：http://tfy.hongshengwenyu.top

================================================================================
来源：http://mkb.jinqigufen.top

[H01] try / catch 基础
来源：http://uyh.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ecn.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rvl.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dsm.hywenlv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://etj.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lwu.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ajm.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://igm.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ljr.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://xgv.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rsz.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qqv.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sjj.hnxiangtu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://can.mhx1999.top

Java: try { f(); } finally { cleanup(); }
来源：http://xal.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://asf.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://chs.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jmr.yanxiufei.cn

[H03] 主动抛出异常
来源：http://upq.vehdjk.com

Py:   raise ValueError("错误信息")
来源：http://vms.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lss.cucudq.cn

JS:   throw new Error("错误信息");
来源：http://jrm.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://ict.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rgq.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://muq.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nhk.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pey.daria6918.cn

[H04] 自定义异常类型
来源：http://zot.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://zbf.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uny.bjfxy.top

JS:   class MyError extends Error {}
来源：http://ekr.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://yqi.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://tik.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://byv.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://jsa.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://myf.svipenyu.cn

[H05] 捕获特定类型
来源：http://jpn.yfazqb.com

Py:   except ValueError as e:
来源：http://gjg.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owt.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://ydf.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://qei.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://gwq.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://paj.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://wzj.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uuu.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://rjc.sxryk.cn

Py:   value = d.get("k") or default
来源：http://ldx.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://evc.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wut.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://usn.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lox.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://shm.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://gcu.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://drd.shanyushiyangkeji.top

[H07] 断言
来源：http://apl.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://gsi.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://oaq.fehbvm.com

JS:   console.assert(x > 0);
来源：http://wwi.zhaomingkeji.xyz

TS:   console.assert(x > 0);
来源：http://ibo.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://qfi.zhaomingkeji.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fpj.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://opx.shanyushiyangtech.top

C#:   Debug.Assert(x > 0);
来源：http://eiy.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://whl.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://klj.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dwn.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://ymm.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ujz.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://reo.haohaochexian.top

Go:   err.Error()
来源：http://rvi.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://qrr.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://rnh.yj202588.top

[H09] 带错误码的异常
来源：http://epz.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kxg.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pht.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oeg.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yby.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bak.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hcc.kuanghao11.cn

Ruby: raise MyError.new("fail", 500)
来源：http://psn.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ryi.yj20258.top

[H10] 资源自动释放
来源：http://vyh.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oai.hesvh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oob.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vva.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://okh.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xsd.jqgfzy.top

Go:   defer f.Close()
来源：http://gcb.daria6918.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kci.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://riq.hnxiangtu.top

================================================================================
来源：http://gxs.mhx1999.top

I. 正则表达式
来源：http://cul.wangdashe.top

================================================================================
来源：http://lmo.zhixingplan.top

[I01] 判断是否匹配
来源：http://dvr.sufxvd.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gpg.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://bgf.ivvv.top

JS:   /\d+/.test(s)
来源：http://jhq.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://ydf.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ahf.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ruv.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://nzl.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yly.nwbrower.top

[I02] 提取所有匹配
来源：http://fur.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://vbu.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vcs.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xmt.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://fdo.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://inb.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jdr.wangshuangyany.cn

Ruby: s.scan(/\d+/)
来源：http://gmt.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bsy.fengsongda.top

[I03] 提取捕获分组
来源：http://tiy.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cus.xziqi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pwc.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nan.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lxr.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://irk.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://alx.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ina.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jjm.chenjidiqi.icu

[I04] 正则替换
来源：http://vkw.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uqg.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cvv.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://lgg.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://zpj.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://dwk.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qgm.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://prl.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kbc.guannengcc.top

[I05] 按正则拆分
来源：http://wwv.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://euj.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cri.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vgn.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://gzk.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://oce.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bbv.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://raz.shangyingyoupin.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rou.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxw.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kuh.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jkm.kuanghao11.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rog.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ndd.bjfxy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kyd.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uxg.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qhd.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yty.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://onb.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hia.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tip.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mzo.hcnkem.com

TS:   /error/gim
来源：http://zoo.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://esz.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://obw.snrcjt.cn


<!-- 参考信息 -->