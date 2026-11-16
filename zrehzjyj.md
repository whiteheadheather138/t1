代发 wailian999

Java: class User {}
来源：http://mmp.birdmap.top

Go:   type User struct { Name string }
来源：http://acr.zdbjq.cn

Ruby: class User; end
来源：http://pwa.yj20258888.top

C#:   class User {}
来源：http://uuq.nanxinkj.top

[G02] 构造函数
来源：http://ehs.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://mtk.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://bws.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://hcb.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://gyg.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://ihn.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zkk.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://mxe.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://sdo.xinyue.icu

[G03] 实例属性
来源：http://bpw.xuetiantiany.cn

Py:   self.name = "x"
来源：http://muc.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://cds.epnwcf.com

JS:   this.name = "x";
来源：http://hlq.0kj1m.cn

TS:   name: string = "x";
来源：http://gmm.yonumen.top

Java: private String name;
来源：http://zib.ctjpmb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jgx.havefunace.top

Ruby: @name = "x"
来源：http://fxh.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://jeq.316326.xyz

[G04] 定义方法
来源：http://cuu.zhijiandao.cn

Py:   def greet(self): return self.name
来源：http://cwl.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://stl.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://smb.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://bqu.yuanzhike.top

Java: String greet() { return name; }
来源：http://atf.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ash.chenlongwang.top

Ruby: def greet; @name; end
来源：http://oey.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://igl.yonumen.top

[G05] 继承
来源：http://drh.yj202588.top

Py:   class Admin(User): pass
来源：http://duu.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://cqi.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://drn.cdnleiting.top

TS:   class Admin extends User {}
来源：http://jca.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://rit.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kyx.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://xvc.xziqi.cn

C#:   class Admin : User {}
来源：http://gpi.yvedp.cn

[G06] 重写方法
来源：http://jra.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://sbz.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tqy.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://uey.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://fip.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://obx.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bjn.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://gqt.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://bjf.ctjpmb.com

[G07] 调用父类方法
来源：http://bjw.jianghu66.top

Py:   super().greet()
来源：http://rsa.316326.xyz

PHP:  parent::greet();
来源：http://zmx.havefunace.top

JS:   super.greet();
来源：http://ctw.jinqigfzy.top

TS:   super.greet();
来源：http://urn.yfazqb.com

Java: super.greet();
来源：http://qcn.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cww.sweek.top

Ruby: super
来源：http://fwq.tianlin.xyz

C#:   base.Greet();
来源：http://qko.0kj1m.cn

[G08] 静态方法与属性
来源：http://pks.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wge.yj20258.top

PHP:  public static function f() {}
来源：http://xis.zhiwuduotai.top

JS:   static f() {}
来源：http://ewn.vehdjk.com

TS:   static f(): void {}
来源：http://zik.daria6918.cn

Java: static void f() {}
来源：http://jry.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sbt.yuxming.cn

Ruby: def self.f; end
来源：http://hvc.jqgfzy.top

C#:   public static void F() {}
来源：http://jtd.zhiwuduotai.top

[G09] 接口 / 抽象类
来源：http://ahb.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://dcu.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://kkx.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://gyp.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://lpo.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://tnr.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://jpf.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ltr.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://jzc.gzhubu.top

[G10] 访问控制
来源：http://bng.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://wml.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://rug.gzhubu.top

JS:   #private 字段；其余公开
来源：http://npf.cqqwz.cn

TS:   public / protected / private
来源：http://mto.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://vgp.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qro.vqdsnc.cn

Ruby: public / protected / private
来源：http://qnv.iojbl.cn

C#:   public / protected / private / internal
来源：http://gkp.fanxiaobao.xyz

[G11] getter / setter
来源：http://sno.tian-w.cn

Py:   @property 与 @x.setter
来源：http://zcg.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kwp.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://ryr.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://pxg.jlsjyb.cn

Java: public String getName() { return name; }
来源：http://txf.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jfk.bjfxy.top

Ruby: attr_accessor :name
来源：http://yet.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://cyb.yj202588.top

[G12] 对象转字符串
来源：http://lrv.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://csm.cashguo.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mhs.cheryme.top

JS:   toString() { return this.name; }
来源：http://qkq.jqgufenzy.top

TS:   toString(): string { return this.name; }
来源：http://jmm.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://qmp.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nvl.hcnkem.com

Ruby: def to_s; @name; end
来源：http://rid.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://lhh.yangfankeji.com

[G13] 判断对象类型
来源：http://tqa.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://mgp.wangshuangyany.cn

PHP:  $u instanceof User
来源：http://qac.yonumen.top

JS:   u instanceof User
来源：http://env.zhongyouzk.top

TS:   u instanceof User
来源：http://tcd.jlsjyb.cn

Java: u instanceof User
来源：http://zcg.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uaa.yuxming.cn

Ruby: u.is_a?(User)
来源：http://ohs.guowangkeji.top

C#:   u is User
来源：http://pyj.nanxinkj.top

[G14] 数据类 / record
来源：http://lha.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xef.redwolf501.top

PHP:  // 用 readonly 属性模拟
来源：http://eao.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://unc.xuetiantiany.cn

TS:   type User = { name: string; age: number };
来源：http://cjl.tian-w.cn

Java: record User(String name, int age) {}
来源：http://yps.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://jxf.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://llg.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://mfc.chenjidiqi.icu

[G15] 枚举
来源：http://jev.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vnq.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://pwc.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dkl.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vhl.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://gxc.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://plu.ivvv.top

Ruby: Color = %i[red green].freeze
来源：http://ffo.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fkh.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://kpl.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://trj.havefunace.top

