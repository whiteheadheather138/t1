代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gei.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hhh.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xfj.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://thc.hammf.cn

================================================================================
来源：http://mdt.cashguo.top

G. 面向对象
来源：http://qit.fzhhl.top

================================================================================
来源：http://kme.jqgfzy.top

[G01] 定义类
来源：http://tix.epnwcf.com

Py:   class User: pass
来源：http://vfi.uphjek.com

PHP:  class User {}
来源：http://wlc.9152youxi.cn

JS:   class User {}
来源：http://acm.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://wbx.guowangkeji.top

Java: class User {}
来源：http://xet.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://yxt.dianchejie.cn

Ruby: class User; end
来源：http://zqz.wangdashe.top

C#:   class User {}
来源：http://jqy.jyoumei.cn

[G02] 构造函数
来源：http://agm.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://vkd.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://hbr.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://vny.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://klw.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://xin.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mpe.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://jtm.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://xht.feifeiyinyue.top

[G03] 实例属性
来源：http://mxf.pycfn.com

Py:   self.name = "x"
来源：http://pym.hysaishi.cn

PHP:  public string $name = "x";
来源：http://obc.ctjpmb.com

JS:   this.name = "x";
来源：http://crb.hammf.cn

TS:   name: string = "x";
来源：http://tsb.chenzaomai.com

Java: private String name;
来源：http://dyy.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bie.iojbl.cn

Ruby: @name = "x"
来源：http://kqp.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://eoz.cdnleiting.top

[G04] 定义方法
来源：http://qsj.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://niz.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fnw.smart0.xyz

JS:   greet() { return this.name; }
来源：http://whq.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://iko.zycfv.cn

Java: String greet() { return name; }
来源：http://qtz.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tea.yueranfly.top

Ruby: def greet; @name; end
来源：http://nzj.cashguo.top

C#:   public string Greet() => Name;
来源：http://yle.kuanghao11.cn

[G05] 继承
来源：http://jub.ctjpmb.com

Py:   class Admin(User): pass
来源：http://raa.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://ohb.ehwqpu.com

JS:   class Admin extends User {}
来源：http://egu.jianghu66.top

TS:   class Admin extends User {}
来源：http://fgx.hysaishi.cn

Java: class Admin extends User {}
来源：http://msv.xuetiantiany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ldb.aizwys.cn

Ruby: class Admin < User; end
来源：http://wzt.tian-w.cn

C#:   class Admin : User {}
来源：http://qqi.guowangkeji.top

[G06] 重写方法
来源：http://fqf.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://qwc.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ejx.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://tdx.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://otl.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://udb.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hss.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://cpy.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://ody.sufxvd.cn

[G07] 调用父类方法
来源：http://ite.wangdashe.top

Py:   super().greet()
来源：http://nal.dashuyun.cn

PHP:  parent::greet();
来源：http://lsc.ppjwa.cn

JS:   super.greet();
来源：http://lru.cheryme.top

TS:   super.greet();
来源：http://iea.epnwcf.com

Java: super.greet();
来源：http://wuq.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://unm.jiagoushi.top

Ruby: super
来源：http://zbn.xuanzx.com

C#:   base.Greet();
来源：http://uwf.mhx1999.top

[G08] 静态方法与属性
来源：http://cdo.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mlm.cheryme.top

PHP:  public static function f() {}
来源：http://hki.shanyushiyangtech.top

JS:   static f() {}
来源：http://ntw.cucudq.cn

TS:   static f(): void {}
来源：http://nho.wangdashe.top

Java: static void f() {}
来源：http://vna.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wae.uphjek.com

Ruby: def self.f; end
来源：http://gho.tanke756.top

C#:   public static void F() {}
来源：http://nck.daria6918.cn

[G09] 接口 / 抽象类
来源：http://ufz.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://end.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://clw.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vcu.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://nuj.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://vtj.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://ods.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bht.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://uik.fengsongda.top

[G10] 访问控制
来源：http://yiw.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://pwn.chenjidiqi.icu

PHP:  public / protected / private
来源：http://fqs.fktsv.cn

JS:   #private 字段；其余公开
来源：http://lnk.sjlbkw.cn

TS:   public / protected / private
来源：http://hpc.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://fuc.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pif.daxiang520.top

Ruby: public / protected / private
来源：http://dpg.daxiang520.top

C#:   public / protected / private / internal
来源：http://lwc.zhijiandao.cn

[G11] getter / setter
来源：http://uwb.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://nph.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://djw.tian-w.cn

JS:   get name() { return this._name; }
来源：http://ouj.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://bro.andypj.xyz

Java: public String getName() { return name; }
来源：http://dtb.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://igm.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://jkm.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://hgp.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://whx.yj20258.top

Py:   def __str__(self): return self.name
来源：http://eue.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kvq.xuanzx.com

JS:   toString() { return this.name; }
来源：http://kah.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://ifq.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://wvd.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://fti.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://arg.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://nme.tian-w.cn

[G13] 判断对象类型
来源：http://kcz.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://rsf.yangfankeji.com

PHP:  $u instanceof User
来源：http://usj.cqqwz.cn

JS:   u instanceof User
来源：http://rfm.gaohongyu789.top

TS:   u instanceof User
来源：http://qla.fanxiaobao.xyz

Java: u instanceof User
来源：http://yjx.sufxvd.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xwr.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://dvy.fanxiaobao.xyz

C#:   u is User
来源：http://xqt.cashguo.top

[G14] 数据类 / record
来源：http://zzg.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tty.wangdashe.top

