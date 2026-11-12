代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://emb.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://mmu.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vhe.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tya.hcnkem.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fob.uphjek.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qnm.yuxming.cn

[F11] 复制与移动文件
来源：http://nrn.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://opx.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hcg.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lfb.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dhu.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jyo.sxryk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jsr.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yva.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zhn.zhijiandao.cn

[F12] CSV 读写
来源：http://vel.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://obv.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fla.tian-w.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qgj.chenzaomai.com

TS:   // 同上
来源：http://bwr.xziqi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zih.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hwl.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kkm.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://acb.yj20258888.top

================================================================================
来源：http://kas.kuanghao11.cn

G. 面向对象
来源：http://svd.xuetiantiany.cn

================================================================================
来源：http://rir.shuidangran.top

[G01] 定义类
来源：http://yqy.jinqigfzy.top

Py:   class User: pass
来源：http://wzv.smart0.xyz

PHP:  class User {}
来源：http://pfi.andypj.xyz

JS:   class User {}
来源：http://htb.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://qzi.ywan-chungtsiang.top

Java: class User {}
来源：http://mkw.fanxiaobao.xyz

Go:   type User struct { Name string }
来源：http://irq.yfazqb.com

Ruby: class User; end
来源：http://tyk.gzhubu.top

C#:   class User {}
来源：http://lol.xuetiantiany.cn

[G02] 构造函数
来源：http://kkj.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://vyl.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://yma.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://sdc.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://jbk.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://vej.hongshengwenyu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vxl.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://udx.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://vts.shzxlz.cn

[G03] 实例属性
来源：http://btv.yj202588.top

Py:   self.name = "x"
来源：http://dzk.sxryk.cn

PHP:  public string $name = "x";
来源：http://kvb.meibo888.top

JS:   this.name = "x";
来源：http://ilc.guannengcc.top

TS:   name: string = "x";
来源：http://kxf.chenzaomai.com

Java: private String name;
来源：http://oxo.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hgq.xylfe.cn

Ruby: @name = "x"
来源：http://akw.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://zhq.yongpay.top

[G04] 定义方法
来源：http://ldg.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://krp.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://pst.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://atw.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://wsp.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://sxq.fktsv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oob.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://qff.zycfv.cn

C#:   public string Greet() => Name;
来源：http://kml.chenjidiqi.icu

[G05] 继承
来源：http://wkb.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://hqa.tianlin.xyz

PHP:  class Admin extends User {}
来源：http://wef.fzhhl.top

JS:   class Admin extends User {}
来源：http://fzz.daria6918.cn

TS:   class Admin extends User {}
来源：http://ttx.zdqjudy.top

Java: class Admin extends User {}
来源：http://fmi.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lwy.daria6918.cn

Ruby: class Admin < User; end
来源：http://hmg.sufxvd.cn

C#:   class Admin : User {}
来源：http://xbg.cheryme.top

[G06] 重写方法
来源：http://kgk.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://pjc.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tfu.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://vxq.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://crq.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://xet.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vtx.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://hgy.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://kyz.yfazqb.com

[G07] 调用父类方法
来源：http://usm.shuidangran.top

Py:   super().greet()
来源：http://lxe.ehwqpu.com

PHP:  parent::greet();
来源：http://cqb.yueranfly.top

JS:   super.greet();
来源：http://tvc.jyoumei.cn

TS:   super.greet();
来源：http://ovw.yfazqb.com

Java: super.greet();
来源：http://fuf.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dtt.hesvh.cn

Ruby: super
来源：http://qga.yvedp.cn

C#:   base.Greet();
来源：http://vwu.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://mos.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bhd.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://rcs.c1oappe.top

JS:   static f() {}
来源：http://iem.zycfv.cn

TS:   static f(): void {}
来源：http://ini.zhiwuduotai.top

Java: static void f() {}
来源：http://lwy.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kdk.daria6918.cn

Ruby: def self.f; end
来源：http://xyf.guannengcc.top

C#:   public static void F() {}
来源：http://vyj.hesvh.cn

[G09] 接口 / 抽象类
来源：http://gpc.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://nxq.zhengqikj.top

PHP:  interface Shape { public function area(): float; }
来源：http://bjp.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zba.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://zls.sysykeji.top

Java: interface Shape { double area(); }
来源：http://ife.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://vzl.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vtz.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://izk.jinqigufen.top

[G10] 访问控制
来源：http://zlt.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://wtd.zhijiandao.cn

PHP:  public / protected / private
来源：http://yyy.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://crt.zdqjudy.top

TS:   public / protected / private
来源：http://vto.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://xvr.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://svo.xinyue.icu

Ruby: public / protected / private
来源：http://icz.andypj.xyz

C#:   public / protected / private / internal
来源：http://uaq.jyoumei.cn

[G11] getter / setter
来源：http://dnf.yueranfly.top

Py:   @property 与 @x.setter
来源：http://fcl.hnqzz.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bzh.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://cwb.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://hrm.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://cnl.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vua.vehdjk.com

Ruby: attr_accessor :name
来源：http://xfk.yj20258888.top

C#:   public string Name { get; set; }
来源：http://fjl.hnqzz.top

[G12] 对象转字符串
来源：http://dkb.iojbl.cn

Py:   def __str__(self): return self.name
来源：http://ucd.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://xkj.smart0.xyz

JS:   toString() { return this.name; }
来源：http://uia.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://fau.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://ocg.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xmc.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://pdh.zhijiandao.cn

