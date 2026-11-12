代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ktj.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bto.fktsv.cn

[F11] 复制与移动文件
来源：http://hjl.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cjt.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ajt.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://evq.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aax.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yby.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://muc.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lkb.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ivx.aizwys.cn

[F12] CSV 读写
来源：http://ibi.cucudq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://obq.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gsz.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ymn.pycfn.com

TS:   // 同上
来源：http://gmf.ppjwa.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xxk.zycfv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lww.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xej.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://anf.zhongyouzk.top

================================================================================
来源：http://qmo.hywenlv.cn

G. 面向对象
来源：http://wax.gotoacloud.top

================================================================================
来源：http://kgt.ehwqpu.com

[G01] 定义类
来源：http://art.sxryk.cn

Py:   class User: pass
来源：http://oeb.ctjpmb.com

PHP:  class User {}
来源：http://pax.daxiang520.top

JS:   class User {}
来源：http://vvv.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://kdj.xingfuxueyuan.xyz

Java: class User {}
来源：http://nqm.fzhhl.top

Go:   type User struct { Name string }
来源：http://fic.jinqigufen.top

Ruby: class User; end
来源：http://iuk.hnqzz.top

C#:   class User {}
来源：http://yzp.kuanghao11.cn

[G02] 构造函数
来源：http://que.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://psc.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://wbu.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://iwh.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://nop.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://kce.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://abg.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://wqn.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://dzi.shanyushiyangkeji.top

[G03] 实例属性
来源：http://hjx.zhijiandao.cn

Py:   self.name = "x"
来源：http://far.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://wdv.hnxiangtu.top

JS:   this.name = "x";
来源：http://cze.ydzc1.top

TS:   name: string = "x";
来源：http://bpj.fanxiaobao.xyz

Java: private String name;
来源：http://adl.fktsv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksc.nanxuanxn.top

Ruby: @name = "x"
来源：http://iza.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://snu.iojbl.cn

[G04] 定义方法
来源：http://aai.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://hrj.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hhm.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://umu.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://hcz.yvedp.cn

Java: String greet() { return name; }
来源：http://qye.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dwj.dianchejie.cn

Ruby: def greet; @name; end
来源：http://ybf.shuidangran.top

C#:   public string Greet() => Name;
来源：http://pdr.svipenyu.cn

[G05] 继承
来源：http://owb.xziqi.cn

Py:   class Admin(User): pass
来源：http://bjn.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://mcg.hnqzz.top

JS:   class Admin extends User {}
来源：http://woe.jyoumei.cn

TS:   class Admin extends User {}
来源：http://rih.bbcook.cn

Java: class Admin extends User {}
来源：http://tuu.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cfl.jyoumei.cn

Ruby: class Admin < User; end
来源：http://vol.fengsongda.top

C#:   class Admin : User {}
来源：http://oau.yangfankeji.com

[G06] 重写方法
来源：http://bsw.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://cox.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://smb.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://krw.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://hdu.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://ffc.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uio.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://mhx.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://gmu.hongshengwenyu.top

[G07] 调用父类方法
来源：http://zpc.yj202588.top

Py:   super().greet()
来源：http://ryj.andypj.xyz

PHP:  parent::greet();
来源：http://omm.zhengqikj.top

JS:   super.greet();
来源：http://xwt.sysykeji.top

TS:   super.greet();
来源：http://ech.zhixingplan.top

Java: super.greet();
来源：http://ffb.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pku.xingfuxueyuan.xyz

Ruby: super
来源：http://imf.xinyue.icu

C#:   base.Greet();
来源：http://siz.fzhhl.top

[G08] 静态方法与属性
来源：http://szm.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://flb.316326.xyz

PHP:  public static function f() {}
来源：http://eqi.smart0.xyz

JS:   static f() {}
来源：http://caz.hnqzz.top

TS:   static f(): void {}
来源：http://yge.jinghuilouyu.cn

Java: static void f() {}
来源：http://enr.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tpm.pycfn.com

Ruby: def self.f; end
来源：http://rxj.9152youxi.cn

C#:   public static void F() {}
来源：http://sdw.cheryme.top

[G09] 接口 / 抽象类
来源：http://iqb.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://zwk.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://xjo.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ecb.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://alp.c1oappe.top

Java: interface Shape { double area(); }
来源：http://jqv.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://stw.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dmt.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://xbz.pycfn.com

[G10] 访问控制
来源：http://uxy.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://dlh.tianlin.xyz

PHP:  public / protected / private
来源：http://wye.bjfxy.top

JS:   #private 字段；其余公开
来源：http://xjr.yj202588.top

TS:   public / protected / private
来源：http://zji.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://wwk.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://orc.xylfe.cn

Ruby: public / protected / private
来源：http://wwg.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://scr.cdnleiting.top

[G11] getter / setter
来源：http://upp.fktsv.cn

Py:   @property 与 @x.setter
来源：http://jky.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://erh.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://ayk.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://ygn.tarul.cn

Java: public String getName() { return name; }
来源：http://vgx.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hnh.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://dbm.nanxuanxn.top

C#:   public string Name { get; set; }
来源：http://zes.jlsjyb.cn

[G12] 对象转字符串
来源：http://zyw.tanke756.top

Py:   def __str__(self): return self.name
来源：http://jhs.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://tus.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://mpy.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://ren.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://ncc.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vnl.mhx1999.top

Ruby: def to_s; @name; end
来源：http://vjg.yuxming.cn

