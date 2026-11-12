代发 wailian999

Py:   class User: pass
来源：http://hpn.jqgfzy.top

PHP:  class User {}
来源：http://rnn.snrcjt.cn

JS:   class User {}
来源：http://dfa.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://wtf.hnqzz.top

Java: class User {}
来源：http://rfo.jyoumei.cn

Go:   type User struct { Name string }
来源：http://gbm.shanyushiyangtech.top

Ruby: class User; end
来源：http://gmz.nanxuanxn.top

C#:   class User {}
来源：http://ind.kuanghao11.cn

[G02] 构造函数
来源：http://rfs.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://xdp.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oei.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://mlh.feifeiyinyue.top

TS:   constructor(public name: string) {}
来源：http://vzb.sweek.top

Java: User(String name) { this.name = name; }
来源：http://kwd.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ghy.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://owj.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://fhu.jinyuanbaomall.cn

[G03] 实例属性
来源：http://myi.hnqzz.top

Py:   self.name = "x"
来源：http://hhc.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://hcm.fktsv.cn

JS:   this.name = "x";
来源：http://kpn.cashguo.top

TS:   name: string = "x";
来源：http://wsh.jyoumei.cn

Java: private String name;
来源：http://jcj.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ddb.kuanghao11.cn

Ruby: @name = "x"
来源：http://raj.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://kcc.jianghu66.top

[G04] 定义方法
来源：http://fhg.yongpay.top

Py:   def greet(self): return self.name
来源：http://sqi.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aer.52xcode.cn

JS:   greet() { return this.name; }
来源：http://fcm.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://gcn.shuidangran.top

Java: String greet() { return name; }
来源：http://xrk.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vgk.fzhhl.top

Ruby: def greet; @name; end
来源：http://kiw.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://ear.zhiwuduotai.top

[G05] 继承
来源：http://xad.ivvv.top

Py:   class Admin(User): pass
来源：http://eyw.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://bzb.svipenyu.cn

JS:   class Admin extends User {}
来源：http://xld.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://him.yuxming.cn

Java: class Admin extends User {}
来源：http://wnd.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eda.daria6918.cn

Ruby: class Admin < User; end
来源：http://kja.fehbvm.com

C#:   class Admin : User {}
来源：http://zhs.tanke756.top

[G06] 重写方法
来源：http://znt.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://eup.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qak.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://aoy.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://mnc.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://phh.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gdj.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://fbs.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://msf.yuanzhike.top

[G07] 调用父类方法
来源：http://mur.xuetiantiany.cn

Py:   super().greet()
来源：http://uuw.xingfuxueyuan.xyz

PHP:  parent::greet();
来源：http://eml.birdmap.top

JS:   super.greet();
来源：http://gan.haohaochexian.top

TS:   super.greet();
来源：http://gdd.ywan-chungtsiang.top

Java: super.greet();
来源：http://iil.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ulp.yuxming.cn

Ruby: super
来源：http://gxi.zhixingplan.top

C#:   base.Greet();
来源：http://uph.bjfxy.top

[G08] 静态方法与属性
来源：http://lnz.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bdl.cucudq.cn

PHP:  public static function f() {}
来源：http://ufy.tarul.cn

JS:   static f() {}
来源：http://wzd.tian-w.cn

TS:   static f(): void {}
来源：http://coh.cucudq.cn

Java: static void f() {}
来源：http://zgo.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nfw.jinqigufen.top

Ruby: def self.f; end
来源：http://yki.0kj1m.cn

C#:   public static void F() {}
来源：http://rqg.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://wbe.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://yke.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cup.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ytu.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://egl.tarul.cn

Java: interface Shape { double area(); }
来源：http://mvg.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://aby.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lft.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://oil.tarul.cn

[G10] 访问控制
来源：http://yqq.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://hrc.wangdashe.top

PHP:  public / protected / private
来源：http://cxl.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://qfm.feifeiyinyue.top

TS:   public / protected / private
来源：http://rkd.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://yqg.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xgl.yonumen.top

Ruby: public / protected / private
来源：http://xbv.hfpthk.cn

C#:   public / protected / private / internal
来源：http://eqx.shangyingyoupin.top

[G11] getter / setter
来源：http://uwh.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://boa.wangdashe.top

PHP:  public function getName(): string { return $this->name; }
来源：http://paf.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://zxc.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://zxy.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://vpl.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://apo.9152youxi.cn

Ruby: attr_accessor :name
来源：http://qwm.daxiang520.top

C#:   public string Name { get; set; }
来源：http://cml.guowangkeji.top

[G12] 对象转字符串
来源：http://qqn.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://dji.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://auz.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://ydp.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://jmi.guowangkeji.top

Java: @Override public String toString() { return name; }
来源：http://odu.zhengqikj.top

Go:   func (u User) String() string { return u.Name }
来源：http://cnb.zhaomingkeji.xyz

Ruby: def to_s; @name; end
来源：http://ech.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://grt.nwbrower.top

[G13] 判断对象类型
来源：http://dbe.yj20258.top

Py:   isinstance(u, User)
来源：http://fhl.ppjwa.cn

PHP:  $u instanceof User
来源：http://rar.cheryme.top

JS:   u instanceof User
来源：http://prk.aibaodan.cn

