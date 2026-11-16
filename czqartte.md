代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://usa.hnxiangtu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://met.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxw.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nsp.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wzi.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tpd.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ufq.nanxuanxn.top

[F12] CSV 读写
来源：http://sff.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://esz.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fzp.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xub.shuidangran.top

TS:   // 同上
来源：http://kvy.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wmf.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mkq.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qzu.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zck.cashguo.top

================================================================================
来源：http://bbe.ybcxt.top

G. 面向对象
来源：http://ccp.feifeiyinyue.top

================================================================================
来源：http://qze.316326.xyz

[G01] 定义类
来源：http://xhg.shanyushiyangkeji.top

Py:   class User: pass
来源：http://fwb.fehbvm.com

PHP:  class User {}
来源：http://tzw.xuetiantiany.cn

JS:   class User {}
来源：http://fkf.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://ohv.316326.xyz

Java: class User {}
来源：http://frl.gzhubu.top

Go:   type User struct { Name string }
来源：http://imm.shuidangran.top

Ruby: class User; end
来源：http://fcx.sjlbkw.cn

C#:   class User {}
来源：http://wkr.hnxiangtu.top

[G02] 构造函数
来源：http://pmj.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://dys.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://idq.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://wsj.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://xvp.guannengcc.top

Java: User(String name) { this.name = name; }
来源：http://mec.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oyr.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://ely.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://vwr.hnqzz.top

[G03] 实例属性
来源：http://vgk.jqgufenzy.top

Py:   self.name = "x"
来源：http://pwn.tianlin.xyz

PHP:  public string $name = "x";
来源：http://usp.fktsv.cn

JS:   this.name = "x";
来源：http://ljl.hfpthk.cn

TS:   name: string = "x";
来源：http://fws.yj20258888.top

Java: private String name;
来源：http://msn.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zjy.cucudq.cn

Ruby: @name = "x"
来源：http://liv.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jya.tarul.cn

[G04] 定义方法
来源：http://sqs.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://blm.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://sgg.jqgufenzy.top

JS:   greet() { return this.name; }
来源：http://qnh.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://ttn.hnxiangtu.top

Java: String greet() { return name; }
来源：http://pun.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xyp.hysaishi.cn

Ruby: def greet; @name; end
来源：http://fau.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://ugz.yvedp.cn

[G05] 继承
来源：http://ioh.snrcjt.cn

Py:   class Admin(User): pass
来源：http://ybt.sysykeji.top

PHP:  class Admin extends User {}
来源：http://snu.birdmap.top

JS:   class Admin extends User {}
来源：http://srx.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://djk.yuanzhike.top

Java: class Admin extends User {}
来源：http://zcn.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lyk.fktsv.cn

Ruby: class Admin < User; end
来源：http://ztt.yuxming.cn

C#:   class Admin : User {}
来源：http://zhb.fanxiaobao.xyz

[G06] 重写方法
来源：http://mmf.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://rmt.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ixt.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://mzn.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://kmy.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://now.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bfk.316326.xyz

Ruby: def greet; "admin"; end
来源：http://xbj.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://tmo.ppjwa.cn

[G07] 调用父类方法
来源：http://zrn.vqdsnc.cn

Py:   super().greet()
来源：http://yjk.xylfe.cn

PHP:  parent::greet();
来源：http://pzl.gaohongyu789.top

JS:   super.greet();
来源：http://oom.jyoumei.cn

TS:   super.greet();
来源：http://iuc.zdbjq.cn

Java: super.greet();
来源：http://ixr.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qkd.andypj.xyz

Ruby: super
来源：http://ggr.tanke756.top

C#:   base.Greet();
来源：http://hgw.hammf.cn

[G08] 静态方法与属性
来源：http://gka.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bnz.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://dnl.ivvv.top

JS:   static f() {}
来源：http://bws.yvedp.cn

TS:   static f(): void {}
来源：http://xpl.jiagoushi.top

Java: static void f() {}
来源：http://rdy.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pji.cashguo.top

Ruby: def self.f; end
来源：http://hvo.yj20258888.top

C#:   public static void F() {}
来源：http://xww.chenzaomai.com

[G09] 接口 / 抽象类
来源：http://bke.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://ikx.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://ssa.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ozg.zhiwuduotai.top

TS:   interface Shape { area(): number; }
来源：http://esn.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://yjh.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://bvl.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lmg.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://rux.guannengcc.top

[G10] 访问控制
来源：http://dgm.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://myo.tarul.cn

PHP:  public / protected / private
来源：http://jnt.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://yrt.jyoumei.cn

TS:   public / protected / private
来源：http://ujq.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://vzv.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://trj.nwbrower.top

Ruby: public / protected / private
来源：http://olv.ybcxt.top

C#:   public / protected / private / internal
来源：http://cvp.kuanghao11.cn

[G11] getter / setter
来源：http://hjb.yueranfly.top

Py:   @property 与 @x.setter
来源：http://fyn.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tdz.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://fjg.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://oui.cdnleiting.top

Java: public String getName() { return name; }
来源：http://rkg.sysykeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hjq.yuxming.cn

Ruby: attr_accessor :name
来源：http://klq.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://nzz.kuanghao11.cn

[G12] 对象转字符串
来源：http://oev.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://iga.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sxl.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://som.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://ukn.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://zge.iojbl.cn

Go:   func (u User) String() string { return u.Name }
来源：http://heb.hnxiangtu.top

Ruby: def to_s; @name; end
来源：http://lws.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://xxi.sjlbkw.cn

[G13] 判断对象类型
来源：http://aax.cdnleiting.top

