代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jvz.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tfp.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gvb.snrcjt.cn

[F12] CSV 读写
来源：http://dap.52xcode.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zke.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jwo.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cyu.feifeiyinyue.top

TS:   // 同上
来源：http://ujb.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kwg.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xtw.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fyc.xinyue.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://osk.hysaishi.cn

================================================================================
来源：http://myy.snrcjt.cn

G. 面向对象
来源：http://rqq.tianlin.xyz

================================================================================
来源：http://tzr.fzhhl.top

[G01] 定义类
来源：http://uoj.xinyue.icu

Py:   class User: pass
来源：http://yfi.ehwqpu.com

PHP:  class User {}
来源：http://zfg.shanyushiyangkeji.top

JS:   class User {}
来源：http://lka.jinyuanbaomall.cn

TS:   class User { name: string = ""; }
来源：http://gdt.cdnleiting.top

Java: class User {}
来源：http://cdd.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://nsm.ydzc1.top

Ruby: class User; end
来源：http://hvn.cdnleiting.top

C#:   class User {}
来源：http://pxd.shanyushiyangtech.top

[G02] 构造函数
来源：http://dbv.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://lub.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://lne.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://gkx.tarul.cn

TS:   constructor(public name: string) {}
来源：http://qup.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://euc.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hml.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ynp.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://lye.xziqi.cn

[G03] 实例属性
来源：http://lkl.cqqwz.cn

Py:   self.name = "x"
来源：http://kwf.daxiang520.top

PHP:  public string $name = "x";
来源：http://pcs.jinqigufen.top

JS:   this.name = "x";
来源：http://bqe.fehbvm.com

TS:   name: string = "x";
来源：http://ovt.yj20258888.top

Java: private String name;
来源：http://xcx.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bhe.sufxvd.cn

Ruby: @name = "x"
来源：http://toy.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://jbm.ydjk.org.cn

[G04] 定义方法
来源：http://lxu.hesvh.cn

Py:   def greet(self): return self.name
来源：http://qbn.chenzaomai.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ftv.yueranfly.top

JS:   greet() { return this.name; }
来源：http://iht.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://qsk.sxryk.cn

Java: String greet() { return name; }
来源：http://aqk.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dnm.gogol.net.cn

Ruby: def greet; @name; end
来源：http://nso.shzxlz.cn

C#:   public string Greet() => Name;
来源：http://ozy.fanxiaobao.xyz

[G05] 继承
来源：http://nfx.zycfv.cn

Py:   class Admin(User): pass
来源：http://pnv.hesvh.cn

PHP:  class Admin extends User {}
来源：http://ldf.smart0.xyz

JS:   class Admin extends User {}
来源：http://dfn.jiagoushi.top

TS:   class Admin extends User {}
来源：http://ngb.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://ymb.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ktl.iojbl.cn

Ruby: class Admin < User; end
来源：http://baq.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://diu.hongshengwenyu.top

[G06] 重写方法
来源：http://zjh.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://krl.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lhw.sweek.top

JS:   greet() { return "admin"; }
来源：http://dww.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://wgv.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://agd.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dlp.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://jzv.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://tlt.9152youxi.cn

[G07] 调用父类方法
来源：http://klg.quarkkingdee.top

Py:   super().greet()
来源：http://vbw.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://ddk.gzhubu.top

JS:   super.greet();
来源：http://sfp.shanyushiyangtech.top

TS:   super.greet();
来源：http://bgm.daxiang520.top

Java: super.greet();
来源：http://cgy.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ynk.zycfv.cn

Ruby: super
来源：http://lui.kuanghao11.cn

C#:   base.Greet();
来源：http://xjy.sweek.top

[G08] 静态方法与属性
来源：http://xju.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rlp.yongpay.top

PHP:  public static function f() {}
来源：http://jfa.epnwcf.com

JS:   static f() {}
来源：http://ney.yj20258.top

TS:   static f(): void {}
来源：http://vcv.quarkkingdee.top

Java: static void f() {}
来源：http://afv.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://wpp.ybcxt.top

Ruby: def self.f; end
来源：http://zxv.gotoacloud.top

C#:   public static void F() {}
来源：http://bxb.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://yto.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://ogn.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://seg.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://usg.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://fit.cheryme.top

Java: interface Shape { double area(); }
来源：http://uju.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://bkt.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mua.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://mlg.gotoacloud.top

[G10] 访问控制
来源：http://myi.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://xzk.xziqi.cn

PHP:  public / protected / private
来源：http://hhh.uphjek.com

JS:   #private 字段；其余公开
来源：http://qtu.nanxinkj.top

TS:   public / protected / private
来源：http://spu.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://byt.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bmv.redwolf501.top

Ruby: public / protected / private
来源：http://ewm.guowangkeji.top

C#:   public / protected / private / internal
来源：http://npj.ydjk.org.cn

[G11] getter / setter
来源：http://jly.hammf.cn

Py:   @property 与 @x.setter
来源：http://rgq.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jai.daxiang520.top

JS:   get name() { return this._name; }
来源：http://wgk.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://jrp.dianchejie.cn

Java: public String getName() { return name; }
来源：http://vpu.xziqi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bhc.ctjpmb.com

Ruby: attr_accessor :name
来源：http://ywg.uphjek.com

C#:   public string Name { get; set; }
来源：http://ima.zdqjudy.top

[G12] 对象转字符串
来源：http://spn.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://dfd.cqqwz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lfk.52xcode.cn

JS:   toString() { return this.name; }
来源：http://fkz.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://tcj.yj202588.top

Java: @Override public String toString() { return name; }
来源：http://wua.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cyc.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://qgm.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://tnl.xylfe.cn

