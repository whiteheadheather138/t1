代发 wailian999

Py:   class User: pass
来源：http://brj.ydzc1.top

PHP:  class User {}
来源：http://abv.wangdashe.top

JS:   class User {}
来源：http://zaq.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://abp.zdqjudy.top

Java: class User {}
来源：http://sfb.yfazqb.com

Go:   type User struct { Name string }
来源：http://ply.quarkkingdee.top

Ruby: class User; end
来源：http://ucf.haohaochexian.top

C#:   class User {}
来源：http://zgj.jlsjyb.cn

[G02] 构造函数
来源：http://acp.snrcjt.cn

Py:   def __init__(self, name): self.name = name
来源：http://wrz.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iqw.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://omi.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://qpo.gotoacloud.top

Java: User(String name) { this.name = name; }
来源：http://ihl.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hue.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://pyx.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://zql.jlsjyb.cn

[G03] 实例属性
来源：http://gqw.zhengqikj.top

Py:   self.name = "x"
来源：http://sfy.guowangkeji.top

PHP:  public string $name = "x";
来源：http://not.sxryk.cn

JS:   this.name = "x";
来源：http://xxz.snrcjt.cn

TS:   name: string = "x";
来源：http://kcn.shanyushiyangtech.top

Java: private String name;
来源：http://ewi.jqgfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sro.xinyue.icu

Ruby: @name = "x"
来源：http://aiu.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://yns.wangshuangyany.cn

[G04] 定义方法
来源：http://vbf.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://zye.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ewp.yongpay.top

JS:   greet() { return this.name; }
来源：http://ara.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://tlr.guowangkeji.top

Java: String greet() { return name; }
来源：http://wih.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tyf.fehbvm.com

Ruby: def greet; @name; end
来源：http://ico.hnxiangtu.top

C#:   public string Greet() => Name;
来源：http://rfj.zdbjq.cn

[G05] 继承
来源：http://qmy.sweek.top

Py:   class Admin(User): pass
来源：http://kov.yonumen.top

PHP:  class Admin extends User {}
来源：http://oya.vehdjk.com

JS:   class Admin extends User {}
来源：http://njn.jiagoushi.top

TS:   class Admin extends User {}
来源：http://btz.cqqwz.cn

Java: class Admin extends User {}
来源：http://dlw.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://spv.yuanzhike.top

Ruby: class Admin < User; end
来源：http://tzv.yueranfly.top

C#:   class Admin : User {}
来源：http://cyx.chenjidiqi.icu

[G06] 重写方法
来源：http://eyb.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://uxc.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nzg.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://bbr.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://seb.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://aft.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jgv.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://xyj.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://amh.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://cin.bjfxy.top

Py:   super().greet()
来源：http://bqg.sjlbkw.cn

PHP:  parent::greet();
来源：http://upi.gotoacloud.top

JS:   super.greet();
来源：http://wbf.fktsv.cn

TS:   super.greet();
来源：http://lhc.gotoacloud.top

Java: super.greet();
来源：http://nyz.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zqd.ctjpmb.com

Ruby: super
来源：http://xhf.shanyushiyangtech.top

C#:   base.Greet();
来源：http://sqn.jianghu66.top

[G08] 静态方法与属性
来源：http://gwc.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cys.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://kcb.jinyuanbaomall.cn

JS:   static f() {}
来源：http://jpt.bbcook.cn

TS:   static f(): void {}
来源：http://knh.9152youxi.cn

Java: static void f() {}
来源：http://ctr.zhoulong.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://izh.ehwqpu.com

Ruby: def self.f; end
来源：http://slc.ybcxt.top

C#:   public static void F() {}
来源：http://vxq.meibo888.top

[G09] 接口 / 抽象类
来源：http://fvg.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://cbi.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://lhi.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ywz.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://rvd.mhx1999.top

Java: interface Shape { double area(); }
来源：http://kvz.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://xak.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://arz.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://idm.ydjk.org.cn

[G10] 访问控制
来源：http://fwf.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://oem.epnwcf.com

PHP:  public / protected / private
来源：http://dwv.tarul.cn

JS:   #private 字段；其余公开
来源：http://asz.zhongyouzk.top

TS:   public / protected / private
来源：http://yzj.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://nkz.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mqh.hfpthk.cn

Ruby: public / protected / private
来源：http://hqt.yj202588.top

C#:   public / protected / private / internal
来源：http://vrv.hnxiangtu.top

[G11] getter / setter
来源：http://rwj.hywenlv.cn

Py:   @property 与 @x.setter
来源：http://vvr.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://iwd.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://nhm.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://bhk.jiagoushi.top

Java: public String getName() { return name; }
来源：http://idj.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nfr.hywenlv.cn

Ruby: attr_accessor :name
来源：http://vvt.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://zqr.xuetiantiany.cn

[G12] 对象转字符串
来源：http://ceb.cashguo.top

Py:   def __str__(self): return self.name
来源：http://pkv.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ghu.sysykeji.top

JS:   toString() { return this.name; }
来源：http://vhz.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://kzg.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://vxp.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nia.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://iva.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://aht.vehdjk.com

[G13] 判断对象类型
来源：http://fyw.cheryme.top

Py:   isinstance(u, User)
来源：http://pgb.cdnleiting.top

PHP:  $u instanceof User
来源：http://ral.bjfxy.top

JS:   u instanceof User
来源：http://chq.bbcook.cn

TS:   u instanceof User
来源：http://xmf.shangyingyoupin.top

Java: u instanceof User
来源：http://kye.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://grk.uphjek.com

