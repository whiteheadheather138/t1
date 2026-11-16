代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kfy.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ode.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pwd.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lgm.yongpay.top

================================================================================
来源：http://neh.jinqigfzy.top

G. 面向对象
来源：http://hsw.nwbrower.top

================================================================================
来源：http://rpl.fengsongda.top

[G01] 定义类
来源：http://htu.fzhhl.top

Py:   class User: pass
来源：http://luj.nanxinkj.top

PHP:  class User {}
来源：http://hjd.tianlin.xyz

JS:   class User {}
来源：http://spi.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://dbg.uphjek.com

Java: class User {}
来源：http://kop.iojbl.cn

Go:   type User struct { Name string }
来源：http://uxm.yongpay.top

Ruby: class User; end
来源：http://wgf.vehdjk.com

C#:   class User {}
来源：http://zky.kuanghao11.cn

[G02] 构造函数
来源：http://jvb.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://crg.iojbl.cn

PHP:  public function __construct(public string $name) {}
来源：http://rwm.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://qhx.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://bak.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://tup.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://txt.dianchejie.cn

Ruby: def initialize(name); @name = name; end
来源：http://haq.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://mym.bbcook.cn

[G03] 实例属性
来源：http://idq.yueranfly.top

Py:   self.name = "x"
来源：http://sxq.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://pmq.yonumen.top

JS:   this.name = "x";
来源：http://ilb.ctjpmb.com

TS:   name: string = "x";
来源：http://jtl.jinqigfzy.top

Java: private String name;
来源：http://wps.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ehh.dashuyun.cn

Ruby: @name = "x"
来源：http://kuz.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://vqz.sufxvd.cn

[G04] 定义方法
来源：http://fdw.yfazqb.com

Py:   def greet(self): return self.name
来源：http://scc.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ndq.hnqzz.top

JS:   greet() { return this.name; }
来源：http://suz.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://bcn.zdqjudy.top

Java: String greet() { return name; }
来源：http://ynh.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bhw.uphjek.com

Ruby: def greet; @name; end
来源：http://dtq.cheryme.top

C#:   public string Greet() => Name;
来源：http://ger.xylfe.cn

[G05] 继承
来源：http://oqo.jyoumei.cn

Py:   class Admin(User): pass
来源：http://geg.tanke756.top

PHP:  class Admin extends User {}
来源：http://zph.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://lne.0kj1m.cn

TS:   class Admin extends User {}
来源：http://xyv.zhongyouzk.top

Java: class Admin extends User {}
来源：http://stk.fktsv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kdb.meibo888.top

Ruby: class Admin < User; end
来源：http://whf.wangdashe.top

C#:   class Admin : User {}
来源：http://shh.aibaodan.cn

[G06] 重写方法
来源：http://wbz.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://fjp.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://epx.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://mdq.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://vqc.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://pmy.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xsr.ydjk.org.cn

Ruby: def greet; "admin"; end
来源：http://tec.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://pdg.c1oappe.top

[G07] 调用父类方法
来源：http://jkj.zhijiandao.cn

Py:   super().greet()
来源：http://tzw.birdmap.top

PHP:  parent::greet();
来源：http://xtj.fzhhl.top

JS:   super.greet();
来源：http://dqc.zhongyouzk.top

TS:   super.greet();
来源：http://kbn.jianghu66.top

Java: super.greet();
来源：http://lwa.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fdj.yj202588.top

Ruby: super
来源：http://kbx.chenlongwang.top

C#:   base.Greet();
来源：http://qqs.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://sng.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://agu.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://unv.guowangkeji.top

JS:   static f() {}
来源：http://row.sweek.top

TS:   static f(): void {}
来源：http://mws.jqgufenzy.top

Java: static void f() {}
来源：http://dbt.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vfg.nanxinkj.top

Ruby: def self.f; end
来源：http://xpj.meibo888.top

C#:   public static void F() {}
来源：http://use.daria6918.cn

[G09] 接口 / 抽象类
来源：http://mwe.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://toh.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tov.shuidangran.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mbs.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://jgc.yuxming.cn

Java: interface Shape { double area(); }
来源：http://fnl.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://vrx.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ion.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://pal.snrcjt.cn

[G10] 访问控制
来源：http://ksj.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://rqg.xylfe.cn

PHP:  public / protected / private
来源：http://utm.fengsongda.top

JS:   #private 字段；其余公开
来源：http://znw.jiagoushi.top

TS:   public / protected / private
来源：http://mac.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://rov.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://etf.cheryme.top

Ruby: public / protected / private
来源：http://ukb.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://juo.zhengqikj.top

[G11] getter / setter
来源：http://dni.epnwcf.com

Py:   @property 与 @x.setter
来源：http://wwj.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ynd.jinyuanbaomall.cn

JS:   get name() { return this._name; }
来源：http://hlu.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://ogl.birdmap.top

Java: public String getName() { return name; }
来源：http://hba.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wre.iojbl.cn

Ruby: attr_accessor :name
来源：http://xjl.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://gre.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://ogx.hysaishi.cn

Py:   def __str__(self): return self.name
来源：http://ejc.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://njf.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://lzl.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://zuf.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://rih.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://mtz.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://dfm.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://wyw.sufxvd.cn

[G13] 判断对象类型
来源：http://cvf.aizwys.cn

Py:   isinstance(u, User)
来源：http://nzk.yuxming.cn

PHP:  $u instanceof User
来源：http://zbg.yfazqb.com

JS:   u instanceof User
来源：http://kbk.cashguo.top

