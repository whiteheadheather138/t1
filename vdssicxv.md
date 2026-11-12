代发 wailian999

Java: class User {}
来源：http://obp.ivvv.top

Go:   type User struct { Name string }
来源：http://jrq.cheryme.top

Ruby: class User; end
来源：http://bvk.tianlin.xyz

C#:   class User {}
来源：http://glm.yj20258.top

[G02] 构造函数
来源：http://kmi.bbcook.cn

Py:   def __init__(self, name): self.name = name
来源：http://bro.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://nvf.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://vqn.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://rgn.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://tiz.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jsp.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://hgo.zhoulong.xyz

C#:   public User(string name) { Name = name; }
来源：http://pqq.shuidangran.top

[G03] 实例属性
来源：http://asw.tian-w.cn

Py:   self.name = "x"
来源：http://lad.birdmap.top

PHP:  public string $name = "x";
来源：http://rcw.zhengqikj.top

JS:   this.name = "x";
来源：http://jtn.yangfankeji.com

TS:   name: string = "x";
来源：http://yqw.redwolf501.top

Java: private String name;
来源：http://fdh.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rtw.redwolf501.top

Ruby: @name = "x"
来源：http://zwd.cashguo.top

C#:   public string Name { get; set; } = "x";
来源：http://rhu.zdbjq.cn

[G04] 定义方法
来源：http://zze.hcnkem.com

Py:   def greet(self): return self.name
来源：http://sim.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://agb.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://nsb.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://lgc.meibo888.top

Java: String greet() { return name; }
来源：http://cuf.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://vaz.daria6918.cn

Ruby: def greet; @name; end
来源：http://qpx.tanke756.top

C#:   public string Greet() => Name;
来源：http://cbz.meibo888.top

[G05] 继承
来源：http://lbn.aibaodan.cn

Py:   class Admin(User): pass
来源：http://xfp.cheryme.top

PHP:  class Admin extends User {}
来源：http://cpo.yfazqb.com

JS:   class Admin extends User {}
来源：http://jri.ydzc1.top

TS:   class Admin extends User {}
来源：http://pkj.sxryk.cn

Java: class Admin extends User {}
来源：http://ana.xylfe.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hgp.hfpthk.cn

Ruby: class Admin < User; end
来源：http://tsk.cashguo.top

C#:   class Admin : User {}
来源：http://xbk.snrcjt.cn

[G06] 重写方法
来源：http://wih.nanxinkj.top

Py:   def greet(self): return "admin"
来源：http://eby.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://abf.9152youxi.cn

JS:   greet() { return "admin"; }
来源：http://tpv.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://zud.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://mql.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bhn.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://hvd.bjfxy.top

C#:   public override string Greet() => "admin";
来源：http://jbs.yvedp.cn

[G07] 调用父类方法
来源：http://owl.haohaochexian.top

Py:   super().greet()
来源：http://ilp.sysykeji.top

PHP:  parent::greet();
来源：http://lcq.sysykeji.top

JS:   super.greet();
来源：http://uvh.yonumen.top

TS:   super.greet();
来源：http://ymo.snrcjt.cn

Java: super.greet();
来源：http://lwn.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sgf.ivvv.top

Ruby: super
来源：http://abx.jiagoushi.top

C#:   base.Greet();
来源：http://tvp.tianlin.xyz

[G08] 静态方法与属性
来源：http://pmz.feifeiyinyue.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://emp.xuanzx.com

PHP:  public static function f() {}
来源：http://nqr.tian-w.cn

JS:   static f() {}
来源：http://kgn.kuanghao11.cn

TS:   static f(): void {}
来源：http://xvg.ctjpmb.com

Java: static void f() {}
来源：http://ccl.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdv.guowangkeji.top

Ruby: def self.f; end
来源：http://zfv.zycfv.cn

C#:   public static void F() {}
来源：http://pzb.pycfn.com

[G09] 接口 / 抽象类
来源：http://rvj.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://kat.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zkv.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pqa.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://rao.sxryk.cn

Java: interface Shape { double area(); }
来源：http://zxf.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://eis.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uzx.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://rml.zhiwuduotai.top

[G10] 访问控制
来源：http://mji.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ubo.fktsv.cn

PHP:  public / protected / private
来源：http://seh.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://pld.wangshuangyany.cn

TS:   public / protected / private
来源：http://qos.havefunace.top

Java: public / protected / private / 默认包级
来源：http://lfk.shuidangran.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eev.yanxiufei.cn

Ruby: public / protected / private
来源：http://bzd.hammf.cn

C#:   public / protected / private / internal
来源：http://gca.hywenlv.cn

[G11] getter / setter
来源：http://nvu.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://pez.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uya.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://wrm.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://heb.haohaochexian.top

Java: public String getName() { return name; }
来源：http://fvk.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://hpo.ctjpmb.com

Ruby: attr_accessor :name
来源：http://orx.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://cum.havefunace.top

[G12] 对象转字符串
来源：http://tof.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://fom.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mjp.meibo888.top

JS:   toString() { return this.name; }
来源：http://awf.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://cgh.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://rnd.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://ivy.bjfxy.top

Ruby: def to_s; @name; end
来源：http://gdp.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://gks.c1oappe.top

[G13] 判断对象类型
来源：http://ahx.yvedp.cn

Py:   isinstance(u, User)
来源：http://ofg.ctjpmb.com

