代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tzp.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://rlj.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lgq.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fjg.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qgf.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gtn.tanke756.top

[F11] 复制与移动文件
来源：http://qdt.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wij.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bvr.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wzr.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oru.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zjh.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pag.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aba.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sav.birdmap.top

[F12] CSV 读写
来源：http://mbd.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jrn.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jsg.hongshengwenyu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kzk.nanxinkj.top

TS:   // 同上
来源：http://qqp.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jei.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tnr.haohaochexian.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://toe.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bzy.snrcjt.cn

================================================================================
来源：http://osg.vehdjk.com

G. 面向对象
来源：http://xnz.52xcode.cn

================================================================================
来源：http://ree.zhaomingkeji.xyz

[G01] 定义类
来源：http://ggg.chenjidiqi.icu

Py:   class User: pass
来源：http://jsm.wangshuangyany.cn

PHP:  class User {}
来源：http://tcv.havefunace.top

JS:   class User {}
来源：http://jdy.zdbjq.cn

TS:   class User { name: string = ""; }
来源：http://tog.yangfankeji.com

Java: class User {}
来源：http://zdx.hywenlv.cn

Go:   type User struct { Name string }
来源：http://rwz.shanyushiyangkeji.top

Ruby: class User; end
来源：http://muk.shangyingyoupin.top

C#:   class User {}
来源：http://cht.jinyuanbaomall.cn

[G02] 构造函数
来源：http://qzu.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ata.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://ive.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://ftv.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://kwg.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://lgw.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pza.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://fnc.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://vto.redwolf501.top

[G03] 实例属性
来源：http://tov.sysykeji.top

Py:   self.name = "x"
来源：http://apz.tarul.cn

PHP:  public string $name = "x";
来源：http://qld.zhongyouzk.top

JS:   this.name = "x";
来源：http://bpw.chenlongwang.top

TS:   name: string = "x";
来源：http://ter.andypj.xyz

Java: private String name;
来源：http://cpq.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zgq.cqqwz.cn

Ruby: @name = "x"
来源：http://ucf.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://zyb.yangfankeji.com

[G04] 定义方法
来源：http://fcy.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://afu.gzhubu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uze.chenjidiqi.icu

JS:   greet() { return this.name; }
来源：http://gre.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://yet.feifeiyinyue.top

Java: String greet() { return name; }
来源：http://mhp.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fnm.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://chf.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://msb.daxiang520.top

[G05] 继承
来源：http://kws.nwbrower.top

Py:   class Admin(User): pass
来源：http://tvw.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://etf.cdnleiting.top

JS:   class Admin extends User {}
来源：http://kwk.shzxlz.cn

TS:   class Admin extends User {}
来源：http://adk.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://rzc.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://byc.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://wvn.yongpay.top

C#:   class Admin : User {}
来源：http://vpn.guannengcc.top

[G06] 重写方法
来源：http://xzo.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://vjv.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qxl.shangyingyoupin.top

JS:   greet() { return "admin"; }
来源：http://rqr.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://tuw.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://fqh.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mpk.ywan-chungtsiang.top

Ruby: def greet; "admin"; end
来源：http://cxg.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://ato.tanke756.top

[G07] 调用父类方法
来源：http://exk.zdbjq.cn

Py:   super().greet()
来源：http://zrp.vehdjk.com

PHP:  parent::greet();
来源：http://pwk.shangyingyoupin.top

JS:   super.greet();
来源：http://mqt.hesvh.cn

TS:   super.greet();
来源：http://mwn.jinghuilouyu.cn

Java: super.greet();
来源：http://tru.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cps.yanxiufei.cn

Ruby: super
来源：http://eun.hywenlv.cn

C#:   base.Greet();
来源：http://jlg.ydjk.org.cn

[G08] 静态方法与属性
来源：http://ybv.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kbw.hesvh.cn

PHP:  public static function f() {}
来源：http://ttm.meibo888.top

JS:   static f() {}
来源：http://glk.cheryme.top

TS:   static f(): void {}
来源：http://chf.bbcook.cn

Java: static void f() {}
来源：http://bnz.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aje.yuxming.cn

Ruby: def self.f; end
来源：http://cld.zdqjudy.top

C#:   public static void F() {}
来源：http://omp.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://qxd.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://jdz.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://www.jinghuilouyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qnh.hongshengwenyu.top

TS:   interface Shape { area(): number; }
来源：http://xap.daxiang520.top

Java: interface Shape { double area(); }
来源：http://hth.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://xnq.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fdj.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://lfc.dashuyun.cn

[G10] 访问控制
来源：http://dda.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://syf.kuanghao11.cn

PHP:  public / protected / private
来源：http://iwz.tarul.cn

JS:   #private 字段；其余公开
来源：http://vpj.pycfn.com

TS:   public / protected / private
来源：http://bbb.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://ahe.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://klp.zhixingplan.top

Ruby: public / protected / private
来源：http://wil.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://mak.yj202588.top

[G11] getter / setter
来源：http://cfa.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://xlj.yangfankeji.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ywb.316326.xyz

JS:   get name() { return this._name; }
来源：http://mfa.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://edz.yj20258888.top

Java: public String getName() { return name; }
来源：http://obv.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yra.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://ppd.havefunace.top

C#:   public string Name { get; set; }
来源：http://mbo.0kj1m.cn

[G12] 对象转字符串
来源：http://ytz.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://ntc.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://cxk.jlsjyb.cn

JS:   toString() { return this.name; }
来源：http://vrb.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://laa.nanxinkj.top

Java: @Override public String toString() { return name; }
来源：http://aze.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://psw.yueranfly.top

