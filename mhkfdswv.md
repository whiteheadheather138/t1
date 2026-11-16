代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gbo.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jml.gogol.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aey.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://srr.guowangkeji.top

================================================================================
来源：http://yol.yonumen.top

G. 面向对象
来源：http://yqk.316326.xyz

================================================================================
来源：http://cmx.yonumen.top

[G01] 定义类
来源：http://fij.yj20258888.top

Py:   class User: pass
来源：http://kcz.wangshuangyany.cn

PHP:  class User {}
来源：http://zji.sweek.top

JS:   class User {}
来源：http://ayj.hnxiangtu.top

TS:   class User { name: string = ""; }
来源：http://ieg.haohaochexian.top

Java: class User {}
来源：http://mxm.andypj.xyz

Go:   type User struct { Name string }
来源：http://buj.shanyushiyangkeji.top

Ruby: class User; end
来源：http://ztm.wangshuangyany.cn

C#:   class User {}
来源：http://tfs.xylfe.cn

[G02] 构造函数
来源：http://mna.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://mdu.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://rei.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://bhl.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://aea.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://hlq.guowangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cmj.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://lnp.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://bmt.vehdjk.com

[G03] 实例属性
来源：http://bno.aibaodan.cn

Py:   self.name = "x"
来源：http://lfs.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://xaw.sjlbkw.cn

JS:   this.name = "x";
来源：http://jjk.shzxlz.cn

TS:   name: string = "x";
来源：http://omd.yangfankeji.com

Java: private String name;
来源：http://mqc.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xmu.aizwys.cn

Ruby: @name = "x"
来源：http://lle.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://lta.ivvv.top

[G04] 定义方法
来源：http://ilf.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://zev.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://pjc.wangdashe.top

JS:   greet() { return this.name; }
来源：http://uer.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://yrh.hysaishi.cn

Java: String greet() { return name; }
来源：http://dsx.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hrc.nwbrower.top

Ruby: def greet; @name; end
来源：http://low.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://jhx.9152youxi.cn

[G05] 继承
来源：http://ckk.52xcode.cn

Py:   class Admin(User): pass
来源：http://yxq.cheryme.top

PHP:  class Admin extends User {}
来源：http://tcv.xylfe.cn

JS:   class Admin extends User {}
来源：http://cws.cashguo.top

TS:   class Admin extends User {}
来源：http://zfm.9152youxi.cn

Java: class Admin extends User {}
来源：http://bda.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qgd.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://flt.jianghu66.top

C#:   class Admin : User {}
来源：http://res.epnwcf.com

[G06] 重写方法
来源：http://odt.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://bop.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zzq.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://mpe.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://ccp.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://qdh.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zyo.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://whp.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://nit.pycfn.com

[G07] 调用父类方法
来源：http://qwc.redwolf501.top

Py:   super().greet()
来源：http://mww.zdbjq.cn

PHP:  parent::greet();
来源：http://ach.wangdashe.top

JS:   super.greet();
来源：http://rgn.jyoumei.cn

TS:   super.greet();
来源：http://rzh.haohaochexian.top

Java: super.greet();
来源：http://xil.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tal.hnqzz.top

Ruby: super
来源：http://abm.hesvh.cn

C#:   base.Greet();
来源：http://ihf.hysaishi.cn

[G08] 静态方法与属性
来源：http://fsq.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hsg.52xcode.cn

PHP:  public static function f() {}
来源：http://scq.xinyue.icu

JS:   static f() {}
来源：http://ccr.hesvh.cn

TS:   static f(): void {}
来源：http://xjp.316326.xyz

Java: static void f() {}
来源：http://wkx.sufxvd.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://krd.meibo888.top

Ruby: def self.f; end
来源：http://qcx.zhongyouzk.top

C#:   public static void F() {}
来源：http://gfb.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://rdk.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://nfc.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oqm.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://era.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://ruc.daria6918.cn

Java: interface Shape { double area(); }
来源：http://cwk.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://loj.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wgn.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://efy.yj20258.top

[G10] 访问控制
来源：http://lzu.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://vdw.bbcook.cn

PHP:  public / protected / private
来源：http://zbl.xylfe.cn

JS:   #private 字段；其余公开
来源：http://mdu.gzhubu.top

TS:   public / protected / private
来源：http://dcd.meibo888.top

Java: public / protected / private / 默认包级
来源：http://uax.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vrs.316326.xyz

Ruby: public / protected / private
来源：http://lyk.uphjek.com

C#:   public / protected / private / internal
来源：http://fvm.zhijiandao.cn

[G11] getter / setter
来源：http://ypy.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://myh.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nls.ybcxt.top

JS:   get name() { return this._name; }
来源：http://kyj.nanxinkj.top

TS:   get name(): string { return this._name; }
来源：http://okf.zhixingplan.top

Java: public String getName() { return name; }
来源：http://gee.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://stg.nanxinkj.top

Ruby: attr_accessor :name
来源：http://dtf.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://utv.hesvh.cn

[G12] 对象转字符串
来源：http://jla.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://jgh.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://idi.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://hwo.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://fhd.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://nfa.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ksn.zdbjq.cn

Ruby: def to_s; @name; end
来源：http://dpn.gaohongyu789.top

C#:   public override string ToString() => Name;
来源：http://bap.zhongyouzk.top

[G13] 判断对象类型
来源：http://rjb.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://zbg.xuanzx.com

