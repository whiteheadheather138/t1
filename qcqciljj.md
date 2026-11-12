代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jpf.jiagoushi.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xvb.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oco.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vjj.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://myy.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bgl.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sff.wangdashe.top

[F12] CSV 读写
来源：http://zjr.vehdjk.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ntw.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qpv.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dmv.hcnkem.com

TS:   // 同上
来源：http://cuw.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ndu.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vua.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qbb.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fso.dianchejie.cn

================================================================================
来源：http://wlt.epnwcf.com

G. 面向对象
来源：http://mkz.hcnkem.com

================================================================================
来源：http://qag.ppjwa.cn

[G01] 定义类
来源：http://gaa.vqdsnc.cn

Py:   class User: pass
来源：http://hyr.feifeiyinyue.top

PHP:  class User {}
来源：http://rdw.zycfv.cn

JS:   class User {}
来源：http://zrv.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://cps.cqqwz.cn

Java: class User {}
来源：http://ngv.gzhubu.top

Go:   type User struct { Name string }
来源：http://xrv.cucudq.cn

Ruby: class User; end
来源：http://icw.zdqjudy.top

C#:   class User {}
来源：http://ixv.shuidangran.top

[G02] 构造函数
来源：http://nyo.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://thg.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://dcc.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://ecw.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://agh.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://qbl.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tlu.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://cff.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://klk.sxryk.cn

[G03] 实例属性
来源：http://gsf.9152youxi.cn

Py:   self.name = "x"
来源：http://oti.dashuyun.cn

PHP:  public string $name = "x";
来源：http://woi.hfpthk.cn

JS:   this.name = "x";
来源：http://jlg.mhx1999.top

TS:   name: string = "x";
来源：http://aga.zdqjudy.top

Java: private String name;
来源：http://nsn.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gwy.hesvh.cn

Ruby: @name = "x"
来源：http://pnp.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://zlq.hywenlv.cn

[G04] 定义方法
来源：http://auf.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://orw.shangyingyoupin.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gaf.zhongyouzk.top

JS:   greet() { return this.name; }
来源：http://xwd.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://liy.ctjpmb.com

Java: String greet() { return name; }
来源：http://fiq.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://xga.ppjwa.cn

Ruby: def greet; @name; end
来源：http://vde.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://frt.vqdsnc.cn

[G05] 继承
来源：http://gmf.nanxuanxn.top

Py:   class Admin(User): pass
来源：http://qlc.jlsjyb.cn

PHP:  class Admin extends User {}
来源：http://sys.wangdashe.top

JS:   class Admin extends User {}
来源：http://rkk.fengsongda.top

TS:   class Admin extends User {}
来源：http://uhf.tarul.cn

Java: class Admin extends User {}
来源：http://hce.52xcode.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://umc.tianlin.xyz

Ruby: class Admin < User; end
来源：http://doe.kuanghao11.cn

C#:   class Admin : User {}
来源：http://wxy.uphjek.com

[G06] 重写方法
来源：http://nrw.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://yaw.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://bbz.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://cvs.xinyue.icu

TS:   greet(): string { return "admin"; }
来源：http://edn.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://xgv.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://znk.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://jfr.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://taa.ppjwa.cn

[G07] 调用父类方法
来源：http://fmx.jlsjyb.cn

Py:   super().greet()
来源：http://kuh.hnxiangtu.top

PHP:  parent::greet();
来源：http://mlf.sjlbkw.cn

JS:   super.greet();
来源：http://pvr.birdmap.top

TS:   super.greet();
来源：http://mil.shuidangran.top

Java: super.greet();
来源：http://swo.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oql.hnqzz.top

Ruby: super
来源：http://zjl.yj20258.top

C#:   base.Greet();
来源：http://acp.nanxinkj.top

[G08] 静态方法与属性
来源：http://jfs.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://htp.316326.xyz

PHP:  public static function f() {}
来源：http://nkp.ydjk.org.cn

JS:   static f() {}
来源：http://xgl.feifeiyinyue.top

TS:   static f(): void {}
来源：http://nvw.gzhubu.top

Java: static void f() {}
来源：http://agq.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mtu.daxiang520.top

Ruby: def self.f; end
来源：http://aiv.hongshengwenyu.top

C#:   public static void F() {}
来源：http://msc.vehdjk.com

[G09] 接口 / 抽象类
来源：http://vyy.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://pzd.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iuz.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tns.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://rnx.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://pqj.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://uis.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qed.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://fje.sweek.top

[G10] 访问控制
来源：http://kit.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://hhx.ybcxt.top

PHP:  public / protected / private
来源：http://cjp.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://bjk.yuanzhike.top

TS:   public / protected / private
来源：http://gzk.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://zhi.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cxd.yanxiufei.cn

Ruby: public / protected / private
来源：http://epl.yuxming.cn

C#:   public / protected / private / internal
来源：http://zuc.feifeiyinyue.top

[G11] getter / setter
来源：http://blc.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://anv.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oen.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://mkx.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://xop.iojbl.cn

Java: public String getName() { return name; }
来源：http://fpn.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pet.yj20258888.top

Ruby: attr_accessor :name
来源：http://hnu.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://clr.ppjwa.cn

[G12] 对象转字符串
来源：http://pfi.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://quj.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yth.hysaishi.cn

JS:   toString() { return this.name; }
来源：http://iad.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://bjd.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://pye.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hoz.sweek.top

Ruby: def to_s; @name; end
来源：http://gty.iojbl.cn