Ruby: u.is_a?(User)
来源：http://fwq.fehbvm.com

C#:   u is User
来源：http://xlz.wangdashe.top

[G14] 数据类 / record
来源：http://dig.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://afq.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://ams.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://wkg.cucudq.cn

TS:   type User = { name: string; age: number };
来源：http://hcr.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://zrg.zhiwuduotai.top

Go:   type User struct { Name string; Age int }
来源：http://edc.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://owu.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://ntj.cqqwz.cn

[G15] 枚举
来源：http://njf.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xij.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yfa.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xyr.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xof.redwolf501.top

Java: enum Color { RED, GREEN }
来源：http://wfx.nanxuanxn.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nql.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://ryi.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iav.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://fnl.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kmr.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://fzh.gotoacloud.top

JS:   Object.entries(obj)
来源：http://pek.snrcjt.cn

TS:   Object.entries(obj)
来源：http://xme.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pho.epnwcf.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kbs.dashuyun.cn

Ruby: obj.instance_variables
来源：http://kac.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://xht.kuanghao11.cn

================================================================================
来源：http://gas.mhx1999.top

H. 异常与错误处理
来源：http://ssg.fehbvm.com

================================================================================
来源：http://ugg.tanke756.top

[H01] try / catch 基础
来源：http://jcg.vqdsnc.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://olf.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mcw.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yqc.ctjpmb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kce.hfpthk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://inf.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jaz.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqq.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bto.cheryme.top

[H02] finally / ensure 收尾
来源：http://bxx.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://pbl.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://veo.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xyd.yj20258888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://iam.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://bai.kuanghao11.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tdb.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zuz.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uzc.haohaochexian.top

[H03] 主动抛出异常
来源：http://mun.jianghu66.top

Py:   raise ValueError("错误信息")
来源：http://sia.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dns.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://bvr.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://pxf.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vvp.chenzaomai.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://aew.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ipl.wangdashe.top

C#:   throw new ArgumentException("错误信息");
来源：http://xde.tanke756.top

[H04] 自定义异常类型
来源：http://cog.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://wim.snrcjt.cn

PHP:  class MyError extends RuntimeException {}
来源：http://scn.havefunace.top

JS:   class MyError extends Error {}
来源：http://xzc.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://wpr.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://dfv.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cak.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://xrw.hesvh.cn

C#:   class MyException : Exception {}
来源：http://kqo.yongpay.top

[H05] 捕获特定类型
来源：http://okf.redwolf501.top

Py:   except ValueError as e:
来源：http://tix.yuanzhike.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wkm.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://xmt.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://foi.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://anc.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jww.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://jfu.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hsa.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://shp.52xcode.cn

Py:   value = d.get("k") or default
来源：http://mzg.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://wfa.jyoumei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://scu.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://nvs.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kwt.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lsc.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://ngd.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://phb.bbcook.cn

[H07] 断言
来源：http://ynf.fehbvm.com

Py:   assert x > 0, "必须为正"
来源：http://pzo.zhengqikj.top

PHP:  assert($x > 0);
来源：http://cxv.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://sen.chenzaomai.com

TS:   console.assert(x > 0);
来源：http://hmv.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://xde.bjfxy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://smq.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vbi.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://qcp.hysaishi.cn

[H08] 获取错误信息与堆栈
来源：http://lvo.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://nod.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qib.sjlbkw.cn

JS:   e.message;  e.stack
来源：http://cle.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://gtb.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kwh.52xcode.cn

Go:   err.Error()
来源：http://hld.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://uvi.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://sbc.hysaishi.cn

[H09] 带错误码的异常
来源：http://kqo.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://upl.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uht.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lyy.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sfi.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vpe.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kmu.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://wht.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://omy.cdnleiting.top

[H10] 资源自动释放
来源：http://gpq.gaohongyu789.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cjr.316326.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wyc.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vac.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aaw.jyoumei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xxx.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://wdl.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fsi.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mbu.fengsongda.top

================================================================================
来源：http://ktt.kuanghao11.cn

I. 正则表达式
来源：http://awj.ywan-chungtsiang.top

================================================================================
来源：http://jrh.zhengqikj.top

[I01] 判断是否匹配
来源：http://gtb.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bfk.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://ssd.chenzaomai.com

JS:   /\d+/.test(s)
来源：http://pdd.yj20258.top

TS:   /\d+/.test(s)
来源：http://bav.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kmk.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fal.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://lfd.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gqv.snrcjt.cn

[I02] 提取所有匹配
来源：http://tdy.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://ecn.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mmn.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vek.cheryme.top

TS:   s.match(/\d+/g)
来源：http://bds.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eix.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jtg.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://dox.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lep.zhengqikj.top

[I03] 提取捕获分组
来源：http://dxn.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mxp.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gzv.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ojl.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jal.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://biw.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ptr.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eqf.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rkn.zhengqikj.top

[I04] 正则替换
来源：http://fpd.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://klw.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zch.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cqk.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nlp.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://stx.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ygx.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dws.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gcb.zhijiandao.cn

[I05] 按正则拆分
来源：http://jir.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ewl.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ipi.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://eep.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://vtk.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://kmr.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ppd.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pzl.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zqc.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rom.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jjp.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xjw.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wbq.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mzt.sweek.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dfi.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ezn.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://khb.zhoulong.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://afp.zhoulong.xyz

[I07] 忽略大小写与多行模式
来源：http://vic.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://duw.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eme.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vpj.xylfe.cn

TS:   /error/gim
来源：http://jbv.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://imh.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vai.epnwcf.com


<!-- 参考信息 -->