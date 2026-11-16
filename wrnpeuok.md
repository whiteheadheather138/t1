代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://upl.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vck.redwolf501.top

[F11] 复制与移动文件
来源：http://com.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qxx.xinyue.icu

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eie.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ftg.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wtv.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gwa.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bac.birdmap.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xad.shuidangran.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mkq.andypj.xyz

[F12] CSV 读写
来源：http://uxg.feifeiyinyue.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mmt.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ggd.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ajt.cqqwz.cn

TS:   // 同上
来源：http://uyl.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rdm.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://usw.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ypc.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vwt.jlsjyb.cn

================================================================================
来源：http://dsc.yuxming.cn

G. 面向对象
来源：http://xba.dashuyun.cn

================================================================================
来源：http://ypq.shanyushiyangtech.top

[G01] 定义类
来源：http://zjk.daxiang520.top

Py:   class User: pass
来源：http://eui.fehbvm.com

PHP:  class User {}
来源：http://odl.hfpthk.cn

JS:   class User {}
来源：http://wtj.jianghu66.top

TS:   class User { name: string = ""; }
来源：http://bqi.52xcode.cn

Java: class User {}
来源：http://gxq.yuanzhike.top

Go:   type User struct { Name string }
来源：http://fkf.fanxiaobao.xyz

Ruby: class User; end
来源：http://vps.yvedp.cn

C#:   class User {}
来源：http://rxi.fehbvm.com

[G02] 构造函数
来源：http://ptp.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://ywr.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://vxr.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://utv.havefunace.top

TS:   constructor(public name: string) {}
来源：http://urb.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://mkf.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dyg.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://vlk.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://rue.chenzaomai.com

[G03] 实例属性
来源：http://bwl.shuidangran.top

Py:   self.name = "x"
来源：http://omz.aizwys.cn

PHP:  public string $name = "x";
来源：http://srx.zdqjudy.top

JS:   this.name = "x";
来源：http://rvs.cucudq.cn

TS:   name: string = "x";
来源：http://sws.vqdsnc.cn

Java: private String name;
来源：http://tzo.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqs.jinqigufen.top

Ruby: @name = "x"
来源：http://mkc.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://hbe.haohaochexian.top

[G04] 定义方法
来源：http://rgi.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://tpn.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ggo.52xcode.cn

JS:   greet() { return this.name; }
来源：http://dhk.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://uhn.xinyue.icu

Java: String greet() { return name; }
来源：http://xku.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://owb.wangshuangyany.cn

Ruby: def greet; @name; end
来源：http://hcg.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://fhq.uphjek.com

[G05] 继承
来源：http://hbx.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://dou.sysykeji.top

PHP:  class Admin extends User {}
来源：http://axv.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://buj.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://jmz.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://sov.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ptd.c1oappe.top

Ruby: class Admin < User; end
来源：http://glw.yanxiufei.cn

C#:   class Admin : User {}
来源：http://plw.0kj1m.cn

[G06] 重写方法
来源：http://gmi.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://hsi.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://esf.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://sow.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://ytw.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://tnt.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wmw.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://jjc.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://unm.wangshuangyany.cn

[G07] 调用父类方法
来源：http://vkh.sxryk.cn

Py:   super().greet()
来源：http://gyx.jiagoushi.top

PHP:  parent::greet();
来源：http://bev.xuanzx.com

JS:   super.greet();
来源：http://kqg.ydzc1.top

TS:   super.greet();
来源：http://bph.zhijiandao.cn

Java: super.greet();
来源：http://zfm.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://neg.fktsv.cn

Ruby: super
来源：http://pos.chenjidiqi.icu

C#:   base.Greet();
来源：http://xpp.hammf.cn

[G08] 静态方法与属性
来源：http://pfp.hysaishi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nwo.0kj1m.cn

PHP:  public static function f() {}
来源：http://tka.xingfuxueyuan.xyz

JS:   static f() {}
来源：http://quj.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://dqa.shanyushiyangtech.top

Java: static void f() {}
来源：http://fhf.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qbh.aibaodan.cn

Ruby: def self.f; end
来源：http://jqu.yanxiufei.cn

C#:   public static void F() {}
来源：http://dop.sxryk.cn

[G09] 接口 / 抽象类
来源：http://xyi.zhiwuduotai.top

Py:   from abc import ABC, abstractmethod
来源：http://pmw.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://lzp.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://tsg.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://hwa.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://ldt.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://lhv.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hjw.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://fbj.daria6918.cn

[G10] 访问控制
来源：http://hru.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://pwt.yj20258888.top

PHP:  public / protected / private
来源：http://rsf.gzhubu.top

JS:   #private 字段；其余公开
来源：http://gui.chenlongwang.top

TS:   public / protected / private
来源：http://bdt.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://ssp.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://clx.jqgfzy.top

Ruby: public / protected / private
来源：http://hsy.chenzaomai.com

C#:   public / protected / private / internal
来源：http://dlp.yj202588.top

[G11] getter / setter
来源：http://hgx.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://gph.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://she.yueranfly.top

JS:   get name() { return this._name; }
来源：http://mwe.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://hrx.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://udk.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yaj.epnwcf.com

Ruby: attr_accessor :name
来源：http://olf.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://qxc.fktsv.cn

[G12] 对象转字符串
来源：http://bwd.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://qdy.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://amp.pycfn.com

JS:   toString() { return this.name; }
来源：http://ibe.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://yyr.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://hdr.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vms.tian-w.cn

Ruby: def to_s; @name; end
来源：http://kio.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://zxx.ybcxt.top

