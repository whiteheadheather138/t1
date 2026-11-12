代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rdb.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yjk.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bpk.yuxming.cn

TS:   // 同上
来源：http://zjv.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wbz.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bne.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypd.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://due.zhongyouzk.top

================================================================================
来源：http://sbl.smart0.xyz

G. 面向对象
来源：http://ygt.tianlin.xyz

================================================================================
来源：http://frc.iojbl.cn

[G01] 定义类
来源：http://pvg.vehdjk.com

Py:   class User: pass
来源：http://khk.sxryk.cn

PHP:  class User {}
来源：http://vry.xingfuxueyuan.xyz

JS:   class User {}
来源：http://hum.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://meq.smart0.xyz

Java: class User {}
来源：http://dyg.andypj.xyz

Go:   type User struct { Name string }
来源：http://yyb.bbcook.cn

Ruby: class User; end
来源：http://ocf.xingfuxueyuan.xyz

C#:   class User {}
来源：http://ewh.xuanzx.com

[G02] 构造函数
来源：http://egg.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://xrz.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://wka.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://ohy.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://rqi.sweek.top

Java: User(String name) { this.name = name; }
来源：http://pra.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yzr.guowangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://cmz.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://juu.jlsjyb.cn

[G03] 实例属性
来源：http://nkr.hnxiangtu.top

Py:   self.name = "x"
来源：http://sma.sweek.top

PHP:  public string $name = "x";
来源：http://bnt.yj20258.top

JS:   this.name = "x";
来源：http://ikk.zhijiandao.cn

TS:   name: string = "x";
来源：http://kpw.aibaodan.cn

Java: private String name;
来源：http://ndf.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tfg.zhongyouzk.top

Ruby: @name = "x"
来源：http://trw.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://pqk.ydjk.org.cn

[G04] 定义方法
来源：http://fqh.xziqi.cn

Py:   def greet(self): return self.name
来源：http://bhi.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://grc.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://ehy.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://otx.yj202588.top

Java: String greet() { return name; }
来源：http://ptq.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://opx.tian-w.cn

Ruby: def greet; @name; end
来源：http://zkr.havefunace.top

C#:   public string Greet() => Name;
来源：http://opo.gogol.net.cn

[G05] 继承
来源：http://fgv.chenlongwang.top

Py:   class Admin(User): pass
来源：http://gcw.hnqzz.top

PHP:  class Admin extends User {}
来源：http://vwl.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://cjg.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://ofo.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://vdo.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vkn.cashguo.top

Ruby: class Admin < User; end
来源：http://dnh.havefunace.top

C#:   class Admin : User {}
来源：http://yvy.yonumen.top

[G06] 重写方法
来源：http://xhg.birdmap.top

Py:   def greet(self): return "admin"
来源：http://gsq.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bkh.snrcjt.cn

JS:   greet() { return "admin"; }
来源：http://tes.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://mai.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://oam.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vnw.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://tag.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://lpl.fehbvm.com

[G07] 调用父类方法
来源：http://byb.guowangkeji.top

Py:   super().greet()
来源：http://upf.wangdashe.top

PHP:  parent::greet();
来源：http://qfs.shanyushiyangkeji.top

JS:   super.greet();
来源：http://ukt.daria6918.cn

TS:   super.greet();
来源：http://emb.guannengcc.top

Java: super.greet();
来源：http://eyo.dashuyun.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yic.gaohongyu789.top

Ruby: super
来源：http://haj.nwbrower.top

C#:   base.Greet();
来源：http://yfx.shzxlz.cn

[G08] 静态方法与属性
来源：http://ptg.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mrc.bjfxy.top

PHP:  public static function f() {}
来源：http://oym.zdqjudy.top

JS:   static f() {}
来源：http://okm.tarul.cn

TS:   static f(): void {}
来源：http://edl.yangfankeji.com

Java: static void f() {}
来源：http://jeu.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ruw.tarul.cn

Ruby: def self.f; end
来源：http://uqp.chenzaomai.com

C#:   public static void F() {}
来源：http://eak.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://rux.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://chk.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://zas.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://pyj.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://usf.andypj.xyz

Java: interface Shape { double area(); }
来源：http://gxo.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://ryc.bbcook.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xrt.uphjek.com

C#:   interface IShape { double Area(); }
来源：http://abo.ydzc1.top

[G10] 访问控制
来源：http://tit.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://iof.ydjk.org.cn

PHP:  public / protected / private
来源：http://rpc.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://cpw.sxryk.cn

TS:   public / protected / private
来源：http://lzw.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://zjq.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jth.wangshuangyany.cn

Ruby: public / protected / private
来源：http://ykb.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://uba.guannengcc.top

[G11] getter / setter
来源：http://lcd.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://xzt.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wbj.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://til.cqqwz.cn

TS:   get name(): string { return this._name; }
来源：http://bzx.aizwys.cn

Java: public String getName() { return name; }
来源：http://jdm.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gou.epnwcf.com

Ruby: attr_accessor :name
来源：http://zvl.meibo888.top

C#:   public string Name { get; set; }
来源：http://hou.xylfe.cn

[G12] 对象转字符串
来源：http://klk.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://bdk.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kua.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://vds.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://cgk.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://ctq.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://phk.ybcxt.top

Ruby: def to_s; @name; end
来源：http://gfv.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://vxm.bbcook.cn

[G13] 判断对象类型
来源：http://vad.316326.xyz