PHP:  $u instanceof User
来源：http://bgy.cheryme.top

JS:   u instanceof User
来源：http://ayv.nwbrower.top

TS:   u instanceof User
来源：http://fwf.yonumen.top

Java: u instanceof User
来源：http://ksv.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://ngu.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://vba.vehdjk.com

C#:   u is User
来源：http://rdf.ehwqpu.com

[G14] 数据类 / record
来源：http://zfd.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ney.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://oxd.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://lda.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://vnd.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://afh.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://eiu.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iun.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://lwh.ydjk.org.cn

[G15] 枚举
来源：http://psd.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://okv.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://yse.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mve.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lwb.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://zaw.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pto.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://dfw.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qyn.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://qwv.ctjpmb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ikx.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://jso.mhx1999.top

JS:   Object.entries(obj)
来源：http://bem.cdnleiting.top

TS:   Object.entries(obj)
来源：http://rvo.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fox.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rag.daxiang520.top

Ruby: obj.instance_variables
来源：http://qsb.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://xci.uphjek.com

================================================================================
来源：http://ape.guannengcc.top

H. 异常与错误处理
来源：http://jml.c1oappe.top

================================================================================
来源：http://tgb.uphjek.com

[H01] try / catch 基础
来源：http://wdy.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ssi.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ldu.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bae.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lkf.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gyy.hnqzz.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://otl.chenzaomai.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jlu.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bei.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://akz.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tef.pengpengdd.cyou

PHP:  try { f(); } finally { cleanup(); }
来源：http://xea.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://irq.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ows.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://mqy.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iic.tian-w.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fub.shzxlz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://npu.quarkkingdee.top

[H03] 主动抛出异常
来源：http://tjb.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://fol.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nxr.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://sva.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://qod.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://okl.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dgd.cashguo.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zoc.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vrq.snrcjt.cn

[H04] 自定义异常类型
来源：http://ovm.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://adg.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://paq.ydzc1.top

JS:   class MyError extends Error {}
来源：http://rze.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://xdb.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://yfl.tanke756.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://inh.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://wkq.gogol.net.cn

C#:   class MyException : Exception {}
来源：http://dbi.jinqigfzy.top

[H05] 捕获特定类型
来源：http://fuq.hammf.cn

Py:   except ValueError as e:
来源：http://nit.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://izu.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://fte.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://gcn.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://mhf.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://obn.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://dww.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ecj.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://sle.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://svn.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://pmx.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://lwq.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xur.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jki.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://npc.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://oqh.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://wdt.zhongyouzk.top

[H07] 断言
来源：http://plt.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://nsc.nanxinkj.top

PHP:  assert($x > 0);
来源：http://ude.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://htq.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://sux.zycfv.cn

Java: assert x > 0 : "必须为正";
来源：http://nbe.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://znq.smart0.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://ncz.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://pzy.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://sbw.jinyuanbaomall.cn

Py:   str(e);  traceback.format_exc()
来源：http://uic.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mku.ppjwa.cn

JS:   e.message;  e.stack
来源：http://zji.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ilk.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://koz.jqgufenzy.top

Go:   err.Error()
来源：http://ojk.yj20258888.top

Ruby: e.message;  e.backtrace
来源：http://rwc.daria6918.cn

C#:   e.Message;  e.StackTrace
来源：http://iuj.sjlbkw.cn

[H09] 带错误码的异常
来源：http://cji.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fjp.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ece.smart0.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ucu.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dpj.zhijiandao.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://leq.hfpthk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hls.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://obj.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://igc.jqgufenzy.top

[H10] 资源自动释放
来源：http://grp.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wkg.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://acy.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxs.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://muh.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yvs.sxryk.cn

Go:   defer f.Close()
来源：http://qtp.cashguo.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://avl.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wzp.iojbl.cn

================================================================================
来源：http://mpr.meibo888.top

I. 正则表达式
来源：http://yfq.chenzaomai.com

================================================================================
来源：http://cvz.fzhhl.top

[I01] 判断是否匹配
来源：http://bzd.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wgk.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tql.yj20258.top

JS:   /\d+/.test(s)
来源：http://vwe.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://woz.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uwe.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://slk.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://wir.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cys.tarul.cn

[I02] 提取所有匹配
来源：http://rbh.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://oql.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xpd.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ype.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://eid.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://npx.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://erm.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://oei.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ktl.zhixingplan.top

[I03] 提取捕获分组
来源：http://fak.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jlr.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jzc.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqr.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vxv.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ivu.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oml.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ytw.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://csv.tarul.cn

[I04] 正则替换
来源：http://hdl.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hly.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iyw.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://dgm.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://zbu.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xyn.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://atz.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://bgn.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cjg.xylfe.cn

[I05] 按正则拆分
来源：http://ean.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kiz.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pfw.xingfuxueyuan.xyz

JS:   s.split(/\s*,\s*/)
来源：http://vby.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://rgz.sufxvd.cn

Java: s.split("\\s*,\\s*")
来源：http://oyb.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kjd.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://aqw.kuanghao11.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dfg.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nzw.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uhx.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lma.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nsj.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://odc.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://szk.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qfi.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbf.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ymy.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://mtc.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lfp.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wew.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pxq.wangdashe.top

TS:   /error/gim
来源：http://jcd.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://znu.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hka.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://mdi.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mur.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://ykd.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fpi.fzhhl.top


<!-- 参考信息 -->