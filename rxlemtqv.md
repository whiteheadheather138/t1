代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzb.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dhe.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oig.sufxvd.cn

TS:   // 同上
来源：http://lht.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gua.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mhf.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rvq.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rgm.xuanzx.com

================================================================================
来源：http://ine.sufxvd.cn

G. 面向对象
来源：http://uzf.hcnkem.com

================================================================================
来源：http://hrl.xylfe.cn

[G01] 定义类
来源：http://qiq.gogol.net.cn

Py:   class User: pass
来源：http://fuh.zhongyouzk.top

PHP:  class User {}
来源：http://rny.snrcjt.cn

JS:   class User {}
来源：http://bhe.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://xvz.dianchejie.cn

Java: class User {}
来源：http://jqy.hcnkem.com

Go:   type User struct { Name string }
来源：http://vzl.iojbl.cn

Ruby: class User; end
来源：http://shl.pengpengdd.cyou

C#:   class User {}
来源：http://see.cheryme.top

[G02] 构造函数
来源：http://hkb.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ran.vqdsnc.cn

PHP:  public function __construct(public string $name) {}
来源：http://jfa.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://qpc.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://cun.zhengqikj.top

Java: User(String name) { this.name = name; }
来源：http://bgu.zhaomingkeji.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xmp.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://cvk.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://oun.bjfxy.top

[G03] 实例属性
来源：http://jug.hongshengwenyu.top

Py:   self.name = "x"
来源：http://wyp.hysaishi.cn

PHP:  public string $name = "x";
来源：http://isf.chenlongwang.top

JS:   this.name = "x";
来源：http://kld.guannengcc.top

TS:   name: string = "x";
来源：http://ein.hnqzz.top

Java: private String name;
来源：http://zcc.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvl.hesvh.cn

Ruby: @name = "x"
来源：http://kxz.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://sez.sysykeji.top

[G04] 定义方法
来源：http://kwf.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://yfk.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxa.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://siq.nanxinkj.top

TS:   greet(): string { return this.name; }
来源：http://yph.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://ksw.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gsz.wangdashe.top

Ruby: def greet; @name; end
来源：http://ocv.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://yvv.mhx1999.top

[G05] 继承
来源：http://hbo.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://xea.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://xtv.9152youxi.cn

JS:   class Admin extends User {}
来源：http://sgp.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://dqy.jinqigfzy.top

Java: class Admin extends User {}
来源：http://dvq.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kna.gotoacloud.top

Ruby: class Admin < User; end
来源：http://hpx.jlsjyb.cn

C#:   class Admin : User {}
来源：http://iir.zhaomingkeji.xyz

[G06] 重写方法
来源：http://kns.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://bxf.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mzy.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://qrx.jinqigufen.top

TS:   greet(): string { return "admin"; }
来源：http://tsk.tarul.cn

Java: @Override String greet() { return "admin"; }
来源：http://awe.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dkf.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://wkx.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://lpv.yj20258.top

[G07] 调用父类方法
来源：http://qir.jinghuilouyu.cn

Py:   super().greet()
来源：http://suy.fzhhl.top

PHP:  parent::greet();
来源：http://bhl.jianghu66.top

JS:   super.greet();
来源：http://nak.xuanzx.com

TS:   super.greet();
来源：http://uhh.shzxlz.cn

Java: super.greet();
来源：http://xga.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kdp.zhixingplan.top

Ruby: super
来源：http://jzh.zycfv.cn

C#:   base.Greet();
来源：http://bsw.vehdjk.com

[G08] 静态方法与属性
来源：http://bho.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://urh.chenzaomai.com

PHP:  public static function f() {}
来源：http://xfd.hywenlv.cn

JS:   static f() {}
来源：http://mdt.yfazqb.com

TS:   static f(): void {}
来源：http://vib.andypj.xyz

Java: static void f() {}
来源：http://qgv.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://edk.tianlin.xyz

Ruby: def self.f; end
来源：http://htw.uphjek.com

C#:   public static void F() {}
来源：http://pul.meibo888.top

[G09] 接口 / 抽象类
来源：http://vjk.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://xjt.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://xyg.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://elc.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://kqg.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://xww.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://nuw.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gsy.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://btv.yfazqb.com

[G10] 访问控制
来源：http://qii.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://ggp.epnwcf.com

PHP:  public / protected / private
来源：http://soz.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://ioe.yuanzhike.top

TS:   public / protected / private
来源：http://lwh.guannengcc.top

Java: public / protected / private / 默认包级
来源：http://oha.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uvh.chenzaomai.com

Ruby: public / protected / private
来源：http://jin.52xcode.cn

C#:   public / protected / private / internal
来源：http://xys.svipenyu.cn

[G11] getter / setter
来源：http://mnn.316326.xyz

Py:   @property 与 @x.setter
来源：http://hoc.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fop.xylfe.cn

JS:   get name() { return this._name; }
来源：http://dah.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://sux.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://cne.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qlu.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://kpe.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://lna.shzxlz.cn

[G12] 对象转字符串
来源：http://zmu.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://ilw.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vih.zycfv.cn

JS:   toString() { return this.name; }
来源：http://uup.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://swy.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://mwv.hammf.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lht.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://ezd.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://wju.ydzc1.top

[G13] 判断对象类型
来源：http://yun.tianlin.xyz

Py:   isinstance(u, User)
来源：http://usw.ydjk.org.cn

PHP:  $u instanceof User
来源：http://fyq.c1oappe.top

