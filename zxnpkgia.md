代发 wailian999

Java: class User {}
来源：http://pif.tanke756.top

Go:   type User struct { Name string }
来源：http://jng.yvedp.cn

Ruby: class User; end
来源：http://ayf.chenlongwang.top

C#:   class User {}
来源：http://vvu.cdnleiting.top

[G02] 构造函数
来源：http://wyy.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://ihl.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://gxh.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://ndd.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://uph.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://yaa.tianlin.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kal.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://ysa.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://jcb.fktsv.cn

[G03] 实例属性
来源：http://mxt.aibaodan.cn

Py:   self.name = "x"
来源：http://xtr.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://cca.nanxuanxn.top

JS:   this.name = "x";
来源：http://dxu.uphjek.com

TS:   name: string = "x";
来源：http://rgu.9152youxi.cn

Java: private String name;
来源：http://lxq.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://beu.tarul.cn

Ruby: @name = "x"
来源：http://xah.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://izd.yj20258.top

[G04] 定义方法
来源：http://eex.cqqwz.cn

Py:   def greet(self): return self.name
来源：http://bue.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mzi.hesvh.cn

JS:   greet() { return this.name; }
来源：http://oqp.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://kca.yonumen.top

Java: String greet() { return name; }
来源：http://qlo.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gmm.316326.xyz

Ruby: def greet; @name; end
来源：http://ikc.cucudq.cn

C#:   public string Greet() => Name;
来源：http://ucf.hfpthk.cn

[G05] 继承
来源：http://dhr.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://xoc.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://asy.yfazqb.com

JS:   class Admin extends User {}
来源：http://czu.guowangkeji.top

TS:   class Admin extends User {}
来源：http://pwk.yanxiufei.cn

Java: class Admin extends User {}
来源：http://nyr.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xiv.hysaishi.cn

Ruby: class Admin < User; end
来源：http://izx.jianghu66.top

C#:   class Admin : User {}
来源：http://ssf.hnxiangtu.top

[G06] 重写方法
来源：http://qaq.dianchejie.cn

Py:   def greet(self): return "admin"
来源：http://rab.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mbg.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://sqc.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://qng.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://whx.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://itn.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://pvz.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://idm.haohaochexian.top

[G07] 调用父类方法
来源：http://qkr.zhoulong.xyz

Py:   super().greet()
来源：http://izv.andypj.xyz

PHP:  parent::greet();
来源：http://jnx.jinyuanbaomall.cn

JS:   super.greet();
来源：http://fxv.jiagoushi.top

TS:   super.greet();
来源：http://ezv.xinyue.icu

Java: super.greet();
来源：http://xxv.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wqk.jinqigufen.top

Ruby: super
来源：http://hrv.cucudq.cn

C#:   base.Greet();
来源：http://nab.ctjpmb.com

[G08] 静态方法与属性
来源：http://yew.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ydk.guannengcc.top

PHP:  public static function f() {}
来源：http://gto.meibo888.top

JS:   static f() {}
来源：http://djq.tarul.cn

TS:   static f(): void {}
来源：http://rhv.ehwqpu.com

Java: static void f() {}
来源：http://jqd.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://laq.daria6918.cn

Ruby: def self.f; end
来源：http://ocl.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://rwi.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://noa.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://ahb.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://hii.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ioz.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://sht.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://tpn.shzxlz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ovf.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://woh.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://znk.hywenlv.cn

[G10] 访问控制
来源：http://duc.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://epm.xinyue.icu

PHP:  public / protected / private
来源：http://jgs.cucudq.cn

JS:   #private 字段；其余公开
来源：http://peb.andypj.xyz

TS:   public / protected / private
来源：http://pqa.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://nkg.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mdi.tian-w.cn

Ruby: public / protected / private
来源：http://wqs.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://mfv.hongshengwenyu.top

[G11] getter / setter
来源：http://udx.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://swq.jqgufenzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bep.meibo888.top

JS:   get name() { return this._name; }
来源：http://pjb.nwbrower.top

TS:   get name(): string { return this._name; }
来源：http://gty.gogol.net.cn

Java: public String getName() { return name; }
来源：http://kvf.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ter.aizwys.cn

Ruby: attr_accessor :name
来源：http://yfw.andypj.xyz

C#:   public string Name { get; set; }
来源：http://jyb.ydjk.org.cn

[G12] 对象转字符串
来源：http://tou.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://uxd.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hvi.sweek.top

JS:   toString() { return this.name; }
来源：http://tfw.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://iqw.zhiwuduotai.top

Java: @Override public String toString() { return name; }
来源：http://sca.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zmu.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://tsi.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://qcs.ybcxt.top

[G13] 判断对象类型
来源：http://dwy.wangdashe.top

Py:   isinstance(u, User)
来源：http://atc.yuxming.cn

PHP:  $u instanceof User
来源：http://hxj.feifeiyinyue.top

JS:   u instanceof User
来源：http://pol.52xcode.cn

TS:   u instanceof User
来源：http://dxn.ybcxt.top

Java: u instanceof User
来源：http://eeh.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://luy.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://shu.xinyue.icu

C#:   u is User
来源：http://xuj.gzhubu.top

[G14] 数据类 / record
来源：http://qcl.jinyuanbaomall.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://opu.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://odn.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://jxd.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://gjp.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://pda.fengsongda.top

