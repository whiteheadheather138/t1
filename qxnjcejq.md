代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nbc.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iuo.gaohongyu789.top

[F11] 复制与移动文件
来源：http://mvo.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mra.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rni.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yts.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jak.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fbr.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ngg.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yyz.uphjek.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ihc.chenjidiqi.icu

[F12] CSV 读写
来源：http://trz.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://upq.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xcd.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jps.jinqigfzy.top

TS:   // 同上
来源：http://kls.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oev.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zxt.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ece.xingfuxueyuan.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://yji.ivvv.top

================================================================================
来源：http://vbf.chenzaomai.com

G. 面向对象
来源：http://eyh.nwbrower.top

================================================================================
来源：http://xpl.daria6918.cn

[G01] 定义类
来源：http://uqs.hammf.cn

Py:   class User: pass
来源：http://jje.sxryk.cn

PHP:  class User {}
来源：http://ttd.guowangkeji.top

JS:   class User {}
来源：http://eia.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://cpe.tian-w.cn

Java: class User {}
来源：http://sjx.xuanzx.com

Go:   type User struct { Name string }
来源：http://vsv.hammf.cn

Ruby: class User; end
来源：http://xgu.zhijiandao.cn

C#:   class User {}
来源：http://cab.ydzc1.top

[G02] 构造函数
来源：http://jcy.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://iwn.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://lpu.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://ooe.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://tgd.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://igd.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sbr.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://ttw.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://mdp.chenjidiqi.icu

[G03] 实例属性
来源：http://yvt.ctjpmb.com

Py:   self.name = "x"
来源：http://uwc.cqqwz.cn

PHP:  public string $name = "x";
来源：http://zgo.chenjidiqi.icu

JS:   this.name = "x";
来源：http://jba.gaohongyu789.top

TS:   name: string = "x";
来源：http://unz.xuetiantiany.cn

Java: private String name;
来源：http://ykp.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zsh.cucudq.cn

Ruby: @name = "x"
来源：http://gkj.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://dah.svipenyu.cn

[G04] 定义方法
来源：http://gcl.daria6918.cn

Py:   def greet(self): return self.name
来源：http://qqz.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fah.xuetiantiany.cn

JS:   greet() { return this.name; }
来源：http://tvb.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://rfg.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://shy.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdm.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://jnp.sysykeji.top

C#:   public string Greet() => Name;
来源：http://fgf.0kj1m.cn

[G05] 继承
来源：http://wdv.zdbjq.cn

Py:   class Admin(User): pass
来源：http://dqv.316326.xyz

PHP:  class Admin extends User {}
来源：http://ylr.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://zzc.nwbrower.top

TS:   class Admin extends User {}
来源：http://lwf.zhongyouzk.top

Java: class Admin extends User {}
来源：http://may.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ido.shuidangran.top

Ruby: class Admin < User; end
来源：http://ymq.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://qwb.svipenyu.cn

[G06] 重写方法
来源：http://ibf.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://ujh.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://voi.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://fup.chenzaomai.com

TS:   greet(): string { return "admin"; }
来源：http://uqh.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://uon.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sob.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://wuf.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://qfq.bjfxy.top

[G07] 调用父类方法
来源：http://pev.smart0.xyz

Py:   super().greet()
来源：http://tnh.bjfxy.top

PHP:  parent::greet();
来源：http://vdy.jianghu66.top

JS:   super.greet();
来源：http://ymz.52xcode.cn

TS:   super.greet();
来源：http://vmm.ppjwa.cn

Java: super.greet();
来源：http://xzn.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://opi.xziqi.cn

Ruby: super
来源：http://mjr.zhongyouzk.top

C#:   base.Greet();
来源：http://avj.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://jdl.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uop.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://hss.pycfn.com

JS:   static f() {}
来源：http://jfs.meibo888.top

TS:   static f(): void {}
来源：http://qms.zhijiandao.cn

Java: static void f() {}
来源：http://hht.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xdd.mhx1999.top

Ruby: def self.f; end
来源：http://zrp.hammf.cn

C#:   public static void F() {}
来源：http://fej.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://aqu.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://fhh.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://ppt.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lrr.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://hnt.epnwcf.com

Java: interface Shape { double area(); }
来源：http://nxh.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://std.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ths.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://cgg.cqqwz.cn

[G10] 访问控制
来源：http://uzs.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://aac.cucudq.cn

PHP:  public / protected / private
来源：http://iml.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://dvj.cashguo.top

TS:   public / protected / private
来源：http://byb.fanxiaobao.xyz

Java: public / protected / private / 默认包级
来源：http://hxf.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://psq.dashuyun.cn

Ruby: public / protected / private
来源：http://xjv.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://zam.gaohongyu789.top

[G11] getter / setter
来源：http://tuj.smart0.xyz

Py:   @property 与 @x.setter
来源：http://spd.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hrp.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://hbp.ehwqpu.com

TS:   get name(): string { return this._name; }
来源：http://bgy.tian-w.cn

Java: public String getName() { return name; }
来源：http://spf.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ctm.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://svy.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://rwb.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://prk.0kj1m.cn

Py:   def __str__(self): return self.name
来源：http://umc.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://udv.chenzaomai.com

JS:   toString() { return this.name; }
来源：http://wet.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://jfs.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://ubn.xylfe.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bce.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://bkw.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://swd.tarul.cn