JS:   u instanceof User
来源：http://uzs.ivvv.top

TS:   u instanceof User
来源：http://ryu.hywenlv.cn

Java: u instanceof User
来源：http://jhu.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jjt.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://ntr.ydzc1.top

C#:   u is User
来源：http://vdn.smart0.xyz

[G14] 数据类 / record
来源：http://jce.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ioe.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://xvj.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://qgx.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://inw.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://mrt.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://hih.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mjj.zycfv.cn

C#:   record User(string Name, int Age);
来源：http://auw.chenjidiqi.icu

[G15] 枚举
来源：http://xaz.hnqzz.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fne.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mdf.havefunace.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yoj.316326.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sdw.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://vqp.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://amu.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://qks.guannengcc.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vri.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://sxg.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wsk.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://pzh.xuetiantiany.cn

JS:   Object.entries(obj)
来源：http://amj.ehwqpu.com

TS:   Object.entries(obj)
来源：http://tbu.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uoi.sysykeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://pfw.nwbrower.top

Ruby: obj.instance_variables
来源：http://mii.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://nxc.guannengcc.top

================================================================================
来源：http://qyb.hfpthk.cn

H. 异常与错误处理
来源：http://cbv.epnwcf.com

================================================================================
来源：http://ika.jinqigufen.top

[H01] try / catch 基础
来源：http://vae.yueranfly.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cbg.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://csp.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zes.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bfn.zhengqikj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xfz.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cgd.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://itp.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gtv.fktsv.cn

[H02] finally / ensure 收尾
来源：http://ssz.c1oappe.top

Py:   try: f()⏎finally: cleanup()
来源：http://ege.yongpay.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://txy.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://pau.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://msz.gaohongyu789.top

Java: try { f(); } finally { cleanup(); }
来源：http://spw.fzhhl.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aas.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://exl.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qay.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://dkq.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://zwu.iojbl.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aok.snrcjt.cn

JS:   throw new Error("错误信息");
来源：http://ohm.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://hcv.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://gpv.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hta.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://crq.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://ykv.52xcode.cn

[H04] 自定义异常类型
来源：http://gcl.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://qms.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://hal.yongpay.top

JS:   class MyError extends Error {}
来源：http://iyj.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://zjw.pycfn.com

Java: class MyException extends RuntimeException {}
来源：http://ect.epnwcf.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vet.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://adt.gzhubu.top

C#:   class MyException : Exception {}
来源：http://ftf.wangdashe.top

[H05] 捕获特定类型
来源：http://rnt.gaohongyu789.top

Py:   except ValueError as e:
来源：http://moz.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hlc.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://pgo.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://dkm.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://apl.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pwg.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://nat.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iwh.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://kxq.fehbvm.com

Py:   value = d.get("k") or default
来源：http://jbj.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mjx.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://mll.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ynh.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dzm.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jiy.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://bro.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://llv.vqdsnc.cn

[H07] 断言
来源：http://ntx.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://fjl.nanxuanxn.top

PHP:  assert($x > 0);
来源：http://cwj.bjfxy.top

JS:   console.assert(x > 0);
来源：http://cer.yvedp.cn

TS:   console.assert(x > 0);
来源：http://lvy.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://luq.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mlz.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mdx.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://slr.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://dij.ybcxt.top

Py:   str(e);  traceback.format_exc()
来源：http://ogz.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://caq.daxiang520.top

JS:   e.message;  e.stack
来源：http://nos.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://tij.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dqt.ppjwa.cn

Go:   err.Error()
来源：http://qih.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://omf.haohaochexian.top

C#:   e.Message;  e.StackTrace
来源：http://dil.dashuyun.cn

[H09] 带错误码的异常
来源：http://ctn.yueranfly.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bgf.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lld.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tjd.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://isn.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rkh.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpu.uphjek.com

Ruby: raise MyError.new("fail", 500)
来源：http://lsy.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tth.shzxlz.cn

[H10] 资源自动释放
来源：http://fji.jqgfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cka.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dgr.hysaishi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awz.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wdy.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tnz.yonumen.top

Go:   defer f.Close()
来源：http://bid.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lhm.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ojy.yj20258888.top

================================================================================
来源：http://lql.chenzaomai.com

I. 正则表达式
来源：http://kfy.aibaodan.cn

================================================================================
来源：http://lci.nanxuanxn.top

[I01] 判断是否匹配
来源：http://igm.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qqs.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://rfv.yanxiufei.cn

JS:   /\d+/.test(s)
来源：http://qko.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://svl.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eqd.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ltz.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://ydt.xylfe.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cwg.ivvv.top

[I02] 提取所有匹配
来源：http://uvi.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://spu.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nyy.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ejs.tarul.cn

TS:   s.match(/\d+/g)
来源：http://woq.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oim.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pzf.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://iqu.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dfd.sxryk.cn

[I03] 提取捕获分组
来源：http://tpd.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rhg.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pan.chenzaomai.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pae.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dxf.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jxe.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ays.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zwt.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gus.yuanzhike.top

[I04] 正则替换
来源：http://fgp.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zyt.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mqv.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://zvo.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hsm.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://xht.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gsl.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://mfg.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nen.jianghu66.top

[I05] 按正则拆分
来源：http://fwj.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ckb.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jev.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://qim.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://alh.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://xme.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bsw.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://gog.chenlongwang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yqb.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kru.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wss.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sjk.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oho.gzhubu.top


<!-- 参考信息 -->