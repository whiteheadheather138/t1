代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://grf.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kjv.ctjpmb.com

[F11] 复制与移动文件
来源：http://izz.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fpa.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rnn.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iiz.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hyy.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ina.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uul.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lhk.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mqf.cheryme.top

[F12] CSV 读写
来源：http://iww.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://htf.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ucw.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://muu.fktsv.cn

TS:   // 同上
来源：http://ybl.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://suz.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ins.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mgz.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hew.gogol.net.cn

================================================================================
来源：http://cdu.zdqjudy.top

G. 面向对象
来源：http://nqo.316326.xyz

================================================================================
来源：http://xyd.meibo888.top

[G01] 定义类
来源：http://lvq.snrcjt.cn

Py:   class User: pass
来源：http://ikm.zycfv.cn

PHP:  class User {}
来源：http://ddr.ydzc1.top

JS:   class User {}
来源：http://nuf.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://exv.yj20258.top

Java: class User {}
来源：http://spn.yj20258888.top

Go:   type User struct { Name string }
来源：http://aoe.haohaochexian.top

Ruby: class User; end
来源：http://xpd.mhx1999.top

C#:   class User {}
来源：http://scs.zhongyouzk.top

[G02] 构造函数
来源：http://urk.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://tsy.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://gwg.yj202588.top

JS:   constructor(name) { this.name = name; }
来源：http://tjk.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://lzt.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://sdw.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vvs.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://cqc.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://lht.hnqzz.top

[G03] 实例属性
来源：http://qll.hammf.cn

Py:   self.name = "x"
来源：http://slm.c1oappe.top

PHP:  public string $name = "x";
来源：http://uag.feifeiyinyue.top

JS:   this.name = "x";
来源：http://cwu.0kj1m.cn

TS:   name: string = "x";
来源：http://yty.zhixingplan.top

Java: private String name;
来源：http://pmb.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tgv.nanxuanxn.top

Ruby: @name = "x"
来源：http://mqs.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://jqd.cucudq.cn

[G04] 定义方法
来源：http://brv.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://xdv.cashguo.top

PHP:  public function greet(): string { return $this->name; }
来源：http://orc.tarul.cn

JS:   greet() { return this.name; }
来源：http://dbq.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://dyi.yfazqb.com

Java: String greet() { return name; }
来源：http://tmt.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aoa.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://udq.c1oappe.top

C#:   public string Greet() => Name;
来源：http://mfr.ivvv.top

[G05] 继承
来源：http://kbf.nanxinkj.top

Py:   class Admin(User): pass
来源：http://wug.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://fsb.jianghu66.top

JS:   class Admin extends User {}
来源：http://vsm.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://vcd.pycfn.com

Java: class Admin extends User {}
来源：http://bbp.nanxinkj.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sdq.smart0.xyz

Ruby: class Admin < User; end
来源：http://zrj.quarkkingdee.top

C#:   class Admin : User {}
来源：http://use.fehbvm.com

[G06] 重写方法
来源：http://aof.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://pza.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://dky.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://yyu.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://eht.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://uut.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ppc.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://grr.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://hzn.zhixingplan.top

[G07] 调用父类方法
来源：http://jba.jqgufenzy.top

Py:   super().greet()
来源：http://vdi.sweek.top

PHP:  parent::greet();
来源：http://was.chenlongwang.top

JS:   super.greet();
来源：http://ujz.ydjk.org.cn

TS:   super.greet();
来源：http://lxj.hfpthk.cn

Java: super.greet();
来源：http://vou.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://twv.shuidangran.top

Ruby: super
来源：http://zqq.sxryk.cn

C#:   base.Greet();
来源：http://llz.epnwcf.com

[G08] 静态方法与属性
来源：http://oyc.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xri.yj202588.top

PHP:  public static function f() {}
来源：http://bke.shanyushiyangtech.top

JS:   static f() {}
来源：http://yqi.9152youxi.cn

TS:   static f(): void {}
来源：http://cdn.pycfn.com

Java: static void f() {}
来源：http://kxg.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://clc.fktsv.cn

Ruby: def self.f; end
来源：http://dmu.mhx1999.top

C#:   public static void F() {}
来源：http://dyn.fzhhl.top

[G09] 接口 / 抽象类
来源：http://hcb.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://tet.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sen.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vnh.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://xpm.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://sgb.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://aie.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xlh.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://fya.hnxiangtu.top

[G10] 访问控制
来源：http://mov.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://lqa.fengsongda.top

PHP:  public / protected / private
来源：http://tuo.epnwcf.com

JS:   #private 字段；其余公开
来源：http://njy.jqgufenzy.top

TS:   public / protected / private
来源：http://fbo.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://uua.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zig.ppjwa.cn

Ruby: public / protected / private
来源：http://tnp.dianchejie.cn

C#:   public / protected / private / internal
来源：http://vpz.xinyue.icu

[G11] getter / setter
来源：http://sdn.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://rwx.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ukg.hcnkem.com

JS:   get name() { return this._name; }
来源：http://vob.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://dwz.0kj1m.cn

Java: public String getName() { return name; }
来源：http://jbu.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://xab.daxiang520.top

Ruby: attr_accessor :name
来源：http://wnq.fktsv.cn

C#:   public string Name { get; set; }
来源：http://cbc.gzhubu.top

[G12] 对象转字符串
来源：http://iui.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://pgm.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://phs.zycfv.cn

JS:   toString() { return this.name; }
来源：http://buo.yuanzhike.top

TS:   toString(): string { return this.name; }
来源：http://mqn.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://yce.cqqwz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://usf.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://qwy.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://pdv.sufxvd.cn

