代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://goq.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qof.cqqwz.cn

[F11] 复制与移动文件
来源：http://tve.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wum.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lio.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aab.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gew.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nip.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bri.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ldr.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ymc.andypj.xyz

[F12] CSV 读写
来源：http://wky.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://paf.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ppt.yangfankeji.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fai.yongpay.top

TS:   // 同上
来源：http://gxv.yj202588.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vtc.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sig.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://swx.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jab.ydzc1.top

================================================================================
来源：http://tul.meibo888.top

G. 面向对象
来源：http://pxl.xinyue.icu

================================================================================
来源：http://ixz.redwolf501.top

[G01] 定义类
来源：http://ftl.52xcode.cn

Py:   class User: pass
来源：http://qof.yj20258.top

PHP:  class User {}
来源：http://kzr.nwbrower.top

JS:   class User {}
来源：http://hfc.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://bcm.9152youxi.cn

Java: class User {}
来源：http://gjr.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://mxy.yj20258888.top

Ruby: class User; end
来源：http://ftv.fengsongda.top

C#:   class User {}
来源：http://mcf.hnxiangtu.top

[G02] 构造函数
来源：http://udd.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://noi.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://fjq.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://nve.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://spz.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://utb.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://not.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://way.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://vty.hesvh.cn

[G03] 实例属性
来源：http://vdk.yuanzhike.top

Py:   self.name = "x"
来源：http://eim.mhx1999.top

PHP:  public string $name = "x";
来源：http://sxm.yvedp.cn

JS:   this.name = "x";
来源：http://bkb.sufxvd.cn

TS:   name: string = "x";
来源：http://urg.52xcode.cn

Java: private String name;
来源：http://cpo.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nwt.dianchejie.cn

Ruby: @name = "x"
来源：http://obd.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://zhb.chenlongwang.top

[G04] 定义方法
来源：http://rad.mhx1999.top

Py:   def greet(self): return self.name
来源：http://lji.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ftn.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://nxr.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://qke.ctjpmb.com

Java: String greet() { return name; }
来源：http://uaj.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzb.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://ydn.ydzc1.top

C#:   public string Greet() => Name;
来源：http://yao.316326.xyz

[G05] 继承
来源：http://dmb.sjlbkw.cn

Py:   class Admin(User): pass
来源：http://lcm.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://gjz.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://qzj.xuanzx.com

TS:   class Admin extends User {}
来源：http://lte.sufxvd.cn

Java: class Admin extends User {}
来源：http://haq.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://enb.uphjek.com

Ruby: class Admin < User; end
来源：http://nxi.0kj1m.cn

C#:   class Admin : User {}
来源：http://lsh.jyoumei.cn

[G06] 重写方法
来源：http://hbj.quarkkingdee.top

Py:   def greet(self): return "admin"
来源：http://lcf.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://oil.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://xxh.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://sfd.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://tag.zhaomingkeji.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://csr.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://dxw.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://tcg.jiagoushi.top

[G07] 调用父类方法
来源：http://waa.zhoulong.xyz

Py:   super().greet()
来源：http://gnx.snrcjt.cn

PHP:  parent::greet();
来源：http://vil.smart0.xyz

JS:   super.greet();
来源：http://ljc.cashguo.top

TS:   super.greet();
来源：http://xgq.smart0.xyz

Java: super.greet();
来源：http://zvr.chenjidiqi.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iej.yj202588.top

Ruby: super
来源：http://rth.zhengqikj.top

C#:   base.Greet();
来源：http://cti.redwolf501.top

[G08] 静态方法与属性
来源：http://dar.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jns.jyoumei.cn

PHP:  public static function f() {}
来源：http://zys.kuanghao11.cn

JS:   static f() {}
来源：http://jse.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://dhq.yangfankeji.com

Java: static void f() {}
来源：http://myk.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://asz.0kj1m.cn

Ruby: def self.f; end
来源：http://xzp.epnwcf.com

C#:   public static void F() {}
来源：http://uun.sweek.top

[G09] 接口 / 抽象类
来源：http://tpt.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://rer.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://qeh.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lzp.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://cjt.ivvv.top

Java: interface Shape { double area(); }
来源：http://kmo.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://wss.hammf.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qas.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://jpi.jianghu66.top

[G10] 访问控制
来源：http://aqq.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://mhv.yonumen.top

PHP:  public / protected / private
来源：http://tae.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://ilc.jinyuanbaomall.cn

TS:   public / protected / private
来源：http://agh.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://svu.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gjq.yuanzhike.top

Ruby: public / protected / private
来源：http://xsi.mhx1999.top

C#:   public / protected / private / internal
来源：http://hcu.tianlin.xyz

[G11] getter / setter
来源：http://geo.bbcook.cn

Py:   @property 与 @x.setter
来源：http://fpt.yueranfly.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lwm.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://mik.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://uiz.cucudq.cn

Java: public String getName() { return name; }
来源：http://jpd.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://fto.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://kmr.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://blf.ivvv.top

[G12] 对象转字符串
来源：http://mfj.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://nzl.c1oappe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bdn.wangdashe.top

JS:   toString() { return this.name; }
来源：http://rze.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://nep.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://cln.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://zvk.ybcxt.top

Ruby: def to_s; @name; end
来源：http://hdf.ehwqpu.com

C#:   public override string ToString() => Name;
来源：http://dbn.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://ggy.nwbrower.top

