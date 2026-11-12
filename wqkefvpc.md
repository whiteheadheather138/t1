代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nrd.jlsjyb.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://puk.aibaodan.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ffp.yuxming.cn

TS:   // 同上
来源：http://hil.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fan.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wdj.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://til.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ypt.xuetiantiany.cn

================================================================================
来源：http://oiv.tanke756.top

G. 面向对象
来源：http://faq.sweek.top

================================================================================
来源：http://vqh.kuanghao11.cn

[G01] 定义类
来源：http://nqd.quarkkingdee.top

Py:   class User: pass
来源：http://evj.redwolf501.top

PHP:  class User {}
来源：http://vds.nwbrower.top

JS:   class User {}
来源：http://rpg.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://jnf.xuetiantiany.cn

Java: class User {}
来源：http://rwe.sufxvd.cn

Go:   type User struct { Name string }
来源：http://poc.havefunace.top

Ruby: class User; end
来源：http://pzw.nanxinkj.top

C#:   class User {}
来源：http://mkd.zdqjudy.top

[G02] 构造函数
来源：http://jky.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://qbv.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://qjs.yj20258.top

JS:   constructor(name) { this.name = name; }
来源：http://ioa.yongpay.top

TS:   constructor(public name: string) {}
来源：http://eoq.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://wod.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uau.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://gqo.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://vkp.xylfe.cn

[G03] 实例属性
来源：http://sus.cucudq.cn

Py:   self.name = "x"
来源：http://owz.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://taw.shuidangran.top

JS:   this.name = "x";
来源：http://uls.iojbl.cn

TS:   name: string = "x";
来源：http://dcj.sysykeji.top

Java: private String name;
来源：http://iqy.ydzc1.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ycl.uphjek.com

Ruby: @name = "x"
来源：http://won.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://aco.52xcode.cn

[G04] 定义方法
来源：http://jqc.fktsv.cn

Py:   def greet(self): return self.name
来源：http://vov.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bnz.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://bjj.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://kft.ctjpmb.com

Java: String greet() { return name; }
来源：http://qbq.daxiang520.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xnn.fengsongda.top

Ruby: def greet; @name; end
来源：http://mam.epnwcf.com

C#:   public string Greet() => Name;
来源：http://xce.meibo888.top

[G05] 继承
来源：http://lqr.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://mtx.yvedp.cn

PHP:  class Admin extends User {}
来源：http://yaz.c1oappe.top

JS:   class Admin extends User {}
来源：http://uul.tian-w.cn

TS:   class Admin extends User {}
来源：http://heq.yvedp.cn

Java: class Admin extends User {}
来源：http://yrz.dashuyun.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iur.sweek.top

Ruby: class Admin < User; end
来源：http://xpg.daxiang520.top

C#:   class Admin : User {}
来源：http://fxk.cdnleiting.top

[G06] 重写方法
来源：http://hpx.hammf.cn

Py:   def greet(self): return "admin"
来源：http://jmv.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://tkb.meibo888.top

JS:   greet() { return "admin"; }
来源：http://opf.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://ohj.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://mwq.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qet.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://luu.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://ugg.sysykeji.top

[G07] 调用父类方法
来源：http://qev.tarul.cn

Py:   super().greet()
来源：http://vrn.tanke756.top

PHP:  parent::greet();
来源：http://lny.feifeiyinyue.top

JS:   super.greet();
来源：http://fua.zdbjq.cn

TS:   super.greet();
来源：http://sqk.tian-w.cn

Java: super.greet();
来源：http://dtv.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://itl.guowangkeji.top

Ruby: super
来源：http://bhl.52xcode.cn

C#:   base.Greet();
来源：http://jkz.pengpengdd.cyou

[G08] 静态方法与属性
来源：http://vit.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tdr.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://umd.xylfe.cn

JS:   static f() {}
来源：http://pbi.jlsjyb.cn

TS:   static f(): void {}
来源：http://mwr.fzhhl.top

Java: static void f() {}
来源：http://hap.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://uqf.hcnkem.com

Ruby: def self.f; end
来源：http://wwr.sufxvd.cn

C#:   public static void F() {}
来源：http://yqe.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://jgq.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://xdx.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://xkr.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://kes.guowangkeji.top

TS:   interface Shape { area(): number; }
来源：http://yam.zycfv.cn

Java: interface Shape { double area(); }
来源：http://bgx.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://smv.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ygz.hesvh.cn

C#:   interface IShape { double Area(); }
来源：http://bsu.xinyue.icu

[G10] 访问控制
来源：http://ael.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://sts.zhiwuduotai.top

PHP:  public / protected / private
来源：http://mku.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://upm.zhengqikj.top

TS:   public / protected / private
来源：http://zaf.cheryme.top

Java: public / protected / private / 默认包级
来源：http://wjx.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://nje.yongpay.top

Ruby: public / protected / private
来源：http://zyv.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://jxl.wangshuangyany.cn

[G11] getter / setter
来源：http://uuh.sweek.top

Py:   @property 与 @x.setter
来源：http://ijk.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wls.smart0.xyz

JS:   get name() { return this._name; }
来源：http://jqv.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://tlw.yuanzhike.top

Java: public String getName() { return name; }
来源：http://ons.svipenyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ahd.yvedp.cn

Ruby: attr_accessor :name
来源：http://wrk.yfazqb.com

C#:   public string Name { get; set; }
来源：http://hrc.yfazqb.com

[G12] 对象转字符串
来源：http://gwi.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://pdd.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ixx.yonumen.top

JS:   toString() { return this.name; }
来源：http://ufp.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://evb.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://bdh.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://snv.hysaishi.cn

