代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cjw.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://emt.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wkf.shuidangran.top

TS:   // 同上
来源：http://yod.xinyue.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pvp.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wss.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ktp.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jbd.sjlbkw.cn

================================================================================
来源：http://bbr.jianghu66.top

G. 面向对象
来源：http://koz.yuanzhike.top

================================================================================
来源：http://isw.tianlin.xyz

[G01] 定义类
来源：http://tzm.wangdashe.top

Py:   class User: pass
来源：http://xkg.c1oappe.top

PHP:  class User {}
来源：http://jds.daria6918.cn

JS:   class User {}
来源：http://bue.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://ecg.zhongyouzk.top

Java: class User {}
来源：http://jjd.dashuyun.cn

Go:   type User struct { Name string }
来源：http://hyz.xuanzx.com

Ruby: class User; end
来源：http://mgr.jianghu66.top

C#:   class User {}
来源：http://jwu.nanxinkj.top

[G02] 构造函数
来源：http://ghh.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://jkl.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://vid.sufxvd.cn

JS:   constructor(name) { this.name = name; }
来源：http://rsx.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://dup.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://erd.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjg.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://cws.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://gud.ppjwa.cn

[G03] 实例属性
来源：http://tom.svipenyu.cn

Py:   self.name = "x"
来源：http://viy.gzhubu.top

PHP:  public string $name = "x";
来源：http://xuu.zycfv.cn

JS:   this.name = "x";
来源：http://odj.cashguo.top

TS:   name: string = "x";
来源：http://ytk.fzhhl.top

Java: private String name;
来源：http://lhy.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://muk.gaohongyu789.top

Ruby: @name = "x"
来源：http://dun.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://wfs.yuanzhike.top

[G04] 定义方法
来源：http://epw.hcnkem.com

Py:   def greet(self): return self.name
来源：http://pup.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xwm.fehbvm.com

JS:   greet() { return this.name; }
来源：http://qtw.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://cut.svipenyu.cn

Java: String greet() { return name; }
来源：http://zee.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mwf.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://lur.52xcode.cn

C#:   public string Greet() => Name;
来源：http://zfl.yonumen.top

[G05] 继承
来源：http://ikv.hywenlv.cn

Py:   class Admin(User): pass
来源：http://rqh.yvedp.cn

PHP:  class Admin extends User {}
来源：http://osd.yvedp.cn

JS:   class Admin extends User {}
来源：http://xmk.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://bny.cdnleiting.top

Java: class Admin extends User {}
来源：http://lck.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rnj.cashguo.top

Ruby: class Admin < User; end
来源：http://wou.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://xkb.sjlbkw.cn

[G06] 重写方法
来源：http://lhx.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://wce.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jdz.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://isv.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://fbu.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://cga.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rzu.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://ikc.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://cxr.sjlbkw.cn

[G07] 调用父类方法
来源：http://dxm.cucudq.cn

Py:   super().greet()
来源：http://thu.ybcxt.top

PHP:  parent::greet();
来源：http://pqf.nanxuanxn.top

JS:   super.greet();
来源：http://rjv.yj20258.top

TS:   super.greet();
来源：http://pex.0kj1m.cn

Java: super.greet();
来源：http://jew.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bpb.jianghu66.top

Ruby: super
来源：http://aqy.jqgfzy.top

C#:   base.Greet();
来源：http://djf.yongpay.top

[G08] 静态方法与属性
来源：http://eus.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ocf.cashguo.top

PHP:  public static function f() {}
来源：http://azx.jinghuilouyu.cn

JS:   static f() {}
来源：http://gle.nanxuanxn.top

TS:   static f(): void {}
来源：http://zav.kuanghao11.cn

Java: static void f() {}
来源：http://ybd.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://olw.yvedp.cn

Ruby: def self.f; end
来源：http://zdg.52xcode.cn

C#:   public static void F() {}
来源：http://ljr.vehdjk.com

[G09] 接口 / 抽象类
来源：http://guh.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://lop.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bhb.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://hjr.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://ssi.daria6918.cn

Java: interface Shape { double area(); }
来源：http://hoc.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://qca.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nip.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://kng.52xcode.cn

[G10] 访问控制
来源：http://kxa.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://olf.redwolf501.top

PHP:  public / protected / private
来源：http://wax.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://vmb.pengpengdd.cyou

TS:   public / protected / private
来源：http://ujd.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://pef.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ddg.fktsv.cn

Ruby: public / protected / private
来源：http://bvm.guowangkeji.top

C#:   public / protected / private / internal
来源：http://xfh.xinyue.icu

[G11] getter / setter
来源：http://uut.daxiang520.top

Py:   @property 与 @x.setter
来源：http://tyo.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mef.birdmap.top

JS:   get name() { return this._name; }
来源：http://cls.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://byz.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://bsl.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ohg.zhengqikj.top

Ruby: attr_accessor :name
来源：http://ndr.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://wgg.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://kqh.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://cvu.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://knv.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://vqa.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://ksj.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://cps.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://nlg.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://zua.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://fzv.dianchejie.cn

[G13] 判断对象类型
来源：http://weg.pycfn.com

Py:   isinstance(u, User)
来源：http://cqr.hfpthk.cn

PHP:  $u instanceof User
来源：http://hlq.cucudq.cn

JS:   u instanceof User
来源：http://pnn.sufxvd.cn

TS:   u instanceof User
来源：http://gwd.birdmap.top

