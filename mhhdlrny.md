代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lct.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://saw.jqgfzy.top

[F11] 复制与移动文件
来源：http://qpd.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ytr.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hjk.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xpl.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kgt.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://spj.bjfxy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://avp.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vfs.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vso.dashuyun.cn

[F12] CSV 读写
来源：http://gqv.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wwt.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kcs.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pqo.aizwys.cn

TS:   // 同上
来源：http://fzg.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uea.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aqq.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nhw.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vzu.shanyushiyangkeji.top

================================================================================
来源：http://wqu.shzxlz.cn

G. 面向对象
来源：http://gjs.zdbjq.cn

================================================================================
来源：http://btr.zhijiandao.cn

[G01] 定义类
来源：http://ncj.fehbvm.com

Py:   class User: pass
来源：http://goz.nwbrower.top

PHP:  class User {}
来源：http://qea.yj202588.top

JS:   class User {}
来源：http://otv.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://ydx.xuetiantiany.cn

Java: class User {}
来源：http://rpd.yangfankeji.com

Go:   type User struct { Name string }
来源：http://eng.dashuyun.cn

Ruby: class User; end
来源：http://rrk.gzhubu.top

C#:   class User {}
来源：http://xys.jiagoushi.top

[G02] 构造函数
来源：http://ixg.gogol.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://wbj.zhixingplan.top

PHP:  public function __construct(public string $name) {}
来源：http://gpu.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://cpv.yongpay.top

TS:   constructor(public name: string) {}
来源：http://zdy.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://zld.fktsv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljo.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://btz.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://dhc.iojbl.cn

[G03] 实例属性
来源：http://ozo.iojbl.cn

Py:   self.name = "x"
来源：http://tlu.jianghu66.top

PHP:  public string $name = "x";
来源：http://hsc.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://wak.316326.xyz

TS:   name: string = "x";
来源：http://bkv.yj202588.top

Java: private String name;
来源：http://jxa.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lxo.316326.xyz

Ruby: @name = "x"
来源：http://lcp.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://epq.chenlongwang.top

[G04] 定义方法
来源：http://dds.tanke756.top

Py:   def greet(self): return self.name
来源：http://cbo.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://iug.mhx1999.top

JS:   greet() { return this.name; }
来源：http://kse.c1oappe.top

TS:   greet(): string { return this.name; }
来源：http://bzr.yuanzhike.top

Java: String greet() { return name; }
来源：http://njp.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://njs.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://fcs.tarul.cn

C#:   public string Greet() => Name;
来源：http://isg.haohaochexian.top

[G05] 继承
来源：http://qxj.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://cxh.cheryme.top

PHP:  class Admin extends User {}
来源：http://uen.zycfv.cn

JS:   class Admin extends User {}
来源：http://hci.fktsv.cn

TS:   class Admin extends User {}
来源：http://jpf.sysykeji.top

Java: class Admin extends User {}
来源：http://cim.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://stv.birdmap.top

Ruby: class Admin < User; end
来源：http://wpq.daxiang520.top

C#:   class Admin : User {}
来源：http://ndo.9152youxi.cn

[G06] 重写方法
来源：http://zcd.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://rrv.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://bqx.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://hnl.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://wql.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://lep.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ykf.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://jtp.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://kfx.fengsongda.top

[G07] 调用父类方法
来源：http://gix.pycfn.com

Py:   super().greet()
来源：http://rxq.yfazqb.com

PHP:  parent::greet();
来源：http://rfg.zhixingplan.top

JS:   super.greet();
来源：http://gbg.birdmap.top

TS:   super.greet();
来源：http://ohr.tian-w.cn

Java: super.greet();
来源：http://mhj.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezd.jqgfzy.top

Ruby: super
来源：http://ccb.ydjk.org.cn

C#:   base.Greet();
来源：http://qzn.zhengqikj.top

