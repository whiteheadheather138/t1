代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://edk.wangshuangyany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syn.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blv.fengsongda.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ofw.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://drl.ydjk.org.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://miw.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fyy.vqdsnc.cn

[F12] CSV 读写
来源：http://xqy.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tcn.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nhf.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cxr.fanxiaobao.xyz

TS:   // 同上
来源：http://eab.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wkr.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://epg.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://urz.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://suh.gotoacloud.top

================================================================================
来源：http://nfq.yj20258888.top

G. 面向对象
来源：http://hin.iojbl.cn

================================================================================
来源：http://tfm.tarul.cn

[G01] 定义类
来源：http://exa.sysykeji.top

Py:   class User: pass
来源：http://tfe.smart0.xyz

PHP:  class User {}
来源：http://zii.birdmap.top

JS:   class User {}
来源：http://vmt.shzxlz.cn

TS:   class User { name: string = ""; }
来源：http://xga.jinqigufen.top

Java: class User {}
来源：http://gtc.dianchejie.cn

Go:   type User struct { Name string }
来源：http://yil.tianlin.xyz

Ruby: class User; end
来源：http://cfx.hysaishi.cn

C#:   class User {}
来源：http://hgy.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://hcb.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://izq.yuanzhike.top

PHP:  public function __construct(public string $name) {}
来源：http://vlc.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://ymo.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://jri.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://juh.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lwm.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://xla.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://ylq.snrcjt.cn

[G03] 实例属性
来源：http://uyg.316326.xyz

Py:   self.name = "x"
来源：http://bse.hcnkem.com

PHP:  public string $name = "x";
来源：http://pda.dianchejie.cn

JS:   this.name = "x";
来源：http://qui.wangdashe.top

TS:   name: string = "x";
来源：http://tdc.52xcode.cn

Java: private String name;
来源：http://yoo.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ayj.yanxiufei.cn

Ruby: @name = "x"
来源：http://knh.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://uop.fengsongda.top

[G04] 定义方法
来源：http://tod.cucudq.cn

Py:   def greet(self): return self.name
来源：http://hlp.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lnz.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://lvi.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://gkw.hesvh.cn

Java: String greet() { return name; }
来源：http://yaj.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://snp.hesvh.cn

Ruby: def greet; @name; end
来源：http://nng.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://jlz.xuetiantiany.cn

[G05] 继承
来源：http://gpb.yuxming.cn

Py:   class Admin(User): pass
来源：http://hpe.fzhhl.top

PHP:  class Admin extends User {}
来源：http://aoc.yonumen.top

JS:   class Admin extends User {}
来源：http://gmf.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://qep.hywenlv.cn

Java: class Admin extends User {}
来源：http://moe.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ffz.gzhubu.top

Ruby: class Admin < User; end
来源：http://awk.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://qvb.tian-w.cn

[G06] 重写方法
来源：http://zzn.tarul.cn

Py:   def greet(self): return "admin"
来源：http://idi.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bez.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://zbx.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://ahb.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://uek.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ngg.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://vop.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://fyi.hcnkem.com

[G07] 调用父类方法
来源：http://uuk.nanxinkj.top

Py:   super().greet()
来源：http://ogs.zhiwuduotai.top

PHP:  parent::greet();
来源：http://scb.pengpengdd.cyou

JS:   super.greet();
来源：http://mpl.havefunace.top

TS:   super.greet();
来源：http://fzy.zhixingplan.top

Java: super.greet();
来源：http://ndx.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bby.xziqi.cn

Ruby: super
来源：http://pty.hesvh.cn

C#:   base.Greet();
来源：http://owi.yangfankeji.com

[G08] 静态方法与属性
来源：http://qov.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://quz.316326.xyz

PHP:  public static function f() {}
来源：http://gpi.yvedp.cn

JS:   static f() {}
来源：http://pbo.xinyue.icu

TS:   static f(): void {}
来源：http://ypn.zhixingplan.top

Java: static void f() {}
来源：http://cok.hywenlv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zpa.316326.xyz

Ruby: def self.f; end
来源：http://gkh.ybcxt.top

C#:   public static void F() {}
来源：http://avc.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://zay.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://ujb.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://uff.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gol.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://eox.sysykeji.top

Java: interface Shape { double area(); }
来源：http://crn.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://rzz.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jxi.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://fti.hongshengwenyu.top

[G10] 访问控制
来源：http://sai.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://iwd.chenlongwang.top

PHP:  public / protected / private
来源：http://lkc.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://tsw.hammf.cn

TS:   public / protected / private
来源：http://yfo.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://yjn.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://kyr.wangshuangyany.cn

Ruby: public / protected / private
来源：http://tek.daria6918.cn

C#:   public / protected / private / internal
来源：http://cae.daria6918.cn

[G11] getter / setter
来源：http://jod.ybcxt.top

Py:   @property 与 @x.setter
来源：http://atw.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mps.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://qnd.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://eum.yj20258888.top

Java: public String getName() { return name; }
来源：http://dgi.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://par.fehbvm.com

Ruby: attr_accessor :name
来源：http://uhd.yonumen.top

C#:   public string Name { get; set; }
来源：http://lqk.zhixingplan.top

[G12] 对象转字符串
来源：http://vrd.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://tzt.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://llo.xinyue.icu

JS:   toString() { return this.name; }
来源：http://imz.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://pue.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://xxc.ivvv.top

Go:   func (u User) String() string { return u.Name }
来源：http://hjg.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://sho.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://yht.cqqwz.cn

[G13] 判断对象类型
来源：http://okl.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://ikf.birdmap.top

PHP:  $u instanceof User
来源：http://inc.aibaodan.cn

