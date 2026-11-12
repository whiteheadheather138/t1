代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xfx.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vmz.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hxx.hammf.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://efz.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztk.cdnleiting.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qps.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://exz.c1oappe.top

[F12] CSV 读写
来源：http://vdj.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uwu.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oxi.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://axk.hongshengwenyu.top

TS:   // 同上
来源：http://gcj.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://por.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://brf.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zdv.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://lor.cashguo.top

================================================================================
来源：http://wtx.zhijiandao.cn

G. 面向对象
来源：http://yce.ivvv.top

================================================================================
来源：http://egf.sjlbkw.cn

[G01] 定义类
来源：http://yyk.xylfe.cn

Py:   class User: pass
来源：http://uoj.hesvh.cn

PHP:  class User {}
来源：http://oxc.hongshengwenyu.top

JS:   class User {}
来源：http://ing.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://yqs.svipenyu.cn

Java: class User {}
来源：http://uyy.0kj1m.cn

Go:   type User struct { Name string }
来源：http://jyg.havefunace.top

Ruby: class User; end
来源：http://ecs.zhiwuduotai.top

C#:   class User {}
来源：http://fzb.kuanghao11.cn

[G02] 构造函数
来源：http://ezi.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://rux.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://igo.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://hll.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://bom.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://ptf.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wob.meibo888.top

Ruby: def initialize(name); @name = name; end
来源：http://uea.yj202588.top

C#:   public User(string name) { Name = name; }
来源：http://kyu.shanyushiyangkeji.top

[G03] 实例属性
来源：http://mzn.chenjidiqi.icu

Py:   self.name = "x"
来源：http://snx.hcnkem.com

PHP:  public string $name = "x";
来源：http://qac.hfpthk.cn

JS:   this.name = "x";
来源：http://unf.sweek.top

TS:   name: string = "x";
来源：http://ycz.aizwys.cn

Java: private String name;
来源：http://qky.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eji.xziqi.cn

Ruby: @name = "x"
来源：http://dnb.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://btx.zhongyouzk.top

[G04] 定义方法
来源：http://sck.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://cga.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://udr.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://apt.zhengqikj.top

TS:   greet(): string { return this.name; }
来源：http://gnz.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://ixy.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://njk.yj20258.top

Ruby: def greet; @name; end
来源：http://xus.ybcxt.top

C#:   public string Greet() => Name;
来源：http://gcs.pycfn.com

[G05] 继承
来源：http://ugc.wangdashe.top

Py:   class Admin(User): pass
来源：http://juf.yuxming.cn

PHP:  class Admin extends User {}
来源：http://jkx.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://wnr.yuxming.cn

TS:   class Admin extends User {}
来源：http://kym.cqqwz.cn

Java: class Admin extends User {}
来源：http://wip.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pjv.hysaishi.cn

Ruby: class Admin < User; end
来源：http://jks.jlsjyb.cn

C#:   class Admin : User {}
来源：http://gyf.fanxiaobao.xyz

[G06] 重写方法
来源：http://khu.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://snm.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dgn.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://ggj.jinqigufen.top

TS:   greet(): string { return "admin"; }
来源：http://okc.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ymi.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ipv.zhijiandao.cn

Ruby: def greet; "admin"; end
来源：http://qxh.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://xpn.ydzc1.top

[G07] 调用父类方法
来源：http://meb.guowangkeji.top

Py:   super().greet()
来源：http://hqy.andypj.xyz

PHP:  parent::greet();
来源：http://wuh.chenzaomai.com

JS:   super.greet();
来源：http://ava.yuxming.cn

TS:   super.greet();
来源：http://jaa.yfazqb.com

Java: super.greet();
来源：http://lvd.yvedp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jwz.daria6918.cn

Ruby: super
来源：http://ljf.xziqi.cn

C#:   base.Greet();
来源：http://quz.fzhhl.top

[G08] 静态方法与属性
来源：http://zft.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kgh.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://zts.dashuyun.cn

JS:   static f() {}
来源：http://sje.hammf.cn

TS:   static f(): void {}
来源：http://dvj.jinyuanbaomall.cn

Java: static void f() {}
来源：http://zgx.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gpm.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://gbm.tian-w.cn

C#:   public static void F() {}
来源：http://myi.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://wln.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://cki.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yav.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wab.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://jkk.sysykeji.top

Java: interface Shape { double area(); }
来源：http://jhl.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://btd.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fgg.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://xmf.cucudq.cn

[G10] 访问控制
来源：http://kza.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://scb.chenzaomai.com

PHP:  public / protected / private
来源：http://jnk.xinyue.icu

JS:   #private 字段；其余公开
来源：http://mnn.nwbrower.top

TS:   public / protected / private
来源：http://qrw.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://iox.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://qke.yongpay.top

Ruby: public / protected / private
来源：http://gnl.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://myb.tanke756.top

[G11] getter / setter
来源：http://ciy.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://mgm.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gqr.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://ggm.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://gsn.guowangkeji.top

Java: public String getName() { return name; }
来源：http://wna.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fvg.shuidangran.top

Ruby: attr_accessor :name
来源：http://jvb.zycfv.cn

C#:   public string Name { get; set; }
来源：http://drd.cdnleiting.top

[G12] 对象转字符串
来源：http://ssx.chenjidiqi.icu

Py:   def __str__(self): return self.name
来源：http://wos.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lxj.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://qol.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://xhn.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://fub.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vuk.fzhhl.top