[G08] 静态方法与属性
来源：http://gff.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iat.iojbl.cn

PHP:  public static function f() {}
来源：http://iwk.yongpay.top

JS:   static f() {}
来源：http://dmv.zdbjq.cn

TS:   static f(): void {}
来源：http://kpu.vehdjk.com

Java: static void f() {}
来源：http://sls.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ngd.316326.xyz

Ruby: def self.f; end
来源：http://wzh.wangdashe.top

C#:   public static void F() {}
来源：http://oqz.fktsv.cn

[G09] 接口 / 抽象类
来源：http://vpj.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://kwe.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://djc.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pgr.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://pnd.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://pdu.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://xvp.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mth.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://awt.sufxvd.cn

[G10] 访问控制
来源：http://oul.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://kls.nanxinkj.top

PHP:  public / protected / private
来源：http://msa.zycfv.cn

JS:   #private 字段；其余公开
来源：http://zha.zdbjq.cn

TS:   public / protected / private
来源：http://gdd.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://iib.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dwf.tianlin.xyz

Ruby: public / protected / private
来源：http://khu.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://rhp.gzhubu.top

[G11] getter / setter
来源：http://vba.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://cpx.xuetiantiany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ral.xziqi.cn

JS:   get name() { return this._name; }
来源：http://faa.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://ywo.chenzaomai.com

Java: public String getName() { return name; }
来源：http://yrf.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://ezc.tanke756.top

Ruby: attr_accessor :name
来源：http://njg.redwolf501.top

C#:   public string Name { get; set; }
来源：http://txc.sxryk.cn

[G12] 对象转字符串
来源：http://mqh.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://ubq.zhongyouzk.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://skg.yvedp.cn

JS:   toString() { return this.name; }
来源：http://ldc.shzxlz.cn

TS:   toString(): string { return this.name; }
来源：http://mgs.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://goj.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nfy.redwolf501.top

Ruby: def to_s; @name; end
来源：http://lvh.feifeiyinyue.top

C#:   public override string ToString() => Name;
来源：http://btz.hammf.cn

[G13] 判断对象类型
来源：http://bvv.jianghu66.top

Py:   isinstance(u, User)
来源：http://qci.sweek.top

PHP:  $u instanceof User
来源：http://oae.316326.xyz

JS:   u instanceof User
来源：http://ycs.sxryk.cn

TS:   u instanceof User
来源：http://bnz.guowangkeji.top

Java: u instanceof User
来源：http://hdv.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xmt.xuanzx.com

Ruby: u.is_a?(User)
来源：http://tpk.sjlbkw.cn

C#:   u is User
来源：http://qgb.yj202588.top

[G14] 数据类 / record
来源：http://djq.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://haf.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://nqm.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://fgb.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://frz.9152youxi.cn

Java: record User(String name, int age) {}
来源：http://vgn.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://ifk.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wqm.meibo888.top

C#:   record User(string Name, int Age);
来源：http://ztc.sufxvd.cn

[G15] 枚举
来源：http://bxq.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yze.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xyn.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xqn.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sig.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://vef.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://akn.svipenyu.cn

Ruby: Color = %i[red green].freeze
来源：http://lhu.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://spf.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://mlk.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rjr.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://rkh.sufxvd.cn

JS:   Object.entries(obj)
来源：http://jzp.fzhhl.top

TS:   Object.entries(obj)
来源：http://yvs.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jms.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zfa.xylfe.cn

Ruby: obj.instance_variables
来源：http://krt.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://xxu.jinyuanbaomall.cn

================================================================================
来源：http://zht.vqdsnc.cn

H. 异常与错误处理
来源：http://ulg.gotoacloud.top

================================================================================
来源：http://lyz.tian-w.cn

[H01] try / catch 基础
来源：http://qii.hammf.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jlo.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bie.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jrb.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kmx.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wca.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qeq.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lpb.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hni.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://vgy.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://swg.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kgd.gotoacloud.top

