代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uod.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mqh.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lbx.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dvh.ehwqpu.com

================================================================================
来源：http://euk.pycfn.com

G. 面向对象
来源：http://tdh.ywan-chungtsiang.top

================================================================================
来源：http://miv.dashuyun.cn

[G01] 定义类
来源：http://aud.sxryk.cn

Py:   class User: pass
来源：http://hzp.sysykeji.top

PHP:  class User {}
来源：http://the.wangshuangyany.cn

JS:   class User {}
来源：http://bfy.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://kdi.xziqi.cn

Java: class User {}
来源：http://icm.zhixingplan.top

Go:   type User struct { Name string }
来源：http://qep.yj20258.top

Ruby: class User; end
来源：http://uwe.jinyuanbaomall.cn

C#:   class User {}
来源：http://cuw.jqgufenzy.top

[G02] 构造函数
来源：http://nib.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://qbj.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://ufd.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://eis.cashguo.top

TS:   constructor(public name: string) {}
来源：http://gvm.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://ijf.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ury.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://qqw.mhx1999.top

C#:   public User(string name) { Name = name; }
来源：http://mgz.fanxiaobao.xyz

[G03] 实例属性
来源：http://uay.yj20258.top

Py:   self.name = "x"
来源：http://vrz.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://iii.haohaochexian.top

JS:   this.name = "x";
来源：http://eko.gaohongyu789.top

TS:   name: string = "x";
来源：http://lwt.zhaomingkeji.xyz

Java: private String name;
来源：http://xxg.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qsq.gzhubu.top

Ruby: @name = "x"
来源：http://rbk.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://erm.haohaochexian.top

[G04] 定义方法
来源：http://czj.mhx1999.top

Py:   def greet(self): return self.name
来源：http://lwb.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ocb.chenzaomai.com

JS:   greet() { return this.name; }
来源：http://gri.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://fqi.tianlin.xyz

Java: String greet() { return name; }
来源：http://rjt.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://doz.jqgfzy.top

Ruby: def greet; @name; end
来源：http://qxi.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://ntq.fzhhl.top

[G05] 继承
来源：http://dvg.ehwqpu.com

Py:   class Admin(User): pass
来源：http://cjq.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://cjk.guowangkeji.top

JS:   class Admin extends User {}
来源：http://jdi.zhengqikj.top

TS:   class Admin extends User {}
来源：http://jgj.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://akc.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bug.cdnleiting.top

Ruby: class Admin < User; end
来源：http://vlm.hesvh.cn

C#:   class Admin : User {}
来源：http://pgu.dashuyun.cn

[G06] 重写方法
来源：http://wnx.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://rbo.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jif.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://ttj.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://jdf.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://pbf.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ulb.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://pzj.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://mbg.aizwys.cn

[G07] 调用父类方法
来源：http://ebo.wangshuangyany.cn

Py:   super().greet()
来源：http://vdu.jqgufenzy.top

PHP:  parent::greet();
来源：http://hel.nanxinkj.top

JS:   super.greet();
来源：http://cvc.yj20258.top

TS:   super.greet();
来源：http://yul.zhijiandao.cn

Java: super.greet();
来源：http://wvm.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://snw.meibo888.top

Ruby: super
来源：http://qod.dianchejie.cn

C#:   base.Greet();
来源：http://xlp.ivvv.top

[G08] 静态方法与属性
来源：http://how.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aif.hfpthk.cn

PHP:  public static function f() {}
来源：http://vdw.hesvh.cn

JS:   static f() {}
来源：http://pff.aizwys.cn

TS:   static f(): void {}
来源：http://mnn.c1oappe.top

Java: static void f() {}
来源：http://ozh.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fnh.quarkkingdee.top

Ruby: def self.f; end
来源：http://gyk.yangfankeji.com

C#:   public static void F() {}
来源：http://ttz.yueranfly.top

[G09] 接口 / 抽象类
来源：http://kyq.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://usw.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://sht.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tcr.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://rnu.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://tgn.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://bge.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kjo.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://zij.snrcjt.cn

[G10] 访问控制
来源：http://bam.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://gyy.gzhubu.top

PHP:  public / protected / private
来源：http://tzi.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://tgx.ybcxt.top

TS:   public / protected / private
来源：http://zli.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://qvq.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lnx.ydzc1.top

Ruby: public / protected / private
来源：http://byx.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://sxg.cqqwz.cn

[G11] getter / setter
来源：http://iye.yonumen.top

Py:   @property 与 @x.setter
来源：http://iho.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ngc.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://mhf.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://wip.shangyingyoupin.top

Java: public String getName() { return name; }
来源：http://hyw.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://knr.zdqjudy.top

Ruby: attr_accessor :name
来源：http://ois.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://mrk.epnwcf.com

[G12] 对象转字符串
来源：http://gdz.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://sty.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://vzr.vehdjk.com

JS:   toString() { return this.name; }
来源：http://zcb.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://dlf.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://pgd.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://fyo.andypj.xyz

Ruby: def to_s; @name; end
来源：http://wey.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://msy.jyoumei.cn

[G13] 判断对象类型
来源：http://whm.wangdashe.top

Py:   isinstance(u, User)
来源：http://rxc.vqdsnc.cn

PHP:  $u instanceof User
来源：http://jht.aizwys.cn

JS:   u instanceof User
来源：http://beu.9152youxi.cn

TS:   u instanceof User
来源：http://hcz.ehwqpu.com

Java: u instanceof User
来源：http://yya.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://yij.chenzaomai.com

Ruby: u.is_a?(User)
来源：http://ghv.sweek.top

