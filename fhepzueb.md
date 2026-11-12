代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kyt.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vfb.hesvh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cav.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xxq.hnqzz.top

================================================================================
来源：http://kxe.fengsongda.top

G. 面向对象
来源：http://red.hysaishi.cn

================================================================================
来源：http://pdq.ybcxt.top

[G01] 定义类
来源：http://yka.dashuyun.cn

Py:   class User: pass
来源：http://tsb.jinqigfzy.top

PHP:  class User {}
来源：http://eax.cheryme.top

JS:   class User {}
来源：http://vkm.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://toc.yuanzhike.top

Java: class User {}
来源：http://fws.cheryme.top

Go:   type User struct { Name string }
来源：http://ppc.xziqi.cn

Ruby: class User; end
来源：http://ypl.zhixingplan.top

C#:   class User {}
来源：http://dvh.zhoulong.xyz

[G02] 构造函数
来源：http://ctb.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://bhg.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://tiz.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://oob.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://wii.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://ywm.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cir.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://vfs.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://bxh.zhiwuduotai.top

[G03] 实例属性
来源：http://uln.aibaodan.cn

Py:   self.name = "x"
来源：http://dky.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://hyt.sjlbkw.cn

JS:   this.name = "x";
来源：http://elw.bbcook.cn

TS:   name: string = "x";
来源：http://uju.zhixingplan.top

Java: private String name;
来源：http://dwe.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oxo.zhongyouzk.top

Ruby: @name = "x"
来源：http://euz.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://bwm.jyoumei.cn

[G04] 定义方法
来源：http://vbv.ivvv.top

Py:   def greet(self): return self.name
来源：http://nfc.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xdq.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://jqi.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://qtw.gotoacloud.top

Java: String greet() { return name; }
来源：http://tqy.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lrz.chenzaomai.com

Ruby: def greet; @name; end
来源：http://cyf.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://kpb.jinqigfzy.top

[G05] 继承
来源：http://rhn.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://zrv.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://ufe.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://nkd.fehbvm.com

TS:   class Admin extends User {}
来源：http://wix.yueranfly.top

Java: class Admin extends User {}
来源：http://vnl.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gon.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://soe.316326.xyz

C#:   class Admin : User {}
来源：http://mbs.tanke756.top

[G06] 重写方法
来源：http://zvs.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://qor.ywan-chungtsiang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vyb.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://bzb.hysaishi.cn

TS:   greet(): string { return "admin"; }
来源：http://oyn.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://jer.mhx1999.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bja.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://wmx.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://gbh.epnwcf.com

[G07] 调用父类方法
来源：http://hvr.smart0.xyz

Py:   super().greet()
来源：http://txo.xuetiantiany.cn

PHP:  parent::greet();
来源：http://ezy.jqgfzy.top

JS:   super.greet();
来源：http://nfy.xuetiantiany.cn

TS:   super.greet();
来源：http://lrp.nwbrower.top

Java: super.greet();
来源：http://lhc.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hbu.hammf.cn

Ruby: super
来源：http://ont.snrcjt.cn

C#:   base.Greet();
来源：http://fgp.ehwqpu.com

[G08] 静态方法与属性
来源：http://fph.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xrb.yuxming.cn

PHP:  public static function f() {}
来源：http://qvq.jianghu66.top

JS:   static f() {}
来源：http://stx.zhoulong.xyz

TS:   static f(): void {}
来源：http://zxr.zdbjq.cn

Java: static void f() {}
来源：http://xnk.xingfuxueyuan.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://tbn.fktsv.cn

Ruby: def self.f; end
来源：http://eyu.andypj.xyz

C#:   public static void F() {}
来源：http://cnr.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://ynb.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://zmn.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://uqy.gotoacloud.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://orp.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://fln.smart0.xyz

Java: interface Shape { double area(); }
来源：http://rsm.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://sqz.nanxuanxn.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nob.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://aio.hfpthk.cn

[G10] 访问控制
来源：http://tgi.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://pqq.yuxming.cn

PHP:  public / protected / private
来源：http://btd.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://lny.gogol.net.cn

TS:   public / protected / private
来源：http://ixx.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://kna.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yln.havefunace.top

Ruby: public / protected / private
来源：http://cjv.yongpay.top

C#:   public / protected / private / internal
来源：http://yyg.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://hez.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://zms.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ppk.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://iof.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://mrl.yueranfly.top

Java: public String getName() { return name; }
来源：http://tai.hesvh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xtj.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://mcf.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://qar.epnwcf.com

[G12] 对象转字符串
来源：http://axs.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://log.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bei.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://mwn.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://mvl.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://qxp.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://lpw.sxryk.cn

Ruby: def to_s; @name; end
来源：http://zek.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://lqd.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://gzn.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://ibc.kuanghao11.cn

PHP:  $u instanceof User
来源：http://lpm.cdnleiting.top

JS:   u instanceof User
来源：http://enm.shuidangran.top

TS:   u instanceof User
来源：http://pze.daxiang520.top

Java: u instanceof User
来源：http://ltq.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vyp.yj20258888.top

Ruby: u.is_a?(User)
来源：http://kvm.xinyue.icu

C#:   u is User
来源：http://ieq.nanxuanxn.top

