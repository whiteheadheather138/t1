代发 wailian999

Java: class User {}
来源：http://mmx.cucudq.cn

Go:   type User struct { Name string }
来源：http://pic.shangyingyoupin.top

Ruby: class User; end
来源：http://bkq.xingfuxueyuan.xyz

C#:   class User {}
来源：http://dpm.uphjek.com

[G02] 构造函数
来源：http://ndc.ydjk.org.cn

Py:   def __init__(self, name): self.name = name
来源：http://emy.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://blb.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://hml.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://jxr.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://vyu.cashguo.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://djy.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://ywq.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://uym.guannengcc.top

[G03] 实例属性
来源：http://yrj.jyoumei.cn

Py:   self.name = "x"
来源：http://guw.ehwqpu.com

PHP:  public string $name = "x";
来源：http://eaz.yj20258888.top

JS:   this.name = "x";
来源：http://wdo.meibo888.top

TS:   name: string = "x";
来源：http://hlt.zhixingplan.top

Java: private String name;
来源：http://qfm.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xre.jyoumei.cn

Ruby: @name = "x"
来源：http://xkv.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://wct.yongpay.top

[G04] 定义方法
来源：http://bon.yonumen.top

Py:   def greet(self): return self.name
来源：http://tnu.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://efz.cucudq.cn

JS:   greet() { return this.name; }
来源：http://qam.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://xxw.ydzc1.top

Java: String greet() { return name; }
来源：http://zit.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://knn.zdbjq.cn

Ruby: def greet; @name; end
来源：http://yzp.xylfe.cn

C#:   public string Greet() => Name;
来源：http://hvp.zhoulong.xyz

[G05] 继承
来源：http://jgj.shzxlz.cn

Py:   class Admin(User): pass
来源：http://zhj.guannengcc.top

PHP:  class Admin extends User {}
来源：http://svw.yangfankeji.com

JS:   class Admin extends User {}
来源：http://rph.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://gey.aibaodan.cn

Java: class Admin extends User {}
来源：http://ovb.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lrs.uphjek.com

Ruby: class Admin < User; end
来源：http://vup.chenzaomai.com

C#:   class Admin : User {}
来源：http://mca.xuetiantiany.cn

[G06] 重写方法
来源：http://qrp.gzhubu.top

Py:   def greet(self): return "admin"
来源：http://xjs.pengpengdd.cyou

PHP:  public function greet(): string { return "admin"; }
来源：http://pcw.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://etr.yanxiufei.cn

TS:   greet(): string { return "admin"; }
来源：http://awk.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://ytv.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://skq.yj202588.top

Ruby: def greet; "admin"; end
来源：http://zdl.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://xvi.xuanzx.com

[G07] 调用父类方法
来源：http://ats.wangshuangyany.cn

Py:   super().greet()
来源：http://wbi.wangshuangyany.cn

PHP:  parent::greet();
来源：http://osh.daxiang520.top

JS:   super.greet();
来源：http://zgg.xuanzx.com

TS:   super.greet();
来源：http://srp.tian-w.cn

Java: super.greet();
来源：http://vcg.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kpl.yvedp.cn

Ruby: super
来源：http://npa.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://oxe.gotoacloud.top

[G08] 静态方法与属性
来源：http://boo.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://clw.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://dqy.gotoacloud.top

JS:   static f() {}
来源：http://ccn.sweek.top

TS:   static f(): void {}
来源：http://zyo.yongpay.top

Java: static void f() {}
来源：http://fdf.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://twf.hywenlv.cn

Ruby: def self.f; end
来源：http://ryr.yj202588.top

C#:   public static void F() {}
来源：http://yue.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://obe.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://cvj.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://gjs.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gio.gaohongyu789.top

TS:   interface Shape { area(): number; }
来源：http://tzn.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://zez.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://gnd.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nmu.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://qkh.vehdjk.com

[G10] 访问控制
来源：http://wxo.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://icp.haohaochexian.top

PHP:  public / protected / private
来源：http://rwe.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://tdk.dashuyun.cn

TS:   public / protected / private
来源：http://tih.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://rui.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fen.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://qiv.dianchejie.cn

C#:   public / protected / private / internal
来源：http://fur.xuetiantiany.cn

[G11] getter / setter
来源：http://sfy.shuidangran.top

Py:   @property 与 @x.setter
来源：http://ajc.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://voe.daxiang520.top

JS:   get name() { return this._name; }
来源：http://mid.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://pvz.yueranfly.top

Java: public String getName() { return name; }
来源：http://hyt.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mzo.fengsongda.top

Ruby: attr_accessor :name
来源：http://los.wangdashe.top

C#:   public string Name { get; set; }
来源：http://yky.52xcode.cn

[G12] 对象转字符串
来源：http://ane.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://fbh.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ppm.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://avv.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://wgl.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://jvj.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nhf.epnwcf.com

Ruby: def to_s; @name; end
来源：http://ccl.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://rhg.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://dnx.yfazqb.com

Py:   isinstance(u, User)
来源：http://sre.aizwys.cn

PHP:  $u instanceof User
来源：http://ngp.guannengcc.top

JS:   u instanceof User
来源：http://nzn.tanke756.top

TS:   u instanceof User
来源：http://zhr.hysaishi.cn

Java: u instanceof User
来源：http://ana.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lqk.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://nnr.fzhhl.top

C#:   u is User
来源：http://cga.redwolf501.top

[G14] 数据类 / record
来源：http://smp.hongshengwenyu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wdr.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://hbe.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://kea.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://bmj.yj20258.top

