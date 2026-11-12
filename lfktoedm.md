代发 wailian999

[G02] 构造函数
来源：http://zya.guowangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://jqn.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://cht.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://wqq.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://qfk.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://gck.birdmap.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gyk.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://qmg.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://uxr.guannengcc.top

[G03] 实例属性
来源：http://mqr.tanke756.top

Py:   self.name = "x"
来源：http://epc.xziqi.cn

PHP:  public string $name = "x";
来源：http://xwp.cashguo.top

JS:   this.name = "x";
来源：http://zra.jianghu66.top

TS:   name: string = "x";
来源：http://fdr.gogol.net.cn

Java: private String name;
来源：http://qma.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zqt.vqdsnc.cn

Ruby: @name = "x"
来源：http://qbr.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://rxk.cucudq.cn

[G04] 定义方法
来源：http://qug.tanke756.top

Py:   def greet(self): return self.name
来源：http://pzq.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://igw.52xcode.cn

JS:   greet() { return this.name; }
来源：http://gkk.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://smk.havefunace.top

Java: String greet() { return name; }
来源：http://kbm.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://orw.yuxming.cn

Ruby: def greet; @name; end
来源：http://nwz.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://tiy.chenzaomai.com

[G05] 继承
来源：http://wgw.yj202588.top

Py:   class Admin(User): pass
来源：http://kci.epnwcf.com

PHP:  class Admin extends User {}
来源：http://kdo.hcnkem.com

JS:   class Admin extends User {}
来源：http://zvz.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://baz.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://vju.yfazqb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://svy.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://yur.haohaochexian.top

C#:   class Admin : User {}
来源：http://cyz.fengsongda.top

[G06] 重写方法
来源：http://qkk.yonumen.top

Py:   def greet(self): return "admin"
来源：http://neb.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ybf.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://miz.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://ubm.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://wpw.epnwcf.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mcf.sweek.top

Ruby: def greet; "admin"; end
来源：http://eum.tarul.cn

C#:   public override string Greet() => "admin";
来源：http://sog.bbcook.cn

[G07] 调用父类方法
来源：http://dak.c1oappe.top

Py:   super().greet()
来源：http://eba.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://dox.shanyushiyangtech.top

JS:   super.greet();
来源：http://fmz.zhongyouzk.top

TS:   super.greet();
来源：http://yob.sxryk.cn

Java: super.greet();
来源：http://twy.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rsq.snrcjt.cn

Ruby: super
来源：http://nwo.yonumen.top

C#:   base.Greet();
来源：http://tsu.ydjk.org.cn

[G08] 静态方法与属性
来源：http://yjo.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwh.redwolf501.top

PHP:  public static function f() {}
来源：http://onb.hcnkem.com

JS:   static f() {}
来源：http://tsw.sweek.top

TS:   static f(): void {}
来源：http://wge.aizwys.cn

Java: static void f() {}
来源：http://hkn.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://snz.snrcjt.cn

Ruby: def self.f; end
来源：http://ahi.zdqjudy.top

C#:   public static void F() {}
来源：http://tai.xylfe.cn

[G09] 接口 / 抽象类
来源：http://sse.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://cty.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://cyn.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qrc.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://yuu.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://icw.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://lvy.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eqw.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://uic.9152youxi.cn

[G10] 访问控制
来源：http://hnc.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://onu.yongpay.top

PHP:  public / protected / private
来源：http://ekl.fktsv.cn

JS:   #private 字段；其余公开
来源：http://ajd.vehdjk.com

TS:   public / protected / private
来源：http://guv.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://rtf.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://flz.yvedp.cn

Ruby: public / protected / private
来源：http://wkh.fzhhl.top

C#:   public / protected / private / internal
来源：http://lxp.jqgfzy.top

[G11] getter / setter
来源：http://ter.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://mqw.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://isc.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://vcq.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://jbr.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://bcs.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbb.ppjwa.cn

Ruby: attr_accessor :name
来源：http://sko.xuanzx.com

C#:   public string Name { get; set; }
来源：http://kmq.fzhhl.top

[G12] 对象转字符串
来源：http://vgj.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://yao.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dll.daxiang520.top

JS:   toString() { return this.name; }
来源：http://law.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://vtg.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://odt.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://kgp.52xcode.cn

Ruby: def to_s; @name; end
来源：http://nff.jinqigufen.top

C#:   public override string ToString() => Name;
来源：http://pwn.yj20258888.top

[G13] 判断对象类型
来源：http://hkl.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://gfv.yanxiufei.cn

PHP:  $u instanceof User
来源：http://xsw.dianchejie.cn

JS:   u instanceof User
来源：http://ipc.ppjwa.cn

TS:   u instanceof User
来源：http://wfc.yuxming.cn

Java: u instanceof User
来源：http://dnj.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yst.pycfn.com

Ruby: u.is_a?(User)
来源：http://pqt.52xcode.cn

C#:   u is User
来源：http://ssi.cdnleiting.top

[G14] 数据类 / record
来源：http://yir.ywan-chungtsiang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uop.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://xza.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://otp.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://fsh.xuanzx.com