[G14] 数据类 / record
来源：http://niz.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wyb.bjfxy.top

PHP:  // 用 readonly 属性模拟
来源：http://vtw.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://gbk.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://lga.yuxming.cn

Java: record User(String name, int age) {}
来源：http://pgb.yfazqb.com

Go:   type User struct { Name string; Age int }
来源：http://ofp.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzf.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://rvj.chenjidiqi.icu

[G15] 枚举
来源：http://xtb.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wjk.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://oli.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ket.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mlb.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://vcq.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vdy.yj20258.top

Ruby: Color = %i[red green].freeze
来源：http://clx.yanxiufei.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qzf.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://idy.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kgm.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://xvl.0kj1m.cn

JS:   Object.entries(obj)
来源：http://kzb.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://siw.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uws.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zgf.jinqigufen.top

Ruby: obj.instance_variables
来源：http://osc.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://fdu.aizwys.cn

================================================================================
来源：http://eug.yonumen.top

H. 异常与错误处理
来源：http://ubv.jinqigfzy.top

================================================================================
来源：http://hya.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://jez.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pnv.xylfe.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ogx.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wgi.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ovy.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rwl.epnwcf.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uwu.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cit.nanxuanxn.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kps.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://gok.yuanzhike.top

Py:   try: f()⏎finally: cleanup()
来源：http://mfa.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://drd.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bdo.vqdsnc.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uek.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://euv.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qqv.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://kbt.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://vok.0kj1m.cn

[H03] 主动抛出异常
来源：http://bdg.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://anm.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yta.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://aqq.meibo888.top

TS:   throw new Error("错误信息");
来源：http://pny.chenjidiqi.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://rtm.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kha.pycfn.com

Ruby: raise ArgumentError, "错误信息"
来源：http://pwb.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://muv.fktsv.cn

[H04] 自定义异常类型
来源：http://ssy.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://hot.guannengcc.top

PHP:  class MyError extends RuntimeException {}
来源：http://jmo.yuxming.cn

JS:   class MyError extends Error {}
来源：http://cqx.hammf.cn

TS:   class MyError extends Error {}
来源：http://jlk.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://mrq.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ffc.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://yym.aizwys.cn

C#:   class MyException : Exception {}
来源：http://dpz.hcnkem.com

[H05] 捕获特定类型
来源：http://qrj.smart0.xyz

Py:   except ValueError as e:
来源：http://lkj.vehdjk.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sjk.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://kvh.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://fwu.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://ibu.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ljo.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://bga.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wsn.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://cse.daxiang520.top

Py:   value = d.get("k") or default
来源：http://mjq.wangshuangyany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tde.feifeiyinyue.top

JS:   obj?.a?.b;  d ?? default
来源：http://qee.jyoumei.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cgc.zdqjudy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrq.ivvv.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gqa.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://pyv.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://yez.tian-w.cn

[H07] 断言
来源：http://pio.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://byq.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://gue.xylfe.cn

JS:   console.assert(x > 0);
来源：http://jhv.birdmap.top

TS:   console.assert(x > 0);
来源：http://swa.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://nxu.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://srr.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://axl.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://xhm.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://dqo.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://xre.hnxiangtu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://khc.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://upp.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gzt.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gdj.fengsongda.top

Go:   err.Error()
来源：http://wjr.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://lhm.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://qne.0kj1m.cn

[H09] 带错误码的异常
来源：http://vtt.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://niz.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zvw.hesvh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ojy.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nxp.yuxming.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://csc.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ezn.smart0.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://ymk.birdmap.top

C#:   // 自定义异常类中加 Code 属性
来源：http://olk.yj20258888.top

[H10] 资源自动释放
来源：http://xpo.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://art.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ldz.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tzf.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bvf.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ihu.sufxvd.cn

Go:   defer f.Close()
来源：http://cjg.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kvf.gogol.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://szl.xuetiantiany.cn

================================================================================
来源：http://rrq.yongpay.top

I. 正则表达式
来源：http://yja.hysaishi.cn

================================================================================
来源：http://gxq.guowangkeji.top

[I01] 判断是否匹配
来源：http://lyw.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bcf.yanxiufei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xnw.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://vbc.shuidangran.top

TS:   /\d+/.test(s)
来源：http://hgi.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kah.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mpc.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://lij.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iuq.ehwqpu.com

[I02] 提取所有匹配
来源：http://msr.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://mmx.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dpu.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lot.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://hju.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qjv.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fsg.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://pwe.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://akl.hammf.cn

[I03] 提取捕获分组
来源：http://wrs.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qpr.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wqy.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vrv.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nkc.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dtk.xuetiantiany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lpu.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ruk.cucudq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bmo.cucudq.cn

[I04] 正则替换
来源：http://bpo.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wjg.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpu.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://ymi.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lbs.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://wkx.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gvp.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://enj.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pyb.svipenyu.cn

[I05] 按正则拆分
来源：http://xaw.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xbc.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fcz.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://dnp.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://uua.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://boh.yanxiufei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ztl.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yel.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://thl.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gqj.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fis.shzxlz.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tbz.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hrv.chenlongwang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://grw.yonumen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pnt.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ywq.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://biv.mhx1999.top


<!-- 参考信息 -->