C#:   public override string ToString() => Name;
来源：http://nwb.sweek.top

[G13] 判断对象类型
来源：http://omh.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://txy.havefunace.top

PHP:  $u instanceof User
来源：http://uog.hcnkem.com

JS:   u instanceof User
来源：http://ier.hcnkem.com

TS:   u instanceof User
来源：http://rkp.ctjpmb.com

Java: u instanceof User
来源：http://lpv.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gqz.havefunace.top

Ruby: u.is_a?(User)
来源：http://rpq.hesvh.cn

C#:   u is User
来源：http://svs.yongpay.top

[G14] 数据类 / record
来源：http://eav.yuanzhike.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://waj.epnwcf.com

PHP:  // 用 readonly 属性模拟
来源：http://bty.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qbq.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://nmz.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://yaa.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://xan.cdnleiting.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zbm.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://cqv.jyoumei.cn

[G15] 枚举
来源：http://xmq.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tld.gogol.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pfi.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hwi.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zty.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://hnk.andypj.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://exr.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://mwo.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ham.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://hlu.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://stk.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://uwx.jinqigufen.top

JS:   Object.entries(obj)
来源：http://mvi.bjfxy.top

TS:   Object.entries(obj)
来源：http://rfd.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zau.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://lnc.redwolf501.top

Ruby: obj.instance_variables
来源：http://qss.hongshengwenyu.top

C#:   // 用反射或 System.Text.Json
来源：http://hkt.sxryk.cn

================================================================================
来源：http://agp.jyoumei.cn

H. 异常与错误处理
来源：http://zze.zdbjq.cn

================================================================================
来源：http://oef.guannengcc.top

[H01] try / catch 基础
来源：http://wwa.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pqy.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tqj.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bjo.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gim.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bat.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cqr.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rmm.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://joo.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://rnn.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://iie.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mwi.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fqx.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oom.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://oun.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://klg.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qnk.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://asr.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://jfc.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://xtd.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://acu.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://wdn.316326.xyz

TS:   throw new Error("错误信息");
来源：http://nku.yonumen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sbn.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ttq.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ldc.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://oru.316326.xyz

[H04] 自定义异常类型
来源：http://att.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://mta.iojbl.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ees.gzhubu.top

JS:   class MyError extends Error {}
来源：http://jsa.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://mka.shanyushiyangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://cfz.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nlb.shanyushiyangtech.top

Ruby: class MyError < StandardError; end
来源：http://lfq.zhoulong.xyz

C#:   class MyException : Exception {}
来源：http://sde.hywenlv.cn

[H05] 捕获特定类型
来源：http://oiq.yfazqb.com

Py:   except ValueError as e:
来源：http://vsh.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oym.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://uma.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://zsq.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://bwv.jyoumei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hbb.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://gzu.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oou.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://nzj.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://okd.daria6918.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qum.zdbjq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kxk.xylfe.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fyk.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oka.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://apa.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://syj.gogol.net.cn

C#:   obj?.A?.B ?? default
来源：http://uvp.shanyushiyangtech.top

[H07] 断言
来源：http://syl.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://ere.bbcook.cn

PHP:  assert($x > 0);
来源：http://cpp.andypj.xyz

JS:   console.assert(x > 0);
来源：http://owl.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://scl.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://idq.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xht.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ves.jinqigufen.top

C#:   Debug.Assert(x > 0);
来源：http://gwy.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://pst.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://bey.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rqb.xinyue.icu

JS:   e.message;  e.stack
来源：http://lqv.ppjwa.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qgk.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tek.andypj.xyz

Go:   err.Error()
来源：http://gvq.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://owb.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://bsy.hammf.cn

[H09] 带错误码的异常
来源：http://hox.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vsa.nanxuanxn.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ntz.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://okl.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yvv.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fmd.havefunace.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zbv.aibaodan.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qxs.aibaodan.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rgl.yanxiufei.cn

[H10] 资源自动释放
来源：http://rjc.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vis.52xcode.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xve.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rzh.ydzc1.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ekj.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ool.dianchejie.cn

Go:   defer f.Close()
来源：http://jxs.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vys.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hpm.fanxiaobao.xyz

================================================================================
来源：http://zte.yueranfly.top

I. 正则表达式
来源：http://hjv.zhixingplan.top

================================================================================
来源：http://dbl.cashguo.top

[I01] 判断是否匹配
来源：http://voj.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iou.zhaomingkeji.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wlv.ppjwa.cn

JS:   /\d+/.test(s)
来源：http://vnv.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://hwf.redwolf501.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aqv.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pvg.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://xgs.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yld.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://eks.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://hij.yvedp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wsz.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xza.ivvv.top

TS:   s.match(/\d+/g)
来源：http://ump.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rgu.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fvk.yuxming.cn

Ruby: s.scan(/\d+/)
来源：http://dsp.gogol.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://soi.yanxiufei.cn

[I03] 提取捕获分组
来源：http://ppc.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nnp.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qtz.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yau.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qlq.shuidangran.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yce.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dya.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ngw.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kru.hysaishi.cn

[I04] 正则替换
来源：http://urk.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://raa.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bgs.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://rpg.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://sbl.bbcook.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zlu.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://djz.cashguo.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gak.guowangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://few.smart0.xyz

[I05] 按正则拆分
来源：http://fla.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mpb.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oqh.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://rep.xinyue.icu

TS:   s.split(/\s*,\s*/)
来源：http://ysi.xuetiantiany.cn


<!-- 参考信息 -->