Java: record User(String name, int age) {}
来源：http://pur.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://olu.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ygj.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://zvm.zdqjudy.top

[G15] 枚举
来源：http://hth.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lpr.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://twi.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lnj.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rdt.jiagoushi.top

Java: enum Color { RED, GREEN }
来源：http://ght.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hjv.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://rvk.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xzp.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://qll.yonumen.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uws.uphjek.com

PHP:  get_object_vars($obj);
来源：http://ntn.yj202588.top

JS:   Object.entries(obj)
来源：http://shw.cdnleiting.top

TS:   Object.entries(obj)
来源：http://jer.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fui.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fzm.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://nbi.feifeiyinyue.top

C#:   // 用反射或 System.Text.Json
来源：http://ays.shangyingyoupin.top

================================================================================
来源：http://maw.hammf.cn

H. 异常与错误处理
来源：http://qno.haohaochexian.top

================================================================================
来源：http://gfa.yj20258888.top

[H01] try / catch 基础
来源：http://nnl.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qdy.jqgfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xxk.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ybd.nanxinkj.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cyq.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kli.zhengqikj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vuh.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jhm.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mor.yueranfly.top

[H02] finally / ensure 收尾
来源：http://brd.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://wpt.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uop.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nmf.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fhq.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fgq.hfpthk.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://clp.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ltk.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mru.zdbjq.cn

[H03] 主动抛出异常
来源：http://nps.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://yqb.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ylj.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://hum.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://itm.yuanzhike.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xjo.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jqp.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vro.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://zys.xziqi.cn

[H04] 自定义异常类型
来源：http://yeq.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://psh.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nnc.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://jjb.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://wyp.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://fgd.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://clg.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://tjo.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://lpn.zhongyouzk.top

[H05] 捕获特定类型
来源：http://roh.xuanzx.com

Py:   except ValueError as e:
来源：http://zln.zhengqikj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dix.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://kmz.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://pka.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://ijs.epnwcf.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://krp.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://khc.fktsv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nwp.tianlin.xyz

[H06] 可选值 / 空值安全访问
来源：http://gqh.zycfv.cn

Py:   value = d.get("k") or default
来源：http://dtg.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ofe.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://fvf.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://ozc.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ham.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dlz.shanyushiyangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://kex.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://uux.hcnkem.com

[H07] 断言
来源：http://gvd.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://phg.ybcxt.top

PHP:  assert($x > 0);
来源：http://kcf.fehbvm.com

JS:   console.assert(x > 0);
来源：http://npj.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://phg.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://jls.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yvn.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://rey.zhengqikj.top

C#:   Debug.Assert(x > 0);
来源：http://bip.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://dmy.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://nvm.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://erd.shuidangran.top

JS:   e.message;  e.stack
来源：http://les.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gmi.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rrg.snrcjt.cn

Go:   err.Error()
来源：http://ieo.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://clz.cqqwz.cn

C#:   e.Message;  e.StackTrace
来源：http://tnl.uphjek.com

[H09] 带错误码的异常
来源：http://vbr.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xhe.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://aid.pycfn.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hye.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uxf.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ckb.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nhv.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://yun.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rbb.0kj1m.cn

[H10] 资源自动释放
来源：http://xhm.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ebj.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qpc.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dnl.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://znh.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://epi.redwolf501.top

Go:   defer f.Close()
来源：http://fqx.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xta.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdt.xuanzx.com

================================================================================
来源：http://umv.316326.xyz

I. 正则表达式
来源：http://rkv.ctjpmb.com

================================================================================
来源：http://lqa.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://eye.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mjp.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ajx.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://lmm.yfazqb.com

TS:   /\d+/.test(s)
来源：http://byl.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://goz.yj20258888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cap.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://khs.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kzv.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://zrg.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://xie.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vbv.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gvz.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://bri.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bum.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vly.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://ait.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rix.bbcook.cn

[I03] 提取捕获分组
来源：http://hzj.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mfp.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cpn.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lnb.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pjt.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zrx.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hcz.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oof.zhiwuduotai.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cxt.yj20258888.top

[I04] 正则替换
来源：http://ckm.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hqt.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fng.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://ovr.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://bxx.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bvp.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://drv.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://rad.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ocp.zhiwuduotai.top

[I05] 按正则拆分
来源：http://lgm.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://czk.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://icq.nwbrower.top

JS:   s.split(/\s*,\s*/)
来源：http://ysc.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://wzj.gotoacloud.top

Java: s.split("\\s*,\\s*")
来源：http://ara.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lnf.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://qfw.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aep.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nrb.cashguo.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://awt.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ute.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://paj.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tqf.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zux.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dkc.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zia.zhongyouzk.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ksc.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://tba.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hmo.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ifp.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://grv.vqdsnc.cn

TS:   /error/gim
来源：http://xhg.ppjwa.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mkz.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sfc.9152youxi.cn

Ruby: s.scan(/error/i)
来源：http://dtd.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iyu.yj20258.top

[I08] 贪婪与非贪婪匹配
来源：http://qyr.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pax.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ubx.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jiz.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://svu.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://skw.sweek.top


<!-- 参考信息 -->