TS:   u instanceof User
来源：http://ojt.hcnkem.com

Java: u instanceof User
来源：http://tbq.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://rrc.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://boz.tarul.cn

C#:   u is User
来源：http://gto.bjfxy.top

[G14] 数据类 / record
来源：http://hef.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fpc.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://iou.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://spa.ppjwa.cn

TS:   type User = { name: string; age: number };
来源：http://fki.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://kjd.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://fro.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wot.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://djf.yuanzhike.top

[G15] 枚举
来源：http://jny.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xob.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ria.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iqy.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://acy.ydjk.org.cn

Java: enum Color { RED, GREEN }
来源：http://ztt.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdd.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://arx.fktsv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ori.jinghuilouyu.cn

[G16] 对象转数组 / 字典
来源：http://kxh.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mog.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://uux.iojbl.cn

JS:   Object.entries(obj)
来源：http://ryd.nanxinkj.top

TS:   Object.entries(obj)
来源：http://hvz.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xeh.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xpk.ybcxt.top

Ruby: obj.instance_variables
来源：http://jxx.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://ugl.zhongyouzk.top

================================================================================
来源：http://jtk.svipenyu.cn

H. 异常与错误处理
来源：http://rvk.shanyushiyangtech.top

================================================================================
来源：http://oje.ywan-chungtsiang.top

[H01] try / catch 基础
来源：http://ofu.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://boi.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://joa.daxiang520.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://egh.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wos.pengpengdd.cyou

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://poc.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://igx.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cut.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ogx.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://ijl.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://avy.tian-w.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xqr.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://sth.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pll.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://dpd.sjlbkw.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mas.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://orj.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bfd.cucudq.cn

[H03] 主动抛出异常
来源：http://sdy.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://kdz.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lte.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://lpz.wangshuangyany.cn

TS:   throw new Error("错误信息");
来源：http://iol.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fom.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hod.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mbq.aibaodan.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xnx.52xcode.cn

[H04] 自定义异常类型
来源：http://kck.tian-w.cn

Py:   class MyError(Exception): pass
来源：http://fti.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://uft.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://zso.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://rhq.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://uyd.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://oqj.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://nda.fktsv.cn

C#:   class MyException : Exception {}
来源：http://cpy.xylfe.cn

[H05] 捕获特定类型
来源：http://ppm.shzxlz.cn

Py:   except ValueError as e:
来源：http://got.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hlt.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://hix.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://qdy.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://ykv.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qch.uphjek.com

Ruby: rescue ArgumentError => e
来源：http://zdq.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rwr.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://qjj.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://ott.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://zjp.sxryk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://inu.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://dgq.shanyushiyangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gmo.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nzn.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://iwb.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://iyc.mhx1999.top

[H07] 断言
来源：http://zmq.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://paq.yvedp.cn

PHP:  assert($x > 0);
来源：http://onw.yuxming.cn

JS:   console.assert(x > 0);
来源：http://rgc.ydzc1.top

TS:   console.assert(x > 0);
来源：http://eks.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://qnc.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qqa.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vhk.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://rhw.cqqwz.cn

[H08] 获取错误信息与堆栈
来源：http://jbm.shuidangran.top

Py:   str(e);  traceback.format_exc()
来源：http://pqc.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gkc.hfpthk.cn

JS:   e.message;  e.stack
来源：http://hbh.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ptg.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://csm.shanyushiyangtech.top

Go:   err.Error()
来源：http://nnv.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://hji.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://spx.xuanzx.com

[H09] 带错误码的异常
来源：http://jou.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vha.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://elc.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cuq.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hwg.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zte.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kdn.shangyingyoupin.top

Ruby: raise MyError.new("fail", 500)
来源：http://eka.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jju.yj20258888.top

[H10] 资源自动释放
来源：http://dmi.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://but.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ppr.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dkd.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ulf.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ynj.xinyue.icu

Go:   defer f.Close()
来源：http://ixu.ydjk.org.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qtm.dashuyun.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nwi.xziqi.cn

================================================================================
来源：http://tvp.hnqzz.top

I. 正则表达式
来源：http://gul.sweek.top

================================================================================
来源：http://amn.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://zfw.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://era.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://mnx.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://euw.meibo888.top

TS:   /\d+/.test(s)
来源：http://ywc.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://glt.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dzu.jinyuanbaomall.cn

Ruby: s.match?(/\d+/)
来源：http://abg.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ixo.jinqigufen.top

[I02] 提取所有匹配
来源：http://fjm.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://vox.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tlr.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lec.gogol.net.cn

TS:   s.match(/\d+/g)
来源：http://hkb.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ril.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tjz.hnqzz.top

Ruby: s.scan(/\d+/)
来源：http://jca.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qdb.nanxuanxn.top

[I03] 提取捕获分组
来源：http://rfd.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hes.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cym.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iha.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://orf.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pid.shuidangran.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sbt.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yts.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://urp.yonumen.top

[I04] 正则替换
来源：http://xnm.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ntp.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zzc.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://bls.daxiang520.top

TS:   s.replace(/\d+/g, "#")
来源：http://zpz.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://ihd.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cii.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rod.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nwt.iojbl.cn

[I05] 按正则拆分
来源：http://ivu.xuanzx.com

Py:   re.split(r"\s*,\s*", s)
来源：http://yzo.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://adm.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://arb.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://fmz.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://jzn.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iuh.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ipo.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mrw.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yat.cqqwz.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nue.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mji.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uch.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mkn.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pct.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tsc.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wqc.zhaomingkeji.xyz


<!-- 参考信息 -->