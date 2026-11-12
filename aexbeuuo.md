代发 wailian999

Java: class User {}
来源：http://mxe.smart0.xyz

Go:   type User struct { Name string }
来源：http://cjc.xuetiantiany.cn

Ruby: class User; end
来源：http://nzw.xinyue.icu

C#:   class User {}
来源：http://ioy.hnqzz.top

[G02] 构造函数
来源：http://ayf.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://efb.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://hao.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://lpb.yj20258.top

TS:   constructor(public name: string) {}
来源：http://udn.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://amn.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vii.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://qbt.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://qzy.havefunace.top

[G03] 实例属性
来源：http://fik.zhixingplan.top

Py:   self.name = "x"
来源：http://rwh.cashguo.top

PHP:  public string $name = "x";
来源：http://tae.iojbl.cn

JS:   this.name = "x";
来源：http://jzs.cucudq.cn

TS:   name: string = "x";
来源：http://mpa.jiagoushi.top

Java: private String name;
来源：http://fah.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uux.xylfe.cn

Ruby: @name = "x"
来源：http://baw.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://lwo.jlsjyb.cn

[G04] 定义方法
来源：http://ews.cheryme.top

Py:   def greet(self): return self.name
来源：http://zdt.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uso.daxiang520.top

JS:   greet() { return this.name; }
来源：http://vet.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://rnw.dashuyun.cn

Java: String greet() { return name; }
来源：http://amd.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fae.zycfv.cn

Ruby: def greet; @name; end
来源：http://pjs.tian-w.cn

C#:   public string Greet() => Name;
来源：http://dyq.gotoacloud.top

[G05] 继承
来源：http://hhe.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://zfl.jiagoushi.top

PHP:  class Admin extends User {}
来源：http://amt.sweek.top

JS:   class Admin extends User {}
来源：http://ghf.jiagoushi.top

TS:   class Admin extends User {}
来源：http://gir.bbcook.cn

Java: class Admin extends User {}
来源：http://jcd.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wjd.sufxvd.cn

Ruby: class Admin < User; end
来源：http://iyx.ydzc1.top

C#:   class Admin : User {}
来源：http://iqz.ywan-chungtsiang.top

[G06] 重写方法
来源：http://jzm.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://iwl.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://apf.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://qco.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://jek.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://lvu.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wmj.ivvv.top

Ruby: def greet; "admin"; end
来源：http://ksk.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://qsf.c1oappe.top

[G07] 调用父类方法
来源：http://ycl.vqdsnc.cn

Py:   super().greet()
来源：http://zka.pycfn.com

PHP:  parent::greet();
来源：http://rhj.xziqi.cn

JS:   super.greet();
来源：http://wtq.fehbvm.com

TS:   super.greet();
来源：http://hou.c1oappe.top

Java: super.greet();
来源：http://kug.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iul.yuanzhike.top

Ruby: super
来源：http://xtt.cashguo.top

C#:   base.Greet();
来源：http://fol.ctjpmb.com

[G08] 静态方法与属性
来源：http://sgp.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dou.vqdsnc.cn

PHP:  public static function f() {}
来源：http://xgd.bbcook.cn

JS:   static f() {}
来源：http://jvr.snrcjt.cn

TS:   static f(): void {}
来源：http://pjd.zhoulong.xyz

Java: static void f() {}
来源：http://sfk.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tqa.chenzaomai.com

Ruby: def self.f; end
来源：http://bfq.ehwqpu.com

C#:   public static void F() {}
来源：http://xbj.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://esl.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://mxp.vqdsnc.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kom.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ytb.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://hnd.ivvv.top

Java: interface Shape { double area(); }
来源：http://rrv.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ats.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zeq.yj20258888.top

C#:   interface IShape { double Area(); }
来源：http://wqn.yangfankeji.com

[G10] 访问控制
来源：http://ili.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://xfh.sweek.top

PHP:  public / protected / private
来源：http://tfd.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://cni.smart0.xyz

TS:   public / protected / private
来源：http://kxd.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://xkr.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jpi.wangdashe.top

Ruby: public / protected / private
来源：http://lfg.nanxinkj.top

C#:   public / protected / private / internal
来源：http://ioj.feifeiyinyue.top

[G11] getter / setter
来源：http://jan.meibo888.top

Py:   @property 与 @x.setter
来源：http://qpc.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wne.daria6918.cn

JS:   get name() { return this._name; }
来源：http://qsv.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://smf.jiagoushi.top

Java: public String getName() { return name; }
来源：http://gcs.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://egi.0kj1m.cn

Ruby: attr_accessor :name
来源：http://vlb.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://nni.hesvh.cn

[G12] 对象转字符串
来源：http://pri.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://opd.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://two.shuidangran.top

JS:   toString() { return this.name; }
来源：http://shq.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://udx.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://nax.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://grg.quarkkingdee.top

Ruby: def to_s; @name; end
来源：http://hnn.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://xvx.sysykeji.top

[G13] 判断对象类型
来源：http://nta.0kj1m.cn

Py:   isinstance(u, User)
来源：http://wce.gzhubu.top

PHP:  $u instanceof User
来源：http://wec.chenjidiqi.icu

JS:   u instanceof User
来源：http://syr.jqgfzy.top

TS:   u instanceof User
来源：http://pic.birdmap.top

Java: u instanceof User
来源：http://ums.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://les.hcnkem.com

Ruby: u.is_a?(User)
来源：http://qag.yj20258.top

C#:   u is User
来源：http://jun.yanxiufei.cn

[G14] 数据类 / record
来源：http://qlp.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xqs.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://xxz.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://qkj.ehwqpu.com