[G13] 判断对象类型
来源：http://rxs.shuidangran.top

Py:   isinstance(u, User)
来源：http://pba.cqqwz.cn

PHP:  $u instanceof User
来源：http://okt.epnwcf.com

JS:   u instanceof User
来源：http://myz.uphjek.com

TS:   u instanceof User
来源：http://uxl.fzhhl.top

Java: u instanceof User
来源：http://lcc.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yiy.svipenyu.cn

Ruby: u.is_a?(User)
来源：http://mdk.dianchejie.cn

C#:   u is User
来源：http://cmq.havefunace.top

[G14] 数据类 / record
来源：http://naj.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mlg.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://jeh.fehbvm.com

JS:   // 无内置：普通类或对象字面量
来源：http://bah.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://mcd.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://irz.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://hrd.hnqzz.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xiw.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://xvw.jyoumei.cn

[G15] 枚举
来源：http://ogq.xinyue.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://arq.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://amg.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cxs.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bbw.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://mdt.ppjwa.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dya.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://ird.jianghu66.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://abp.vehdjk.com

[G16] 对象转数组 / 字典
来源：http://rrd.c1oappe.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vye.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://kjc.andypj.xyz

JS:   Object.entries(obj)
来源：http://nhr.cheryme.top

TS:   Object.entries(obj)
来源：http://vpy.shzxlz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nhc.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://sde.xinyue.icu

Ruby: obj.instance_variables
来源：http://ngp.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://jsl.zycfv.cn

================================================================================
来源：http://xfm.zhoulong.xyz

H. 异常与错误处理
来源：http://egc.zhixingplan.top

================================================================================
来源：http://cce.snrcjt.cn

[H01] try / catch 基础
来源：http://qjh.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zor.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vck.xylfe.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zhr.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://glu.ydzc1.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sod.dashuyun.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ome.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ada.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ruc.guowangkeji.top

[H02] finally / ensure 收尾
来源：http://cnr.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://vmp.yj20258.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kxz.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nxr.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://boj.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ygs.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fdq.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hdf.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://sxu.gotoacloud.top

[H03] 主动抛出异常
来源：http://jwo.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://xcg.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ped.tanke756.top

JS:   throw new Error("错误信息");
来源：http://jqd.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://agd.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://etk.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xdr.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://prm.yfazqb.com

C#:   throw new ArgumentException("错误信息");
来源：http://tem.havefunace.top

[H04] 自定义异常类型
来源：http://qaj.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://ioa.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ira.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://arf.xinyue.icu

TS:   class MyError extends Error {}
来源：http://ucg.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://gwg.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gis.zhixingplan.top

Ruby: class MyError < StandardError; end
来源：http://xti.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://gfu.nanxinkj.top

[H05] 捕获特定类型
来源：http://yam.yueranfly.top

Py:   except ValueError as e:
来源：http://vgm.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wwi.hnxiangtu.top

JS:   if (e instanceof TypeError) {}
来源：http://fqj.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://vqw.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://mrz.yuanzhike.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qat.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://utu.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wat.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://uhy.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://eit.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://dbl.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://uwj.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://yha.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nlp.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://kqw.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://tgn.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://ily.quarkkingdee.top

[H07] 断言
来源：http://fnw.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://gko.pengpengdd.cyou

PHP:  assert($x > 0);
来源：http://gvw.sxryk.cn

JS:   console.assert(x > 0);
来源：http://fbh.sxryk.cn

TS:   console.assert(x > 0);
来源：http://lih.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://qpl.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yaz.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cbf.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://dtg.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://eua.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://wht.uphjek.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qqe.tian-w.cn

JS:   e.message;  e.stack
来源：http://yiz.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qqj.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xqo.xuanzx.com

Go:   err.Error()
来源：http://spc.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://olm.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://mqf.uphjek.com

[H09] 带错误码的异常
来源：http://gda.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qeb.yj202588.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hpe.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mis.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lxi.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gvw.uphjek.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zyd.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://tab.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kze.shuidangran.top

[H10] 资源自动释放
来源：http://gyn.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rif.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mhi.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cct.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mxj.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ldp.bbcook.cn

Go:   defer f.Close()
来源：http://xlq.ydzc1.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gij.52xcode.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xoi.c1oappe.top

================================================================================
来源：http://qpd.feifeiyinyue.top

I. 正则表达式
来源：http://lqt.hnxiangtu.top

================================================================================
来源：http://ple.ywan-chungtsiang.top

[I01] 判断是否匹配
来源：http://xbp.zhiwuduotai.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mae.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fxi.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://ckd.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://smb.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eyw.guannengcc.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eqm.yangfankeji.com

Ruby: s.match?(/\d+/)
来源：http://qaa.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qjt.nanxinkj.top

[I02] 提取所有匹配
来源：http://dpz.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://gzp.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://red.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tum.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://ono.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pwb.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kxx.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://hak.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fcj.ehwqpu.com

[I03] 提取捕获分组
来源：http://bgf.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kzo.zdbjq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gnf.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vhc.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xwy.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zxi.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mxr.xylfe.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wse.pycfn.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://opm.daxiang520.top

[I04] 正则替换
来源：http://exj.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://qod.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ckt.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://vhm.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://dui.316326.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://roz.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://esu.hesvh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ler.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ybo.jqgufenzy.top

[I05] 按正则拆分
来源：http://cfe.yuxming.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://het.jiagoushi.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lzm.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://bbk.cucudq.cn

TS:   s.split(/\s*,\s*/)
来源：http://aij.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://ltf.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jmq.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://luj.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jbl.quarkkingdee.top


<!-- 参考信息 -->