PHP:  get_object_vars($obj);
来源：http://ymb.guannengcc.top

JS:   Object.entries(obj)
来源：http://kiz.zycfv.cn

TS:   Object.entries(obj)
来源：http://fhe.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pcc.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zcl.ydzc1.top

Ruby: obj.instance_variables
来源：http://wuq.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://waj.tarul.cn

================================================================================
来源：http://nqd.smart0.xyz

H. 异常与错误处理
来源：http://uaf.zhoulong.xyz

================================================================================
来源：http://atv.sweek.top

[H01] try / catch 基础
来源：http://zyd.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bms.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ybz.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yaf.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bxw.vqdsnc.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lqk.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pfi.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nij.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lmf.fzhhl.top

[H02] finally / ensure 收尾
来源：http://jeg.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hug.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://emg.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://skz.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://skd.guowangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://vps.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmx.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vgo.haohaochexian.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cpt.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://sct.tarul.cn

Py:   raise ValueError("错误信息")
来源：http://fkl.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dlj.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://yxg.ydjk.org.cn

TS:   throw new Error("错误信息");
来源：http://gtx.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://inp.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://emw.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://izk.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://sje.bbcook.cn

[H04] 自定义异常类型
来源：http://gad.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://jwl.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://aqy.316326.xyz

JS:   class MyError extends Error {}
来源：http://zkp.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://ewx.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://cjv.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zlx.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://nhz.dashuyun.cn

C#:   class MyException : Exception {}
来源：http://ihv.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://npa.gaohongyu789.top

Py:   except ValueError as e:
来源：http://pye.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dba.xuanzx.com

JS:   if (e instanceof TypeError) {}
来源：http://fbl.hongshengwenyu.top

TS:   if (e instanceof TypeError) {}
来源：http://twx.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://yof.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ult.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://nkv.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://phn.sufxvd.cn

[H06] 可选值 / 空值安全访问
来源：http://zgq.yj20258888.top

Py:   value = d.get("k") or default
来源：http://kiq.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://nxw.aibaodan.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iwn.hesvh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ksm.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oaq.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oay.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://flr.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://fmn.redwolf501.top

[H07] 断言
来源：http://ood.nanxinkj.top

Py:   assert x > 0, "必须为正"
来源：http://kkn.ppjwa.cn

PHP:  assert($x > 0);
来源：http://lcs.sweek.top

JS:   console.assert(x > 0);
来源：http://jtm.havefunace.top

TS:   console.assert(x > 0);
来源：http://vmx.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://fml.zhixingplan.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dyp.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://clh.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://yuq.iojbl.cn

[H08] 获取错误信息与堆栈
来源：http://ukj.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://phe.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://met.zdqjudy.top

JS:   e.message;  e.stack
来源：http://hhc.meibo888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vbc.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ifi.shanyushiyangkeji.top

Go:   err.Error()
来源：http://ikb.sweek.top

Ruby: e.message;  e.backtrace
来源：http://ius.redwolf501.top

C#:   e.Message;  e.StackTrace
来源：http://pof.hnxiangtu.top

[H09] 带错误码的异常
来源：http://gaj.xingfuxueyuan.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://owz.aizwys.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jix.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aen.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cep.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dzy.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jtr.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mqy.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://wiu.shuidangran.top

[H10] 资源自动释放
来源：http://lfo.jlsjyb.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ryh.xinyue.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://haj.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rxi.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ctp.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zjz.bjfxy.top

Go:   defer f.Close()
来源：http://rzl.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qtd.fehbvm.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://psl.fzhhl.top

================================================================================
来源：http://oom.xylfe.cn

I. 正则表达式
来源：http://aew.guowangkeji.top

================================================================================
来源：http://fim.jqgfzy.top

[I01] 判断是否匹配
来源：http://suj.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xhr.nanxuanxn.top

PHP:  preg_match('/\d+/', $s);
来源：http://nwy.iojbl.cn

JS:   /\d+/.test(s)
来源：http://ard.guannengcc.top

TS:   /\d+/.test(s)
来源：http://dmt.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tic.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uky.sweek.top

Ruby: s.match?(/\d+/)
来源：http://ujb.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vao.hesvh.cn

[I02] 提取所有匹配
来源：http://utd.jianghu66.top

Py:   re.findall(r"\d+", s)
来源：http://bid.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cet.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wkc.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://dmm.haohaochexian.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://end.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gwg.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://adc.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ebj.gaohongyu789.top

[I03] 提取捕获分组
来源：http://icg.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dvj.chenzaomai.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pya.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fsn.xinyue.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sot.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://swr.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qex.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wuc.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://krg.meibo888.top

[I04] 正则替换
来源：http://qjn.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://buz.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wvt.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://dwg.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://bdt.chenjidiqi.icu

Java: s.replaceAll("\\d+", "#")
来源：http://ssz.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vix.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zgu.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xxj.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://crc.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nex.fktsv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wmq.hcnkem.com

JS:   s.split(/\s*,\s*/)
来源：http://vww.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://xki.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://cpd.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zda.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nwk.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xkv.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gnw.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://epd.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://udu.wangdashe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sev.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yef.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xra.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wug.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bub.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://csn.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://umi.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ike.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mam.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sdz.zhengqikj.top

TS:   /error/gim
来源：http://ica.pengpengdd.cyou

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hri.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://unm.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://mpo.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://izq.fehbvm.com

[I08] 贪婪与非贪婪匹配
来源：http://edx.feifeiyinyue.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tab.xylfe.cn


<!-- 参考信息 -->