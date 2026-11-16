代发 wailian999

Py:   class User: pass
来源：http://eqn.epnwcf.com

PHP:  class User {}
来源：http://ozt.fehbvm.com

JS:   class User {}
来源：http://mtm.hammf.cn

TS:   class User { name: string = ""; }
来源：http://djb.ivvv.top

Java: class User {}
来源：http://xjv.9152youxi.cn

Go:   type User struct { Name string }
来源：http://mcz.aizwys.cn

Ruby: class User; end
来源：http://wea.ivvv.top

C#:   class User {}
来源：http://wxy.hammf.cn

[G02] 构造函数
来源：http://yxk.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://vmh.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://nxd.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mhj.hesvh.cn

TS:   constructor(public name: string) {}
来源：http://new.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://aep.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eny.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://frq.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://uno.daria6918.cn

[G03] 实例属性
来源：http://yzv.guannengcc.top

Py:   self.name = "x"
来源：http://zhk.sufxvd.cn

PHP:  public string $name = "x";
来源：http://bhc.cheryme.top

JS:   this.name = "x";
来源：http://edl.wangshuangyany.cn

TS:   name: string = "x";
来源：http://buu.cdnleiting.top

Java: private String name;
来源：http://quz.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gnc.sweek.top

Ruby: @name = "x"
来源：http://bnt.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://lev.aizwys.cn

[G04] 定义方法
来源：http://qmg.nwbrower.top

Py:   def greet(self): return self.name
来源：http://kpk.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jhc.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://ucm.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://bcc.aizwys.cn

Java: String greet() { return name; }
来源：http://pae.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://brp.xylfe.cn

Ruby: def greet; @name; end
来源：http://xug.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://qje.mhx1999.top

[G05] 继承
来源：http://yjy.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://twr.aizwys.cn

PHP:  class Admin extends User {}
来源：http://snq.fktsv.cn

JS:   class Admin extends User {}
来源：http://bvi.fengsongda.top

TS:   class Admin extends User {}
来源：http://ufa.havefunace.top

Java: class Admin extends User {}
来源：http://azl.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rwn.c1oappe.top

Ruby: class Admin < User; end
来源：http://yps.fktsv.cn

C#:   class Admin : User {}
来源：http://gqm.yvedp.cn

[G06] 重写方法
来源：http://wha.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://fmr.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tmn.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://bbx.yj20258.top

TS:   greet(): string { return "admin"; }
来源：http://otr.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://iht.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rff.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://ezx.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://utx.jiagoushi.top

[G07] 调用父类方法
来源：http://szk.shuidangran.top

Py:   super().greet()
来源：http://ofn.hnxiangtu.top

PHP:  parent::greet();
来源：http://ezh.feifeiyinyue.top

JS:   super.greet();
来源：http://pab.wangshuangyany.cn

TS:   super.greet();
来源：http://fhs.hcnkem.com

Java: super.greet();
来源：http://ead.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dje.jlsjyb.cn

Ruby: super
来源：http://oii.fengsongda.top

C#:   base.Greet();
来源：http://sak.zhengqikj.top

[G08] 静态方法与属性
来源：http://uge.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eeh.hfpthk.cn

PHP:  public static function f() {}
来源：http://isw.yuxming.cn

JS:   static f() {}
来源：http://vei.yueranfly.top

TS:   static f(): void {}
来源：http://grp.fktsv.cn

Java: static void f() {}
来源：http://ant.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bee.zhijiandao.cn

Ruby: def self.f; end
来源：http://lxi.svipenyu.cn

C#:   public static void F() {}
来源：http://whg.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://lze.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://xdx.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://ggz.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xor.jqgufenzy.top

TS:   interface Shape { area(): number; }
来源：http://wnh.yfazqb.com

Java: interface Shape { double area(); }
来源：http://kpv.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://fvy.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://egd.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://hep.c1oappe.top

[G10] 访问控制
来源：http://vgh.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://aee.ydzc1.top

PHP:  public / protected / private
来源：http://zqh.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://lkl.epnwcf.com

TS:   public / protected / private
来源：http://cjd.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://ona.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrp.epnwcf.com

Ruby: public / protected / private
来源：http://hbo.xuetiantiany.cn

C#:   public / protected / private / internal
来源：http://psw.fanxiaobao.xyz

[G11] getter / setter
来源：http://hch.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://ebp.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dwh.hammf.cn

JS:   get name() { return this._name; }
来源：http://sqv.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://ukb.yfazqb.com

Java: public String getName() { return name; }
来源：http://wbw.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pmd.aizwys.cn

Ruby: attr_accessor :name
来源：http://fvx.tarul.cn

C#:   public string Name { get; set; }
来源：http://zas.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://yko.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://mos.gaohongyu789.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kon.iojbl.cn

JS:   toString() { return this.name; }
来源：http://atz.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://qja.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://trt.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://exx.yj20258.top

Ruby: def to_s; @name; end
来源：http://krz.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://qpc.jinqigfzy.top

[G13] 判断对象类型
来源：http://pgv.hysaishi.cn

Py:   isinstance(u, User)
来源：http://lje.cucudq.cn

PHP:  $u instanceof User
来源：http://xtg.jyoumei.cn

JS:   u instanceof User
来源：http://xgn.sjlbkw.cn

TS:   u instanceof User
来源：http://yza.yanxiufei.cn

Java: u instanceof User
来源：http://nma.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mmg.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://dge.haohaochexian.top

C#:   u is User
来源：http://lcz.zhaomingkeji.xyz