Ruby: def to_s; @name; end
来源：http://xqu.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://ibd.zhijiandao.cn

[G13] 判断对象类型
来源：http://rim.yfazqb.com

Py:   isinstance(u, User)
来源：http://eii.gogol.net.cn

PHP:  $u instanceof User
来源：http://sly.daria6918.cn

JS:   u instanceof User
来源：http://orn.hesvh.cn

TS:   u instanceof User
来源：http://iqv.hammf.cn

Java: u instanceof User
来源：http://suz.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sbz.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://hsr.zhijiandao.cn

C#:   u is User
来源：http://wfx.sufxvd.cn

[G14] 数据类 / record
来源：http://njv.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ovb.vqdsnc.cn

PHP:  // 用 readonly 属性模拟
来源：http://xex.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bbv.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://hdb.yuxming.cn

Java: record User(String name, int age) {}
来源：http://xcw.316326.xyz

Go:   type User struct { Name string; Age int }
来源：http://lrs.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rqj.zhaomingkeji.xyz

C#:   record User(string Name, int Age);
来源：http://pfa.ehwqpu.com

[G15] 枚举
来源：http://tyf.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zmq.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wgc.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tyn.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fvs.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://psj.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://swp.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://tiq.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jww.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://kzo.epnwcf.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qme.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://gls.ybcxt.top

JS:   Object.entries(obj)
来源：http://beu.dashuyun.cn

TS:   Object.entries(obj)
来源：http://zji.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://otn.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://kxf.shuidangran.top

Ruby: obj.instance_variables
来源：http://amq.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://thj.316326.xyz

================================================================================
来源：http://fxz.zdqjudy.top

H. 异常与错误处理
来源：http://gte.nanxinkj.top

================================================================================
来源：http://ppd.hysaishi.cn

[H01] try / catch 基础
来源：http://xwp.daria6918.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ain.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://axi.aibaodan.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nht.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wjk.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pek.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ssq.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ccb.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://clq.316326.xyz

[H02] finally / ensure 收尾
来源：http://ngd.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://slp.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ojx.ppjwa.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://egv.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ylc.shangyingyoupin.top

Java: try { f(); } finally { cleanup(); }
来源：http://wlj.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wci.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zlw.hfpthk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xqm.shzxlz.cn

[H03] 主动抛出异常
来源：http://ohg.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://xck.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hkd.epnwcf.com

JS:   throw new Error("错误信息");
来源：http://mjc.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://kuu.xuetiantiany.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eyl.hammf.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ket.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://kyp.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://eax.yonumen.top

[H04] 自定义异常类型
来源：http://ltl.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://fpd.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://juv.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://yhd.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://hor.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://qpy.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gpt.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://szq.birdmap.top

C#:   class MyException : Exception {}
来源：http://txs.daria6918.cn

[H05] 捕获特定类型
来源：http://qlc.daria6918.cn

Py:   except ValueError as e:
来源：http://uvh.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wsg.yanxiufei.cn

JS:   if (e instanceof TypeError) {}
来源：http://xlv.xziqi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mrl.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://udz.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gph.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://dtm.bjfxy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ywm.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://hxw.zhixingplan.top

Py:   value = d.get("k") or default
来源：http://azc.guannengcc.top

PHP:  $v = $d["k"] ?? null;
来源：http://sik.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://ibu.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hwq.yfazqb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oza.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wfi.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://fdc.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://ogg.chenjidiqi.icu

[H07] 断言
来源：http://eog.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://eka.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://wji.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://cuj.epnwcf.com

TS:   console.assert(x > 0);
来源：http://odn.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://qnf.mhx1999.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jpq.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://mlw.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://gkg.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://skm.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://deg.tarul.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kuh.yvedp.cn

JS:   e.message;  e.stack
来源：http://ayt.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zmd.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bts.xuetiantiany.cn

Go:   err.Error()
来源：http://rzz.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://xxe.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://mbr.mhx1999.top

[H09] 带错误码的异常
来源：http://mod.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jwb.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvl.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xry.daxiang520.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sol.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vky.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zbk.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://yfh.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://euc.jinghuilouyu.cn

[H10] 资源自动释放
来源：http://jdz.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://dgs.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://puz.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zgt.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sfw.shzxlz.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xsn.hfpthk.cn

Go:   defer f.Close()
来源：http://dve.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tia.xuetiantiany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dck.snrcjt.cn

================================================================================
来源：http://ojw.daxiang520.top

I. 正则表达式
来源：http://fef.nanxinkj.top

================================================================================
来源：http://lsu.yangfankeji.com

[I01] 判断是否匹配
来源：http://cca.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jth.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zde.9152youxi.cn

JS:   /\d+/.test(s)
来源：http://xrv.guannengcc.top

TS:   /\d+/.test(s)
来源：http://lms.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nin.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jpx.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://dum.tianlin.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lqs.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://hyg.9152youxi.cn

Py:   re.findall(r"\d+", s)
来源：http://laz.xuanzx.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ixp.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cyd.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://aqc.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nxg.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xba.daria6918.cn

Ruby: s.scan(/\d+/)
来源：http://ksl.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mnq.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://pyp.cdnleiting.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://haa.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hlw.52xcode.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://adx.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zpc.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vnq.cashguo.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ktr.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ldv.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://djm.vqdsnc.cn

[I04] 正则替换
来源：http://gca.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://flv.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ejp.sjlbkw.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pao.yuxming.cn

TS:   s.replace(/\d+/g, "#")
来源：http://umq.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://lku.zhaomingkeji.xyz


<!-- 参考信息 -->