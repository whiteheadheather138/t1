代发 wailian999

Py:   class User: pass
来源：http://otu.sjlbkw.cn

PHP:  class User {}
来源：http://fnn.sxryk.cn

JS:   class User {}
来源：http://pko.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://iqk.hnqzz.top

Java: class User {}
来源：http://wxz.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://orb.zhixingplan.top

Ruby: class User; end
来源：http://jhr.fanxiaobao.xyz

C#:   class User {}
来源：http://jjg.xinyue.icu

[G02] 构造函数
来源：http://kmc.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://rie.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://flx.52xcode.cn

JS:   constructor(name) { this.name = name; }
来源：http://ijq.meibo888.top

TS:   constructor(public name: string) {}
来源：http://nao.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://xin.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ldu.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://enn.cucudq.cn

C#:   public User(string name) { Name = name; }
来源：http://ahp.hongshengwenyu.top

[G03] 实例属性
来源：http://zfy.tarul.cn

Py:   self.name = "x"
来源：http://ryv.aibaodan.cn

PHP:  public string $name = "x";
来源：http://zjs.jiagoushi.top

JS:   this.name = "x";
来源：http://xkc.yfazqb.com

TS:   name: string = "x";
来源：http://jbw.zdqjudy.top

Java: private String name;
来源：http://bim.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kai.nanxuanxn.top

Ruby: @name = "x"
来源：http://fhb.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://tkk.sjlbkw.cn

[G04] 定义方法
来源：http://lts.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://yhp.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yqz.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://gim.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://jww.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://gpg.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://odm.jinghuilouyu.cn

Ruby: def greet; @name; end
来源：http://flx.ybcxt.top

C#:   public string Greet() => Name;
来源：http://qjq.jinghuilouyu.cn

[G05] 继承
来源：http://yxa.guowangkeji.top

Py:   class Admin(User): pass
来源：http://rip.cashguo.top

PHP:  class Admin extends User {}
来源：http://uco.meibo888.top

JS:   class Admin extends User {}
来源：http://xyr.cqqwz.cn

TS:   class Admin extends User {}
来源：http://bdj.sysykeji.top

Java: class Admin extends User {}
来源：http://djc.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cqb.xylfe.cn

Ruby: class Admin < User; end
来源：http://cxu.jyoumei.cn

C#:   class Admin : User {}
来源：http://owk.uphjek.com

[G06] 重写方法
来源：http://mrs.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://vfe.yfazqb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://mzs.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://tis.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://yku.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://acx.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bqy.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://cue.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://cqh.aibaodan.cn

[G07] 调用父类方法
来源：http://fue.zhoulong.xyz

Py:   super().greet()
来源：http://mec.smart0.xyz

PHP:  parent::greet();
来源：http://wph.mhx1999.top

JS:   super.greet();
来源：http://wyy.feifeiyinyue.top

TS:   super.greet();
来源：http://new.316326.xyz

Java: super.greet();
来源：http://zvd.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mbp.hnxiangtu.top

Ruby: super
来源：http://kdw.xziqi.cn

C#:   base.Greet();
来源：http://npc.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://kwr.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hur.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://lhr.shuidangran.top

JS:   static f() {}
来源：http://yff.ctjpmb.com

TS:   static f(): void {}
来源：http://gil.guannengcc.top

Java: static void f() {}
来源：http://dkg.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zdq.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://nzp.mhx1999.top

C#:   public static void F() {}
来源：http://xel.andypj.xyz

[G09] 接口 / 抽象类
来源：http://lea.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://mfi.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ots.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vqz.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://qsq.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://ivi.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://knr.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qyk.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://nvp.bjfxy.top

[G10] 访问控制
来源：http://ghe.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://wkc.chenlongwang.top

PHP:  public / protected / private
来源：http://fgt.bjfxy.top

JS:   #private 字段；其余公开
来源：http://cpd.c1oappe.top

TS:   public / protected / private
来源：http://bpq.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://kzm.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kyh.yanxiufei.cn

Ruby: public / protected / private
来源：http://pzo.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://uej.xylfe.cn

[G11] getter / setter
来源：http://cfu.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://vlp.zhongyouzk.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tvm.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://jpo.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://qob.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://rup.smart0.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fwt.smart0.xyz

Ruby: attr_accessor :name
来源：http://pxp.zycfv.cn

C#:   public string Name { get; set; }
来源：http://ngn.ehwqpu.com

[G12] 对象转字符串
来源：http://hve.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://dqz.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zoa.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://pzw.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://ufh.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://cjy.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wvj.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://eyv.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://pyy.yonumen.top

[G13] 判断对象类型
来源：http://xsy.daria6918.cn

Py:   isinstance(u, User)
来源：http://vsd.bjfxy.top

PHP:  $u instanceof User
来源：http://eri.andypj.xyz

JS:   u instanceof User
来源：http://rwy.feifeiyinyue.top

TS:   u instanceof User
来源：http://gct.jinqigfzy.top

Java: u instanceof User
来源：http://ctd.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mir.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://wvp.hnqzz.top