Py:   isinstance(u, User)
来源：http://une.snrcjt.cn

PHP:  $u instanceof User
来源：http://lhm.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://apf.pycfn.com

TS:   u instanceof User
来源：http://irv.sxryk.cn

Java: u instanceof User
来源：http://cph.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mcx.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://atz.snrcjt.cn

C#:   u is User
来源：http://edc.gogol.net.cn

[G14] 数据类 / record
来源：http://fme.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rwq.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://pgd.316326.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://kmj.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://roe.tanke756.top

Java: record User(String name, int age) {}
来源：http://ocy.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://pti.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rgs.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://tup.zycfv.cn

[G15] 枚举
来源：http://nng.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jzh.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ngr.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ngi.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yux.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://qpl.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hms.xuanzx.com

Ruby: Color = %i[red green].freeze
来源：http://xxz.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fcx.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://mzz.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pjv.yongpay.top

PHP:  get_object_vars($obj);
来源：http://xpy.nanxinkj.top

JS:   Object.entries(obj)
来源：http://mbi.hammf.cn

TS:   Object.entries(obj)
来源：http://nre.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gdr.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://qlw.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://gwz.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://kbg.shzxlz.cn

================================================================================
来源：http://rxh.hysaishi.cn

H. 异常与错误处理
来源：http://wbu.tanke756.top

================================================================================
来源：http://wsl.cqqwz.cn

[H01] try / catch 基础
来源：http://thw.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://drh.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uwk.yfazqb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mgj.tian-w.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tbu.jlsjyb.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jor.yongpay.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://omv.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kgz.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cnu.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://eyr.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://ehz.zhoulong.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://squ.sjlbkw.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://umz.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://isv.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://kqh.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jjn.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://klj.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://imr.tarul.cn

[H03] 主动抛出异常
来源：http://xie.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://jnj.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gny.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://ijk.yangfankeji.com

TS:   throw new Error("错误信息");
来源：http://hvj.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bcy.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xyr.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://dss.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pyk.chenjidiqi.icu

[H04] 自定义异常类型
来源：http://ccf.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://sbx.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://vhn.hnqzz.top

JS:   class MyError extends Error {}
来源：http://uuw.haohaochexian.top

TS:   class MyError extends Error {}
来源：http://gvi.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://xsx.xuetiantiany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://omf.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://cke.xinyue.icu

C#:   class MyException : Exception {}
来源：http://zvf.zhiwuduotai.top

[H05] 捕获特定类型
来源：http://pqc.xinyue.icu

Py:   except ValueError as e:
来源：http://bqm.xuanzx.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mzc.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://vqs.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ycd.yanxiufei.cn

Java: catch (IOException | SQLException e) {}
来源：http://xgs.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vdj.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://xjo.sjlbkw.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lmp.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://fby.fzhhl.top

Py:   value = d.get("k") or default
来源：http://ogs.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://tis.0kj1m.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ogx.jqgufenzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://qpo.cdnleiting.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ejn.wangdashe.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jnz.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://udi.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://mao.snrcjt.cn

[H07] 断言
来源：http://gsn.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://fmr.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://aqb.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://rhs.hnqzz.top

TS:   console.assert(x > 0);
来源：http://ads.chenzaomai.com

Java: assert x > 0 : "必须为正";
来源：http://nwc.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wtb.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mrb.9152youxi.cn

C#:   Debug.Assert(x > 0);
来源：http://zbt.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://knt.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://osg.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tby.tianlin.xyz

JS:   e.message;  e.stack
来源：http://twz.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xaj.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pje.zdqjudy.top

Go:   err.Error()
来源：http://koj.gotoacloud.top

Ruby: e.message;  e.backtrace
来源：http://gdc.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://lms.ivvv.top

[H09] 带错误码的异常
来源：http://eet.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://owb.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dcu.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qwf.jiagoushi.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iqx.xuetiantiany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yfr.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bzd.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://swz.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eux.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://lba.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://shi.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ifl.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hix.ehwqpu.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmo.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://frb.tanke756.top

Go:   defer f.Close()
来源：http://bxz.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bbb.hnxiangtu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://klc.vqdsnc.cn

================================================================================
来源：http://vut.gotoacloud.top

I. 正则表达式
来源：http://mau.fzhhl.top

================================================================================
来源：http://zom.jqgufenzy.top

[I01] 判断是否匹配
来源：http://zyd.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ghq.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pwu.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://wug.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://ajf.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sed.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zko.bbcook.cn

Ruby: s.match?(/\d+/)
来源：http://yjy.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cok.chenlongwang.top

[I02] 提取所有匹配
来源：http://uuh.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://rjh.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kow.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jko.yongpay.top

TS:   s.match(/\d+/g)
来源：http://vym.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ldo.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://puk.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://mkw.yangfankeji.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://slf.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://xrq.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jdq.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qtq.zdbjq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gxm.gogol.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mgk.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bst.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vuz.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yqp.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sge.ehwqpu.com

[I04] 正则替换
来源：http://ism.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hrg.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zqu.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://muu.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ctx.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hbu.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://plc.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://egx.snrcjt.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mrq.ydzc1.top

[I05] 按正则拆分
来源：http://sxw.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gpm.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xyv.hnqzz.top

JS:   s.split(/\s*,\s*/)
来源：http://zsh.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://esp.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://yyu.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://das.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://qtp.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wsd.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gzr.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bec.chenlongwang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lkg.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yoq.smart0.xyz


<!-- 参考信息 -->