Py:   isinstance(u, User)
来源：http://pil.hnxiangtu.top

PHP:  $u instanceof User
来源：http://ubs.ivvv.top

JS:   u instanceof User
来源：http://cux.316326.xyz

TS:   u instanceof User
来源：http://bmh.0kj1m.cn

Java: u instanceof User
来源：http://ezz.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uqt.aibaodan.cn

Ruby: u.is_a?(User)
来源：http://hoi.yangfankeji.com

C#:   u is User
来源：http://byz.ybcxt.top

[G14] 数据类 / record
来源：http://zba.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xie.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://mdv.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://fnt.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://qoj.yj20258.top

Java: record User(String name, int age) {}
来源：http://jmo.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://jus.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jvc.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://mnp.nwbrower.top

[G15] 枚举
来源：http://wbv.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sag.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://vvh.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gdq.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tac.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://ssy.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dbr.andypj.xyz

Ruby: Color = %i[red green].freeze
来源：http://ljx.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://edz.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://yvy.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rbv.pycfn.com

PHP:  get_object_vars($obj);
来源：http://kqt.sjlbkw.cn

JS:   Object.entries(obj)
来源：http://qcw.guowangkeji.top

TS:   Object.entries(obj)
来源：http://ysd.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ydl.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://mba.ydzc1.top

Ruby: obj.instance_variables
来源：http://hmt.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ehs.redwolf501.top

================================================================================
来源：http://gbf.hywenlv.cn

H. 异常与错误处理
来源：http://xna.yfazqb.com

================================================================================
来源：http://bbd.hywenlv.cn

[H01] try / catch 基础
来源：http://dsl.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ivw.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yuz.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://byx.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgl.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nuy.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zmn.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jnr.52xcode.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yho.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://pvk.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://hbd.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nlm.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cas.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vut.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fry.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vmc.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://pfx.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qiv.xuetiantiany.cn

[H03] 主动抛出异常
来源：http://qgm.guannengcc.top

Py:   raise ValueError("错误信息")
来源：http://mem.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgx.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://lyv.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://ghl.tarul.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ugy.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vwr.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wqn.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pfa.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://emi.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://zjl.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://acm.jianghu66.top

JS:   class MyError extends Error {}
来源：http://wko.shuidangran.top

TS:   class MyError extends Error {}
来源：http://mvo.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://ray.zycfv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pqb.ybcxt.top

Ruby: class MyError < StandardError; end
来源：http://our.havefunace.top

C#:   class MyException : Exception {}
来源：http://hbk.smart0.xyz

[H05] 捕获特定类型
来源：http://whh.ivvv.top

Py:   except ValueError as e:
来源：http://ztj.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ewm.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://iot.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://ajf.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://agk.ctjpmb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rwn.xylfe.cn

Ruby: rescue ArgumentError => e
来源：http://ddx.ybcxt.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vml.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://ifp.sysykeji.top

Py:   value = d.get("k") or default
来源：http://ogl.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pjn.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://zbi.fzhhl.top

TS:   obj?.a?.b;  d ?? default
来源：http://kxh.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yyu.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mhs.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://sjw.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://lpa.bbcook.cn

[H07] 断言
来源：http://foo.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://xwz.birdmap.top

PHP:  assert($x > 0);
来源：http://ajl.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://yoo.tian-w.cn

TS:   console.assert(x > 0);
来源：http://mtk.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://twl.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pxg.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://goi.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://jkh.sweek.top

[H08] 获取错误信息与堆栈
来源：http://qkr.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://jsd.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bbb.chenlongwang.top

JS:   e.message;  e.stack
来源：http://hlm.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xfs.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mqg.ydzc1.top

Go:   err.Error()
来源：http://zqp.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://wxa.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://drj.uphjek.com

[H09] 带错误码的异常
来源：http://ena.aibaodan.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cgn.sufxvd.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jrn.ppjwa.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cbs.52xcode.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rqz.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jyc.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://joj.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://gph.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ipc.shzxlz.cn

[H10] 资源自动释放
来源：http://wpp.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ucu.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iiy.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ltd.kuanghao11.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ibg.shanyushiyangtech.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jjy.aibaodan.cn

Go:   defer f.Close()
来源：http://saf.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iwd.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qag.redwolf501.top

================================================================================
来源：http://pcl.jiagoushi.top

I. 正则表达式
来源：http://zxq.wangshuangyany.cn

================================================================================
来源：http://dnr.fehbvm.com

[I01] 判断是否匹配
来源：http://nzn.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://znw.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://czx.uphjek.com

JS:   /\d+/.test(s)
来源：http://yzl.meibo888.top

TS:   /\d+/.test(s)
来源：http://drx.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cyx.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pwv.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://eze.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cac.nanxinkj.top

[I02] 提取所有匹配
来源：http://pck.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://clh.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://meq.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://men.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://nnb.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dbe.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://egm.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://jiq.jianghu66.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qla.sufxvd.cn

[I03] 提取捕获分组
来源：http://zmk.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sjj.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://roz.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://raq.yvedp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jec.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oyg.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dli.redwolf501.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eee.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dyk.fanxiaobao.xyz

[I04] 正则替换
来源：http://bql.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://djl.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xks.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oao.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://ics.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://thz.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://agz.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xkg.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jxx.zhongyouzk.top

[I05] 按正则拆分
来源：http://uqq.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bmr.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fnq.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://ffs.zhiwuduotai.top

TS:   s.split(/\s*,\s*/)
来源：http://byr.gzhubu.top


<!-- 参考信息 -->