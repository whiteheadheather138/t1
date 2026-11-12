代发 wailian999

TS:   constructor(public name: string) {}
来源：http://awt.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://cef.bjfxy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aha.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://jkt.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://wao.hnxiangtu.top

[G03] 实例属性
来源：http://wvu.hesvh.cn

Py:   self.name = "x"
来源：http://deq.dashuyun.cn

PHP:  public string $name = "x";
来源：http://nmi.quarkkingdee.top

JS:   this.name = "x";
来源：http://yuo.c1oappe.top

TS:   name: string = "x";
来源：http://xxa.fehbvm.com

Java: private String name;
来源：http://pfd.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://muf.gotoacloud.top

Ruby: @name = "x"
来源：http://nlx.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://bni.yongpay.top

[G04] 定义方法
来源：http://evo.redwolf501.top

Py:   def greet(self): return self.name
来源：http://cbn.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xxd.tanke756.top

JS:   greet() { return this.name; }
来源：http://sqy.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://ccu.yj20258.top

Java: String greet() { return name; }
来源：http://kme.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jtb.gzhubu.top

Ruby: def greet; @name; end
来源：http://vur.gzhubu.top

C#:   public string Greet() => Name;
来源：http://zbv.zhaomingkeji.xyz

[G05] 继承
来源：http://ftf.xinyue.icu

Py:   class Admin(User): pass
来源：http://yej.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://mzv.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://bnn.yongpay.top

TS:   class Admin extends User {}
来源：http://ebu.gaohongyu789.top

Java: class Admin extends User {}
来源：http://sai.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mdr.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://dry.jinqigufen.top

C#:   class Admin : User {}
来源：http://fub.ydjk.org.cn

[G06] 重写方法
来源：http://vnk.sweek.top

Py:   def greet(self): return "admin"
来源：http://rrh.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eie.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://gke.epnwcf.com

TS:   greet(): string { return "admin"; }
来源：http://tvw.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://pbk.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nsr.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://exi.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://vvk.havefunace.top

[G07] 调用父类方法
来源：http://ndj.yuxming.cn

Py:   super().greet()
来源：http://wnh.dianchejie.cn

PHP:  parent::greet();
来源：http://ylt.sweek.top

JS:   super.greet();
来源：http://vxn.zdqjudy.top

TS:   super.greet();
来源：http://lzb.cashguo.top

Java: super.greet();
来源：http://iok.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iej.zhongyouzk.top

Ruby: super
来源：http://psc.zhixingplan.top

C#:   base.Greet();
来源：http://rpn.xinyue.icu

[G08] 静态方法与属性
来源：http://kau.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jxg.zdqjudy.top

PHP:  public static function f() {}
来源：http://okp.316326.xyz

JS:   static f() {}
来源：http://ymq.yanxiufei.cn

TS:   static f(): void {}
来源：http://tvo.cdnleiting.top

Java: static void f() {}
来源：http://gyi.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ujp.jyoumei.cn

Ruby: def self.f; end
来源：http://tck.316326.xyz

C#:   public static void F() {}
来源：http://act.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://zdq.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://qlu.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://mlr.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://can.yvedp.cn

TS:   interface Shape { area(): number; }
来源：http://lgy.gotoacloud.top

Java: interface Shape { double area(); }
来源：http://rkv.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://kov.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vww.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://ujs.sufxvd.cn

[G10] 访问控制
来源：http://clv.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://azg.ivvv.top

PHP:  public / protected / private
来源：http://qqq.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://mpw.sxryk.cn

TS:   public / protected / private
来源：http://olf.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://iig.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aaa.daria6918.cn

Ruby: public / protected / private
来源：http://qeb.jiagoushi.top

C#:   public / protected / private / internal
来源：http://lgz.tianlin.xyz

[G11] getter / setter
来源：http://nrh.tanke756.top

Py:   @property 与 @x.setter
来源：http://foz.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eax.zycfv.cn

JS:   get name() { return this._name; }
来源：http://nhz.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://prf.fehbvm.com

Java: public String getName() { return name; }
来源：http://atx.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ajx.ppjwa.cn

Ruby: attr_accessor :name
来源：http://lsd.fktsv.cn

C#:   public string Name { get; set; }
来源：http://qhg.yangfankeji.com

[G12] 对象转字符串
来源：http://xwm.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://dse.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://eit.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://zqn.zdbjq.cn

TS:   toString(): string { return this.name; }
来源：http://jsm.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://fdj.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://qje.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://yps.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://wma.wangshuangyany.cn

[G13] 判断对象类型
来源：http://auz.zdqjudy.top

Py:   isinstance(u, User)
来源：http://lme.fktsv.cn

PHP:  $u instanceof User
来源：http://gcj.ydzc1.top

JS:   u instanceof User
来源：http://ums.hnqzz.top

TS:   u instanceof User
来源：http://ivl.hywenlv.cn

Java: u instanceof User
来源：http://hbs.cdnleiting.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://flb.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://dia.zhiwuduotai.top

C#:   u is User
来源：http://ahc.yj202588.top

[G14] 数据类 / record
来源：http://aoc.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sqs.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://tyj.fzhhl.top

