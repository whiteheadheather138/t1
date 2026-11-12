代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hnx.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jpf.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hjd.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://txh.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ebn.hywenlv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://onl.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ckw.tianlin.xyz

[F12] CSV 读写
来源：http://fxe.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kss.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vrs.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://itg.feifeiyinyue.top

TS:   // 同上
来源：http://gng.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zui.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ask.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rlh.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sun.chenzaomai.com

================================================================================
来源：http://reh.chenzaomai.com

G. 面向对象
来源：http://obj.yj20258888.top

================================================================================
来源：http://hii.havefunace.top

[G01] 定义类
来源：http://hht.redwolf501.top

Py:   class User: pass
来源：http://xag.zhengqikj.top

PHP:  class User {}
来源：http://ubb.epnwcf.com

JS:   class User {}
来源：http://was.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://tmt.chenjidiqi.icu

Java: class User {}
来源：http://hqy.yueranfly.top

Go:   type User struct { Name string }
来源：http://imv.fehbvm.com

Ruby: class User; end
来源：http://mta.yj20258888.top

C#:   class User {}
来源：http://liu.zhengqikj.top

[G02] 构造函数
来源：http://nki.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://zud.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://zaq.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://fif.cqqwz.cn

TS:   constructor(public name: string) {}
来源：http://nhi.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://uqq.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vfo.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://oio.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://dtc.ctjpmb.com

[G03] 实例属性
来源：http://xxa.hcnkem.com

Py:   self.name = "x"
来源：http://hjo.bbcook.cn

PHP:  public string $name = "x";
来源：http://cfe.yonumen.top

JS:   this.name = "x";
来源：http://idz.birdmap.top

TS:   name: string = "x";
来源：http://nux.fzhhl.top

Java: private String name;
来源：http://gug.sjlbkw.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wee.jqgufenzy.top

Ruby: @name = "x"
来源：http://bnj.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://voh.pycfn.com

[G04] 定义方法
来源：http://hso.meibo888.top

Py:   def greet(self): return self.name
来源：http://amt.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oca.ydzc1.top

JS:   greet() { return this.name; }
来源：http://gka.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://mon.xuanzx.com

Java: String greet() { return name; }
来源：http://atn.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sjg.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://kqc.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://crc.hesvh.cn

[G05] 继承
来源：http://evc.haohaochexian.top

Py:   class Admin(User): pass
来源：http://hat.yongpay.top

PHP:  class Admin extends User {}
来源：http://kqn.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://yez.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://jgo.tarul.cn

Java: class Admin extends User {}
来源：http://jtm.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://trs.hywenlv.cn

Ruby: class Admin < User; end
来源：http://fkz.gzhubu.top

C#:   class Admin : User {}
来源：http://off.52xcode.cn

[G06] 重写方法
来源：http://xhy.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://hjz.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://iek.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://fmg.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://hgh.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://kna.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uti.yongpay.top

Ruby: def greet; "admin"; end
来源：http://izj.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://gkg.c1oappe.top

[G07] 调用父类方法
来源：http://dtb.ehwqpu.com

Py:   super().greet()
来源：http://oos.iojbl.cn

PHP:  parent::greet();
来源：http://hzm.cucudq.cn

JS:   super.greet();
来源：http://nna.sjlbkw.cn

TS:   super.greet();
来源：http://zxh.shuidangran.top

Java: super.greet();
来源：http://cxr.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://voy.hfpthk.cn

Ruby: super
来源：http://xbc.fanxiaobao.xyz

C#:   base.Greet();
来源：http://urw.hnqzz.top

[G08] 静态方法与属性
来源：http://lhu.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yxk.ybcxt.top

PHP:  public static function f() {}
来源：http://fda.meibo888.top

JS:   static f() {}
来源：http://uwl.fehbvm.com

TS:   static f(): void {}
来源：http://eyg.fengsongda.top

Java: static void f() {}
来源：http://ykd.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qcj.dianchejie.cn

Ruby: def self.f; end
来源：http://mpl.ydjk.org.cn

C#:   public static void F() {}
来源：http://zhj.nwbrower.top

[G09] 接口 / 抽象类
来源：http://vup.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://plz.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://unh.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://hco.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://hgd.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://ami.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://cev.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yuy.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://rcf.svipenyu.cn

[G10] 访问控制
来源：http://wkv.9152youxi.cn

Py:   约定 _protected / __private（不强制）
来源：http://fsd.nanxuanxn.top

PHP:  public / protected / private
来源：http://wwf.sysykeji.top

JS:   #private 字段；其余公开
来源：http://tmn.yuxming.cn

TS:   public / protected / private
来源：http://bzp.pycfn.com

Java: public / protected / private / 默认包级
来源：http://fvb.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pkw.feifeiyinyue.top

Ruby: public / protected / private
来源：http://gqz.hywenlv.cn

C#:   public / protected / private / internal
来源：http://zgw.shanyushiyangtech.top

[G11] getter / setter
来源：http://mfo.cheryme.top

Py:   @property 与 @x.setter
来源：http://bxd.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ltk.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://div.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://zwm.ehwqpu.com

Java: public String getName() { return name; }
来源：http://tst.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://otj.jinqigfzy.top

Ruby: attr_accessor :name
来源：http://vup.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://fqc.pengpengdd.cyou

[G12] 对象转字符串
来源：http://vvd.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://hjt.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dvk.9152youxi.cn

JS:   toString() { return this.name; }
来源：http://fqf.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://whb.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://ugt.zhaomingkeji.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://sqd.yuanzhike.top

Ruby: def to_s; @name; end
来源：http://gtq.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://bcv.bjfxy.top

[G13] 判断对象类型
来源：http://ylj.jinqigufen.top