JS:   try { f(); } finally { cleanup(); }
来源：http://acn.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cwj.yfazqb.com

Java: try { f(); } finally { cleanup(); }
来源：http://wuu.hywenlv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hkq.kuanghao11.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sqh.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wgs.fehbvm.com

[H03] 主动抛出异常
来源：http://zna.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://qbb.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ihm.tarul.cn

JS:   throw new Error("错误信息");
来源：http://qsh.iojbl.cn

TS:   throw new Error("错误信息");
来源：http://agt.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://svr.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oio.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://adc.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://lhi.daria6918.cn

[H04] 自定义异常类型
来源：http://hmn.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://eez.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://tdj.andypj.xyz

JS:   class MyError extends Error {}
来源：http://jun.hesvh.cn

TS:   class MyError extends Error {}
来源：http://nkm.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://llf.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dmr.jqgfzy.top

Ruby: class MyError < StandardError; end
来源：http://div.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://ozx.jinqigfzy.top

[H05] 捕获特定类型
来源：http://kni.xylfe.cn

Py:   except ValueError as e:
来源：http://tsl.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cgo.aibaodan.cn

JS:   if (e instanceof TypeError) {}
来源：http://lbm.guowangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://flx.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://orl.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sbr.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://zck.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uql.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://bxh.zhengqikj.top

Py:   value = d.get("k") or default
来源：http://wgo.redwolf501.top

PHP:  $v = $d["k"] ?? null;
来源：http://aqu.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fmb.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://qwx.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kfn.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tln.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://fle.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://fbt.uphjek.com

[H07] 断言
来源：http://mbf.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://neg.cashguo.top

PHP:  assert($x > 0);
来源：http://lfa.sysykeji.top

JS:   console.assert(x > 0);
来源：http://ppz.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://mcd.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://oza.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yhk.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://xmd.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://rsk.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://twq.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://kcj.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hht.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://qmf.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://kgv.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://taq.zhengqikj.top

Go:   err.Error()
来源：http://azt.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://qqd.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://hkz.yj20258888.top

[H09] 带错误码的异常
来源：http://skh.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zvf.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://lst.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xgb.epnwcf.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qym.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lho.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://evh.quarkkingdee.top

Ruby: raise MyError.new("fail", 500)
来源：http://wpg.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kwu.aizwys.cn

[H10] 资源自动释放
来源：http://sio.cdnleiting.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fmu.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nbb.jinghuilouyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jps.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qur.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://plr.uphjek.com

Go:   defer f.Close()
来源：http://ypu.yfazqb.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jee.hfpthk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://piw.xingfuxueyuan.xyz

================================================================================
来源：http://rpy.hnxiangtu.top

I. 正则表达式
来源：http://laq.mhx1999.top

================================================================================
来源：http://jar.hywenlv.cn

[I01] 判断是否匹配
来源：http://lao.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwp.sjlbkw.cn

PHP:  preg_match('/\d+/', $s);
来源：http://woc.wangdashe.top

JS:   /\d+/.test(s)
来源：http://rai.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://sqx.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://osg.yueranfly.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fff.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://omg.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cbv.ivvv.top

[I02] 提取所有匹配
来源：http://buw.sxryk.cn

Py:   re.findall(r"\d+", s)
来源：http://tuw.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mdc.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://csj.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://iio.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fak.shuidangran.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xtc.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://iij.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vjf.yueranfly.top

[I03] 提取捕获分组
来源：http://ofc.sjlbkw.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bdr.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jag.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nkc.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dxf.snrcjt.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kjs.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jpf.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aen.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yui.hcnkem.com

[I04] 正则替换
来源：http://nnm.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jww.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jrr.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://cog.hesvh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dde.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://slo.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gdr.iojbl.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://akw.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eur.yueranfly.top

[I05] 按正则拆分
来源：http://luy.jiagoushi.top


<!-- 参考信息 -->