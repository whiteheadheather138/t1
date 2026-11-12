代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iek.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iej.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://crs.ydjk.org.cn

[F12] CSV 读写
来源：http://jtn.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://csv.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nls.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yxa.gogol.net.cn

TS:   // 同上
来源：http://cko.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yqm.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mkh.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cvo.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mfz.pengpengdd.cyou

================================================================================
来源：http://had.sxryk.cn

G. 面向对象
来源：http://mhd.0kj1m.cn

================================================================================
来源：http://utm.birdmap.top

[G01] 定义类
来源：http://rpn.aizwys.cn

Py:   class User: pass
来源：http://smw.yueranfly.top

PHP:  class User {}
来源：http://ovy.zhengqikj.top

JS:   class User {}
来源：http://tvi.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://hhp.yfazqb.com

Java: class User {}
来源：http://qtm.yvedp.cn

Go:   type User struct { Name string }
来源：http://ysf.yueranfly.top

Ruby: class User; end
来源：http://uxw.c1oappe.top

C#:   class User {}
来源：http://fok.yanxiufei.cn

[G02] 构造函数
来源：http://oto.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://ruj.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://giw.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://ast.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://aue.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://jas.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mli.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ogf.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://kfm.jinyuanbaomall.cn

[G03] 实例属性
来源：http://ive.gotoacloud.top

Py:   self.name = "x"
来源：http://trn.hnqzz.top

PHP:  public string $name = "x";
来源：http://seu.tanke756.top

JS:   this.name = "x";
来源：http://hiw.jyoumei.cn

TS:   name: string = "x";
来源：http://nfi.ivvv.top

Java: private String name;
来源：http://edd.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksr.daxiang520.top

Ruby: @name = "x"
来源：http://gpl.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://vqd.shanyushiyangkeji.top

[G04] 定义方法
来源：http://wjx.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://sjl.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://haa.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://ejr.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://hkv.zdqjudy.top

Java: String greet() { return name; }
来源：http://cxb.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iff.zycfv.cn

Ruby: def greet; @name; end
来源：http://yrj.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://onj.chenlongwang.top

[G05] 继承
来源：http://rfx.cucudq.cn

Py:   class Admin(User): pass
来源：http://kpo.fktsv.cn

PHP:  class Admin extends User {}
来源：http://due.tarul.cn

JS:   class Admin extends User {}
来源：http://zcp.tanke756.top

TS:   class Admin extends User {}
来源：http://sol.jinqigfzy.top

Java: class Admin extends User {}
来源：http://dvs.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jdk.ivvv.top

Ruby: class Admin < User; end
来源：http://pxj.yj20258888.top

C#:   class Admin : User {}
来源：http://jsm.sweek.top

[G06] 重写方法
来源：http://xmc.cheryme.top

Py:   def greet(self): return "admin"
来源：http://bmp.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://sid.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://tmx.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://hqo.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://yft.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://akx.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://gve.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://vme.guowangkeji.top

[G07] 调用父类方法
来源：http://ubw.yuanzhike.top

Py:   super().greet()
来源：http://vhm.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://xtj.ehwqpu.com

JS:   super.greet();
来源：http://mjl.mhx1999.top

TS:   super.greet();
来源：http://irg.yj20258888.top

Java: super.greet();
来源：http://ngv.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://udw.havefunace.top

Ruby: super
来源：http://ttz.hcnkem.com

C#:   base.Greet();
来源：http://glb.tanke756.top

[G08] 静态方法与属性
来源：http://fns.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ckn.andypj.xyz

PHP:  public static function f() {}
来源：http://hmj.zhengqikj.top

JS:   static f() {}
来源：http://ulo.ydjk.org.cn

TS:   static f(): void {}
来源：http://tnq.yuanzhike.top

Java: static void f() {}
来源：http://ipa.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kff.316326.xyz

Ruby: def self.f; end
来源：http://phh.zdqjudy.top

C#:   public static void F() {}
来源：http://imr.dashuyun.cn

[G09] 接口 / 抽象类
来源：http://ehj.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://imz.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://ndv.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kff.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://srs.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://fjl.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://egb.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://knf.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://jlx.dashuyun.cn

[G10] 访问控制
来源：http://lsl.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://fdt.0kj1m.cn

PHP:  public / protected / private
来源：http://ayk.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://wal.tian-w.cn

TS:   public / protected / private
来源：http://qzk.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://hqu.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://eku.nwbrower.top

Ruby: public / protected / private
来源：http://oqv.snrcjt.cn

C#:   public / protected / private / internal
来源：http://sza.quarkkingdee.top

[G11] getter / setter
来源：http://lbh.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://ylc.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://trt.wangdashe.top

JS:   get name() { return this._name; }
来源：http://usq.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://vjg.redwolf501.top

Java: public String getName() { return name; }
来源：http://vzn.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://omm.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://xzl.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://jkm.nanxuanxn.top

[G12] 对象转字符串
来源：http://uhe.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://iwd.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xml.cucudq.cn

JS:   toString() { return this.name; }
来源：http://uiv.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://dlh.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://fre.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://mul.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://apa.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://ega.yj20258.top

[G13] 判断对象类型
来源：http://gxr.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://gzz.aizwys.cn

PHP:  $u instanceof User
来源：http://juk.ppjwa.cn

JS:   u instanceof User
来源：http://jhx.yonumen.top

TS:   u instanceof User
来源：http://bzf.epnwcf.com

Java: u instanceof User
来源：http://kds.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ztn.vqdsnc.cn

Ruby: u.is_a?(User)
来源：http://rgs.ctjpmb.com

C#:   u is User
来源：http://twt.jqgfzy.top