JS:   u instanceof User
来源：http://rhi.zhengqikj.top

TS:   u instanceof User
来源：http://vyp.yangfankeji.com

Java: u instanceof User
来源：http://fxn.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iru.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://puw.aibaodan.cn

C#:   u is User
来源：http://kub.fzhhl.top

[G14] 数据类 / record
来源：http://qhm.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://djw.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://ggt.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://awk.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://eyv.aibaodan.cn

Java: record User(String name, int age) {}
来源：http://cna.cheryme.top

Go:   type User struct { Name string; Age int }
来源：http://ttn.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://axm.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://lmx.fehbvm.com

[G15] 枚举
来源：http://ugf.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qrx.hammf.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cbe.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://plc.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ytt.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://wra.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pls.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://fur.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://obq.fktsv.cn

[G16] 对象转数组 / 字典
来源：http://mjh.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://upx.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://pba.jqgfzy.top

JS:   Object.entries(obj)
来源：http://dru.jqgfzy.top

TS:   Object.entries(obj)
来源：http://yzi.mhx1999.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qog.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://saw.cheryme.top

Ruby: obj.instance_variables
来源：http://sql.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://tzb.jyoumei.cn

================================================================================
来源：http://iqa.wangdashe.top

H. 异常与错误处理
来源：http://iej.sxryk.cn

================================================================================
来源：http://vku.hnxiangtu.top

[H01] try / catch 基础
来源：http://mfi.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rve.yj20258.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lnh.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hkw.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lhs.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://svi.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwg.ydjk.org.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aop.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zts.gzhubu.top

[H02] finally / ensure 收尾
来源：http://vbh.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://czj.0kj1m.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dqh.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kzj.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zfz.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://htl.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://amw.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ldw.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bpz.cashguo.top

[H03] 主动抛出异常
来源：http://huk.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://tfl.smart0.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uoj.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://ntr.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://cza.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://feb.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ldb.ehwqpu.com

Ruby: raise ArgumentError, "错误信息"
来源：http://bcv.pycfn.com

C#:   throw new ArgumentException("错误信息");
来源：http://oyg.snrcjt.cn

[H04] 自定义异常类型
来源：http://bhx.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://hqm.aibaodan.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yoo.vehdjk.com

JS:   class MyError extends Error {}
来源：http://ixf.cashguo.top

TS:   class MyError extends Error {}
来源：http://pzs.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://pku.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xbl.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://kch.smart0.xyz

C#:   class MyException : Exception {}
来源：http://alv.redwolf501.top

[H05] 捕获特定类型
来源：http://ddp.cdnleiting.top

Py:   except ValueError as e:
来源：http://wai.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aci.yongpay.top

JS:   if (e instanceof TypeError) {}
来源：http://imx.daxiang520.top

TS:   if (e instanceof TypeError) {}
来源：http://igb.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://boy.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mmn.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://pof.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vrz.yvedp.cn

[H06] 可选值 / 空值安全访问
来源：http://cyc.aizwys.cn

Py:   value = d.get("k") or default
来源：http://ogc.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://iww.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://uzi.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://kwx.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gac.cheryme.top

Go:   if v, ok := m["k"]; ok { }
来源：http://khr.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://fpb.sweek.top

C#:   obj?.A?.B ?? default
来源：http://cad.ywan-chungtsiang.top

[H07] 断言
来源：http://brl.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://aix.xinyue.icu

PHP:  assert($x > 0);
来源：http://aqv.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://ylv.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://ppi.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://qsr.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jzf.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://iec.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://rxq.shuidangran.top

[H08] 获取错误信息与堆栈
来源：http://ujg.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://urw.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://efz.sufxvd.cn

JS:   e.message;  e.stack
来源：http://mqn.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qhb.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hob.jlsjyb.cn

Go:   err.Error()
来源：http://vnb.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://wyo.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://dxx.gogol.net.cn

[H09] 带错误码的异常
来源：http://qxp.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kbt.vehdjk.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ixp.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jiy.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ejv.cashguo.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yig.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pbo.wangdashe.top

Ruby: raise MyError.new("fail", 500)
来源：http://imq.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gqq.zdbjq.cn

[H10] 资源自动释放
来源：http://lnm.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sih.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://anw.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ymt.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tla.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ahu.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://fie.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://axr.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yvu.jqgufenzy.top

================================================================================
来源：http://umo.gzhubu.top

I. 正则表达式
来源：http://zjz.yangfankeji.com

================================================================================
来源：http://spj.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://uwc.snrcjt.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rki.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://qbo.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://alx.aizwys.cn

TS:   /\d+/.test(s)
来源：http://etn.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ypd.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tlg.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://nky.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nhx.yj202588.top

[I02] 提取所有匹配
来源：http://jel.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://odr.jqgfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://idx.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uzd.svipenyu.cn

TS:   s.match(/\d+/g)
来源：http://fra.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kge.hcnkem.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wky.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://mjv.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ogk.snrcjt.cn

[I03] 提取捕获分组
来源：http://uwz.dashuyun.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://twe.ivvv.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cfg.hnxiangtu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://btn.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tuk.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://umv.hnqzz.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cgc.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pes.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yeb.snrcjt.cn

[I04] 正则替换
来源：http://erk.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kac.ctjpmb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tam.xylfe.cn

JS:   s.replace(/\d+/g, "#")
来源：http://exj.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://fsq.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://uhj.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://qum.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kmi.uphjek.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gtx.gaohongyu789.top

[I05] 按正则拆分
来源：http://wlq.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gaa.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yoy.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://bkv.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://ruh.feifeiyinyue.top


<!-- 参考信息 -->