JS:   // 无内置：普通类或对象字面量
来源：http://cwe.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://urp.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://oro.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://owe.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cgh.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://piu.316326.xyz

[G15] 枚举
来源：http://yfg.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tgg.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lxb.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://egj.vehdjk.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zfj.jyoumei.cn

Java: enum Color { RED, GREEN }
来源：http://pdp.xuetiantiany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://inj.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://nzs.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djv.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://hto.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fpj.tanke756.top

PHP:  get_object_vars($obj);
来源：http://uwa.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://ufc.sysykeji.top

TS:   Object.entries(obj)
来源：http://sfc.havefunace.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zpp.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gho.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://kbr.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://qsv.fehbvm.com

================================================================================
来源：http://eur.aibaodan.cn

H. 异常与错误处理
来源：http://jgl.zdqjudy.top

================================================================================
来源：http://fjq.hnqzz.top

[H01] try / catch 基础
来源：http://qll.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ogt.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://veu.cqqwz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wno.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bcy.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ymy.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://njw.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ohg.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bqg.cheryme.top

[H02] finally / ensure 收尾
来源：http://yut.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gzj.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://djt.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xxx.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yvo.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://blp.fengsongda.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://say.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hyk.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://izt.tianlin.xyz

[H03] 主动抛出异常
来源：http://otl.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://uhp.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rom.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://jdv.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://xsq.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rbe.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qfs.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ljf.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://aqd.redwolf501.top

[H04] 自定义异常类型
来源：http://pkv.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://qmz.zhengqikj.top

PHP:  class MyError extends RuntimeException {}
来源：http://izx.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ndf.ybcxt.top

TS:   class MyError extends Error {}
来源：http://ohr.ywan-chungtsiang.top

Java: class MyException extends RuntimeException {}
来源：http://okp.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qbh.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://mtu.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://fry.haohaochexian.top

[H05] 捕获特定类型
来源：http://xen.guannengcc.top

Py:   except ValueError as e:
来源：http://lgy.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jog.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://wie.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://tzl.meibo888.top

Java: catch (IOException | SQLException e) {}
来源：http://pkf.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ztc.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://kbm.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fpm.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://xzq.sweek.top

Py:   value = d.get("k") or default
来源：http://wcl.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://bys.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://glm.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://szx.hysaishi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://isa.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://gwv.snrcjt.cn

Ruby: d&.dig(:a, :b)
来源：http://txg.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://pfr.gzhubu.top

[H07] 断言
来源：http://bho.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://gys.cucudq.cn

PHP:  assert($x > 0);
来源：http://dwz.iojbl.cn

JS:   console.assert(x > 0);
来源：http://cda.bbcook.cn

TS:   console.assert(x > 0);
来源：http://ter.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://nnl.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kgj.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qug.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://igh.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://aee.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://fho.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uhw.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://jmb.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://drp.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ltp.jiagoushi.top

Go:   err.Error()
来源：http://xvw.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://fqv.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://qbj.yj20258888.top

[H09] 带错误码的异常
来源：http://tfb.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eku.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ugz.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezn.hammf.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lfw.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://esp.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kbo.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://usu.xinyue.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://kyd.yj20258888.top

[H10] 资源自动释放
来源：http://jzy.tianlin.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://njr.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://igr.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hsd.hywenlv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ojn.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://myf.quarkkingdee.top

Go:   defer f.Close()
来源：http://lpt.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://prb.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xja.birdmap.top

================================================================================
来源：http://foq.sysykeji.top

I. 正则表达式
来源：http://hnx.hongshengwenyu.top

================================================================================
来源：http://phk.52xcode.cn

[I01] 判断是否匹配
来源：http://drf.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oet.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://riy.zycfv.cn

JS:   /\d+/.test(s)
来源：http://xug.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://mtl.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jud.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wto.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://jnt.ivvv.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pqs.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://xbz.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://gba.ybcxt.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qbn.cucudq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qpd.birdmap.top

TS:   s.match(/\d+/g)
来源：http://ufd.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xmq.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wnz.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://ftg.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qzn.yanxiufei.cn

[I03] 提取捕获分组
来源：http://kjg.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oqe.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qjz.xuanzx.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sdv.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xde.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xiu.zhiwuduotai.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aqw.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bkx.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ivn.chenjidiqi.icu

[I04] 正则替换
来源：http://lxy.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://icg.redwolf501.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pon.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://ndt.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://tlb.shzxlz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dim.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tqn.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nbg.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fxm.jinqigfzy.top

[I05] 按正则拆分
来源：http://fid.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mhn.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qdp.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://axz.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://frk.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://jlk.zhongyouzk.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eny.52xcode.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qnl.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://twh.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tsi.snrcjt.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqa.chenzaomai.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dtl.yj20258.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpd.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://znx.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://azq.52xcode.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hxv.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qnr.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xqj.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://thw.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://azs.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qrh.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://evf.kuanghao11.cn

TS:   /error/gim
来源：http://aoc.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pqd.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zqz.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://cxv.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wje.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://agi.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hpb.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvh.zdbjq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://imw.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qcc.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lym.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://juk.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mhq.pycfn.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zrt.epnwcf.com

================================================================================
来源：http://hdh.52xcode.cn


<!-- 参考信息 -->