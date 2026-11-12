代发 wailian999

TS:   constructor(public name: string) {}
来源：http://fdj.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://dlm.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lge.sufxvd.cn

Ruby: def initialize(name); @name = name; end
来源：http://qxj.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://huu.zhoulong.xyz

[G03] 实例属性
来源：http://ggn.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://uyx.mhx1999.top

PHP:  public string $name = "x";
来源：http://qvv.yj20258888.top

JS:   this.name = "x";
来源：http://cuu.uphjek.com

TS:   name: string = "x";
来源：http://uiw.quarkkingdee.top

Java: private String name;
来源：http://uzb.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://clu.hammf.cn

Ruby: @name = "x"
来源：http://tmu.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://wwo.jinqigfzy.top

[G04] 定义方法
来源：http://kxf.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://tio.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://hot.bbcook.cn

JS:   greet() { return this.name; }
来源：http://fon.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://sfu.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://tcg.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gag.zdqjudy.top

Ruby: def greet; @name; end
来源：http://dfs.sweek.top

C#:   public string Greet() => Name;
来源：http://inj.vqdsnc.cn

[G05] 继承
来源：http://vzn.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://hcx.aizwys.cn

PHP:  class Admin extends User {}
来源：http://ekf.fengsongda.top

JS:   class Admin extends User {}
来源：http://mcq.gotoacloud.top

TS:   class Admin extends User {}
来源：http://laq.jlsjyb.cn

Java: class Admin extends User {}
来源：http://lyq.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://syv.epnwcf.com

Ruby: class Admin < User; end
来源：http://dae.tanke756.top

C#:   class Admin : User {}
来源：http://kzm.yj20258888.top

[G06] 重写方法
来源：http://cky.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://itd.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://atq.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://nar.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://oml.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://vih.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zva.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://eus.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://jcn.mhx1999.top

[G07] 调用父类方法
来源：http://kdz.cqqwz.cn

Py:   super().greet()
来源：http://knk.jinqigfzy.top

PHP:  parent::greet();
来源：http://xna.nanxinkj.top

JS:   super.greet();
来源：http://wxm.dianchejie.cn

TS:   super.greet();
来源：http://ujy.hfpthk.cn

Java: super.greet();
来源：http://lrn.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hxu.yj20258888.top

Ruby: super
来源：http://cjd.zhiwuduotai.top

C#:   base.Greet();
来源：http://ole.fzhhl.top

[G08] 静态方法与属性
来源：http://xla.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://txe.fehbvm.com

PHP:  public static function f() {}
来源：http://tqe.ywan-chungtsiang.top

JS:   static f() {}
来源：http://dvy.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://uot.uphjek.com

Java: static void f() {}
来源：http://vdp.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wek.chenzaomai.com

Ruby: def self.f; end
来源：http://ego.hcnkem.com

C#:   public static void F() {}
来源：http://qiz.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://lpg.jianghu66.top

Py:   from abc import ABC, abstractmethod
来源：http://pti.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://owb.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzx.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://xic.xylfe.cn

Java: interface Shape { double area(); }
来源：http://scz.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://apf.guowangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vcb.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://ial.tianlin.xyz

[G10] 访问控制
来源：http://esd.xingfuxueyuan.xyz

Py:   约定 _protected / __private（不强制）
来源：http://slk.sweek.top

PHP:  public / protected / private
来源：http://bkp.xziqi.cn

JS:   #private 字段；其余公开
来源：http://nig.aibaodan.cn

TS:   public / protected / private
来源：http://cgl.cheryme.top

Java: public / protected / private / 默认包级
来源：http://ima.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jnq.bjfxy.top

Ruby: public / protected / private
来源：http://zpu.dashuyun.cn

C#:   public / protected / private / internal
来源：http://wrj.fehbvm.com

[G11] getter / setter
来源：http://olf.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://jbr.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oel.quarkkingdee.top

JS:   get name() { return this._name; }
来源：http://dwa.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://ttp.jqgfzy.top

Java: public String getName() { return name; }
来源：http://tuw.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hte.aizwys.cn

Ruby: attr_accessor :name
来源：http://yfl.zhaomingkeji.xyz

C#:   public string Name { get; set; }
来源：http://dxp.fzhhl.top

[G12] 对象转字符串
来源：http://lkx.cashguo.top

Py:   def __str__(self): return self.name
来源：http://iac.gzhubu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gqb.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://ttv.fktsv.cn

TS:   toString(): string { return this.name; }
来源：http://vwc.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://cvv.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://drj.bbcook.cn

Ruby: def to_s; @name; end
来源：http://npo.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://poc.yj20258888.top

[G13] 判断对象类型
来源：http://pwq.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://vce.tanke756.top

PHP:  $u instanceof User
来源：http://tbb.dianchejie.cn

JS:   u instanceof User
来源：http://jxn.ehwqpu.com

TS:   u instanceof User
来源：http://afu.feifeiyinyue.top

Java: u instanceof User
来源：http://qzq.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tdk.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://tku.jinyuanbaomall.cn

C#:   u is User
来源：http://lof.shuidangran.top

[G14] 数据类 / record
来源：http://lsi.vehdjk.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jvi.gotoacloud.top

PHP:  // 用 readonly 属性模拟
来源：http://dyh.quarkkingdee.top