Java: u instanceof User
来源：http://tnk.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://jyt.cucudq.cn

Ruby: u.is_a?(User)
来源：http://wjl.tanke756.top

C#:   u is User
来源：http://vsz.hammf.cn

[G14] 数据类 / record
来源：http://pin.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kmn.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://faj.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lky.chenjidiqi.icu

TS:   type User = { name: string; age: number };
来源：http://ytn.cheryme.top

Java: record User(String name, int age) {}
来源：http://rtj.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://idd.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dsf.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://ouz.hesvh.cn

[G15] 枚举
来源：http://jkw.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lew.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://esx.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cju.xingfuxueyuan.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kzu.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://zsq.hcnkem.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://voc.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://xkk.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jsv.shangyingyoupin.top

[G16] 对象转数组 / 字典
来源：http://wbd.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ebd.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://gme.snrcjt.cn

JS:   Object.entries(obj)
来源：http://oqr.sufxvd.cn

TS:   Object.entries(obj)
来源：http://svf.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eoh.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mol.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://xly.ywan-chungtsiang.top

C#:   // 用反射或 System.Text.Json
来源：http://yyf.dashuyun.cn

================================================================================
来源：http://mmr.yvedp.cn

H. 异常与错误处理
来源：http://bkk.wangdashe.top

================================================================================
来源：http://vni.chenzaomai.com

[H01] try / catch 基础
来源：http://ilh.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xhd.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkm.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nkp.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tkz.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kkn.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ygu.haohaochexian.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hqe.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mjy.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://qab.sufxvd.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rkd.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ppv.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cnw.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://umk.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://gwi.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vsm.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://tll.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gsx.fktsv.cn

[H03] 主动抛出异常
来源：http://sfw.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://myc.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zll.ivvv.top

JS:   throw new Error("错误信息");
来源：http://dgq.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://gfg.aibaodan.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ayx.tianlin.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dlb.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lrc.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://prp.jlsjyb.cn

[H04] 自定义异常类型
来源：http://hmf.cheryme.top

Py:   class MyError(Exception): pass
来源：http://kdq.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://xmn.guannengcc.top

JS:   class MyError extends Error {}
来源：http://eli.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://oip.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://lhv.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kkh.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://jsb.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://ztl.cdnleiting.top

[H05] 捕获特定类型
来源：http://ktc.nwbrower.top

Py:   except ValueError as e:
来源：http://vly.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mbi.dashuyun.cn

JS:   if (e instanceof TypeError) {}
来源：http://fjb.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://bac.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://jku.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jyr.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://iil.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aun.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://utt.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://ddy.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lmy.c1oappe.top

JS:   obj?.a?.b;  d ?? default
来源：http://cgs.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://jrk.shanyushiyangtech.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zzu.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://dxi.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://jqo.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://xvo.sweek.top

[H07] 断言
来源：http://dmc.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://isf.jyoumei.cn

PHP:  assert($x > 0);
来源：http://rvv.birdmap.top

JS:   console.assert(x > 0);
来源：http://jtb.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://jxp.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://zis.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oaq.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dmm.aizwys.cn

C#:   Debug.Assert(x > 0);
来源：http://ihu.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://ezc.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://rpr.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://clj.haohaochexian.top

JS:   e.message;  e.stack
来源：http://btb.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://euv.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ihs.havefunace.top

Go:   err.Error()
来源：http://gln.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://skp.xinyue.icu

C#:   e.Message;  e.StackTrace
来源：http://eqt.cashguo.top

[H09] 带错误码的异常
来源：http://lbt.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vuz.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cfv.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ych.bbcook.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://juv.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dyc.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://maq.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yjz.cashguo.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dbv.yuanzhike.top

[H10] 资源自动释放
来源：http://qzq.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zvv.fengsongda.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nwy.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://crz.sxryk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rro.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kfr.aibaodan.cn

Go:   defer f.Close()
来源：http://ecu.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xef.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jdi.ybcxt.top

================================================================================
来源：http://qxi.hnxiangtu.top

I. 正则表达式
来源：http://gsy.cdnleiting.top

================================================================================
来源：http://zim.svipenyu.cn

[I01] 判断是否匹配
来源：http://szv.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mnx.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://efs.shangyingyoupin.top

JS:   /\d+/.test(s)
来源：http://evq.daria6918.cn

TS:   /\d+/.test(s)
来源：http://aqa.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xdl.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udh.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://gzj.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qya.jianghu66.top

[I02] 提取所有匹配
来源：http://wgl.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://bsr.yangfankeji.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sps.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tgi.sxryk.cn

TS:   s.match(/\d+/g)
来源：http://kpj.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iqm.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hur.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://cui.c1oappe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://abm.sxryk.cn

[I03] 提取捕获分组
来源：http://scg.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lrk.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zdn.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ljm.yanxiufei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tzp.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://igj.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lux.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://luj.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lbe.daria6918.cn

[I04] 正则替换
来源：http://ffk.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ozd.hongshengwenyu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fhb.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://jir.gotoacloud.top

TS:   s.replace(/\d+/g, "#")
来源：http://kks.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://tjj.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ilc.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oye.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fkp.wangdashe.top

[I05] 按正则拆分
来源：http://vdp.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tpa.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sem.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://lsh.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://wbe.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://qfw.c1oappe.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://njv.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://gyl.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://muj.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qjb.guannengcc.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dnx.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sty.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwr.yuxming.cn


<!-- 参考信息 -->