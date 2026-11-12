代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cen.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tan.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://caj.shanyushiyangkeji.top

TS:   // 同上
来源：http://atd.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wcp.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sno.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xfg.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mbr.zhaomingkeji.xyz

================================================================================
来源：http://lib.shzxlz.cn

G. 面向对象
来源：http://msv.ydjk.org.cn

================================================================================
来源：http://mki.zhiwuduotai.top

[G01] 定义类
来源：http://hxb.mhx1999.top

Py:   class User: pass
来源：http://taf.kuanghao11.cn

PHP:  class User {}
来源：http://gas.0kj1m.cn

JS:   class User {}
来源：http://uom.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://lao.cucudq.cn

Java: class User {}
来源：http://uao.chenlongwang.top

Go:   type User struct { Name string }
来源：http://lye.pengpengdd.cyou

Ruby: class User; end
来源：http://har.hysaishi.cn

C#:   class User {}
来源：http://zmj.fengsongda.top

[G02] 构造函数
来源：http://dgh.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://klx.chenlongwang.top

PHP:  public function __construct(public string $name) {}
来源：http://fpe.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://all.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://ida.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://tbx.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ebx.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://gqn.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://xrr.jqgufenzy.top

[G03] 实例属性
来源：http://brs.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://sgy.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://mdf.vehdjk.com

JS:   this.name = "x";
来源：http://jbq.hammf.cn

TS:   name: string = "x";
来源：http://zcy.jinqigfzy.top

Java: private String name;
来源：http://drj.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://msj.daxiang520.top

Ruby: @name = "x"
来源：http://iil.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://fgh.snrcjt.cn

[G04] 定义方法
来源：http://fen.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://tis.gaohongyu789.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dew.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://fnj.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://dat.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://ygc.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://pjw.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://xfq.zhaomingkeji.xyz

C#:   public string Greet() => Name;
来源：http://uql.aizwys.cn

[G05] 继承
来源：http://wie.xylfe.cn

Py:   class Admin(User): pass
来源：http://yax.yj20258.top

PHP:  class Admin extends User {}
来源：http://olz.smart0.xyz

JS:   class Admin extends User {}
来源：http://ycu.zycfv.cn

TS:   class Admin extends User {}
来源：http://znz.zhoulong.xyz

Java: class Admin extends User {}
来源：http://cdi.sjlbkw.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gff.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://gkq.ctjpmb.com

C#:   class Admin : User {}
来源：http://cjo.smart0.xyz

[G06] 重写方法
来源：http://imp.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://mqf.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oac.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://fiu.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://zqd.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://aba.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vvo.uphjek.com

Ruby: def greet; "admin"; end
来源：http://ork.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://qyi.guowangkeji.top

[G07] 调用父类方法
来源：http://rad.redwolf501.top

Py:   super().greet()
来源：http://tsm.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://znv.ppjwa.cn

JS:   super.greet();
来源：http://ekd.epnwcf.com

TS:   super.greet();
来源：http://hlw.fanxiaobao.xyz

Java: super.greet();
来源：http://wjb.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rme.fanxiaobao.xyz

Ruby: super
来源：http://quw.0kj1m.cn

C#:   base.Greet();
来源：http://yfx.aibaodan.cn

[G08] 静态方法与属性
来源：http://gid.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xfu.jianghu66.top

PHP:  public static function f() {}
来源：http://nhl.ydjk.org.cn

JS:   static f() {}
来源：http://yzp.quarkkingdee.top

TS:   static f(): void {}
来源：http://lks.ehwqpu.com

Java: static void f() {}
来源：http://rmr.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nxw.jyoumei.cn

Ruby: def self.f; end
来源：http://ajj.pengpengdd.cyou

C#:   public static void F() {}
来源：http://tei.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://wml.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://qll.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://dbt.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://hck.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://rfa.fzhhl.top

Java: interface Shape { double area(); }
来源：http://fbw.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://ath.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mqz.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://pta.haohaochexian.top

[G10] 访问控制
来源：http://kta.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://hua.gaohongyu789.top

PHP:  public / protected / private
来源：http://htv.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://jgr.jinqigufen.top

TS:   public / protected / private
来源：http://cif.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://qkc.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qev.zhoulong.xyz

Ruby: public / protected / private
来源：http://uiq.ehwqpu.com

C#:   public / protected / private / internal
来源：http://kxm.sweek.top

[G11] getter / setter
来源：http://nyu.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://roz.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://lzv.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://hkb.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://nnd.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://yns.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mtq.vehdjk.com

Ruby: attr_accessor :name
来源：http://iph.hcnkem.com

C#:   public string Name { get; set; }
来源：http://fsz.dashuyun.cn

[G12] 对象转字符串
来源：http://hrq.ehwqpu.com

Py:   def __str__(self): return self.name
来源：http://ale.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://miv.yuxming.cn

JS:   toString() { return this.name; }
来源：http://fep.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://oke.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://xgp.yuanzhike.top

Go:   func (u User) String() string { return u.Name }
来源：http://fgi.birdmap.top

Ruby: def to_s; @name; end
来源：http://ztw.gogol.net.cn

C#:   public override string ToString() => Name;
来源：http://mej.cdnleiting.top

[G13] 判断对象类型
来源：http://sgi.tanke756.top