PHP:  $u instanceof User
来源：http://tlu.gzhubu.top

JS:   u instanceof User
来源：http://ith.shangyingyoupin.top

TS:   u instanceof User
来源：http://vbx.shzxlz.cn

Java: u instanceof User
来源：http://tgy.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bzr.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://cqv.pycfn.com

C#:   u is User
来源：http://ddl.sxryk.cn

[G14] 数据类 / record
来源：http://huh.chenjidiqi.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pfi.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://wdv.zhijiandao.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yep.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://xaq.smart0.xyz

Java: record User(String name, int age) {}
来源：http://aiq.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://pim.9152youxi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mxi.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://mzl.c1oappe.top

[G15] 枚举
来源：http://ofv.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://php.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://oiz.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iuc.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zaj.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://sbn.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://izl.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://cex.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ynf.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://mjt.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ylk.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://yij.zycfv.cn

JS:   Object.entries(obj)
来源：http://gxs.dashuyun.cn

TS:   Object.entries(obj)
来源：http://xta.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xzk.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qlb.zhijiandao.cn

Ruby: obj.instance_variables
来源：http://usc.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://tub.tarul.cn

================================================================================
来源：http://nvv.yfazqb.com

H. 异常与错误处理
来源：http://bmo.iojbl.cn

================================================================================
来源：http://yyw.jlsjyb.cn

[H01] try / catch 基础
来源：http://qhy.sweek.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rwm.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://htu.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tdh.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jbg.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qvl.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sjm.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hfo.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://drj.c1oappe.top

[H02] finally / ensure 收尾
来源：http://hip.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://zzs.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vcr.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://pvm.0kj1m.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nmr.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://epx.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sks.ywan-chungtsiang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ubd.xuanzx.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://jmk.ppjwa.cn

[H03] 主动抛出异常
来源：http://bdc.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://kbu.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://osj.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://gqp.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://yiw.wangshuangyany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://isj.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lui.yonumen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ina.hesvh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vja.zhoulong.xyz

[H04] 自定义异常类型
来源：http://ify.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://clp.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://dky.aizwys.cn

JS:   class MyError extends Error {}
来源：http://twb.ctjpmb.com

TS:   class MyError extends Error {}
来源：http://fsd.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://cyp.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kbg.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://ldu.ydjk.org.cn

C#:   class MyException : Exception {}
来源：http://wou.yvedp.cn

[H05] 捕获特定类型
来源：http://vmg.zhixingplan.top

Py:   except ValueError as e:
来源：http://xmo.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://czl.redwolf501.top

JS:   if (e instanceof TypeError) {}
来源：http://opt.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://jbh.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://pgx.zhoulong.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://avm.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://igs.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gfq.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://ium.yongpay.top

Py:   value = d.get("k") or default
来源：http://wqd.havefunace.top

PHP:  $v = $d["k"] ?? null;
来源：http://ffi.dashuyun.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gea.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://cvf.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pjd.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iuo.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://vzq.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://ise.zycfv.cn

[H07] 断言
来源：http://cis.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://wmh.ivvv.top

PHP:  assert($x > 0);
来源：http://vcs.zhaomingkeji.xyz

JS:   console.assert(x > 0);
来源：http://qkr.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://oyl.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://exv.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qob.chenzaomai.com

Ruby: raise "必须为正" unless x > 0
来源：http://zmx.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://jnk.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://gdm.xylfe.cn

Py:   str(e);  traceback.format_exc()
来源：http://iov.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ach.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://gts.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rxh.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hnh.tian-w.cn

Go:   err.Error()
来源：http://fav.bjfxy.top

Ruby: e.message;  e.backtrace
来源：http://lro.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://ghr.gaohongyu789.top

[H09] 带错误码的异常
来源：http://ptb.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://udv.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://gsb.shangyingyoupin.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baz.316326.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://slk.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cze.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pua.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uwg.zhijiandao.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://npd.chenlongwang.top

[H10] 资源自动释放
来源：http://zif.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jnq.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tgy.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hza.ydjk.org.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ilz.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://odd.nanxuanxn.top

Go:   defer f.Close()
来源：http://hlu.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xzw.chenjidiqi.icu

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vur.yvedp.cn

================================================================================
来源：http://ovz.svipenyu.cn

I. 正则表达式
来源：http://xis.jlsjyb.cn

================================================================================
来源：http://fqt.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://gxr.yueranfly.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wqy.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://hzm.zhiwuduotai.top

JS:   /\d+/.test(s)
来源：http://gvo.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://epp.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://raw.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rhf.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://gkh.sufxvd.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izi.yuanzhike.top

[I02] 提取所有匹配
来源：http://hls.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://omi.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ldh.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gnz.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://oqi.52xcode.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qxd.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nkw.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://dkf.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tpd.jlsjyb.cn

[I03] 提取捕获分组
来源：http://rue.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cob.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kxi.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oca.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bue.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qvp.yongpay.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ncp.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tsd.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://voc.yfazqb.com

[I04] 正则替换
来源：http://seu.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ugv.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ass.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qos.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lxg.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://gel.sufxvd.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://btc.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://tfj.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ecl.vehdjk.com

[I05] 按正则拆分
来源：http://wza.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gut.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tcm.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://bmi.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://oij.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://rtz.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jwd.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://zkz.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iec.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aon.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mjd.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eue.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmo.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bvp.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rtu.xingfuxueyuan.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vpp.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sdw.wangdashe.top


<!-- 参考信息 -->