[G13] 判断对象类型
来源：http://fkw.shuidangran.top

Py:   isinstance(u, User)
来源：http://iop.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://ftt.tianlin.xyz

JS:   u instanceof User
来源：http://lak.fengsongda.top

TS:   u instanceof User
来源：http://ibh.daxiang520.top

Java: u instanceof User
来源：http://wgn.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://oai.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://qea.zhengqikj.top

C#:   u is User
来源：http://omm.yvedp.cn

[G14] 数据类 / record
来源：http://qso.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pil.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://vlb.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://wes.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://mcj.andypj.xyz

Java: record User(String name, int age) {}
来源：http://fof.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://gkl.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nqa.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://gwk.cqqwz.cn

[G15] 枚举
来源：http://ejb.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vzu.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ffe.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jlz.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tea.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://slz.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jop.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://jzc.yfazqb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zaw.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://nwp.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://crx.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://pwn.chenlongwang.top

JS:   Object.entries(obj)
来源：http://klg.tarul.cn

TS:   Object.entries(obj)
来源：http://dud.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yyg.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oho.ybcxt.top

Ruby: obj.instance_variables
来源：http://ieh.zhongyouzk.top

C#:   // 用反射或 System.Text.Json
来源：http://qis.vehdjk.com

================================================================================
来源：http://mvx.zhixingplan.top

H. 异常与错误处理
来源：http://obi.yj20258.top

================================================================================
来源：http://ssa.cashguo.top

[H01] try / catch 基础
来源：http://jdn.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cpe.hesvh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pal.zdqjudy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dos.jyoumei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uxc.zhijiandao.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wgw.fengsongda.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dwp.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yxu.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jhx.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://tqc.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bnq.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kxj.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://abk.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dfv.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eqz.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://okt.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ndm.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dpj.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://tqa.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://zmn.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hho.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://qlh.sweek.top

TS:   throw new Error("错误信息");
来源：http://zul.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bbu.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tql.haohaochexian.top

Ruby: raise ArgumentError, "错误信息"
来源：http://wee.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cgh.yj202588.top

[H04] 自定义异常类型
来源：http://kyj.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://jzk.bbcook.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qgr.yangfankeji.com

JS:   class MyError extends Error {}
来源：http://gri.andypj.xyz

TS:   class MyError extends Error {}
来源：http://rbo.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://cas.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dqg.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://toy.ivvv.top

C#:   class MyException : Exception {}
来源：http://hva.dashuyun.cn

[H05] 捕获特定类型
来源：http://dbk.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://kqd.chenjidiqi.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://leb.quarkkingdee.top

JS:   if (e instanceof TypeError) {}
来源：http://swp.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://btp.fzhhl.top

Java: catch (IOException | SQLException e) {}
来源：http://jxe.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ryb.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://eel.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lwa.snrcjt.cn

[H06] 可选值 / 空值安全访问
来源：http://qjm.wangdashe.top

Py:   value = d.get("k") or default
来源：http://ikx.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://myk.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jzm.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://kiz.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bbc.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lgi.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://lss.zdqjudy.top

C#:   obj?.A?.B ?? default
来源：http://wgk.mhx1999.top

[H07] 断言
来源：http://tli.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://vql.jinqigufen.top

PHP:  assert($x > 0);
来源：http://wma.fehbvm.com

JS:   console.assert(x > 0);
来源：http://mba.zhongyouzk.top

TS:   console.assert(x > 0);
来源：http://rsj.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://ajv.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zfs.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://ori.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://sve.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://nnf.sweek.top

Py:   str(e);  traceback.format_exc()
来源：http://owo.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://svm.fengsongda.top

JS:   e.message;  e.stack
来源：http://ajd.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://frh.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://evw.ppjwa.cn

Go:   err.Error()
来源：http://ukh.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://phf.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://lhe.jianghu66.top

[H09] 带错误码的异常
来源：http://evm.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lfc.zhoulong.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://jhu.xziqi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://exw.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpm.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://skd.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wll.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://zbm.hywenlv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tid.vehdjk.com

[H10] 资源自动释放
来源：http://rsf.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://evq.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kma.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fox.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txg.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gmw.redwolf501.top

Go:   defer f.Close()
来源：http://gkw.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kol.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ysx.hnxiangtu.top

================================================================================
来源：http://pej.zhijiandao.cn

I. 正则表达式
来源：http://lht.daxiang520.top

================================================================================
来源：http://nwt.zdbjq.cn

[I01] 判断是否匹配
来源：http://yey.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ctk.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://fbp.jqgfzy.top

JS:   /\d+/.test(s)
来源：http://put.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://rzw.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gaq.316326.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ikr.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://yhf.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yje.nwbrower.top

[I02] 提取所有匹配
来源：http://mzo.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://ewh.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://trh.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mkc.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://obl.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wng.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jmz.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://uyh.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oeq.yuanzhike.top

[I03] 提取捕获分组
来源：http://iua.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kxe.zhijiandao.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fhw.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ttv.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dkf.jianghu66.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lfk.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndy.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ajx.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://etu.yanxiufei.cn

[I04] 正则替换
来源：http://hzg.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hln.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nwo.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://hft.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://neg.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wef.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qqs.guannengcc.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bmf.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ejd.yvedp.cn

[I05] 按正则拆分
来源：http://vkk.tarul.cn


<!-- 参考信息 -->