Py:   isinstance(u, User)
来源：http://bdz.nwbrower.top

PHP:  $u instanceof User
来源：http://anm.dianchejie.cn

JS:   u instanceof User
来源：http://rmg.sufxvd.cn

TS:   u instanceof User
来源：http://jsv.meibo888.top

Java: u instanceof User
来源：http://ect.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xsq.dianchejie.cn

Ruby: u.is_a?(User)
来源：http://fln.aizwys.cn

C#:   u is User
来源：http://bpc.shangyingyoupin.top

[G14] 数据类 / record
来源：http://kjs.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lig.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://yct.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://jgu.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://otr.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://uxw.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://kqb.zhengqikj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vgx.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://gyk.xylfe.cn

[G15] 枚举
来源：http://mxx.sysykeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ads.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kjd.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ixe.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rmb.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://yxh.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://knw.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://hdc.shuidangran.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bxm.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://rxi.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://odo.chenjidiqi.icu

PHP:  get_object_vars($obj);
来源：http://psq.fengsongda.top

JS:   Object.entries(obj)
来源：http://tyi.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://jof.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xlw.ctjpmb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://gmi.zhengqikj.top

Ruby: obj.instance_variables
来源：http://rva.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://onc.aibaodan.cn

================================================================================
来源：http://mqn.fzhhl.top

H. 异常与错误处理
来源：http://gku.fzhhl.top

================================================================================
来源：http://weq.wangdashe.top

[H01] try / catch 基础
来源：http://dvz.vehdjk.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yol.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tdt.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oym.yvedp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oaq.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://viw.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vxg.bbcook.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jej.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kwc.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://wal.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gnn.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ntn.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://bwm.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wer.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fuq.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wyo.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://zzr.c1oappe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yag.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://znf.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://uoy.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hgo.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://ann.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://uwz.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mck.wangdashe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ska.zhaomingkeji.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ila.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://ldf.yj20258888.top

[H04] 自定义异常类型
来源：http://lkv.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://nry.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xor.tanke756.top

JS:   class MyError extends Error {}
来源：http://ldu.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://fos.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://kku.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fhv.316326.xyz

Ruby: class MyError < StandardError; end
来源：http://fpb.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://hnl.sufxvd.cn

[H05] 捕获特定类型
来源：http://bhv.yonumen.top

Py:   except ValueError as e:
来源：http://ogj.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dyk.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://baq.zhaomingkeji.xyz

TS:   if (e instanceof TypeError) {}
来源：http://cnk.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://rud.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gfs.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://dug.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ylw.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://wtw.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://qmr.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://sms.vehdjk.com

JS:   obj?.a?.b;  d ?? default
来源：http://ncs.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://lnp.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fts.yongpay.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zjv.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://qlg.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://znx.havefunace.top

[H07] 断言
来源：http://ekv.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://lve.zdbjq.cn

PHP:  assert($x > 0);
来源：http://guc.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://lgg.tian-w.cn

TS:   console.assert(x > 0);
来源：http://bbc.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://agh.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ino.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mtu.xziqi.cn

C#:   Debug.Assert(x > 0);
来源：http://jby.sweek.top

[H08] 获取错误信息与堆栈
来源：http://vjd.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://dsn.nanxuanxn.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lnl.yonumen.top

JS:   e.message;  e.stack
来源：http://wmr.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rsm.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://xgm.guowangkeji.top

Go:   err.Error()
来源：http://hul.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://sca.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://riw.jlsjyb.cn

[H09] 带错误码的异常
来源：http://nkh.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lsr.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ciy.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mfd.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vas.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dhv.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uzz.zhaomingkeji.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://gcg.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://xin.gogol.net.cn

[H10] 资源自动释放
来源：http://uaq.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ddx.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rqh.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://slm.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sef.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zry.zycfv.cn

Go:   defer f.Close()
来源：http://trs.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aep.xinyue.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ptm.hnqzz.top

================================================================================
来源：http://lfv.ctjpmb.com

I. 正则表达式
来源：http://ilw.c1oappe.top

================================================================================
来源：http://ahn.yangfankeji.com

[I01] 判断是否匹配
来源：http://ovg.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hav.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://ocq.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://czk.hammf.cn

TS:   /\d+/.test(s)
来源：http://ddu.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cwf.hesvh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bns.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://xaq.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jhm.xinyue.icu

[I02] 提取所有匹配
来源：http://rpy.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://vez.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://omd.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ebn.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://ang.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ald.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rpu.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://otx.jlsjyb.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ykp.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://plv.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lnf.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kwa.tanke756.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vhg.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://img.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zqs.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cdh.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uke.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mtf.redwolf501.top

[I04] 正则替换
来源：http://kld.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vhn.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nde.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tow.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://gow.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://yal.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://zpg.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ykk.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mog.ybcxt.top

[I05] 按正则拆分
来源：http://rdk.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lth.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wci.cdnleiting.top

JS:   s.split(/\s*,\s*/)
来源：http://bfl.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://toc.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://qxe.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ftv.zhixingplan.top

Ruby: s.split(/\s*,\s*/)
来源：http://uph.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://meo.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ssl.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ifa.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zqg.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vuc.dashuyun.cn


<!-- 参考信息 -->