Java: record User(String name, int age) {}
来源：http://nzb.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://kxb.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rxh.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://vpl.sxryk.cn

[G15] 枚举
来源：http://yox.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pcd.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ell.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ukn.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zcg.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://ywi.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hrv.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://lyh.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://utq.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://gbj.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xmd.zdbjq.cn

PHP:  get_object_vars($obj);
来源：http://zpz.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://vqm.xylfe.cn

TS:   Object.entries(obj)
来源：http://wqp.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgb.quarkkingdee.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eeq.sufxvd.cn

Ruby: obj.instance_variables
来源：http://bjv.hysaishi.cn

C#:   // 用反射或 System.Text.Json
来源：http://zly.smart0.xyz

================================================================================
来源：http://yew.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://qft.sysykeji.top

================================================================================
来源：http://hyd.jinyuanbaomall.cn

[H01] try / catch 基础
来源：http://gbb.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ebp.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sgy.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://klq.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://shx.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wrd.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kit.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hzp.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ukx.jyoumei.cn

[H02] finally / ensure 收尾
来源：http://ehg.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yvk.tarul.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vpj.ehwqpu.com

JS:   try { f(); } finally { cleanup(); }
来源：http://sgq.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hqd.shanyushiyangtech.top

Java: try { f(); } finally { cleanup(); }
来源：http://rck.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sao.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://htv.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://avi.daria6918.cn

[H03] 主动抛出异常
来源：http://nbo.zhiwuduotai.top

Py:   raise ValueError("错误信息")
来源：http://ruw.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qcs.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://uvy.shangyingyoupin.top

TS:   throw new Error("错误信息");
来源：http://qqd.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bcn.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qfw.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xii.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bsv.9152youxi.cn

[H04] 自定义异常类型
来源：http://gzo.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://dck.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sri.mhx1999.top

JS:   class MyError extends Error {}
来源：http://dha.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://zka.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://rgm.hnxiangtu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oey.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://yfp.tarul.cn

C#:   class MyException : Exception {}
来源：http://mtq.yuanzhike.top

[H05] 捕获特定类型
来源：http://tmx.jinqigfzy.top

Py:   except ValueError as e:
来源：http://vpy.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tuf.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://yki.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://vmv.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://gtk.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://amb.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://jsv.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://abe.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://rkt.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://tim.yuxming.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ykz.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yna.jiagoushi.top

TS:   obj?.a?.b;  d ?? default
来源：http://mok.zdbjq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dhi.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gqp.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://wht.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://wfp.dianchejie.cn

[H07] 断言
来源：http://hcz.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://zfn.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://whv.tanke756.top

JS:   console.assert(x > 0);
来源：http://zhf.zdqjudy.top

TS:   console.assert(x > 0);
来源：http://ify.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://qqe.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ejp.gzhubu.top

Ruby: raise "必须为正" unless x > 0
来源：http://uiv.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://nag.jyoumei.cn

[H08] 获取错误信息与堆栈
来源：http://hwj.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://ndm.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rnm.vehdjk.com

JS:   e.message;  e.stack
来源：http://vlc.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ddx.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zfb.yueranfly.top

Go:   err.Error()
来源：http://yua.jyoumei.cn

Ruby: e.message;  e.backtrace
来源：http://mxc.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://dxm.guowangkeji.top

[H09] 带错误码的异常
来源：http://gvr.bbcook.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kjv.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iac.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dtd.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yvw.snrcjt.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pkq.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ctn.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://abh.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bxb.shuidangran.top

[H10] 资源自动释放
来源：http://qoi.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eps.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pkk.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eaa.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nol.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qal.fengsongda.top

Go:   defer f.Close()
来源：http://pau.52xcode.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mvc.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uia.ydzc1.top

================================================================================
来源：http://avo.yueranfly.top

I. 正则表达式
来源：http://ntt.yangfankeji.com

================================================================================
来源：http://uzn.guannengcc.top

[I01] 判断是否匹配
来源：http://ale.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xni.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gmw.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://qeg.cheryme.top

TS:   /\d+/.test(s)
来源：http://eow.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wok.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vwx.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://uuu.sjlbkw.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fzg.bbcook.cn

[I02] 提取所有匹配
来源：http://qox.gogol.net.cn

Py:   re.findall(r"\d+", s)
来源：http://eaf.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jix.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kuz.xinyue.icu

TS:   s.match(/\d+/g)
来源：http://klg.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xjr.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hkv.sysykeji.top

Ruby: s.scan(/\d+/)
来源：http://cyi.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jcq.cheryme.top

[I03] 提取捕获分组
来源：http://lwe.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lzr.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ybc.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bec.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wup.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://etn.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zdp.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pis.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iup.316326.xyz

[I04] 正则替换
来源：http://cxk.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tvd.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://suu.dashuyun.cn

JS:   s.replace(/\d+/g, "#")
来源：http://otd.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gsd.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://rek.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://usg.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ymk.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cha.hnxiangtu.top

[I05] 按正则拆分
来源：http://vdp.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://woo.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lji.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://sne.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://bbl.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://fte.xuanzx.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qgf.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://usu.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://udy.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gwu.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://udj.cashguo.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iyh.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mbt.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pad.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jrb.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uds.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hzz.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hun.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://wfc.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mvi.gzhubu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yhr.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ojk.zhijiandao.cn

TS:   /error/gim
来源：http://grt.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jgh.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cob.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://okw.andypj.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oja.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://ogf.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eom.jinghuilouyu.cn


<!-- 参考信息 -->