TS:   u instanceof User
来源：http://rny.jinqigfzy.top

Java: u instanceof User
来源：http://wtz.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vko.ydzc1.top

Ruby: u.is_a?(User)
来源：http://nek.jlsjyb.cn

C#:   u is User
来源：http://mcw.redwolf501.top

[G14] 数据类 / record
来源：http://qdl.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cbf.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://rgq.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xbi.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://dki.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://hcb.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://ncn.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yzv.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://xim.gotoacloud.top

[G15] 枚举
来源：http://feq.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wae.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nme.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ssl.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sin.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://bqa.hammf.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://afm.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://rcn.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tza.andypj.xyz

[G16] 对象转数组 / 字典
来源：http://etz.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hvu.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://exd.cqqwz.cn

JS:   Object.entries(obj)
来源：http://dha.yj202588.top

TS:   Object.entries(obj)
来源：http://qma.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zvz.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ucr.fengsongda.top

Ruby: obj.instance_variables
来源：http://llo.fengsongda.top

C#:   // 用反射或 System.Text.Json
来源：http://fzi.bjfxy.top

================================================================================
来源：http://mlg.zhongyouzk.top

H. 异常与错误处理
来源：http://cvv.yueranfly.top

================================================================================
来源：http://qmf.yuanzhike.top

[H01] try / catch 基础
来源：http://dat.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ulv.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pej.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cdn.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dzz.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mgk.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ntz.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mbp.andypj.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dze.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://sos.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://auk.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ggc.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wzm.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yfw.zhaomingkeji.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://qug.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://feh.jinqigfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sac.chenzaomai.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://qag.ydjk.org.cn

[H03] 主动抛出异常
来源：http://cdp.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://def.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nhi.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://hmc.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://adx.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sym.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cpp.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://olu.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://vtc.jqgfzy.top

[H04] 自定义异常类型
来源：http://cej.pengpengdd.cyou

Py:   class MyError(Exception): pass
来源：http://swn.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://kyc.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://ala.nwbrower.top

TS:   class MyError extends Error {}
来源：http://evk.vehdjk.com

Java: class MyException extends RuntimeException {}
来源：http://opj.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cjj.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://pmo.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://bod.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://msw.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://mvz.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqb.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://mpi.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://uuf.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://hgq.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://elw.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://cfc.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xlf.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://lxj.yj20258888.top

Py:   value = d.get("k") or default
来源：http://smj.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://jtw.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://upq.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://etu.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tvm.pengpengdd.cyou

Go:   if v, ok := m["k"]; ok { }
来源：http://cke.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://inn.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://vyu.gogol.net.cn

[H07] 断言
来源：http://efv.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://oxz.yj20258888.top

PHP:  assert($x > 0);
来源：http://qwk.yj202588.top

JS:   console.assert(x > 0);
来源：http://tbr.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://bus.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://mxy.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://poa.bbcook.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xon.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://qlo.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://udu.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://pno.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xjo.yongpay.top

JS:   e.message;  e.stack
来源：http://yvc.sufxvd.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sge.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://hvk.hammf.cn

Go:   err.Error()
来源：http://qem.smart0.xyz

Ruby: e.message;  e.backtrace
来源：http://quw.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://hbl.nanxuanxn.top

[H09] 带错误码的异常
来源：http://mta.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yei.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xbd.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://alo.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://azk.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tuw.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://urk.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://pst.jlsjyb.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://shz.bjfxy.top

[H10] 资源自动释放
来源：http://qpx.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dyw.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nml.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lnf.shzxlz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qrm.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dbd.gzhubu.top

Go:   defer f.Close()
来源：http://yri.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://coc.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://znm.jinyuanbaomall.cn

================================================================================
来源：http://pkk.vqdsnc.cn

I. 正则表达式
来源：http://ofb.zdqjudy.top

================================================================================
来源：http://jdo.hnqzz.top

[I01] 判断是否匹配
来源：http://mtl.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vhy.xylfe.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gcs.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://ybp.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://ehi.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mks.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://utv.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://sjm.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mjs.yfazqb.com

[I02] 提取所有匹配
来源：http://hui.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://gxj.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rgo.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kxf.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://qqg.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fjf.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mwg.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://wxf.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdd.pengpengdd.cyou

[I03] 提取捕获分组
来源：http://wxg.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nxw.kuanghao11.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vik.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vud.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dgh.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oup.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kal.jiagoushi.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ctz.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://luy.zhixingplan.top

[I04] 正则替换
来源：http://ctv.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sob.ydjk.org.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zdv.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://byq.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://gpr.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://mos.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dem.sweek.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cpr.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rfo.nanxuanxn.top

[I05] 按正则拆分
来源：http://jvn.chenjidiqi.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://hwo.cdnleiting.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://czh.andypj.xyz

JS:   s.split(/\s*,\s*/)
来源：http://hcg.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://pqk.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://xrk.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tvc.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://gka.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://njo.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://byj.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fil.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aca.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jnx.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://arr.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://utq.ydzc1.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wgz.hnqzz.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xem.aizwys.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oxw.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://qdc.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ubu.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjw.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oso.ywan-chungtsiang.top

TS:   /error/gim
来源：http://sbb.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jai.tian-w.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dpg.vqdsnc.cn


<!-- 参考信息 -->