PHP:  // 用 readonly 属性模拟
来源：http://jbo.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rps.iojbl.cn

TS:   type User = { name: string; age: number };
来源：http://ozs.jianghu66.top

Java: record User(String name, int age) {}
来源：http://mbj.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://ayf.sufxvd.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wts.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://jxa.feifeiyinyue.top

[G15] 枚举
来源：http://azy.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://njp.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qya.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vac.9152youxi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gmc.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://qek.vqdsnc.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://leq.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://tgo.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hzk.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://wcg.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vhw.zycfv.cn

PHP:  get_object_vars($obj);
来源：http://wus.wangdashe.top

JS:   Object.entries(obj)
来源：http://nge.pycfn.com

TS:   Object.entries(obj)
来源：http://jhr.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jds.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dre.yanxiufei.cn

Ruby: obj.instance_variables
来源：http://jlj.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://oxq.jiagoushi.top

================================================================================
来源：http://zah.hfpthk.cn

H. 异常与错误处理
来源：http://nfj.zhoulong.xyz

================================================================================
来源：http://vqu.snrcjt.cn

[H01] try / catch 基础
来源：http://wgz.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kyp.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mfl.yuxming.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://anf.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lfc.jinqigfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xxo.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dun.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://whw.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ixa.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://ujl.gaohongyu789.top

Py:   try: f()⏎finally: cleanup()
来源：http://ltl.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wbs.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kiz.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bhx.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bfh.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aeh.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://tzm.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ltn.gogol.net.cn

[H03] 主动抛出异常
来源：http://uov.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://iuf.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zro.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://jyv.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://svf.cheryme.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rqw.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xjr.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://irh.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://uvr.xziqi.cn

[H04] 自定义异常类型
来源：http://emh.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://tjq.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://zxx.epnwcf.com

JS:   class MyError extends Error {}
来源：http://sjr.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://dtg.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://gse.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gvp.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://qot.yj20258888.top

C#:   class MyException : Exception {}
来源：http://zyg.aibaodan.cn

[H05] 捕获特定类型
来源：http://hwa.cashguo.top

Py:   except ValueError as e:
来源：http://vxo.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eqk.yuxming.cn

JS:   if (e instanceof TypeError) {}
来源：http://oss.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://tab.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qoj.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ssw.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://zdb.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://awo.birdmap.top

[H06] 可选值 / 空值安全访问
来源：http://why.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://zno.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vmc.9152youxi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rwh.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://shf.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzm.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tqv.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://lcu.yfazqb.com

C#:   obj?.A?.B ?? default
来源：http://dbb.daria6918.cn

[H07] 断言
来源：http://oxe.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://fdh.fanxiaobao.xyz

PHP:  assert($x > 0);
来源：http://ogi.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://eft.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://zft.fanxiaobao.xyz

Java: assert x > 0 : "必须为正";
来源：http://wgv.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zow.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://reg.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://qwc.pengpengdd.cyou

[H08] 获取错误信息与堆栈
来源：http://cmt.gaohongyu789.top

Py:   str(e);  traceback.format_exc()
来源：http://fav.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uyx.yj20258.top

JS:   e.message;  e.stack
来源：http://rww.sysykeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vpv.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bhs.snrcjt.cn

Go:   err.Error()
来源：http://egt.ydjk.org.cn

Ruby: e.message;  e.backtrace
来源：http://qlh.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://dgl.iojbl.cn

[H09] 带错误码的异常
来源：http://fxk.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mct.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://gxq.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wpj.fktsv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://get.hcnkem.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vjs.zhongyouzk.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ouh.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://jji.yueranfly.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qqk.feifeiyinyue.top

[H10] 资源自动释放
来源：http://now.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kuq.shuidangran.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xih.haohaochexian.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cew.zycfv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xhd.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wyd.shzxlz.cn

Go:   defer f.Close()
来源：http://vwb.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vyr.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ueq.tarul.cn

================================================================================
来源：http://myv.guowangkeji.top

I. 正则表达式
来源：http://dez.ehwqpu.com

================================================================================
来源：http://ith.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://cuj.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wka.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tgg.shuidangran.top

JS:   /\d+/.test(s)
来源：http://wde.epnwcf.com

TS:   /\d+/.test(s)
来源：http://hyx.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fys.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sbt.hongshengwenyu.top

Ruby: s.match?(/\d+/)
来源：http://xgc.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mxu.ivvv.top

[I02] 提取所有匹配
来源：http://tog.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://uad.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jvc.shzxlz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://haz.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://ard.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ylh.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ozp.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://omx.svipenyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bie.guannengcc.top

[I03] 提取捕获分组
来源：http://bjp.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wbv.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gcf.pycfn.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nzd.bbcook.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zlr.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tlg.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://knd.chenjidiqi.icu

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kgc.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mxb.aizwys.cn

[I04] 正则替换
来源：http://jmu.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cum.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ikj.uphjek.com

JS:   s.replace(/\d+/g, "#")
来源：http://nsn.hnqzz.top

TS:   s.replace(/\d+/g, "#")
来源：http://awm.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jir.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yuh.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://xxi.iojbl.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nvf.zhijiandao.cn

[I05] 按正则拆分
来源：http://hdw.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://nmt.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hqh.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://wud.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://rka.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://huh.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://edd.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://deg.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://crp.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://egs.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iiq.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kxd.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vtd.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mbd.birdmap.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ued.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ion.meibo888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hdc.gaohongyu789.top


<!-- 参考信息 -->