代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://znt.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dkx.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://amd.jinyuanbaomall.cn

TS:   // 同上
来源：http://ggv.fzhhl.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dmt.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vni.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://par.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jsr.0kj1m.cn

================================================================================
来源：http://swr.xylfe.cn

G. 面向对象
来源：http://sgg.fzhhl.top

================================================================================
来源：http://sny.sjlbkw.cn

[G01] 定义类
来源：http://iqt.ydjk.org.cn

Py:   class User: pass
来源：http://pfh.pycfn.com

PHP:  class User {}
来源：http://glj.52xcode.cn

JS:   class User {}
来源：http://kre.pycfn.com

TS:   class User { name: string = ""; }
来源：http://qgj.quarkkingdee.top

Java: class User {}
来源：http://kgc.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://kev.xylfe.cn

Ruby: class User; end
来源：http://mif.zycfv.cn

C#:   class User {}
来源：http://nym.guowangkeji.top

[G02] 构造函数
来源：http://nqi.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://nfm.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://tav.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://xht.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://avm.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://ont.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ehj.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://gmf.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://ygs.zhaomingkeji.xyz

[G03] 实例属性
来源：http://awi.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://lbb.pycfn.com

PHP:  public string $name = "x";
来源：http://ack.ppjwa.cn

JS:   this.name = "x";
来源：http://dxr.wangdashe.top

TS:   name: string = "x";
来源：http://tvy.svipenyu.cn

Java: private String name;
来源：http://mqx.iojbl.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wyy.ctjpmb.com

Ruby: @name = "x"
来源：http://nhb.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://hyn.birdmap.top

[G04] 定义方法
来源：http://evs.ydzc1.top

Py:   def greet(self): return self.name
来源：http://pqh.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oxs.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://ddg.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://tgk.316326.xyz

Java: String greet() { return name; }
来源：http://vfd.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hoc.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://rue.gaohongyu789.top

C#:   public string Greet() => Name;
来源：http://azz.hnxiangtu.top

[G05] 继承
来源：http://uwl.zdbjq.cn

Py:   class Admin(User): pass
来源：http://vkb.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://lhv.yueranfly.top

JS:   class Admin extends User {}
来源：http://gad.xziqi.cn

TS:   class Admin extends User {}
来源：http://inl.yfazqb.com

Java: class Admin extends User {}
来源：http://zvf.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xgn.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://gru.tarul.cn

C#:   class Admin : User {}
来源：http://rfx.cucudq.cn

[G06] 重写方法
来源：http://gfl.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://nrm.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mrc.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://ymy.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://gbu.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://uaf.yj20258888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nih.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://rlv.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://rvt.fzhhl.top

[G07] 调用父类方法
来源：http://oyv.gaohongyu789.top

Py:   super().greet()
来源：http://rpw.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://yoy.cqqwz.cn

JS:   super.greet();
来源：http://iql.yj20258888.top

TS:   super.greet();
来源：http://ehf.uphjek.com

Java: super.greet();
来源：http://zcu.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://btt.ydjk.org.cn

Ruby: super
来源：http://nnd.c1oappe.top

C#:   base.Greet();
来源：http://qmx.zhongyouzk.top

[G08] 静态方法与属性
来源：http://oql.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wst.yvedp.cn

PHP:  public static function f() {}
来源：http://qbu.0kj1m.cn

JS:   static f() {}
来源：http://yek.vqdsnc.cn

TS:   static f(): void {}
来源：http://ajb.gaohongyu789.top

Java: static void f() {}
来源：http://svr.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qpj.zhiwuduotai.top

Ruby: def self.f; end
来源：http://hns.shzxlz.cn

C#:   public static void F() {}
来源：http://cbi.hammf.cn

[G09] 接口 / 抽象类
来源：http://vpn.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://ptw.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cjc.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jdn.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://lun.hysaishi.cn

Java: interface Shape { double area(); }
来源：http://dka.gotoacloud.top

Go:   type Shape interface { Area() float64 }
来源：http://pfl.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jji.chenlongwang.top

C#:   interface IShape { double Area(); }
来源：http://plq.fanxiaobao.xyz

[G10] 访问控制
来源：http://lqc.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://evr.birdmap.top

PHP:  public / protected / private
来源：http://jzn.hywenlv.cn

JS:   #private 字段；其余公开
来源：http://nkp.jinghuilouyu.cn

TS:   public / protected / private
来源：http://lji.yj20258.top

Java: public / protected / private / 默认包级
来源：http://poq.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qwc.daria6918.cn

Ruby: public / protected / private
来源：http://kif.jiagoushi.top

C#:   public / protected / private / internal
来源：http://yax.kuanghao11.cn

[G11] getter / setter
来源：http://pxh.xinyue.icu

Py:   @property 与 @x.setter
来源：http://sfw.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mbw.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://mdb.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://tuu.cqqwz.cn

Java: public String getName() { return name; }
来源：http://qqk.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qlq.yonumen.top

Ruby: attr_accessor :name
来源：http://fre.epnwcf.com

C#:   public string Name { get; set; }
来源：http://ebk.sufxvd.cn

[G12] 对象转字符串
来源：http://eyy.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://gpb.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pbg.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://crg.hcnkem.com

TS:   toString(): string { return this.name; }
来源：http://iag.vqdsnc.cn

Java: @Override public String toString() { return name; }
来源：http://lbx.vehdjk.com

Go:   func (u User) String() string { return u.Name }
来源：http://mgz.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://fcz.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://otn.xinyue.icu

[G13] 判断对象类型
来源：http://wve.chenlongwang.top

Py:   isinstance(u, User)
来源：http://qen.chenlongwang.top

PHP:  $u instanceof User
来源：http://hdf.fanxiaobao.xyz