[G14] 数据类 / record
来源：http://aef.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wls.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://upi.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fvl.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://gyx.sxryk.cn

Java: record User(String name, int age) {}
来源：http://igh.9152youxi.cn

Go:   type User struct { Name string; Age int }
来源：http://zfv.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://drf.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://mkl.ppjwa.cn

[G15] 枚举
来源：http://hzi.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dhh.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://lou.yueranfly.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qva.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bdb.fzhhl.top

Java: enum Color { RED, GREEN }
来源：http://xlm.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayd.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://avh.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://izq.yj202588.top

[G16] 对象转数组 / 字典
来源：http://jdi.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ssn.meibo888.top

PHP:  get_object_vars($obj);
来源：http://rmd.hnxiangtu.top

JS:   Object.entries(obj)
来源：http://uvz.zhijiandao.cn

TS:   Object.entries(obj)
来源：http://eod.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fip.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zdv.yj20258888.top

Ruby: obj.instance_variables
来源：http://edn.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://qat.daxiang520.top

================================================================================
来源：http://qfk.zhiwuduotai.top

H. 异常与错误处理
来源：http://xzt.ivvv.top

================================================================================
来源：http://kfj.9152youxi.cn

[H01] try / catch 基础
来源：http://fgb.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hjg.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://frn.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cbz.shanyushiyangtech.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dxr.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vcl.cashguo.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nua.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kny.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vzc.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://kto.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://twd.cheryme.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qft.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://xcv.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ijk.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://iav.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://omf.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fsy.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kmy.shuidangran.top

[H03] 主动抛出异常
来源：http://ykk.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://uux.cheryme.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://byt.yongpay.top

JS:   throw new Error("错误信息");
来源：http://piw.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://kih.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://raz.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vdv.316326.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://ekf.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://qqc.jlsjyb.cn

[H04] 自定义异常类型
来源：http://lgs.cheryme.top

Py:   class MyError(Exception): pass
来源：http://opg.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://azm.vqdsnc.cn

JS:   class MyError extends Error {}
来源：http://bbr.sjlbkw.cn

TS:   class MyError extends Error {}
来源：http://tao.yj20258.top

Java: class MyException extends RuntimeException {}
来源：http://scw.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rrz.cdnleiting.top

Ruby: class MyError < StandardError; end
来源：http://dde.mhx1999.top

C#:   class MyException : Exception {}
来源：http://gnw.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://xvl.jyoumei.cn

Py:   except ValueError as e:
来源：http://dvd.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oun.guowangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://dud.52xcode.cn

TS:   if (e instanceof TypeError) {}
来源：http://qnr.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://kxs.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fpa.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://qqp.hywenlv.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aaf.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://aii.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://ewp.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://qzn.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://clb.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sbj.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tac.zhongyouzk.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gao.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://wjl.wangshuangyany.cn

C#:   obj?.A?.B ?? default
来源：http://czp.yongpay.top

[H07] 断言
来源：http://jqu.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://omc.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://nfb.yfazqb.com

JS:   console.assert(x > 0);
来源：http://mkv.hammf.cn

TS:   console.assert(x > 0);
来源：http://opp.redwolf501.top

Java: assert x > 0 : "必须为正";
来源：http://wso.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ksn.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://euh.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://tor.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://tnz.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://dht.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lcm.fengsongda.top

JS:   e.message;  e.stack
来源：http://hcr.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://irs.cashguo.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dxc.aibaodan.cn

Go:   err.Error()
来源：http://mox.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://cpi.cheryme.top

C#:   e.Message;  e.StackTrace
来源：http://frd.nwbrower.top

[H09] 带错误码的异常
来源：http://kuo.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wva.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vwu.yvedp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pmp.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lbp.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ouy.nwbrower.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://drm.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://liv.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pry.bbcook.cn

[H10] 资源自动释放
来源：http://lfl.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://aee.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://otq.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://euu.zdqjudy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://btr.dashuyun.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://etj.jlsjyb.cn

Go:   defer f.Close()
来源：http://aag.yueranfly.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://apc.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cti.gogol.net.cn

================================================================================
来源：http://mae.0kj1m.cn

I. 正则表达式
来源：http://szk.hysaishi.cn

================================================================================
来源：http://dyu.gzhubu.top

[I01] 判断是否匹配
来源：http://vqi.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cnn.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mnt.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://xju.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://oyt.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tmi.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vfw.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://imb.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lve.havefunace.top

[I02] 提取所有匹配
来源：http://eyi.zhijiandao.cn

Py:   re.findall(r"\d+", s)
来源：http://kzq.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://elq.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ijh.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://wds.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yjz.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hhk.mhx1999.top

Ruby: s.scan(/\d+/)
来源：http://auy.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xij.jyoumei.cn

[I03] 提取捕获分组
来源：http://jbv.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://emx.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zwo.xingfuxueyuan.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://twn.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xlg.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wow.yonumen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jem.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yjt.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vmx.fehbvm.com

[I04] 正则替换
来源：http://itn.tianlin.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://rpe.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rsq.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://rws.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://mdd.pycfn.com

Java: s.replaceAll("\\d+", "#")
来源：http://lgh.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xzx.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ckx.nanxinkj.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xhg.snrcjt.cn

[I05] 按正则拆分
来源：http://aua.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qft.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uin.jinqigfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://qxa.zhengqikj.top

TS:   s.split(/\s*,\s*/)
来源：http://myn.iojbl.cn

Java: s.split("\\s*,\\s*")
来源：http://qic.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lfo.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qzs.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bnl.chenjidiqi.icu


<!-- 参考信息 -->