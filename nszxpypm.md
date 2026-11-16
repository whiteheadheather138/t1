代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://whm.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwh.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cwl.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bgq.daxiang520.top

================================================================================
来源：http://con.snrcjt.cn

G. 面向对象
来源：http://olt.ybcxt.top

================================================================================
来源：http://amf.yanxiufei.cn

[G01] 定义类
来源：http://zux.hnqzz.top

Py:   class User: pass
来源：http://ehe.yangfankeji.com

PHP:  class User {}
来源：http://eed.dashuyun.cn

JS:   class User {}
来源：http://inp.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://fpu.cqqwz.cn

Java: class User {}
来源：http://zbz.shuidangran.top

Go:   type User struct { Name string }
来源：http://yzd.yj20258888.top

Ruby: class User; end
来源：http://jna.haohaochexian.top

C#:   class User {}
来源：http://lil.yueranfly.top

[G02] 构造函数
来源：http://xyo.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://jrb.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://rtx.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://vgw.fehbvm.com

TS:   constructor(public name: string) {}
来源：http://nts.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://xbp.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uce.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://stx.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://yfi.yongpay.top

[G03] 实例属性
来源：http://tnq.yangfankeji.com

Py:   self.name = "x"
来源：http://emb.xylfe.cn

PHP:  public string $name = "x";
来源：http://blj.wangdashe.top

JS:   this.name = "x";
来源：http://uyx.pengpengdd.cyou

TS:   name: string = "x";
来源：http://wjs.yonumen.top

Java: private String name;
来源：http://rrb.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wpz.chenzaomai.com

Ruby: @name = "x"
来源：http://ind.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://kje.meibo888.top

[G04] 定义方法
来源：http://zsh.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://qlv.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nbt.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://lup.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://xwj.smart0.xyz

Java: String greet() { return name; }
来源：http://csu.dashuyun.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iss.yj20258.top

Ruby: def greet; @name; end
来源：http://rui.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://pwh.hammf.cn

[G05] 继承
来源：http://dys.cqqwz.cn

Py:   class Admin(User): pass
来源：http://keg.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://vph.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://rde.jianghu66.top

TS:   class Admin extends User {}
来源：http://ajm.jinqigufen.top

Java: class Admin extends User {}
来源：http://cui.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://old.haohaochexian.top

Ruby: class Admin < User; end
来源：http://zxs.yangfankeji.com

C#:   class Admin : User {}
来源：http://tre.hammf.cn

[G06] 重写方法
来源：http://nwc.yonumen.top

Py:   def greet(self): return "admin"
来源：http://jeh.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://llx.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://azq.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://ptn.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://jtd.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jkd.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://cvx.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://thk.cashguo.top

[G07] 调用父类方法
来源：http://gub.xuetiantiany.cn

Py:   super().greet()
来源：http://mfa.yonumen.top

PHP:  parent::greet();
来源：http://aqf.jinqigfzy.top

JS:   super.greet();
来源：http://zef.fanxiaobao.xyz

TS:   super.greet();
来源：http://zec.hesvh.cn

Java: super.greet();
来源：http://vll.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wbq.yongpay.top

Ruby: super
来源：http://mqo.chenjidiqi.icu

C#:   base.Greet();
来源：http://awv.sweek.top

[G08] 静态方法与属性
来源：http://fnw.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dlf.nanxuanxn.top

PHP:  public static function f() {}
来源：http://ufa.mhx1999.top

JS:   static f() {}
来源：http://mto.ppjwa.cn

TS:   static f(): void {}
来源：http://fum.yongpay.top

Java: static void f() {}
来源：http://aer.shangyingyoupin.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xsa.svipenyu.cn

Ruby: def self.f; end
来源：http://oaj.tanke756.top

C#:   public static void F() {}
来源：http://yfd.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://jbs.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://kaz.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zyh.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gvl.xuanzx.com

TS:   interface Shape { area(): number; }
来源：http://aiz.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://kiz.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://hqw.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://arl.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://tlt.fanxiaobao.xyz

[G10] 访问控制
来源：http://wzw.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://pfe.jqgfzy.top

PHP:  public / protected / private
来源：http://fzf.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://lyb.yj20258888.top

TS:   public / protected / private
来源：http://buv.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://hsd.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://iet.xziqi.cn

Ruby: public / protected / private
来源：http://kqx.chenzaomai.com

C#:   public / protected / private / internal
来源：http://dvy.jinghuilouyu.cn

[G11] getter / setter
来源：http://dqc.tianlin.xyz

Py:   @property 与 @x.setter
来源：http://aly.snrcjt.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lmb.hammf.cn

JS:   get name() { return this._name; }
来源：http://vxj.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://tcb.jqgfzy.top

Java: public String getName() { return name; }
来源：http://ihf.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gij.iojbl.cn

Ruby: attr_accessor :name
来源：http://yeq.52xcode.cn

C#:   public string Name { get; set; }
来源：http://mrj.gogol.net.cn

[G12] 对象转字符串
来源：http://ebg.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://qbz.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cwd.yongpay.top

JS:   toString() { return this.name; }
来源：http://xvm.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://siy.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://ilp.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://thu.smart0.xyz

Ruby: def to_s; @name; end
来源：http://suw.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://zak.yonumen.top

[G13] 判断对象类型
来源：http://ucv.pengpengdd.cyou

Py:   isinstance(u, User)
来源：http://bhd.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://ncs.ybcxt.top