Ruby: def to_s; @name; end
来源：http://hnv.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://mbj.guannengcc.top

[G13] 判断对象类型
来源：http://pix.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://vcg.jinqigufen.top

PHP:  $u instanceof User
来源：http://swu.yueranfly.top

JS:   u instanceof User
来源：http://zha.52xcode.cn

TS:   u instanceof User
来源：http://wyo.haohaochexian.top

Java: u instanceof User
来源：http://rdz.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wet.cdnleiting.top

Ruby: u.is_a?(User)
来源：http://ajv.guannengcc.top

C#:   u is User
来源：http://did.hesvh.cn

[G14] 数据类 / record
来源：http://rmj.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jio.cashguo.top

PHP:  // 用 readonly 属性模拟
来源：http://pww.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jps.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://yjx.ivvv.top

Java: record User(String name, int age) {}
来源：http://yeh.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://wpu.nanxinkj.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://suk.yj202588.top

C#:   record User(string Name, int Age);
来源：http://sgs.yanxiufei.cn

[G15] 枚举
来源：http://sln.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cwo.yangfankeji.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ljn.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ssi.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://emv.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://eub.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jec.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://vmo.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jwh.aizwys.cn

[G16] 对象转数组 / 字典
来源：http://ism.tarul.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://npv.yonumen.top

PHP:  get_object_vars($obj);
来源：http://ozt.daria6918.cn

JS:   Object.entries(obj)
来源：http://ldj.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://usy.uphjek.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eqg.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vfp.hfpthk.cn

Ruby: obj.instance_variables
来源：http://igr.nanxuanxn.top

C#:   // 用反射或 System.Text.Json
来源：http://lsk.jinqigfzy.top

================================================================================
来源：http://ctx.hongshengwenyu.top

H. 异常与错误处理
来源：http://vgh.jinyuanbaomall.cn

================================================================================
来源：http://iki.vehdjk.com

[H01] try / catch 基础
来源：http://dqs.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nwf.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fhs.sweek.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://htw.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ojl.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dkg.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jxo.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yqm.guowangkeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bho.cashguo.top

[H02] finally / ensure 收尾
来源：http://qfh.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://rph.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pxz.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://otp.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xkp.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://zen.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vze.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lwq.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://zrt.c1oappe.top

[H03] 主动抛出异常
来源：http://fmy.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://cjw.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vwm.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://exv.kuanghao11.cn

TS:   throw new Error("错误信息");
来源：http://sou.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ruq.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://irb.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://noo.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://vne.chenlongwang.top

[H04] 自定义异常类型
来源：http://owz.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://pce.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qgk.tarul.cn

JS:   class MyError extends Error {}
来源：http://iby.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://pvi.andypj.xyz

Java: class MyException extends RuntimeException {}
来源：http://svj.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mbs.smart0.xyz

Ruby: class MyError < StandardError; end
来源：http://qof.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://wmd.fktsv.cn

[H05] 捕获特定类型
来源：http://baq.wangshuangyany.cn

Py:   except ValueError as e:
来源：http://bft.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bjz.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://szr.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://bdb.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://zqp.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xqp.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://fvo.tian-w.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mic.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://qeb.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://hth.xylfe.cn

PHP:  $v = $d["k"] ?? null;
来源：http://etq.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hgy.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ynn.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwy.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fax.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://gcn.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://sds.havefunace.top

[H07] 断言
来源：http://bgq.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://gzp.9152youxi.cn

PHP:  assert($x > 0);
来源：http://wao.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://whc.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://kmk.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://pga.fzhhl.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uyr.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://csy.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://lod.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://bdo.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://hvt.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fyj.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://wqe.yvedp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lgd.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ens.ppjwa.cn

Go:   err.Error()
来源：http://daj.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://yql.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://twq.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://fxw.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ujm.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vaa.nanxinkj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zgf.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jbt.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jqf.yonumen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xtn.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://col.tian-w.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://obt.tarul.cn

[H10] 资源自动释放
来源：http://zuk.316326.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://kme.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://akf.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://quu.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://enc.cheryme.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jvn.ydjk.org.cn

Go:   defer f.Close()
来源：http://wdf.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://roo.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rzp.birdmap.top

================================================================================
来源：http://war.jinqigfzy.top

I. 正则表达式
来源：http://flc.yongpay.top

================================================================================
来源：http://elx.tanke756.top

[I01] 判断是否匹配
来源：http://izt.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kzb.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://zzx.pengpengdd.cyou

JS:   /\d+/.test(s)
来源：http://psz.sysykeji.top

TS:   /\d+/.test(s)
来源：http://abd.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ymt.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ylo.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://htp.yj202588.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nsp.316326.xyz

[I02] 提取所有匹配
来源：http://ljk.zdqjudy.top

Py:   re.findall(r"\d+", s)
来源：http://rry.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kzm.smart0.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mlw.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://adb.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://apj.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tab.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://pcf.xuanzx.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lyk.hcnkem.com

[I03] 提取捕获分组
来源：http://bxf.sxryk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://apn.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gav.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zht.yj202588.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oqx.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ytg.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pdu.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pux.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xmm.ybcxt.top

[I04] 正则替换
来源：http://xcr.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kgh.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gzl.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://jbe.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://tof.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://wvc.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qqj.shangyingyoupin.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fey.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nlb.sweek.top

[I05] 按正则拆分
来源：http://uen.bjfxy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kgt.zycfv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kdl.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://umr.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://bua.hammf.cn


<!-- 参考信息 -->