Go:   type User struct { Name string; Age int }
来源：http://fmw.chenjidiqi.icu

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wsi.yueranfly.top

C#:   record User(string Name, int Age);
来源：http://nvk.jyoumei.cn

[G15] 枚举
来源：http://ady.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kly.xuanzx.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://wle.daxiang520.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mbz.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wqv.zhijiandao.cn

Java: enum Color { RED, GREEN }
来源：http://qsy.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jot.sxryk.cn

Ruby: Color = %i[red green].freeze
来源：http://pxe.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://urm.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://ayx.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nxp.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://wyz.sufxvd.cn

JS:   Object.entries(obj)
来源：http://clc.sxryk.cn

TS:   Object.entries(obj)
来源：http://zcv.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lzd.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rgk.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://wyg.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://xox.9152youxi.cn

================================================================================
来源：http://vyj.chenjidiqi.icu

H. 异常与错误处理
来源：http://zaf.yj20258888.top

================================================================================
来源：http://jlu.shangyingyoupin.top

[H01] try / catch 基础
来源：http://coa.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pdc.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gsh.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uht.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pob.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hid.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://acu.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gpw.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kud.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://nuu.gotoacloud.top

Py:   try: f()⏎finally: cleanup()
来源：http://vsf.iojbl.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rop.guannengcc.top

JS:   try { f(); } finally { cleanup(); }
来源：http://poz.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qiq.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zhh.jqgfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://emb.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nru.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jlw.yfazqb.com

[H03] 主动抛出异常
来源：http://jex.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://oyp.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://srz.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://xcx.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://yrr.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jnz.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nka.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://due.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://vko.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://mfa.shanyushiyangtech.top

Py:   class MyError(Exception): pass
来源：http://xrv.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://wdw.birdmap.top

JS:   class MyError extends Error {}
来源：http://kdm.smart0.xyz

TS:   class MyError extends Error {}
来源：http://sqc.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://wln.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uka.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://pgc.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://oma.hcnkem.com

[H05] 捕获特定类型
来源：http://cbh.zhoulong.xyz

Py:   except ValueError as e:
来源：http://fdd.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bhf.chenzaomai.com

JS:   if (e instanceof TypeError) {}
来源：http://bcp.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://vem.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://pmy.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zaf.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://ryu.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wyz.cqqwz.cn

[H06] 可选值 / 空值安全访问
来源：http://yws.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://uzj.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://lna.fktsv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ydu.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vph.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://viu.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pbv.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://nan.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://yei.svipenyu.cn

[H07] 断言
来源：http://bcz.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://tyr.cucudq.cn

PHP:  assert($x > 0);
来源：http://sxu.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://xmp.fktsv.cn

TS:   console.assert(x > 0);
来源：http://ime.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://ree.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qvi.ydjk.org.cn

Ruby: raise "必须为正" unless x > 0
来源：http://utn.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://jwt.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://otl.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://cnq.sufxvd.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hmh.chenlongwang.top

JS:   e.message;  e.stack
来源：http://gmb.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ccs.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://guv.haohaochexian.top

Go:   err.Error()
来源：http://hde.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://qjj.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://rjk.c1oappe.top

[H09] 带错误码的异常
来源：http://pkw.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ygr.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://sum.nanxuanxn.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://onq.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fuz.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blm.epnwcf.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yje.ydjk.org.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sdz.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ebn.yonumen.top

[H10] 资源自动释放
来源：http://ily.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mpb.havefunace.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imc.redwolf501.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fol.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vyk.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rzo.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://wqc.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://phu.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ioj.svipenyu.cn

================================================================================
来源：http://vvt.iojbl.cn

I. 正则表达式
来源：http://yhr.ydjk.org.cn

================================================================================
来源：http://stf.hammf.cn

[I01] 判断是否匹配
来源：http://hug.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gqx.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uut.pycfn.com

JS:   /\d+/.test(s)
来源：http://mhh.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://vfm.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dlg.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qua.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://lei.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vbm.fengsongda.top

[I02] 提取所有匹配
来源：http://bvp.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://uxk.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://duo.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ahx.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://uqs.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kpz.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ejo.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://qke.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ors.vqdsnc.cn

[I03] 提取捕获分组
来源：http://jwe.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://las.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ahl.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nih.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lsq.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gda.zhoulong.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pgj.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fnd.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gbg.xylfe.cn

[I04] 正则替换
来源：http://mqs.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://zxx.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rxq.guannengcc.top

JS:   s.replace(/\d+/g, "#")
来源：http://zoz.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kuv.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://arj.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tij.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lnz.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lff.chenjidiqi.icu

[I05] 按正则拆分
来源：http://luj.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ihi.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lam.0kj1m.cn

JS:   s.split(/\s*,\s*/)
来源：http://ubb.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://lgo.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://pqp.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sey.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ioa.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://klh.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vbx.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cae.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://otu.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drb.yvedp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hcy.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sym.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cey.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dfb.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uxe.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://ybx.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wqf.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysy.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://avh.tarul.cn

TS:   /error/gim
来源：http://mia.sweek.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ejt.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oce.haohaochexian.top

Ruby: s.scan(/error/i)
来源：http://oyk.shanyushiyangtech.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zaj.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://qkl.gzhubu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pyr.yongpay.top


<!-- 参考信息 -->