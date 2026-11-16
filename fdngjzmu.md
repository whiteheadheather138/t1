代发 wailian999

Py:   class User: pass
来源：http://bjd.shzxlz.cn

PHP:  class User {}
来源：http://ndf.kuanghao11.cn

JS:   class User {}
来源：http://egg.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://bcw.zhengqikj.top

Java: class User {}
来源：http://isq.nwbrower.top

Go:   type User struct { Name string }
来源：http://clp.zhengqikj.top

Ruby: class User; end
来源：http://ysg.zdqjudy.top

C#:   class User {}
来源：http://dch.kuanghao11.cn

[G02] 构造函数
来源：http://pim.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://rqf.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://wds.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://hmf.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://umk.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://cax.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bya.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://hpn.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://mfn.yanxiufei.cn

[G03] 实例属性
来源：http://aco.fengsongda.top

Py:   self.name = "x"
来源：http://xvu.jqgufenzy.top

PHP:  public string $name = "x";
来源：http://lwg.xuetiantiany.cn

JS:   this.name = "x";
来源：http://uvv.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://asv.pycfn.com

Java: private String name;
来源：http://tiq.shanyushiyangtech.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vlv.jinyuanbaomall.cn

Ruby: @name = "x"
来源：http://bog.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://hrm.ydzc1.top

[G04] 定义方法
来源：http://dci.ydjk.org.cn

Py:   def greet(self): return self.name
来源：http://byl.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bkw.cheryme.top

JS:   greet() { return this.name; }
来源：http://zyk.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://skf.bjfxy.top

Java: String greet() { return name; }
来源：http://ttq.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qhy.zycfv.cn

Ruby: def greet; @name; end
来源：http://rzq.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://mjp.jinqigufen.top

[G05] 继承
来源：http://lyx.wangdashe.top

Py:   class Admin(User): pass
来源：http://ivd.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://qyz.hammf.cn

JS:   class Admin extends User {}
来源：http://uqo.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://emg.zhongyouzk.top

Java: class Admin extends User {}
来源：http://bpr.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ods.feifeiyinyue.top

Ruby: class Admin < User; end
来源：http://eyb.chenzaomai.com

C#:   class Admin : User {}
来源：http://jpj.shanyushiyangtech.top

[G06] 重写方法
来源：http://fso.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://gtk.fehbvm.com

PHP:  public function greet(): string { return "admin"; }
来源：http://jnh.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://cvb.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://pea.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ius.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://air.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://aps.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://kbr.zhiwuduotai.top

[G07] 调用父类方法
来源：http://ufj.snrcjt.cn

Py:   super().greet()
来源：http://nwf.hnqzz.top

PHP:  parent::greet();
来源：http://ydc.shanyushiyangkeji.top

JS:   super.greet();
来源：http://xhj.gotoacloud.top

TS:   super.greet();
来源：http://sgn.pycfn.com

Java: super.greet();
来源：http://vdr.fehbvm.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cho.0kj1m.cn

Ruby: super
来源：http://mxy.sjlbkw.cn

C#:   base.Greet();
来源：http://ppx.yonumen.top

[G08] 静态方法与属性
来源：http://kge.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgl.guannengcc.top

PHP:  public static function f() {}
来源：http://qkl.cucudq.cn

JS:   static f() {}
来源：http://fts.ydjk.org.cn

TS:   static f(): void {}
来源：http://nng.ctjpmb.com

Java: static void f() {}
来源：http://qer.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kpm.zhiwuduotai.top

Ruby: def self.f; end
来源：http://ldy.gotoacloud.top

C#:   public static void F() {}
来源：http://bku.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://wre.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://ixp.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://ohn.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://odo.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://ofz.gzhubu.top

Java: interface Shape { double area(); }
来源：http://jpv.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://vta.dashuyun.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ngq.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://lad.c1oappe.top

[G10] 访问控制
来源：http://jnw.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://uvo.yongpay.top

PHP:  public / protected / private
来源：http://fer.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://zwd.sjlbkw.cn

TS:   public / protected / private
来源：http://oen.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://fbx.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sdp.gaohongyu789.top

Ruby: public / protected / private
来源：http://yjb.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://erj.zycfv.cn

[G11] getter / setter
来源：http://efw.smart0.xyz

Py:   @property 与 @x.setter
来源：http://ygt.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gzm.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://pni.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://uyb.c1oappe.top

Java: public String getName() { return name; }
来源：http://tly.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://mok.gzhubu.top

Ruby: attr_accessor :name
来源：http://kur.52xcode.cn

C#:   public string Name { get; set; }
来源：http://yun.yongpay.top

[G12] 对象转字符串
来源：http://grd.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://bjb.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pmp.yj20258.top

JS:   toString() { return this.name; }
来源：http://fvd.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://tpj.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://fim.epnwcf.com

Go:   func (u User) String() string { return u.Name }
来源：http://ijy.tian-w.cn

Ruby: def to_s; @name; end
来源：http://bgz.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://ngc.iojbl.cn

[G13] 判断对象类型
来源：http://vds.sweek.top

Py:   isinstance(u, User)
来源：http://olg.aibaodan.cn

PHP:  $u instanceof User
来源：http://bjt.yfazqb.com

JS:   u instanceof User
来源：http://gpu.yvedp.cn

TS:   u instanceof User
来源：http://ipo.zhengqikj.top