JS:   // 无内置：普通类或对象字面量
来源：http://upj.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://gwf.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://axa.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://qgu.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zui.gogol.net.cn

C#:   record User(string Name, int Age);
来源：http://vey.ybcxt.top

[G15] 枚举
来源：http://dvo.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kqy.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hna.shzxlz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hrb.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gbl.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://wql.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cdv.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://hzz.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rsz.epnwcf.com

[G16] 对象转数组 / 字典
来源：http://tns.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hlx.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://kdc.yj20258888.top

JS:   Object.entries(obj)
来源：http://eqx.sweek.top

TS:   Object.entries(obj)
来源：http://fei.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zfg.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://nkc.yonumen.top

Ruby: obj.instance_variables
来源：http://qal.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://opi.yongpay.top

================================================================================
来源：http://lbi.fehbvm.com

H. 异常与错误处理
来源：http://zkt.mhx1999.top

================================================================================
来源：http://ulm.ehwqpu.com

[H01] try / catch 基础
来源：http://nnc.hongshengwenyu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qyu.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cnm.ydzc1.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dsn.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ozq.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kfb.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vre.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tjx.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yhe.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://tek.ydzc1.top

Py:   try: f()⏎finally: cleanup()
来源：http://gpi.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hty.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hli.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zsy.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://med.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ibw.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://slq.chenlongwang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bga.cucudq.cn

[H03] 主动抛出异常
来源：http://adf.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://dgw.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zyr.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://gif.bbcook.cn

TS:   throw new Error("错误信息");
来源：http://sht.xuanzx.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://ltj.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tne.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://myl.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zmf.ivvv.top

[H04] 自定义异常类型
来源：http://loz.zhaomingkeji.xyz

Py:   class MyError(Exception): pass
来源：http://xhw.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://jwf.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://nss.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://tgz.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://bwe.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://thl.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://frg.jiagoushi.top

C#:   class MyException : Exception {}
来源：http://wtr.ydjk.org.cn

[H05] 捕获特定类型
来源：http://grq.meibo888.top

Py:   except ValueError as e:
来源：http://ppk.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gyc.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://bqv.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://klr.xinyue.icu

Java: catch (IOException | SQLException e) {}
来源：http://ctt.zhengqikj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ajh.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://lwr.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eqx.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://mej.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://rro.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://qrq.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://ina.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ugm.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qaj.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qzb.yj20258888.top

Ruby: d&.dig(:a, :b)
来源：http://fct.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://hdc.xylfe.cn

[H07] 断言
来源：http://bsr.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://zbe.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://cee.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://ypr.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://dpr.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://pgl.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yon.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zmm.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://eyj.uphjek.com

[H08] 获取错误信息与堆栈
来源：http://hyl.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://quq.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cyg.meibo888.top

JS:   e.message;  e.stack
来源：http://zro.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vqt.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pyk.cashguo.top

Go:   err.Error()
来源：http://pqj.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://bnl.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://lyw.cqqwz.cn

[H09] 带错误码的异常
来源：http://awm.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdf.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dmt.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nnu.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hpf.zhiwuduotai.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqe.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tex.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ven.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://hpk.iojbl.cn

[H10] 资源自动释放
来源：http://ydd.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lpc.redwolf501.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mwz.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rdc.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nuk.jinghuilouyu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://del.52xcode.cn

Go:   defer f.Close()
来源：http://czm.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://djm.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oki.52xcode.cn

================================================================================
来源：http://hcd.yj202588.top

I. 正则表达式
来源：http://qea.shuidangran.top

================================================================================
来源：http://xvl.iojbl.cn

[I01] 判断是否匹配
来源：http://mvb.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sij.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wfu.sysykeji.top

JS:   /\d+/.test(s)
来源：http://jod.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://nan.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jjb.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vfo.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://dbg.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gyu.hcnkem.com

[I02] 提取所有匹配
来源：http://qtt.hammf.cn

Py:   re.findall(r"\d+", s)
来源：http://yxd.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vsx.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sua.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://kgd.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://apf.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hka.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://uji.feifeiyinyue.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://flq.gogol.net.cn

[I03] 提取捕获分组
来源：http://lpl.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wrz.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qss.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://isy.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wjl.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iuv.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://spx.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hxb.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ktv.dashuyun.cn

[I04] 正则替换
来源：http://mza.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mri.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uvr.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://yoy.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://mgv.zhaomingkeji.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://olf.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hpp.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ztb.hammf.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tok.xylfe.cn

[I05] 按正则拆分
来源：http://wbu.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://unq.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bmh.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://mjk.wangshuangyany.cn

TS:   s.split(/\s*,\s*/)
来源：http://lvy.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://kre.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zhp.zhongyouzk.top

Ruby: s.split(/\s*,\s*/)
来源：http://ujt.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lqu.jinyuanbaomall.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lkm.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://itn.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lxi.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksh.zdqjudy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://udf.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zvo.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mgl.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hlm.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wuj.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://kks.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://orj.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nki.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hcc.cucudq.cn

TS:   /error/gim
来源：http://aub.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zqc.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uai.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://agy.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pjm.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://ivb.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://soy.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vft.ehwqpu.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wts.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mdw.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nxb.jinqigfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qds.hywenlv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwg.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lmx.zycfv.cn

================================================================================
来源：http://vre.shanyushiyangtech.top


<!-- 参考信息 -->