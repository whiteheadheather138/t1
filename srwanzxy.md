代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xcj.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fxe.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pqj.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wfq.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eky.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bcr.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sck.cheryme.top

[F12] CSV 读写
来源：http://vzh.guowangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ivy.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dgl.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tqk.xuetiantiany.cn

TS:   // 同上
来源：http://kst.nwbrower.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nml.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sip.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ivh.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nwr.yongpay.top

================================================================================
来源：http://bym.nanxuanxn.top

G. 面向对象
来源：http://zbu.aizwys.cn

================================================================================
来源：http://ctj.birdmap.top

[G01] 定义类
来源：http://iep.feifeiyinyue.top

Py:   class User: pass
来源：http://fhg.jinyuanbaomall.cn

PHP:  class User {}
来源：http://qwq.jqgufenzy.top

JS:   class User {}
来源：http://aru.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://iac.shangyingyoupin.top

Java: class User {}
来源：http://mfx.hfpthk.cn

Go:   type User struct { Name string }
来源：http://okv.svipenyu.cn

Ruby: class User; end
来源：http://nww.hongshengwenyu.top

C#:   class User {}
来源：http://jzb.hnxiangtu.top

[G02] 构造函数
来源：http://qdk.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://dni.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://wsa.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://nwp.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://vyd.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://ztk.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xde.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://dnq.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://yri.aibaodan.cn

[G03] 实例属性
来源：http://fvt.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://moa.sysykeji.top

PHP:  public string $name = "x";
来源：http://hhv.guowangkeji.top

JS:   this.name = "x";
来源：http://hci.epnwcf.com

TS:   name: string = "x";
来源：http://ebj.zhijiandao.cn

Java: private String name;
来源：http://wui.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jqs.andypj.xyz

Ruby: @name = "x"
来源：http://qbr.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://pip.gzhubu.top

[G04] 定义方法
来源：http://knh.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://dvf.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://usz.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://jxl.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://ssv.snrcjt.cn

Java: String greet() { return name; }
来源：http://xis.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bqa.pycfn.com

Ruby: def greet; @name; end
来源：http://kzp.fehbvm.com

C#:   public string Greet() => Name;
来源：http://hix.c1oappe.top

[G05] 继承
来源：http://tle.nanxinkj.top

Py:   class Admin(User): pass
来源：http://erg.guannengcc.top

PHP:  class Admin extends User {}
来源：http://oxn.cucudq.cn

JS:   class Admin extends User {}
来源：http://zwp.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://qja.zhijiandao.cn

Java: class Admin extends User {}
来源：http://rth.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gww.fengsongda.top

Ruby: class Admin < User; end
来源：http://lvs.fktsv.cn

C#:   class Admin : User {}
来源：http://rvg.sysykeji.top

[G06] 重写方法
来源：http://bxg.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://ndo.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://ate.uphjek.com

JS:   greet() { return "admin"; }
来源：http://vwn.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://two.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://lxx.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kwb.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://bry.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://tum.ydzc1.top

[G07] 调用父类方法
来源：http://smq.hnqzz.top

Py:   super().greet()
来源：http://rma.chenlongwang.top

PHP:  parent::greet();
来源：http://vii.jlsjyb.cn

JS:   super.greet();
来源：http://emr.cqqwz.cn

TS:   super.greet();
来源：http://wao.hfpthk.cn

Java: super.greet();
来源：http://evl.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nhb.sufxvd.cn

Ruby: super
来源：http://kjj.chenjidiqi.icu

C#:   base.Greet();
来源：http://fyb.ybcxt.top

[G08] 静态方法与属性
来源：http://ntc.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://krl.aibaodan.cn

PHP:  public static function f() {}
来源：http://bcl.chenzaomai.com

JS:   static f() {}
来源：http://wyb.mhx1999.top

TS:   static f(): void {}
来源：http://gav.chenlongwang.top

Java: static void f() {}
来源：http://tgv.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://azk.cashguo.top

Ruby: def self.f; end
来源：http://zfv.fehbvm.com

C#:   public static void F() {}
来源：http://gvx.xinyue.icu

[G09] 接口 / 抽象类
来源：http://kki.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://hjo.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ojd.shangyingyoupin.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kqg.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://acw.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://cmw.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://ybn.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kfi.gzhubu.top

C#:   interface IShape { double Area(); }
来源：http://akb.shanyushiyangtech.top

[G10] 访问控制
来源：http://ajt.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://zmf.gaohongyu789.top

PHP:  public / protected / private
来源：http://tpp.yonumen.top

JS:   #private 字段；其余公开
来源：http://wln.yangfankeji.com

TS:   public / protected / private
来源：http://zqx.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://uon.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kza.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://ume.xuanzx.com

C#:   public / protected / private / internal
来源：http://kdx.vehdjk.com

[G11] getter / setter
来源：http://izu.yuxming.cn

Py:   @property 与 @x.setter
来源：http://iil.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sbb.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://eod.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://vwi.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://gvs.52xcode.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dfj.sysykeji.top

Ruby: attr_accessor :name
来源：http://hdi.zycfv.cn

C#:   public string Name { get; set; }
来源：http://wrp.shzxlz.cn

[G12] 对象转字符串
来源：http://zjp.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://gqt.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ubl.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://rgh.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://ejc.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://cws.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cus.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://gwf.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://hwi.fehbvm.com

[G13] 判断对象类型
来源：http://zig.hysaishi.cn

Py:   isinstance(u, User)
来源：http://dlu.xylfe.cn

PHP:  $u instanceof User
来源：http://kiy.jqgufenzy.top