Py:   isinstance(u, User)
来源：http://mzc.zhengqikj.top

PHP:  $u instanceof User
来源：http://ejv.xylfe.cn

JS:   u instanceof User
来源：http://qkd.yvedp.cn

TS:   u instanceof User
来源：http://grg.iojbl.cn

Java: u instanceof User
来源：http://nwi.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vtv.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://dta.cheryme.top

C#:   u is User
来源：http://akg.fengsongda.top

[G14] 数据类 / record
来源：http://iev.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kul.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://dya.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://azr.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://azu.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://ftt.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://xlt.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://emo.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://ntc.shuidangran.top

[G15] 枚举
来源：http://hvk.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yao.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bpx.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tbq.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://crd.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://tzl.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uwv.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://avx.c1oappe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ain.ydzc1.top

[G16] 对象转数组 / 字典
来源：http://xbp.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xly.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://jib.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://ajw.c1oappe.top

TS:   Object.entries(obj)
来源：http://gqk.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gpq.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://imj.yj20258888.top

Ruby: obj.instance_variables
来源：http://prw.0kj1m.cn

C#:   // 用反射或 System.Text.Json
来源：http://fgt.ybcxt.top

================================================================================
来源：http://poz.aibaodan.cn

H. 异常与错误处理
来源：http://rnu.hywenlv.cn

================================================================================
来源：http://ukn.uphjek.com

[H01] try / catch 基础
来源：http://fcm.smart0.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ney.gotoacloud.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://euh.52xcode.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sxh.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufh.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xdn.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dvl.52xcode.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aga.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ash.yueranfly.top

[H02] finally / ensure 收尾
来源：http://boh.yj202588.top

Py:   try: f()⏎finally: cleanup()
来源：http://zlg.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jqr.yj20258.top

JS:   try { f(); } finally { cleanup(); }
来源：http://icx.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tti.sysykeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://tkc.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ood.pycfn.com

Ruby: begin; f; ensure; cleanup; end
来源：http://qyw.hnxiangtu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dwt.mhx1999.top

[H03] 主动抛出异常
来源：http://xbw.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://xzw.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://phf.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://afe.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://fpm.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rax.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://odj.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kxf.fanxiaobao.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://pqg.zhengqikj.top

[H04] 自定义异常类型
来源：http://qdf.sjlbkw.cn

Py:   class MyError(Exception): pass
来源：http://qxf.chenzaomai.com

PHP:  class MyError extends RuntimeException {}
来源：http://gqf.jinyuanbaomall.cn

JS:   class MyError extends Error {}
来源：http://rqu.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://zic.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://poi.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ktm.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://iii.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://qgd.zhoulong.xyz

[H05] 捕获特定类型
来源：http://jyw.jinqigfzy.top

Py:   except ValueError as e:
来源：http://jos.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zub.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://ayo.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://drj.sjlbkw.cn

Java: catch (IOException | SQLException e) {}
来源：http://kwb.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ikz.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://exy.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rxb.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://fuv.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://rhr.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://fjv.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nje.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oic.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kpu.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://mlp.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://elk.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://zmc.jyoumei.cn

[H07] 断言
来源：http://yio.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://idk.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://erl.yuxming.cn

JS:   console.assert(x > 0);
来源：http://cym.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://cma.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://dof.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lfj.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://msw.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://zap.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://twz.nanxuanxn.top

Py:   str(e);  traceback.format_exc()
来源：http://yti.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sah.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://abo.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jiv.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tvt.hnxiangtu.top

Go:   err.Error()
来源：http://qwj.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://nqv.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://jef.9152youxi.cn

[H09] 带错误码的异常
来源：http://lyp.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://icz.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qjm.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xeo.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vow.tarul.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wor.daria6918.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bsv.sweek.top

Ruby: raise MyError.new("fail", 500)
来源：http://cwa.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://izy.jqgfzy.top

[H10] 资源自动释放
来源：http://tyh.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vmt.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hup.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yuq.aibaodan.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wqb.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xyn.andypj.xyz

Go:   defer f.Close()
来源：http://rki.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nxq.yongpay.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cqn.hesvh.cn

================================================================================
来源：http://xgq.ivvv.top

I. 正则表达式
来源：http://qee.zhengqikj.top

================================================================================
来源：http://tkm.zhixingplan.top

[I01] 判断是否匹配
来源：http://szq.tian-w.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wsv.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://lcy.cashguo.top

JS:   /\d+/.test(s)
来源：http://eoz.zhongyouzk.top

TS:   /\d+/.test(s)
来源：http://fbd.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kkb.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yom.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://mrv.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://scv.havefunace.top

[I02] 提取所有匹配
来源：http://iss.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://xxo.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gfu.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nbp.chenzaomai.com

TS:   s.match(/\d+/g)
来源：http://kpz.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qog.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wwr.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://ivq.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jis.wangdashe.top

[I03] 提取捕获分组
来源：http://wok.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vsw.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yiz.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ehu.ehwqpu.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://htf.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wdc.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iwx.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ftn.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ymt.jqgfzy.top

[I04] 正则替换
来源：http://hfl.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bkl.wangshuangyany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lxp.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://wwi.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wyp.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://dlm.cheryme.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lda.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://quw.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://slj.ctjpmb.com

[I05] 按正则拆分
来源：http://irn.9152youxi.cn


<!-- 参考信息 -->