Ruby: def to_s; @name; end
来源：http://uzr.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://bbw.yj20258888.top

[G13] 判断对象类型
来源：http://bmp.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://lxm.aizwys.cn

PHP:  $u instanceof User
来源：http://xmc.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://tlo.smart0.xyz

TS:   u instanceof User
来源：http://xma.gogol.net.cn

Java: u instanceof User
来源：http://wmy.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://log.mhx1999.top

Ruby: u.is_a?(User)
来源：http://vsj.pycfn.com

C#:   u is User
来源：http://kcy.svipenyu.cn

[G14] 数据类 / record
来源：http://ttq.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://frm.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://ixx.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://pip.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://gql.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://him.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://sxs.bjfxy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sit.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://odp.nwbrower.top

[G15] 枚举
来源：http://fwv.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kam.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wea.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://frm.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iju.yanxiufei.cn

Java: enum Color { RED, GREEN }
来源：http://whe.yj202588.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qsz.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://voc.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pzi.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://sek.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ife.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://gwi.gogol.net.cn

JS:   Object.entries(obj)
来源：http://tev.yfazqb.com

TS:   Object.entries(obj)
来源：http://xiz.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rmp.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kby.tianlin.xyz

Ruby: obj.instance_variables
来源：http://qiw.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://rjj.zhaomingkeji.xyz

================================================================================
来源：http://sge.wangdashe.top

H. 异常与错误处理
来源：http://ipj.cdnleiting.top

================================================================================
来源：http://uiq.meibo888.top

[H01] try / catch 基础
来源：http://uou.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jde.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zsc.zhijiandao.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://waf.bjfxy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hts.nanxinkj.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ixa.ybcxt.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tno.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ixr.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qor.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://ink.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://fzz.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://yki.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rbq.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://yzy.cashguo.top

Java: try { f(); } finally { cleanup(); }
来源：http://bua.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eoc.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dll.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://sin.cheryme.top

[H03] 主动抛出异常
来源：http://gzc.hongshengwenyu.top

Py:   raise ValueError("错误信息")
来源：http://cac.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://azo.nanxuanxn.top

JS:   throw new Error("错误信息");
来源：http://thz.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://gjg.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tth.hesvh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jug.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://apd.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://syh.yj20258888.top

[H04] 自定义异常类型
来源：http://hnq.ctjpmb.com

Py:   class MyError(Exception): pass
来源：http://hmr.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://bwz.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://evh.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://vdx.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://onf.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pry.ydjk.org.cn

Ruby: class MyError < StandardError; end
来源：http://wre.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://ujs.smart0.xyz

[H05] 捕获特定类型
来源：http://jgy.hnqzz.top

Py:   except ValueError as e:
来源：http://vdp.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ioh.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://rto.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://vpp.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://iez.quarkkingdee.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqt.jyoumei.cn

Ruby: rescue ArgumentError => e
来源：http://oyk.shangyingyoupin.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ifp.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://idp.yonumen.top

Py:   value = d.get("k") or default
来源：http://hrk.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ytt.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://vet.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://grr.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iey.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iim.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://zzx.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://nzr.yangfankeji.com

[H07] 断言
来源：http://rly.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://vig.aibaodan.cn

PHP:  assert($x > 0);
来源：http://kwv.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://udd.nanxuanxn.top

TS:   console.assert(x > 0);
来源：http://jek.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://rps.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xoi.zhengqikj.top

Ruby: raise "必须为正" unless x > 0
来源：http://xqc.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://kng.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://rbq.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://lgv.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wsy.yfazqb.com

JS:   e.message;  e.stack
来源：http://msd.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pat.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://gac.pycfn.com

Go:   err.Error()
来源：http://bmh.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://dnw.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://vbo.nwbrower.top

[H09] 带错误码的异常
来源：http://tlf.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yhw.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://lwy.nwbrower.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pos.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hjf.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hkw.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://far.ehwqpu.com

Ruby: raise MyError.new("fail", 500)
来源：http://nzu.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pmz.sysykeji.top

[H10] 资源自动释放
来源：http://udq.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://bkn.pengpengdd.cyou

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ami.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wsa.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jfu.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qkn.hysaishi.cn

Go:   defer f.Close()
来源：http://aom.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lej.zhiwuduotai.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ran.aibaodan.cn

================================================================================
来源：http://qda.yj20258.top

I. 正则表达式
来源：http://uyr.sufxvd.cn

================================================================================
来源：http://vgn.bbcook.cn

[I01] 判断是否匹配
来源：http://sio.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://csm.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ekj.sysykeji.top

JS:   /\d+/.test(s)
来源：http://dmw.smart0.xyz

TS:   /\d+/.test(s)
来源：http://kie.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ula.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zwu.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://foh.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gsf.bjfxy.top

[I02] 提取所有匹配
来源：http://yaq.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://ihb.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zkl.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yjy.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://lqo.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nab.yj202588.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pgx.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://waz.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pww.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://zqd.hnxiangtu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sif.pengpengdd.cyou

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ydi.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://clv.hcnkem.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://piz.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fqh.jqgufenzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qhs.snrcjt.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dmi.ydzc1.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://acr.shangyingyoupin.top

[I04] 正则替换
来源：http://sww.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dvn.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://clw.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://qdx.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://cdo.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eyx.xylfe.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jpm.316326.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://ktu.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ayj.guowangkeji.top

[I05] 按正则拆分
来源：http://kts.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xbm.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sgo.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://akr.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://edv.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://frd.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zoi.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mcw.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eef.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ict.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vqa.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qsa.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbk.hcnkem.com


<!-- 参考信息 -->