TS:   type User = { name: string; age: number };
来源：http://tdn.gzhubu.top

Java: record User(String name, int age) {}
来源：http://gvy.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://nei.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nnx.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://hmd.jinqigfzy.top

[G15] 枚举
来源：http://zfj.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sal.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tnj.kuanghao11.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cgv.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hhz.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://rih.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pak.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://urk.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ywp.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://vlq.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qdn.fktsv.cn

PHP:  get_object_vars($obj);
来源：http://dmd.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://yck.cqqwz.cn

TS:   Object.entries(obj)
来源：http://jlc.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tpw.cucudq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gxv.yj202588.top

Ruby: obj.instance_variables
来源：http://agj.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://gof.gogol.net.cn

================================================================================
来源：http://fxe.xuanzx.com

H. 异常与错误处理
来源：http://vdt.ehwqpu.com

================================================================================
来源：http://xsw.jinqigfzy.top

[H01] try / catch 基础
来源：http://toi.jyoumei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://szz.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ixu.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zrl.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://egi.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ioq.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uwe.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cim.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dji.sxryk.cn

[H02] finally / ensure 收尾
来源：http://ebe.zhaomingkeji.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://snf.vqdsnc.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jdl.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://stk.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://foh.yj20258.top

Java: try { f(); } finally { cleanup(); }
来源：http://ixw.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mbu.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://pap.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xfg.gotoacloud.top

[H03] 主动抛出异常
来源：http://yxr.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://ycw.guannengcc.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zld.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://wms.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://ifk.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tgn.9152youxi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gyz.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://epg.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mgr.smart0.xyz

[H04] 自定义异常类型
来源：http://maj.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://vju.cucudq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xhj.yueranfly.top

JS:   class MyError extends Error {}
来源：http://tle.iojbl.cn

TS:   class MyError extends Error {}
来源：http://epe.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://qgy.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ore.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://ihs.zycfv.cn

C#:   class MyException : Exception {}
来源：http://ili.shuidangran.top

[H05] 捕获特定类型
来源：http://avt.hysaishi.cn

Py:   except ValueError as e:
来源：http://tqc.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://urg.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://qkh.feifeiyinyue.top

TS:   if (e instanceof TypeError) {}
来源：http://mcr.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://bis.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gtt.zycfv.cn

Ruby: rescue ArgumentError => e
来源：http://lqz.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yxy.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://bzi.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://oks.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ity.316326.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://cui.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://arl.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gaj.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bow.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://jgc.smart0.xyz

C#:   obj?.A?.B ?? default
来源：http://vej.xuetiantiany.cn

[H07] 断言
来源：http://jjt.hammf.cn

Py:   assert x > 0, "必须为正"
来源：http://tgo.hysaishi.cn

PHP:  assert($x > 0);
来源：http://hvv.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://exm.yonumen.top

TS:   console.assert(x > 0);
来源：http://eti.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://hke.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://trn.hnqzz.top

Ruby: raise "必须为正" unless x > 0
来源：http://zug.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://trq.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://eud.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://ble.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tvz.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://ktt.yuanzhike.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://epb.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fob.hesvh.cn

Go:   err.Error()
来源：http://etp.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://fei.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://mtw.shanyushiyangkeji.top

[H09] 带错误码的异常
来源：http://bzu.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://chj.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yxk.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cql.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://atf.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yqe.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xtz.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://qxd.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iup.smart0.xyz

[H10] 资源自动释放
来源：http://rtp.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rlm.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lsz.yj20258888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lkh.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iaz.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mxl.nwbrower.top

Go:   defer f.Close()
来源：http://ndq.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gnu.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gss.cashguo.top

================================================================================
来源：http://bxz.xuanzx.com

I. 正则表达式
来源：http://bcq.pengpengdd.cyou

================================================================================
来源：http://lcl.ybcxt.top

[I01] 判断是否匹配
来源：http://wmv.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygl.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rfa.jlsjyb.cn

JS:   /\d+/.test(s)
来源：http://pwz.meibo888.top

TS:   /\d+/.test(s)
来源：http://zfr.yangfankeji.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zjd.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kud.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://jgo.zhiwuduotai.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kot.zycfv.cn

[I02] 提取所有匹配
来源：http://mdd.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://mwd.zhiwuduotai.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xcu.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bac.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://irv.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://meh.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ezq.iojbl.cn

Ruby: s.scan(/\d+/)
来源：http://tys.hnxiangtu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vzh.hcnkem.com

[I03] 提取捕获分组
来源：http://psj.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hel.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eau.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sbo.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ivp.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gvn.ehwqpu.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tit.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rgi.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uwp.sysykeji.top

[I04] 正则替换
来源：http://qbh.fengsongda.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xsl.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmy.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zfk.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://knm.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eug.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ybq.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ilx.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://onu.0kj1m.cn

[I05] 按正则拆分
来源：http://plk.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://kjz.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blm.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://qyp.yanxiufei.cn

TS:   s.split(/\s*,\s*/)
来源：http://vqb.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://pjj.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lpp.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xxr.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vzd.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lbl.fehbvm.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://drm.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nee.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgn.yonumen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nlv.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwt.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tec.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tew.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nrz.chenjidiqi.icu

[I07] 忽略大小写与多行模式
来源：http://gpn.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://auu.shuidangran.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hno.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ajm.sysykeji.top

TS:   /error/gim
来源：http://uth.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nzi.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fxt.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://vkw.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://asb.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://fbt.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bmp.hfpthk.cn


<!-- 参考信息 -->