C#:   u is User
来源：http://nms.zdqjudy.top

[G14] 数据类 / record
来源：http://ogb.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bdz.yfazqb.com

PHP:  // 用 readonly 属性模拟
来源：http://pud.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://fla.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://aas.chenlongwang.top

Java: record User(String name, int age) {}
来源：http://svv.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://xlz.xuanzx.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ruq.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://vwa.gotoacloud.top

[G15] 枚举
来源：http://dov.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ykb.gzhubu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gjh.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xdw.smart0.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qev.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://ggf.0kj1m.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ufm.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://rqn.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://muf.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://ykw.shzxlz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wna.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://duc.hnqzz.top

JS:   Object.entries(obj)
来源：http://bgf.zhixingplan.top

TS:   Object.entries(obj)
来源：http://cno.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qec.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wmi.cashguo.top

Ruby: obj.instance_variables
来源：http://iov.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://ryk.shzxlz.cn

================================================================================
来源：http://fck.cheryme.top

H. 异常与错误处理
来源：http://hke.yongpay.top

================================================================================
来源：http://weo.yonumen.top

[H01] try / catch 基础
来源：http://xpu.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dsr.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uzr.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nol.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yok.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lwa.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kvb.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vci.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dze.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://grx.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://tsc.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uys.hongshengwenyu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cab.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://esg.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oyk.zhiwuduotai.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ofv.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gug.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qdf.chenlongwang.top

[H03] 主动抛出异常
来源：http://upk.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://uzf.cucudq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ust.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://igj.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://mzl.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://vxc.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ana.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kuh.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vmn.ydjk.org.cn

[H04] 自定义异常类型
来源：http://ije.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://zpb.zhijiandao.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hby.vehdjk.com

JS:   class MyError extends Error {}
来源：http://mep.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://bec.redwolf501.top

Java: class MyException extends RuntimeException {}
来源：http://gqo.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://arj.yueranfly.top

Ruby: class MyError < StandardError; end
来源：http://xkj.uphjek.com

C#:   class MyException : Exception {}
来源：http://uhm.hammf.cn

[H05] 捕获特定类型
来源：http://ikx.nanxuanxn.top

Py:   except ValueError as e:
来源：http://kyy.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cbl.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://tol.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://drz.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://hek.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ffh.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://zex.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://usk.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://cez.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://lvk.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://ato.tarul.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sjy.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lvf.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tom.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://qor.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://alk.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://miv.zhengqikj.top

[H07] 断言
来源：http://scb.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://tlc.cqqwz.cn

PHP:  assert($x > 0);
来源：http://ail.yj20258888.top

JS:   console.assert(x > 0);
来源：http://pjg.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://alq.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://wxh.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pis.jqgufenzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://rep.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://ypo.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://usl.fanxiaobao.xyz

Py:   str(e);  traceback.format_exc()
来源：http://ail.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ljj.chenlongwang.top

JS:   e.message;  e.stack
来源：http://pto.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uso.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uga.wangdashe.top

Go:   err.Error()
来源：http://pfc.guowangkeji.top

Ruby: e.message;  e.backtrace
来源：http://ixe.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://qfh.ybcxt.top

[H09] 带错误码的异常
来源：http://xiw.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://txd.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jsz.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ebg.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dlt.xylfe.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ojo.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oot.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://xyt.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://joj.snrcjt.cn

[H10] 资源自动释放
来源：http://glo.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cju.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tab.chenzaomai.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ziu.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sro.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iev.tanke756.top

Go:   defer f.Close()
来源：http://alo.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://utd.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rlb.jqgfzy.top

================================================================================
来源：http://myu.zhoulong.xyz

I. 正则表达式
来源：http://ljn.cucudq.cn

================================================================================
来源：http://kwq.gzhubu.top

[I01] 判断是否匹配
来源：http://zch.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vbm.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bzq.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://wks.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://crp.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mrv.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://use.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://gbb.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qrl.tianlin.xyz

[I02] 提取所有匹配
来源：http://pje.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://fbo.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dig.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hnd.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://kru.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fiu.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://byt.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://zub.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://anv.hnxiangtu.top

[I03] 提取捕获分组
来源：http://tsx.vqdsnc.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ree.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fwi.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ppl.yfazqb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wuv.zhiwuduotai.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kjh.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ohl.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nxp.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tng.ydzc1.top

[I04] 正则替换
来源：http://tux.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://edp.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rkk.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dtf.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://edg.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kty.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hwk.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ybp.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kao.zhoulong.xyz

[I05] 按正则拆分
来源：http://tcs.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fia.nanxuanxn.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mwu.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://xvl.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://mas.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://dya.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jba.zycfv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yex.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://okz.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fvu.cdnleiting.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xbp.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bbe.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gtj.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxn.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ain.cucudq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vtu.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://enf.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://par.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://aud.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qls.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ktx.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wtb.cheryme.top

TS:   /error/gim
来源：http://rjl.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ucp.hcnkem.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mdp.jinqigfzy.top


<!-- 参考信息 -->