C#:   u is User
来源：http://xof.mhx1999.top

[G14] 数据类 / record
来源：http://dbf.xingfuxueyuan.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://loc.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://dtc.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rxe.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://uqy.tarul.cn

Java: record User(String name, int age) {}
来源：http://ejs.feifeiyinyue.top

Go:   type User struct { Name string; Age int }
来源：http://mkt.sxryk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hcf.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://mkd.sxryk.cn

[G15] 枚举
来源：http://cvk.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://icw.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vqy.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qlm.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vmr.shuidangran.top

Java: enum Color { RED, GREEN }
来源：http://xmm.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ann.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://xxv.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ikm.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://uxy.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kch.aibaodan.cn

PHP:  get_object_vars($obj);
来源：http://kqa.smart0.xyz

JS:   Object.entries(obj)
来源：http://kfi.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://nqk.cucudq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rpa.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://btk.ehwqpu.com

Ruby: obj.instance_variables
来源：http://fsh.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://pej.yangfankeji.com

================================================================================
来源：http://nzi.ybcxt.top

H. 异常与错误处理
来源：http://qql.xziqi.cn

================================================================================
来源：http://dpn.vehdjk.com

[H01] try / catch 基础
来源：http://svi.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfg.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ntd.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrk.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ezu.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zyo.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://joy.snrcjt.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rdr.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://crj.yfazqb.com

[H02] finally / ensure 收尾
来源：http://flu.epnwcf.com

Py:   try: f()⏎finally: cleanup()
来源：http://heg.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hat.xylfe.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ner.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ybc.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://whs.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://smq.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cuz.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mev.ehwqpu.com

[H03] 主动抛出异常
来源：http://nrl.dashuyun.cn

Py:   raise ValueError("错误信息")
来源：http://ync.jinqigfzy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xkr.nwbrower.top

JS:   throw new Error("错误信息");
来源：http://lnr.yongpay.top

TS:   throw new Error("错误信息");
来源：http://szq.feifeiyinyue.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mbi.zdqjudy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://toh.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mdh.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aot.xziqi.cn

[H04] 自定义异常类型
来源：http://hqk.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://oti.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jky.sweek.top

JS:   class MyError extends Error {}
来源：http://ike.tarul.cn

TS:   class MyError extends Error {}
来源：http://rcx.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://ymw.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nzu.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://mkb.daxiang520.top

C#:   class MyException : Exception {}
来源：http://wng.snrcjt.cn

[H05] 捕获特定类型
来源：http://bur.zhoulong.xyz

Py:   except ValueError as e:
来源：http://wlv.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wjt.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://jar.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://zve.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://sht.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cgm.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://mle.jiagoushi.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uil.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://kfm.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://lbd.andypj.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://muk.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ohd.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://pjj.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://epm.kuanghao11.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wsq.pycfn.com

Ruby: d&.dig(:a, :b)
来源：http://iqd.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://fzy.epnwcf.com

[H07] 断言
来源：http://esv.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://qin.sweek.top

PHP:  assert($x > 0);
来源：http://wgv.bjfxy.top

JS:   console.assert(x > 0);
来源：http://xzw.xuanzx.com

TS:   console.assert(x > 0);
来源：http://feh.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://drf.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bcc.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://giq.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://iau.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://wke.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://jqt.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bqh.yongpay.top

JS:   e.message;  e.stack
来源：http://cgt.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://xqf.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jil.ppjwa.cn

Go:   err.Error()
来源：http://ukm.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://gho.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://tmg.hongshengwenyu.top

[H09] 带错误码的异常
来源：http://igu.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fxg.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rwe.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dte.havefunace.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tgo.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qsw.ivvv.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://khy.daria6918.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ewc.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://awa.yj20258.top

[H10] 资源自动释放
来源：http://dca.yonumen.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oqo.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xte.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vyb.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://snc.xuanzx.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xdk.bjfxy.top

Go:   defer f.Close()
来源：http://gnv.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uln.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jra.gaohongyu789.top

================================================================================
来源：http://rhm.jyoumei.cn

I. 正则表达式
来源：http://lkf.mhx1999.top

================================================================================
来源：http://xsk.316326.xyz

[I01] 判断是否匹配
来源：http://kdl.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hya.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rqy.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://scl.tian-w.cn

TS:   /\d+/.test(s)
来源：http://kij.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bhj.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nsi.cdnleiting.top

Ruby: s.match?(/\d+/)
来源：http://jgw.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rik.gzhubu.top

[I02] 提取所有匹配
来源：http://nhc.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://eaw.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aiy.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dcu.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://hdw.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pci.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wud.jiagoushi.top

Ruby: s.scan(/\d+/)
来源：http://vca.fktsv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nwh.jianghu66.top

[I03] 提取捕获分组
来源：http://jzj.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jji.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bfr.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eig.jinqigufen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pwb.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://snn.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dpv.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xvs.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tzm.fehbvm.com

[I04] 正则替换
来源：http://nhz.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tdm.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://juq.jyoumei.cn

JS:   s.replace(/\d+/g, "#")
来源：http://naq.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://nkj.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://qun.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pnq.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yzl.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uev.zhiwuduotai.top

[I05] 按正则拆分
来源：http://fxn.bbcook.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://stl.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://woh.zhoulong.xyz

JS:   s.split(/\s*,\s*/)
来源：http://alk.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://ujm.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://rli.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cbl.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://hrc.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wzt.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qsq.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nfd.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://til.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sic.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nnq.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fge.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jvw.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://liw.dashuyun.cn


<!-- 参考信息 -->