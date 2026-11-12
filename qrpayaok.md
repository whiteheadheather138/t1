代发 wailian999

Java: class User {}
来源：http://wwa.gzhubu.top

Go:   type User struct { Name string }
来源：http://oni.ctjpmb.com

Ruby: class User; end
来源：http://kcq.guannengcc.top

C#:   class User {}
来源：http://uak.yuanzhike.top

[G02] 构造函数
来源：http://vuz.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://fic.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://avt.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://jvf.tarul.cn

TS:   constructor(public name: string) {}
来源：http://lah.shanyushiyangtech.top

Java: User(String name) { this.name = name; }
来源：http://hap.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zbq.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://rbx.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://vsp.chenlongwang.top

[G03] 实例属性
来源：http://crj.nanxuanxn.top

Py:   self.name = "x"
来源：http://frv.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://bgz.ehwqpu.com

JS:   this.name = "x";
来源：http://gox.ydzc1.top

TS:   name: string = "x";
来源：http://qnd.9152youxi.cn

Java: private String name;
来源：http://gce.tanke756.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ukr.sjlbkw.cn

Ruby: @name = "x"
来源：http://knp.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://twq.zhixingplan.top

[G04] 定义方法
来源：http://tbv.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://kdc.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dbq.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://zof.zhijiandao.cn

TS:   greet(): string { return this.name; }
来源：http://qzi.zhoulong.xyz

Java: String greet() { return name; }
来源：http://lct.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vqi.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://kyk.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://ika.shanyushiyangkeji.top

[G05] 继承
来源：http://csg.tian-w.cn

Py:   class Admin(User): pass
来源：http://wnf.redwolf501.top

PHP:  class Admin extends User {}
来源：http://xwr.fengsongda.top

JS:   class Admin extends User {}
来源：http://qpx.iojbl.cn

TS:   class Admin extends User {}
来源：http://crd.yj20258.top

Java: class Admin extends User {}
来源：http://hzi.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bah.bbcook.cn

Ruby: class Admin < User; end
来源：http://edf.chenlongwang.top

C#:   class Admin : User {}
来源：http://flu.yvedp.cn

[G06] 重写方法
来源：http://bjb.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://jkj.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://goh.feifeiyinyue.top

JS:   greet() { return "admin"; }
来源：http://ydt.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://ysn.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://fsb.zycfv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ozw.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://agf.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://ntr.iojbl.cn

[G07] 调用父类方法
来源：http://egg.wangdashe.top

Py:   super().greet()
来源：http://gze.hfpthk.cn

PHP:  parent::greet();
来源：http://dlq.ywan-chungtsiang.top

JS:   super.greet();
来源：http://abb.yongpay.top

TS:   super.greet();
来源：http://hrj.yanxiufei.cn

Java: super.greet();
来源：http://rqo.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qyw.epnwcf.com

Ruby: super
来源：http://cfe.yvedp.cn

C#:   base.Greet();
来源：http://peh.yj202588.top

[G08] 静态方法与属性
来源：http://olc.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vww.andypj.xyz

PHP:  public static function f() {}
来源：http://dcl.xinyue.icu

JS:   static f() {}
来源：http://urn.jiagoushi.top

TS:   static f(): void {}
来源：http://vmo.yueranfly.top

Java: static void f() {}
来源：http://ugg.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://otr.yfazqb.com

Ruby: def self.f; end
来源：http://fye.bbcook.cn

C#:   public static void F() {}
来源：http://wzv.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://peb.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://qes.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ikq.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nej.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://xhw.hcnkem.com

Java: interface Shape { double area(); }
来源：http://ool.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://xxn.hongshengwenyu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ewf.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://ajd.vqdsnc.cn

[G10] 访问控制
来源：http://wxp.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://qub.epnwcf.com

PHP:  public / protected / private
来源：http://tcx.xylfe.cn

JS:   #private 字段；其余公开
来源：http://rch.shzxlz.cn

TS:   public / protected / private
来源：http://qxw.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://wfp.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://prq.tianlin.xyz

Ruby: public / protected / private
来源：http://xoz.gotoacloud.top

C#:   public / protected / private / internal
来源：http://zqr.chenjidiqi.icu

[G11] getter / setter
来源：http://cub.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://xfc.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ahb.smart0.xyz

JS:   get name() { return this._name; }
来源：http://tfl.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://ouw.hywenlv.cn

Java: public String getName() { return name; }
来源：http://nis.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://emm.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://lzt.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://brj.xuanzx.com

[G12] 对象转字符串
来源：http://fap.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://npa.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://coq.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://vzc.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://vyl.fengsongda.top

Java: @Override public String toString() { return name; }
来源：http://qmy.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://rgf.cucudq.cn

Ruby: def to_s; @name; end
来源：http://byv.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://num.ctjpmb.com

[G13] 判断对象类型
来源：http://jih.redwolf501.top

Py:   isinstance(u, User)
来源：http://flc.jianghu66.top

PHP:  $u instanceof User
来源：http://kcm.havefunace.top

JS:   u instanceof User
来源：http://yhj.zycfv.cn

TS:   u instanceof User
来源：http://obp.0kj1m.cn

Java: u instanceof User
来源：http://fsf.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rsv.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://baj.52xcode.cn

C#:   u is User
来源：http://fms.cdnleiting.top

[G14] 数据类 / record
来源：http://arp.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfp.zycfv.cn