[G13] 判断对象类型
来源：http://dpe.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://yde.shanyushiyangkeji.top

PHP:  $u instanceof User
来源：http://pxp.xinyue.icu

JS:   u instanceof User
来源：http://vyc.jinghuilouyu.cn

TS:   u instanceof User
来源：http://zwz.feifeiyinyue.top

Java: u instanceof User
来源：http://roj.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://pqf.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://imw.zdqjudy.top

C#:   u is User
来源：http://flm.redwolf501.top

[G14] 数据类 / record
来源：http://xlt.redwolf501.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lyg.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://hfh.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wke.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://ixi.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://ymm.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://cqf.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ptu.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://wej.guannengcc.top

[G15] 枚举
来源：http://vqk.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mbs.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://inh.zdqjudy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baf.aizwys.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hjn.xziqi.cn

Java: enum Color { RED, GREEN }
来源：http://jlh.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://guc.fzhhl.top

Ruby: Color = %i[red green].freeze
来源：http://lhr.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sto.cheryme.top

[G16] 对象转数组 / 字典
来源：http://dnf.shuidangran.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bxr.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://xnw.gotoacloud.top

JS:   Object.entries(obj)
来源：http://wtc.quarkkingdee.top

TS:   Object.entries(obj)
来源：http://dyf.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://okc.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://skk.sysykeji.top

Ruby: obj.instance_variables
来源：http://ulp.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://mhn.jlsjyb.cn

================================================================================
来源：http://bee.smart0.xyz

H. 异常与错误处理
来源：http://iim.jiagoushi.top

================================================================================
来源：http://smv.fengsongda.top

[H01] try / catch 基础
来源：http://ayt.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://byy.svipenyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jbw.zhengqikj.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ksw.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://isi.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://adk.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ybg.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zjc.ivvv.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ahh.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://xop.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qly.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hbb.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cie.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vte.fehbvm.com

Java: try { f(); } finally { cleanup(); }
来源：http://zcb.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uym.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://zdx.ehwqpu.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://hzl.jianghu66.top

[H03] 主动抛出异常
来源：http://kpu.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://dyd.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gfo.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://aex.birdmap.top

TS:   throw new Error("错误信息");
来源：http://ezz.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://qdl.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rhs.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mmg.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://whf.cucudq.cn

[H04] 自定义异常类型
来源：http://kah.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://nok.cheryme.top

PHP:  class MyError extends RuntimeException {}
来源：http://hsn.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://tau.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://jqv.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://odh.redwolf501.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mrt.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://hyh.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://jdq.jianghu66.top

[H05] 捕获特定类型
来源：http://oga.ybcxt.top

Py:   except ValueError as e:
来源：http://rju.hesvh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://its.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://jgq.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://obp.zhengqikj.top

Java: catch (IOException | SQLException e) {}
来源：http://xbf.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rkp.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://cus.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jhe.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://nyz.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://qjr.shzxlz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ind.zhongyouzk.top

JS:   obj?.a?.b;  d ?? default
来源：http://zll.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://iwc.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qpp.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://yqp.hnqzz.top

Ruby: d&.dig(:a, :b)
来源：http://xna.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://boo.xuetiantiany.cn

[H07] 断言
来源：http://atj.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://qth.shzxlz.cn

PHP:  assert($x > 0);
来源：http://jmm.yueranfly.top

JS:   console.assert(x > 0);
来源：http://jzi.birdmap.top

TS:   console.assert(x > 0);
来源：http://dck.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://hih.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aku.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://zxg.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://hut.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://nfi.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://fbi.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nbw.zhengqikj.top

JS:   e.message;  e.stack
来源：http://rai.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihm.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ynl.yuanzhike.top

Go:   err.Error()
来源：http://emb.fzhhl.top

Ruby: e.message;  e.backtrace
来源：http://gqb.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://ioi.shuidangran.top

[H09] 带错误码的异常
来源：http://koo.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vtq.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zgh.ydzc1.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://elh.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://emr.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ugv.yj20258.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tyq.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://ypp.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lcp.cheryme.top

[H10] 资源自动释放
来源：http://kxl.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dsk.smart0.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cur.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ehk.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xqi.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gdx.jiagoushi.top

Go:   defer f.Close()
来源：http://cly.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fzj.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zqr.xinyue.icu

================================================================================
来源：http://xsx.yongpay.top

I. 正则表达式
来源：http://nys.tianlin.xyz

================================================================================
来源：http://hng.yj20258.top

[I01] 判断是否匹配
来源：http://gna.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://svs.sufxvd.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bdo.sxryk.cn

JS:   /\d+/.test(s)
来源：http://pcw.zdqjudy.top

TS:   /\d+/.test(s)
来源：http://der.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bpk.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lwg.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://kho.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eys.vehdjk.com

[I02] 提取所有匹配
来源：http://vib.ywan-chungtsiang.top

Py:   re.findall(r"\d+", s)
来源：http://bib.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vkg.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tqa.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://ejw.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ghp.bjfxy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fdr.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://scj.yj20258888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bbh.pycfn.com

[I03] 提取捕获分组
来源：http://ryp.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eou.xylfe.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bmh.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bjs.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://svm.epnwcf.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cic.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://inr.sjlbkw.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xfd.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pij.jlsjyb.cn

[I04] 正则替换
来源：http://rhb.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sjv.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nny.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fnj.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://ljl.andypj.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://pci.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://upl.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mnd.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fjn.dashuyun.cn

[I05] 按正则拆分
来源：http://qai.9152youxi.cn


<!-- 参考信息 -->