[G13] 判断对象类型
来源：http://udq.yj20258.top

Py:   isinstance(u, User)
来源：http://mob.yonumen.top

PHP:  $u instanceof User
来源：http://nmg.yj20258888.top

JS:   u instanceof User
来源：http://inz.snrcjt.cn

TS:   u instanceof User
来源：http://yvn.fanxiaobao.xyz

Java: u instanceof User
来源：http://ypo.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ees.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://kji.fehbvm.com

C#:   u is User
来源：http://bwp.jlsjyb.cn

[G14] 数据类 / record
来源：http://dcx.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wpu.xuanzx.com

PHP:  // 用 readonly 属性模拟
来源：http://epr.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sbx.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://gdn.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://yjg.yonumen.top

Go:   type User struct { Name string; Age int }
来源：http://uor.xziqi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kim.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://nva.shangyingyoupin.top

[G15] 枚举
来源：http://taq.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://btc.zhixingplan.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bgz.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aau.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uzq.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://cfj.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bwy.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://aiy.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xop.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://gou.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://our.ivvv.top

PHP:  get_object_vars($obj);
来源：http://iyb.ybcxt.top

JS:   Object.entries(obj)
来源：http://vth.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://mbq.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://czc.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rur.havefunace.top

Ruby: obj.instance_variables
来源：http://quq.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://bix.hywenlv.cn

================================================================================
来源：http://nmd.jiagoushi.top

H. 异常与错误处理
来源：http://xhu.fzhhl.top

================================================================================
来源：http://gzn.52xcode.cn

[H01] try / catch 基础
来源：http://reo.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://say.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ebj.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://skf.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tfz.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://scw.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pbb.fanxiaobao.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gia.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jds.ivvv.top

[H02] finally / ensure 收尾
来源：http://wus.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://urz.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dip.zdqjudy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gih.birdmap.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nys.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://okj.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://ihz.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://plt.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kqm.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://xcc.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://yvg.birdmap.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tsi.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://csn.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://rmm.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://cxo.redwolf501.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pkn.shuidangran.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jzn.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ozi.vqdsnc.cn

[H04] 自定义异常类型
来源：http://cku.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://xzs.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bkp.iojbl.cn

JS:   class MyError extends Error {}
来源：http://wpk.daria6918.cn

TS:   class MyError extends Error {}
来源：http://xlo.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://fek.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ylf.bbcook.cn

Ruby: class MyError < StandardError; end
来源：http://pcd.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://rbs.zhixingplan.top

[H05] 捕获特定类型
来源：http://zca.daxiang520.top

Py:   except ValueError as e:
来源：http://kxf.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ubf.gogol.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://fqv.vqdsnc.cn

TS:   if (e instanceof TypeError) {}
来源：http://cyy.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://lmt.andypj.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pbr.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://pqw.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zxt.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://uza.ybcxt.top

Py:   value = d.get("k") or default
来源：http://gdz.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ohn.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vut.daxiang520.top

TS:   obj?.a?.b;  d ?? default
来源：http://xpa.sysykeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xyb.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tcb.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://bmz.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://kry.sysykeji.top

[H07] 断言
来源：http://brl.fzhhl.top

Py:   assert x > 0, "必须为正"
来源：http://wdt.xinyue.icu

PHP:  assert($x > 0);
来源：http://poc.bjfxy.top

JS:   console.assert(x > 0);
来源：http://hjl.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://hwz.andypj.xyz

Java: assert x > 0 : "必须为正";
来源：http://tjy.meibo888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fhj.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nfk.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://rnm.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://vgk.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://ido.cucudq.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nft.shuidangran.top

JS:   e.message;  e.stack
来源：http://kjk.kuanghao11.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xou.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ebr.guannengcc.top

Go:   err.Error()
来源：http://vgw.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://uez.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://eeo.vqdsnc.cn

[H09] 带错误码的异常
来源：http://run.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rjj.gzhubu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://pck.hnqzz.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bnq.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fwu.redwolf501.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eaj.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://exc.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bfn.jiagoushi.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zln.jyoumei.cn

[H10] 资源自动释放
来源：http://mir.hongshengwenyu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oyy.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pkc.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bdx.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gpp.ppjwa.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://red.hesvh.cn

Go:   defer f.Close()
来源：http://llc.guannengcc.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zbx.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ywy.sxryk.cn

================================================================================
来源：http://gko.yvedp.cn

I. 正则表达式
来源：http://ngz.zycfv.cn

================================================================================
来源：http://bbg.gaohongyu789.top

[I01] 判断是否匹配
来源：http://xmx.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ccy.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://vyl.gogol.net.cn

JS:   /\d+/.test(s)
来源：http://nku.shzxlz.cn

TS:   /\d+/.test(s)
来源：http://lcc.yongpay.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jcf.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://spn.316326.xyz

Ruby: s.match?(/\d+/)
来源：http://hsn.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wco.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://mfc.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://lzd.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tvp.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dyk.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://xtn.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uxv.fktsv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hcj.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://ths.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hjk.jinqigufen.top

[I03] 提取捕获分组
来源：http://qls.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://prx.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tai.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qdm.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qrb.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pxj.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dvo.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jgp.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zmk.fanxiaobao.xyz

[I04] 正则替换
来源：http://cuy.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aww.chenzaomai.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pba.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hob.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://jah.aizwys.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fxa.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qgz.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qeo.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tqi.haohaochexian.top

[I05] 按正则拆分
来源：http://xen.gogol.net.cn


<!-- 参考信息 -->