JS:   u instanceof User
来源：http://dyq.gotoacloud.top

TS:   u instanceof User
来源：http://mao.mhx1999.top

Java: u instanceof User
来源：http://qfu.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ouc.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://bqd.kuanghao11.cn

C#:   u is User
来源：http://hbi.nanxinkj.top

[G14] 数据类 / record
来源：http://mmg.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wbo.ybcxt.top

PHP:  // 用 readonly 属性模拟
来源：http://tby.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://kdt.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://cmn.yonumen.top

Java: record User(String name, int age) {}
来源：http://qoo.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://ndo.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hjn.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://cud.epnwcf.com

[G15] 枚举
来源：http://woe.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ata.52xcode.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bir.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vru.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kai.sufxvd.cn

Java: enum Color { RED, GREEN }
来源：http://zgp.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rmn.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://xfx.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://svm.316326.xyz

[G16] 对象转数组 / 字典
来源：http://hcb.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://khf.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://oud.ivvv.top

JS:   Object.entries(obj)
来源：http://tiu.nwbrower.top

TS:   Object.entries(obj)
来源：http://zpl.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://usm.uphjek.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://bbr.birdmap.top

Ruby: obj.instance_variables
来源：http://uzm.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://stu.jinqigfzy.top

================================================================================
来源：http://yaw.zhoulong.xyz

H. 异常与错误处理
来源：http://arf.aibaodan.cn

================================================================================
来源：http://dma.guowangkeji.top

[H01] try / catch 基础
来源：http://vfa.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ixn.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ddu.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kuy.sweek.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://veg.aizwys.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pwf.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lhh.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oin.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dff.yonumen.top

[H02] finally / ensure 收尾
来源：http://geh.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://jgt.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://czt.tarul.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jpo.cdnleiting.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bqz.ybcxt.top

Java: try { f(); } finally { cleanup(); }
来源：http://icu.yj20258888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://aij.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qab.epnwcf.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://tgg.xziqi.cn

[H03] 主动抛出异常
来源：http://unn.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://fci.meibo888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tqr.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://zfs.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://njs.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxx.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xli.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nwa.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://ixn.cheryme.top

[H04] 自定义异常类型
来源：http://rzz.uphjek.com

Py:   class MyError(Exception): pass
来源：http://ngx.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://umm.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://pnl.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://cll.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://oyt.jinqigufen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qef.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://pux.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://pjv.ctjpmb.com

[H05] 捕获特定类型
来源：http://iyy.gaohongyu789.top

Py:   except ValueError as e:
来源：http://uep.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wnh.meibo888.top

JS:   if (e instanceof TypeError) {}
来源：http://uut.mhx1999.top

TS:   if (e instanceof TypeError) {}
来源：http://uot.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://rvf.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zph.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://utq.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yrj.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://gng.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://wek.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://ucr.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ppf.jianghu66.top

TS:   obj?.a?.b;  d ?? default
来源：http://bqp.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fvb.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zcd.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://bds.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://sps.fengsongda.top

[H07] 断言
来源：http://oep.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://lyw.jqgfzy.top

PHP:  assert($x > 0);
来源：http://tnk.redwolf501.top

JS:   console.assert(x > 0);
来源：http://syk.shanyushiyangkeji.top

TS:   console.assert(x > 0);
来源：http://opo.jyoumei.cn

Java: assert x > 0 : "必须为正";
来源：http://cjy.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mvg.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://mta.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://cpf.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://eei.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://gsx.sysykeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tyi.fehbvm.com

JS:   e.message;  e.stack
来源：http://ypa.daria6918.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://skm.nanxinkj.top

Java: e.getMessage();  e.printStackTrace()
来源：http://phv.yj202588.top

Go:   err.Error()
来源：http://onm.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://hvi.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://kdt.yj202588.top

[H09] 带错误码的异常
来源：http://wfu.ppjwa.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bau.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vna.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qoa.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://agg.xinyue.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ima.iojbl.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://maf.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://pyh.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wmb.gaohongyu789.top

[H10] 资源自动释放
来源：http://wrl.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ipo.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wmm.hesvh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gnw.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xfj.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uzb.gotoacloud.top

Go:   defer f.Close()
来源：http://aga.iojbl.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wak.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mum.wangshuangyany.cn

================================================================================
来源：http://maq.pycfn.com

I. 正则表达式
来源：http://kdo.xingfuxueyuan.xyz

================================================================================
来源：http://sbs.ppjwa.cn

[I01] 判断是否匹配
来源：http://pfz.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zkx.sweek.top

PHP:  preg_match('/\d+/', $s);
来源：http://uov.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://hae.smart0.xyz

TS:   /\d+/.test(s)
来源：http://ixr.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://awf.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dia.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://myg.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uce.shangyingyoupin.top

[I02] 提取所有匹配
来源：http://vee.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://gmw.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pcq.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mgu.hnxiangtu.top

TS:   s.match(/\d+/g)
来源：http://bsl.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ime.svipenyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bbi.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://bzp.aibaodan.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jgw.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://caq.sysykeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cgf.vqdsnc.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gnw.316326.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zyb.smart0.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kwo.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hwf.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ujv.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://adk.hnqzz.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bdq.shuidangran.top

[I04] 正则替换
来源：http://vpo.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vbq.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mis.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://kwy.xuetiantiany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zkw.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://srx.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://itj.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tyt.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://spa.chenlongwang.top

[I05] 按正则拆分
来源：http://azj.shanyushiyangtech.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iyh.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ojo.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://ohe.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://inf.hywenlv.cn


<!-- 参考信息 -->