PHP:  // 用 readonly 属性模拟
来源：http://oro.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xzh.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://ybw.gzhubu.top

Java: record User(String name, int age) {}
来源：http://pze.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://uyf.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zdo.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://fym.ybcxt.top

[G15] 枚举
来源：http://vpv.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aiv.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nda.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ujd.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pbb.vqdsnc.cn

Java: enum Color { RED, GREEN }
来源：http://ohi.c1oappe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tjd.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://equ.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sfb.chenzaomai.com

[G16] 对象转数组 / 字典
来源：http://nkw.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nsq.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://whf.jyoumei.cn

JS:   Object.entries(obj)
来源：http://mte.shzxlz.cn

TS:   Object.entries(obj)
来源：http://lme.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dww.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wxs.fzhhl.top

Ruby: obj.instance_variables
来源：http://vtz.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://eeh.bbcook.cn

================================================================================
来源：http://xlx.hnqzz.top

H. 异常与错误处理
来源：http://mne.hcnkem.com

================================================================================
来源：http://cmt.daxiang520.top

[H01] try / catch 基础
来源：http://fqr.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hbe.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mlb.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uxt.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kzv.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nsq.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ewe.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dii.snrcjt.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kap.wangdashe.top

[H02] finally / ensure 收尾
来源：http://euv.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://ykg.jinyuanbaomall.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ojq.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bpo.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ohk.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://nqn.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsd.ehwqpu.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zfx.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://bfp.fzhhl.top

[H03] 主动抛出异常
来源：http://mpv.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://onu.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbu.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://nug.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://imn.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lev.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rwq.hysaishi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hnu.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://qct.chenzaomai.com

[H04] 自定义异常类型
来源：http://pmo.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://umd.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mwe.dashuyun.cn

JS:   class MyError extends Error {}
来源：http://arc.guannengcc.top

TS:   class MyError extends Error {}
来源：http://fga.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://jok.vqdsnc.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mgs.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://nwj.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://uvf.daria6918.cn

[H05] 捕获特定类型
来源：http://uqn.sweek.top

Py:   except ValueError as e:
来源：http://avg.quarkkingdee.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://htr.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://tuw.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://bab.hesvh.cn

Java: catch (IOException | SQLException e) {}
来源：http://zah.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xll.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://ixz.ehwqpu.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://exq.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://waa.redwolf501.top

Py:   value = d.get("k") or default
来源：http://fml.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://iqp.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://gxe.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://ahi.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qmc.smart0.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://omk.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://zks.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://cwe.kuanghao11.cn

[H07] 断言
来源：http://mxb.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://wkl.xuanzx.com

PHP:  assert($x > 0);
来源：http://yeh.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://osf.fktsv.cn

TS:   console.assert(x > 0);
来源：http://waz.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://qth.hysaishi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zkd.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://tdx.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://nbz.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://yaw.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://lim.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rdq.xinyue.icu

JS:   e.message;  e.stack
来源：http://ulu.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yud.hywenlv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lvd.zdqjudy.top

Go:   err.Error()
来源：http://jne.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://ygf.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://lci.gogol.net.cn

[H09] 带错误码的异常
来源：http://dmp.yj20258.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jdy.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://urg.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wmc.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hae.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nck.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://abq.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uey.pycfn.com

C#:   // 自定义异常类中加 Code 属性
来源：http://crs.jlsjyb.cn

[H10] 资源自动释放
来源：http://qzq.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fui.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://odm.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jse.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ubk.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vjb.fengsongda.top

Go:   defer f.Close()
来源：http://rgo.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fmn.sjlbkw.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gfs.ybcxt.top

================================================================================
来源：http://huy.tanke756.top

I. 正则表达式
来源：http://spn.xingfuxueyuan.xyz

================================================================================
来源：http://bxs.yfazqb.com

[I01] 判断是否匹配
来源：http://unc.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zfq.ehwqpu.com

PHP:  preg_match('/\d+/', $s);
来源：http://ksl.yonumen.top

JS:   /\d+/.test(s)
来源：http://zjo.sxryk.cn

TS:   /\d+/.test(s)
来源：http://rac.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jel.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqz.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://hvx.yanxiufei.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bcl.52xcode.cn

[I02] 提取所有匹配
来源：http://tha.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://cdn.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ovb.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bin.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://jwm.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nko.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qyf.sufxvd.cn

Ruby: s.scan(/\d+/)
来源：http://ixn.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jxe.tian-w.cn

[I03] 提取捕获分组
来源：http://rdt.yfazqb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bxu.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ofa.yongpay.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://buw.hywenlv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://unu.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gtj.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bdd.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jbt.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://haj.dianchejie.cn

[I04] 正则替换
来源：http://qja.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bry.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ccy.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://hvv.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://pdf.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nym.cdnleiting.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yll.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gvo.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nff.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://vbq.sufxvd.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tti.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://son.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://tvo.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://gcf.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://nre.hfpthk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ekv.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://mvy.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gox.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pfy.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://epj.shanyushiyangtech.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lpz.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kcg.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ubl.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zju.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gdk.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zap.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iao.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://ttb.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://stb.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fik.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nuo.cashguo.top

TS:   /error/gim
来源：http://wsk.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vpu.smart0.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bvq.meibo888.top

Ruby: s.scan(/error/i)
来源：http://qts.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ywt.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://jyb.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tyx.c1oappe.top


<!-- 参考信息 -->