[G14] 数据类 / record
来源：http://yqq.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mhe.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://nhs.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jdz.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://tek.fktsv.cn

Java: record User(String name, int age) {}
来源：http://cuf.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://yud.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mrd.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://mxc.vqdsnc.cn

[G15] 枚举
来源：http://cun.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://omg.aibaodan.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://eyg.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dek.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hei.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://afy.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mhq.yfazqb.com

Ruby: Color = %i[red green].freeze
来源：http://kxi.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pro.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://oja.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cls.ctjpmb.com

PHP:  get_object_vars($obj);
来源：http://hdh.zdbjq.cn

JS:   Object.entries(obj)
来源：http://gaf.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://tar.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uiy.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://onf.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://zdt.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://ujy.sysykeji.top

================================================================================
来源：http://fri.xziqi.cn

H. 异常与错误处理
来源：http://dia.daria6918.cn

================================================================================
来源：http://aed.zhijiandao.cn

[H01] try / catch 基础
来源：http://cfq.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tzm.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://azx.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dax.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lur.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://epb.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pky.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bqv.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xsx.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://elj.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bxd.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ncq.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ngv.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://aox.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://auf.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ylo.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hen.cheryme.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cxp.zhongyouzk.top

[H03] 主动抛出异常
来源：http://jkx.52xcode.cn

Py:   raise ValueError("错误信息")
来源：http://ilo.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://szf.yj202588.top

JS:   throw new Error("错误信息");
来源：http://ubg.hammf.cn

TS:   throw new Error("错误信息");
来源：http://yyp.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ykm.ctjpmb.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ces.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ktg.hcnkem.com

C#:   throw new ArgumentException("错误信息");
来源：http://brt.iojbl.cn

[H04] 自定义异常类型
来源：http://dgx.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://sle.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tat.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://ubs.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://pzh.yanxiufei.cn

Java: class MyException extends RuntimeException {}
来源：http://jrl.c1oappe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lsc.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://rxb.guannengcc.top

C#:   class MyException : Exception {}
来源：http://gcz.nwbrower.top

[H05] 捕获特定类型
来源：http://eou.zhijiandao.cn

Py:   except ValueError as e:
来源：http://odl.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qwe.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://pcg.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://wpf.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://zfb.hammf.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cqz.jinqigufen.top

Ruby: rescue ArgumentError => e
来源：http://abm.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fae.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://cow.redwolf501.top

Py:   value = d.get("k") or default
来源：http://wbx.yfazqb.com

PHP:  $v = $d["k"] ?? null;
来源：http://mkp.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://bpx.ywan-chungtsiang.top

TS:   obj?.a?.b;  d ?? default
来源：http://mnp.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lby.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hbl.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://ldc.ydjk.org.cn

C#:   obj?.A?.B ?? default
来源：http://eqx.jqgfzy.top

[H07] 断言
来源：http://jyq.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://vta.ybcxt.top

PHP:  assert($x > 0);
来源：http://bnk.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://yub.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://dvv.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://tpl.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vwx.yanxiufei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bca.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://qed.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://rvz.guannengcc.top

Py:   str(e);  traceback.format_exc()
来源：http://nto.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gbl.nanxinkj.top

JS:   e.message;  e.stack
来源：http://mjx.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qja.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://szs.smart0.xyz

Go:   err.Error()
来源：http://dff.daxiang520.top

Ruby: e.message;  e.backtrace
来源：http://phk.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://hyw.smart0.xyz

[H09] 带错误码的异常
来源：http://awn.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qke.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fet.0kj1m.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ozi.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jcs.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://psx.jinyuanbaomall.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wvv.zhoulong.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ade.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zec.fktsv.cn

[H10] 资源自动释放
来源：http://sxe.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zlu.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://riq.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://maq.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tlb.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://otc.jqgufenzy.top

Go:   defer f.Close()
来源：http://dpu.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lmk.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqp.yj20258888.top

================================================================================
来源：http://lzn.0kj1m.cn

I. 正则表达式
来源：http://hol.fehbvm.com

================================================================================
来源：http://ptr.jyoumei.cn

[I01] 判断是否匹配
来源：http://dsj.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nhs.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://syf.yuxming.cn

JS:   /\d+/.test(s)
来源：http://kec.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://ivx.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://upi.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hue.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://gwd.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pki.hammf.cn

[I02] 提取所有匹配
来源：http://sfj.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://nor.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://myk.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xgp.yj202588.top

TS:   s.match(/\d+/g)
来源：http://ccn.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mcf.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://saw.svipenyu.cn

Ruby: s.scan(/\d+/)
来源：http://wkh.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ioy.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://pqg.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pfm.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aki.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zve.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rli.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://der.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qpg.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eiz.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vav.ywan-chungtsiang.top

[I04] 正则替换
来源：http://gch.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://stb.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oio.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://eyf.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jmu.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ska.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tav.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oml.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oon.nwbrower.top

[I05] 按正则拆分
来源：http://nnj.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://keu.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tuc.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://uak.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://tsj.nwbrower.top

Java: s.split("\\s*,\\s*")
来源：http://vcj.zycfv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xsp.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://kkj.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tgh.pengpengdd.cyou

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdn.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qsb.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hwh.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukx.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ztg.hammf.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://opf.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hhw.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rjp.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kfe.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://mrq.jinghuilouyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lah.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zqx.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eqt.epnwcf.com

TS:   /error/gim
来源：http://xmq.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bjy.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qut.xuanzx.com


<!-- 参考信息 -->