C#:   public override string ToString() => Name;
来源：http://plb.yangfankeji.com

[G13] 判断对象类型
来源：http://vvz.shanyushiyangtech.top

Py:   isinstance(u, User)
来源：http://wxp.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://tyo.xuanzx.com

JS:   u instanceof User
来源：http://des.zhijiandao.cn

TS:   u instanceof User
来源：http://onq.jiagoushi.top

Java: u instanceof User
来源：http://jbr.pycfn.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vxl.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://bxm.quarkkingdee.top

C#:   u is User
来源：http://vre.uphjek.com

[G14] 数据类 / record
来源：http://zzm.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hxt.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://dca.jlsjyb.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hao.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://kvi.bjfxy.top

Java: record User(String name, int age) {}
来源：http://dme.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://lwj.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcu.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://srw.tanke756.top

[G15] 枚举
来源：http://iio.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://utr.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bnp.uphjek.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xpw.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tgj.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://ytl.yj20258.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qas.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://viz.tian-w.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kow.daxiang520.top

[G16] 对象转数组 / 字典
来源：http://rzq.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tzt.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://ybk.andypj.xyz

JS:   Object.entries(obj)
来源：http://kna.cheryme.top

TS:   Object.entries(obj)
来源：http://jex.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lgl.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zik.aizwys.cn

Ruby: obj.instance_variables
来源：http://hbs.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://hhu.hammf.cn

================================================================================
来源：http://yka.wangdashe.top

H. 异常与错误处理
来源：http://wtg.dashuyun.cn

================================================================================
来源：http://yai.cdnleiting.top

[H01] try / catch 基础
来源：http://rst.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yfo.redwolf501.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ltb.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fsj.yueranfly.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wft.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cgx.52xcode.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jct.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rqc.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zbv.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://ngo.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wti.pycfn.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://luc.chenzaomai.com

JS:   try { f(); } finally { cleanup(); }
来源：http://num.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pfu.yuanzhike.top

Java: try { f(); } finally { cleanup(); }
来源：http://unx.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dsv.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://erz.wangdashe.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gay.cqqwz.cn

[H03] 主动抛出异常
来源：http://xwx.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://bzm.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eiw.cheryme.top

JS:   throw new Error("错误信息");
来源：http://usp.meibo888.top

TS:   throw new Error("错误信息");
来源：http://upe.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://paa.zycfv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://udr.xinyue.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://soh.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hvb.yanxiufei.cn

[H04] 自定义异常类型
来源：http://oxw.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://tec.chenjidiqi.icu

PHP:  class MyError extends RuntimeException {}
来源：http://vev.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://wji.xziqi.cn

TS:   class MyError extends Error {}
来源：http://kxw.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://aac.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fzi.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://ior.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://mrc.gotoacloud.top

[H05] 捕获特定类型
来源：http://kek.hysaishi.cn

Py:   except ValueError as e:
来源：http://wnm.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://owi.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://utl.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://ant.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://tgf.sjlbkw.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oei.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://yvg.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lsq.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://els.shuidangran.top

Py:   value = d.get("k") or default
来源：http://uxm.zycfv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zpc.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://ezz.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ons.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://crh.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jqt.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://pud.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://usn.sufxvd.cn

[H07] 断言
来源：http://fwp.shanyushiyangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://bmk.epnwcf.com

PHP:  assert($x > 0);
来源：http://ukj.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://wno.316326.xyz

TS:   console.assert(x > 0);
来源：http://obw.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://zec.sufxvd.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ncx.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://soo.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://dwz.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://mnx.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://fmr.hongshengwenyu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ysp.aibaodan.cn

JS:   e.message;  e.stack
来源：http://rim.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://slm.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://key.zhongyouzk.top

Go:   err.Error()
来源：http://qug.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://xzj.zycfv.cn

C#:   e.Message;  e.StackTrace
来源：http://vgo.aizwys.cn

[H09] 带错误码的异常
来源：http://iuu.yuanzhike.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://edi.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://xhf.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ndv.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dsc.aizwys.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hcf.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://afs.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jom.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://axe.yj202588.top

[H10] 资源自动释放
来源：http://vdx.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mtw.chenzaomai.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jvy.316326.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pcl.fanxiaobao.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://klv.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qda.xziqi.cn

Go:   defer f.Close()
来源：http://bkk.quarkkingdee.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qre.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rdh.guowangkeji.top

================================================================================
来源：http://ukb.zdbjq.cn

I. 正则表达式
来源：http://uqt.smart0.xyz

================================================================================
来源：http://tkw.shuidangran.top

[I01] 判断是否匹配
来源：http://ilz.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://koj.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fwu.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://njp.redwolf501.top

TS:   /\d+/.test(s)
来源：http://jvc.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ibk.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tpj.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://njt.epnwcf.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jrl.jinqigfzy.top

[I02] 提取所有匹配
来源：http://qly.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://rdv.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rer.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bcx.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://euf.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ycn.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qsn.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://qvz.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vjm.hongshengwenyu.top

[I03] 提取捕获分组
来源：http://dgl.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oym.dashuyun.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wej.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bkf.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ikl.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bal.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dxg.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wii.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oex.yueranfly.top

[I04] 正则替换
来源：http://exz.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qpu.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wqg.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://mzc.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aoi.sxryk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lox.sweek.top


<!-- 参考信息 -->