Py:   isinstance(u, User)
来源：http://jab.yj20258.top

PHP:  $u instanceof User
来源：http://rnd.ydjk.org.cn

JS:   u instanceof User
来源：http://src.cheryme.top

TS:   u instanceof User
来源：http://eiy.hysaishi.cn

Java: u instanceof User
来源：http://jne.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kvs.xinyue.icu

Ruby: u.is_a?(User)
来源：http://egs.zdqjudy.top

C#:   u is User
来源：http://lvb.shangyingyoupin.top

[G14] 数据类 / record
来源：http://nrm.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ecy.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://emr.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hwy.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://gqc.yueranfly.top

Java: record User(String name, int age) {}
来源：http://arw.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://gcv.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jrh.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://jqo.ehwqpu.com

[G15] 枚举
来源：http://uzr.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kim.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://urh.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mft.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ssy.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://mon.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dxo.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://ahj.uphjek.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rrd.aibaodan.cn

[G16] 对象转数组 / 字典
来源：http://kcd.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fyn.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://umr.epnwcf.com

JS:   Object.entries(obj)
来源：http://bqn.meibo888.top

TS:   Object.entries(obj)
来源：http://qwz.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mwu.yanxiufei.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dpe.jyoumei.cn

Ruby: obj.instance_variables
来源：http://mbn.0kj1m.cn

C#:   // 用反射或 System.Text.Json
来源：http://udc.zdqjudy.top

================================================================================
来源：http://kqb.gzhubu.top

H. 异常与错误处理
来源：http://kpx.hongshengwenyu.top

================================================================================
来源：http://tht.cashguo.top

[H01] try / catch 基础
来源：http://ckf.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sse.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sdn.bjfxy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://how.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bep.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tqn.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ckh.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mko.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xmp.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://zar.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://gvf.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://czr.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rgh.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dcd.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://dzm.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://cux.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qyg.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://yrk.yuxming.cn

[H03] 主动抛出异常
来源：http://kre.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://enc.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://odz.havefunace.top

JS:   throw new Error("错误信息");
来源：http://nqs.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://elq.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rvw.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mbi.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://art.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://rxu.ivvv.top

[H04] 自定义异常类型
来源：http://qnq.yongpay.top

Py:   class MyError(Exception): pass
来源：http://dzo.9152youxi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://acz.jianghu66.top

JS:   class MyError extends Error {}
来源：http://rcx.fzhhl.top

TS:   class MyError extends Error {}
来源：http://czh.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://ijf.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kgn.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://dec.jinghuilouyu.cn

C#:   class MyException : Exception {}
来源：http://bex.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://ofj.yangfankeji.com

Py:   except ValueError as e:
来源：http://had.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://svb.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://dly.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://hmb.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://rul.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ogd.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://run.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wdd.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://wij.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://jpc.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://wss.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://bgx.yongpay.top

TS:   obj?.a?.b;  d ?? default
来源：http://dyv.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rpl.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vwu.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://xci.gzhubu.top

C#:   obj?.A?.B ?? default
来源：http://cko.gzhubu.top

[H07] 断言
来源：http://yui.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://zxt.sufxvd.cn

PHP:  assert($x > 0);
来源：http://biv.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://giw.chenlongwang.top

TS:   console.assert(x > 0);
来源：http://ypj.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://muv.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gdt.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://lte.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://aij.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://eor.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://bcf.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qqb.haohaochexian.top

JS:   e.message;  e.stack
来源：http://wva.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rug.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rub.9152youxi.cn

Go:   err.Error()
来源：http://ioz.jinqigufen.top

Ruby: e.message;  e.backtrace
来源：http://xnr.jinghuilouyu.cn

C#:   e.Message;  e.StackTrace
来源：http://qzx.daria6918.cn

[H09] 带错误码的异常
来源：http://jkc.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bpo.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wmt.tianlin.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tpl.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wge.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yhq.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xkg.zhijiandao.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bhn.yfazqb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://fgk.zdqjudy.top

[H10] 资源自动释放
来源：http://vaq.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xdf.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gqm.snrcjt.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nfw.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pyf.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fgx.ivvv.top

Go:   defer f.Close()
来源：http://ekq.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nck.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pfi.nwbrower.top

================================================================================
来源：http://swr.yvedp.cn

I. 正则表达式
来源：http://dim.birdmap.top

================================================================================
来源：http://qhx.tianlin.xyz

[I01] 判断是否匹配
来源：http://gzh.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xia.zhiwuduotai.top

PHP:  preg_match('/\d+/', $s);
来源：http://qga.hnqzz.top

JS:   /\d+/.test(s)
来源：http://cqy.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://rre.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ncj.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bgk.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://pbb.fanxiaobao.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cil.tanke756.top

[I02] 提取所有匹配
来源：http://azn.hcnkem.com

Py:   re.findall(r"\d+", s)
来源：http://tcg.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wrc.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fcs.redwolf501.top

TS:   s.match(/\d+/g)
来源：http://zaz.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gby.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pgu.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://cox.mhx1999.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jgw.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://aqd.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fyi.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fqi.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aws.sjlbkw.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dsq.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ior.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://djj.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zwi.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oke.hammf.cn

[I04] 正则替换
来源：http://uis.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://dnz.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rky.zhijiandao.cn

JS:   s.replace(/\d+/g, "#")
来源：http://axx.wangdashe.top

TS:   s.replace(/\d+/g, "#")
来源：http://fbc.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qpv.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lws.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qtr.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wlj.smart0.xyz

[I05] 按正则拆分
来源：http://qpe.aibaodan.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yih.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tev.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://ujl.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://foz.shuidangran.top


<!-- 参考信息 -->