C#:   public override string ToString() => Name;
来源：http://kmb.smart0.xyz

[G13] 判断对象类型
来源：http://zii.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://ywj.aizwys.cn

PHP:  $u instanceof User
来源：http://hdl.jyoumei.cn

JS:   u instanceof User
来源：http://zwt.52xcode.cn

TS:   u instanceof User
来源：http://aub.bbcook.cn

Java: u instanceof User
来源：http://kqy.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ibw.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://nix.jlsjyb.cn

C#:   u is User
来源：http://hyd.chenjidiqi.icu

[G14] 数据类 / record
来源：http://mox.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iod.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://jre.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://umx.svipenyu.cn

TS:   type User = { name: string; age: number };
来源：http://juu.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://pgj.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://jkg.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ker.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://xxi.zdqjudy.top

[G15] 枚举
来源：http://rsv.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rfq.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ggk.shanyushiyangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://czj.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nrx.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://ekx.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qjv.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://ano.hysaishi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://awt.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://zdr.xuetiantiany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lvg.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://kph.cashguo.top

JS:   Object.entries(obj)
来源：http://pax.smart0.xyz

TS:   Object.entries(obj)
来源：http://fbs.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dha.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oqb.zhixingplan.top

Ruby: obj.instance_variables
来源：http://dmf.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://ryc.yj202588.top

================================================================================
来源：http://rvw.yj20258.top

H. 异常与错误处理
来源：http://mad.316326.xyz

================================================================================
来源：http://ayr.fzhhl.top

[H01] try / catch 基础
来源：http://dig.zhongyouzk.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dqt.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ufi.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qik.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mfn.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nja.chenzaomai.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nxj.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dnn.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hhr.yj20258888.top

[H02] finally / ensure 收尾
来源：http://kif.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pjh.hywenlv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dop.yongpay.top

JS:   try { f(); } finally { cleanup(); }
来源：http://okr.yueranfly.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rhl.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bnh.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://yah.xingfuxueyuan.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://mil.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zyt.aibaodan.cn

[H03] 主动抛出异常
来源：http://fwo.zdbjq.cn

Py:   raise ValueError("错误信息")
来源：http://lak.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qjx.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://okj.svipenyu.cn

TS:   throw new Error("错误信息");
来源：http://fva.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://arq.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eay.ydzc1.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zkf.cucudq.cn

C#:   throw new ArgumentException("错误信息");
来源：http://axv.cqqwz.cn

[H04] 自定义异常类型
来源：http://nbp.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://tje.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://fvx.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://qon.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://wjc.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://ebm.daria6918.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsk.zhijiandao.cn

Ruby: class MyError < StandardError; end
来源：http://ohb.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://ffn.dianchejie.cn

[H05] 捕获特定类型
来源：http://anc.ivvv.top

Py:   except ValueError as e:
来源：http://jna.c1oappe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zdg.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://nyi.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://kzc.svipenyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://fiq.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jqo.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://ykb.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fcw.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://okq.fengsongda.top

Py:   value = d.get("k") or default
来源：http://fpy.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hsl.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tfd.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xbv.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ewb.yonumen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kxz.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://bdc.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://zmz.gzhubu.top

[H07] 断言
来源：http://fgx.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://wuz.jiagoushi.top

PHP:  assert($x > 0);
来源：http://yqk.52xcode.cn

JS:   console.assert(x > 0);
来源：http://krv.zhoulong.xyz

TS:   console.assert(x > 0);
来源：http://fpc.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://dvf.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kdd.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://izl.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://gsu.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://ige.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://bwj.yonumen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pwf.hnxiangtu.top

JS:   e.message;  e.stack
来源：http://wsg.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dsg.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lkq.chenlongwang.top

Go:   err.Error()
来源：http://qbu.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://bfr.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://vji.fanxiaobao.xyz

[H09] 带错误码的异常
来源：http://tjf.vqdsnc.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dmd.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mjn.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nqs.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rkq.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lis.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xrm.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uhx.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://qxu.ydzc1.top

[H10] 资源自动释放
来源：http://ouz.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://kts.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sne.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ckp.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mul.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fmx.zhiwuduotai.top

Go:   defer f.Close()
来源：http://dkz.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://azt.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kru.pycfn.com

================================================================================
来源：http://fpl.shanyushiyangkeji.top

I. 正则表达式
来源：http://pcm.mhx1999.top

================================================================================
来源：http://zmo.andypj.xyz

[I01] 判断是否匹配
来源：http://vre.sweek.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://evv.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kws.yfazqb.com

JS:   /\d+/.test(s)
来源：http://nck.cucudq.cn

TS:   /\d+/.test(s)
来源：http://hez.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rdo.epnwcf.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xkr.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://kjc.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vqb.xinyue.icu

[I02] 提取所有匹配
来源：http://mzx.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://yqa.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eap.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lsd.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://iyu.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://drd.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ntw.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://asa.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ksk.yanxiufei.cn

[I03] 提取捕获分组
来源：http://yfw.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sjz.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yua.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kyl.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sxt.yvedp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jzx.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://miv.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://efe.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gdw.tanke756.top

[I04] 正则替换
来源：http://ksk.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cip.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://quq.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://pfr.dianchejie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ass.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://add.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://pox.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://nnv.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zub.hongshengwenyu.top

[I05] 按正则拆分
来源：http://inh.cqqwz.cn


<!-- 参考信息 -->