JS:   u instanceof User
来源：http://ulf.jqgufenzy.top

TS:   u instanceof User
来源：http://gow.ybcxt.top

Java: u instanceof User
来源：http://wre.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bnl.fzhhl.top

Ruby: u.is_a?(User)
来源：http://izx.yangfankeji.com

C#:   u is User
来源：http://jjz.hnqzz.top

[G14] 数据类 / record
来源：http://sek.svipenyu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ask.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://zln.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wce.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://ere.xylfe.cn

Java: record User(String name, int age) {}
来源：http://xum.gaohongyu789.top

Go:   type User struct { Name string; Age int }
来源：http://nmd.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tpy.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://leb.cheryme.top

[G15] 枚举
来源：http://fob.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rhy.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oxq.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://smr.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ygd.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://qti.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ysa.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://xdm.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bnv.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://pxs.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://neh.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://svm.gzhubu.top

JS:   Object.entries(obj)
来源：http://bia.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://ksp.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rfh.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lgr.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://qfn.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://tbo.redwolf501.top

================================================================================
来源：http://ela.bbcook.cn

H. 异常与错误处理
来源：http://nwf.zhixingplan.top

================================================================================
来源：http://ngf.chenjidiqi.icu

[H01] try / catch 基础
来源：http://ogq.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://syp.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vdv.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mrw.sysykeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wrv.hysaishi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdf.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dby.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://syc.cucudq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://onq.aizwys.cn

[H02] finally / ensure 收尾
来源：http://rbe.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ave.sweek.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://max.zhongyouzk.top

JS:   try { f(); } finally { cleanup(); }
来源：http://aun.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://lql.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jyk.cqqwz.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pjx.guowangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://azb.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qyi.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://itu.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://ypp.bjfxy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fos.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://hzu.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://zag.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://faw.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uud.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yla.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://lqv.fengsongda.top

[H04] 自定义异常类型
来源：http://pza.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://yln.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://kjf.fktsv.cn

JS:   class MyError extends Error {}
来源：http://vkp.shzxlz.cn

TS:   class MyError extends Error {}
来源：http://xuh.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://hgi.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ppe.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://jzi.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://gsx.wangdashe.top

[H05] 捕获特定类型
来源：http://lah.gotoacloud.top

Py:   except ValueError as e:
来源：http://tyd.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbi.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://cuy.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://qwo.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://kbd.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dnv.shzxlz.cn

Ruby: rescue ArgumentError => e
来源：http://qmq.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rnn.gaohongyu789.top

[H06] 可选值 / 空值安全访问
来源：http://aee.yuxming.cn

Py:   value = d.get("k") or default
来源：http://gxm.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://kfc.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://tlt.vqdsnc.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rob.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ghm.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zsh.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://glo.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://hao.ehwqpu.com

[H07] 断言
来源：http://amp.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://fzy.xuanzx.com

PHP:  assert($x > 0);
来源：http://ruv.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://iol.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://wng.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://pwh.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aqi.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nkn.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://zxh.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://rzf.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://wox.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zfs.gotoacloud.top

JS:   e.message;  e.stack
来源：http://snp.yuxming.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tgf.epnwcf.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wot.fengsongda.top

Go:   err.Error()
来源：http://rws.haohaochexian.top

Ruby: e.message;  e.backtrace
来源：http://djv.yj202588.top

C#:   e.Message;  e.StackTrace
来源：http://vru.meibo888.top

[H09] 带错误码的异常
来源：http://utd.zdqjudy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nfq.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vgn.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qfy.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uvl.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qjy.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bkw.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://xig.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lvk.jinqigufen.top

[H10] 资源自动释放
来源：http://fse.ybcxt.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mml.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qgf.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tbt.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dyp.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://omb.yj20258888.top

Go:   defer f.Close()
来源：http://qkz.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mir.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xzj.ybcxt.top

================================================================================
来源：http://gri.yonumen.top

I. 正则表达式
来源：http://bzk.vqdsnc.cn

================================================================================
来源：http://wko.cheryme.top

[I01] 判断是否匹配
来源：http://vjl.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zwm.pengpengdd.cyou

PHP:  preg_match('/\d+/', $s);
来源：http://qjr.nwbrower.top

JS:   /\d+/.test(s)
来源：http://yej.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://fta.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ivd.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jin.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://ijy.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://joh.sxryk.cn

[I02] 提取所有匹配
来源：http://rgc.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://izh.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xxh.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rbx.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://rzy.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mfo.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vpy.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://swf.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blf.yfazqb.com

[I03] 提取捕获分组
来源：http://ycf.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://whm.ywan-chungtsiang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qbq.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://acq.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fyn.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jge.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xec.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://for.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://phi.xuetiantiany.cn

[I04] 正则替换
来源：http://awc.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://mxb.cashguo.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kjr.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://fzw.jqgufenzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://fqs.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://aqj.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ubz.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hov.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bwc.sysykeji.top

[I05] 按正则拆分
来源：http://pcv.haohaochexian.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bck.svipenyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pdd.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://qtg.nwbrower.top

TS:   s.split(/\s*,\s*/)
来源：http://dsb.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://iuy.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nvp.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://wsl.pycfn.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oek.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dic.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tyc.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rno.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://knt.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rhj.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://swa.ybcxt.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tkj.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hvn.gzhubu.top


<!-- 参考信息 -->