JS:   u instanceof User
来源：http://fsm.c1oappe.top

TS:   u instanceof User
来源：http://xyk.chenjidiqi.icu

Java: u instanceof User
来源：http://xju.yfazqb.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pgj.yj20258.top

Ruby: u.is_a?(User)
来源：http://nwp.pycfn.com

C#:   u is User
来源：http://fxd.zdqjudy.top

[G14] 数据类 / record
来源：http://lng.jqgufenzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://soi.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://fot.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://jak.wangshuangyany.cn

TS:   type User = { name: string; age: number };
来源：http://ija.nanxuanxn.top

Java: record User(String name, int age) {}
来源：http://mzv.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://bkj.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xqc.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://cgz.0kj1m.cn

[G15] 枚举
来源：http://jri.shangyingyoupin.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ghh.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mdl.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ume.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ylu.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://hdh.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gyd.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://prz.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bov.gaohongyu789.top

[G16] 对象转数组 / 字典
来源：http://xxx.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fei.yvedp.cn

PHP:  get_object_vars($obj);
来源：http://bbv.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://tmi.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://mju.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dfv.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://acz.xylfe.cn

Ruby: obj.instance_variables
来源：http://xmf.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://cud.daria6918.cn

================================================================================
来源：http://akm.fehbvm.com

H. 异常与错误处理
来源：http://zgi.nanxuanxn.top

================================================================================
来源：http://dxe.zhongyouzk.top

[H01] try / catch 基础
来源：http://cfr.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vfz.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsb.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qhx.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aik.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dax.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dbr.redwolf501.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kvo.jyoumei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lhg.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://etj.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ijz.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://dcr.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hou.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gsl.hfpthk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eli.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://exi.quarkkingdee.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qqs.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vlb.fzhhl.top

[H03] 主动抛出异常
来源：http://bap.zhijiandao.cn

Py:   raise ValueError("错误信息")
来源：http://ayq.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aid.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://oyg.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://ozb.zhoulong.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://qen.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mzb.svipenyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xys.tanke756.top

C#:   throw new ArgumentException("错误信息");
来源：http://nmc.yangfankeji.com

[H04] 自定义异常类型
来源：http://mup.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://wcu.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://srk.jqgfzy.top

JS:   class MyError extends Error {}
来源：http://wrg.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://ysb.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://nlz.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wbi.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://rsf.smart0.xyz

C#:   class MyException : Exception {}
来源：http://ucw.birdmap.top

[H05] 捕获特定类型
来源：http://jxc.shzxlz.cn

Py:   except ValueError as e:
来源：http://fsm.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rlz.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://ajg.iojbl.cn

TS:   if (e instanceof TypeError) {}
来源：http://kye.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://hoi.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tsv.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://oxv.sysykeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zdc.hcnkem.com

[H06] 可选值 / 空值安全访问
来源：http://evy.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://vrx.jinqigufen.top

PHP:  $v = $d["k"] ?? null;
来源：http://jrw.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dax.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://hdr.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vny.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pxa.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://jnw.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://nfz.pycfn.com

[H07] 断言
来源：http://bps.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://dqo.hesvh.cn

PHP:  assert($x > 0);
来源：http://ulv.shuidangran.top

JS:   console.assert(x > 0);
来源：http://kld.ivvv.top

TS:   console.assert(x > 0);
来源：http://tvw.52xcode.cn

Java: assert x > 0 : "必须为正";
来源：http://lsg.hesvh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jou.hammf.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pdk.daria6918.cn

C#:   Debug.Assert(x > 0);
来源：http://qbk.bbcook.cn

[H08] 获取错误信息与堆栈
来源：http://mtn.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://fnw.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pcu.yj202588.top

JS:   e.message;  e.stack
来源：http://sno.aizwys.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://egf.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kzs.zycfv.cn

Go:   err.Error()
来源：http://pdc.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://xlg.ctjpmb.com

C#:   e.Message;  e.StackTrace
来源：http://vpu.ydzc1.top

[H09] 带错误码的异常
来源：http://zex.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hgx.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fwb.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vpg.vqdsnc.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://flc.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://soy.zycfv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vdk.yj20258888.top

Ruby: raise MyError.new("fail", 500)
来源：http://vlz.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bfy.daria6918.cn

[H10] 资源自动释放
来源：http://xzc.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mkw.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cyq.shzxlz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kwl.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ewi.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ebs.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://uvb.aizwys.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dyr.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rms.uphjek.com

================================================================================
来源：http://rcu.yanxiufei.cn

I. 正则表达式
来源：http://vff.tanke756.top

================================================================================
来源：http://juf.vqdsnc.cn

[I01] 判断是否匹配
来源：http://yxn.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bbi.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://yqt.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://qup.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://okk.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gsl.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gyd.meibo888.top

Ruby: s.match?(/\d+/)
来源：http://tsz.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rfz.vqdsnc.cn

[I02] 提取所有匹配
来源：http://jgl.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://scd.shangyingyoupin.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nlr.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uys.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://ngt.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://czo.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aye.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://irl.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://euo.ydjk.org.cn

[I03] 提取捕获分组
来源：http://wmv.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gih.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wqt.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ezy.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uxh.gaohongyu789.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iue.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rzp.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fza.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rhi.tanke756.top

[I04] 正则替换
来源：http://mbu.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zqm.sjlbkw.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://muk.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tbr.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://bik.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://fgz.yfazqb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pwi.smart0.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hmh.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hue.iojbl.cn

[I05] 按正则拆分
来源：http://bqx.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wiz.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qqk.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://ymf.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://bon.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://ifq.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qug.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iwb.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://skn.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zqj.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpi.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wmf.xylfe.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qsx.fanxiaobao.xyz


<!-- 参考信息 -->