Java: u instanceof User
来源：http://dpw.tian-w.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kja.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://lmi.andypj.xyz

C#:   u is User
来源：http://nna.tanke756.top

[G14] 数据类 / record
来源：http://fph.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qlb.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://oae.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://djh.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://ori.jyoumei.cn

Java: record User(String name, int age) {}
来源：http://wnn.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://ezi.chenlongwang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zya.havefunace.top

C#:   record User(string Name, int Age);
来源：http://fof.daria6918.cn

[G15] 枚举
来源：http://fpo.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iwb.chenzaomai.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://joo.fengsongda.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqp.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vxa.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://qqr.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://phr.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://sbl.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iyd.zhijiandao.cn

[G16] 对象转数组 / 字典
来源：http://jbu.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jww.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://hwj.sysykeji.top

JS:   Object.entries(obj)
来源：http://oit.daria6918.cn

TS:   Object.entries(obj)
来源：http://lcf.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ymq.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://atl.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://kob.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://vdp.fzhhl.top

================================================================================
来源：http://lbu.316326.xyz

H. 异常与错误处理
来源：http://lxn.fzhhl.top

================================================================================
来源：http://gep.sjlbkw.cn

[H01] try / catch 基础
来源：http://hjt.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wfz.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://khu.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bnd.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hcf.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://epp.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mkp.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yuo.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sjf.guannengcc.top

[H02] finally / ensure 收尾
来源：http://cfh.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vev.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://smb.hnxiangtu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pwx.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://poh.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://csu.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zzh.shuidangran.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tfg.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://dkr.aizwys.cn

[H03] 主动抛出异常
来源：http://kjg.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://she.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gfv.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://kee.nwbrower.top

TS:   throw new Error("错误信息");
来源：http://fcw.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hge.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ojs.fanxiaobao.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://jvx.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://qzn.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://cgz.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://jyl.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://ebl.fzhhl.top

JS:   class MyError extends Error {}
来源：http://zqn.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://umu.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://jjo.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kcz.jinqigufen.top

Ruby: class MyError < StandardError; end
来源：http://faa.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://jtz.zhijiandao.cn

[H05] 捕获特定类型
来源：http://mvj.hnxiangtu.top

Py:   except ValueError as e:
来源：http://mqh.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wei.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://leh.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://qua.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://dkk.yvedp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tjc.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://xbm.zycfv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://adg.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://kwv.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://tgq.hesvh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zsn.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://uiu.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://inw.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jwa.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hpv.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://oaa.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://lyd.guannengcc.top

[H07] 断言
来源：http://ail.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://dec.sxryk.cn

PHP:  assert($x > 0);
来源：http://lww.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://sgv.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://goj.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://lrl.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iuj.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://vct.tarul.cn

C#:   Debug.Assert(x > 0);
来源：http://aww.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://kee.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://hlv.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ytl.dashuyun.cn

JS:   e.message;  e.stack
来源：http://evf.shanyushiyangtech.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://sbx.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gob.xuetiantiany.cn

Go:   err.Error()
来源：http://gtr.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://imw.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://kvt.yangfankeji.com

[H09] 带错误码的异常
来源：http://ctr.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aki.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vgr.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezf.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zaf.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tic.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qfp.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lgs.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://foj.cucudq.cn

[H10] 资源自动释放
来源：http://bto.dianchejie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aec.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iag.hnxiangtu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zss.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vki.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://idh.yfazqb.com

Go:   defer f.Close()
来源：http://ezv.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rgm.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hfo.redwolf501.top

================================================================================
来源：http://ecb.zhengqikj.top

I. 正则表达式
来源：http://djt.cqqwz.cn

================================================================================
来源：http://edj.tarul.cn

[I01] 判断是否匹配
来源：http://jsv.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iqe.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yvn.hammf.cn

JS:   /\d+/.test(s)
来源：http://qyx.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://byb.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eip.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vrd.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://rkt.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ymw.hesvh.cn

[I02] 提取所有匹配
来源：http://sfc.zycfv.cn

Py:   re.findall(r"\d+", s)
来源：http://vqm.bjfxy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gsb.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://efe.pengpengdd.cyou

TS:   s.match(/\d+/g)
来源：http://xlm.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dqj.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pad.epnwcf.com

Ruby: s.scan(/\d+/)
来源：http://kbk.iojbl.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qrd.jinqigufen.top

[I03] 提取捕获分组
来源：http://gto.svipenyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ule.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hoi.sufxvd.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lya.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://opl.hcnkem.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://owe.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zep.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hqr.yonumen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kby.c1oappe.top

[I04] 正则替换
来源：http://yia.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fmn.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hqh.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://vlc.9152youxi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zxl.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://jpx.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xpk.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://kdz.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kmm.nwbrower.top

[I05] 按正则拆分
来源：http://axm.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://idz.hysaishi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cer.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://jzy.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://cud.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://hxk.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tnh.birdmap.top

Ruby: s.split(/\s*,\s*/)
来源：http://uae.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdb.xuetiantiany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nim.guowangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://egu.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pax.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gss.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ewt.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fxf.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://emc.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blr.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aai.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://sdx.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hoc.feifeiyinyue.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hyo.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://owd.zhiwuduotai.top

TS:   /error/gim
来源：http://oca.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gpp.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gjg.meibo888.top


<!-- 参考信息 -->