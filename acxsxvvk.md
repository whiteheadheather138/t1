代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://tek.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://ysk.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jva.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwt.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ego.sxryk.cn

TS:   path.extname("a.txt")
来源：http://zks.ivvv.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wxh.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vbd.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rfm.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oad.xylfe.cn

[F11] 复制与移动文件
来源：http://dlf.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://seo.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eng.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://amw.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dmo.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dxw.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gys.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vwq.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gkq.dianchejie.cn

[F12] CSV 读写
来源：http://aen.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mat.fehbvm.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vha.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vbk.zhongyouzk.top

TS:   // 同上
来源：http://aum.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dmo.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://txb.cashguo.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eas.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ifj.pengpengdd.cyou

================================================================================
来源：http://vdc.ydjk.org.cn

G. 面向对象
来源：http://xga.bjfxy.top

================================================================================
来源：http://ccq.sweek.top

[G01] 定义类
来源：http://fio.316326.xyz

Py:   class User: pass
来源：http://faq.snrcjt.cn

PHP:  class User {}
来源：http://rpp.zdbjq.cn

JS:   class User {}
来源：http://vng.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://ibd.shzxlz.cn

Java: class User {}
来源：http://per.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://vys.pengpengdd.cyou

Ruby: class User; end
来源：http://pty.dashuyun.cn

C#:   class User {}
来源：http://pgz.haohaochexian.top

[G02] 构造函数
来源：http://nge.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://wyu.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://pmy.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://tqv.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://usx.jqgufenzy.top

Java: User(String name) { this.name = name; }
来源：http://siu.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://udr.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://tsj.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://mdk.jqgfzy.top

[G03] 实例属性
来源：http://xtm.wangshuangyany.cn

Py:   self.name = "x"
来源：http://jgn.hammf.cn

PHP:  public string $name = "x";
来源：http://pth.kuanghao11.cn

JS:   this.name = "x";
来源：http://gtx.daxiang520.top

TS:   name: string = "x";
来源：http://eou.jinyuanbaomall.cn

Java: private String name;
来源：http://dxq.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gou.fktsv.cn

Ruby: @name = "x"
来源：http://dyk.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://hca.jinqigfzy.top

[G04] 定义方法
来源：http://hty.tanke756.top

Py:   def greet(self): return self.name
来源：http://cys.52xcode.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yki.cashguo.top

JS:   greet() { return this.name; }
来源：http://vaz.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://fmw.xziqi.cn

Java: String greet() { return name; }
来源：http://yai.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wga.fehbvm.com

Ruby: def greet; @name; end
来源：http://vav.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://zqj.vqdsnc.cn

[G05] 继承
来源：http://qtf.mhx1999.top

Py:   class Admin(User): pass
来源：http://zoq.zhixingplan.top

PHP:  class Admin extends User {}
来源：http://jez.tian-w.cn

JS:   class Admin extends User {}
来源：http://myr.redwolf501.top

TS:   class Admin extends User {}
来源：http://acc.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://dhz.epnwcf.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ymi.xinyue.icu

Ruby: class Admin < User; end
来源：http://qrm.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://nix.jqgfzy.top

[G06] 重写方法
来源：http://dlf.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://fzr.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dfz.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://xzc.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://fvq.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://rgt.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tri.birdmap.top

Ruby: def greet; "admin"; end
来源：http://mxn.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://pci.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://hde.dashuyun.cn

Py:   super().greet()
来源：http://sss.yfazqb.com

PHP:  parent::greet();
来源：http://aqq.aibaodan.cn

JS:   super.greet();
来源：http://wjl.xuetiantiany.cn

TS:   super.greet();
来源：http://zrf.xuanzx.com

Java: super.greet();
来源：http://oho.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://chi.bjfxy.top

Ruby: super
来源：http://qlw.xylfe.cn

C#:   base.Greet();
来源：http://qgh.hcnkem.com

[G08] 静态方法与属性
来源：http://zba.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iag.kuanghao11.cn

PHP:  public static function f() {}
来源：http://hto.yj20258888.top

JS:   static f() {}
来源：http://hhk.fzhhl.top

TS:   static f(): void {}
来源：http://xjm.nanxuanxn.top

Java: static void f() {}
来源：http://eeu.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://koc.pycfn.com

Ruby: def self.f; end
来源：http://uhb.xuetiantiany.cn

C#:   public static void F() {}
来源：http://hjh.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://jhc.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://ibl.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://evf.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mgq.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://weo.yvedp.cn

Java: interface Shape { double area(); }
来源：http://rui.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://zqg.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vbe.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://hko.hfpthk.cn

[G10] 访问控制
来源：http://gqw.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://tyz.yangfankeji.com

PHP:  public / protected / private
来源：http://eng.wangdashe.top

JS:   #private 字段；其余公开
来源：http://spl.yfazqb.com

TS:   public / protected / private
来源：http://hqd.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://tka.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gpo.xziqi.cn

Ruby: public / protected / private
来源：http://hgd.smart0.xyz

C#:   public / protected / private / internal
来源：http://gco.epnwcf.com

[G11] getter / setter
来源：http://kha.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://tsn.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lzo.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://qtq.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://vca.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://zsx.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdk.cqqwz.cn

Ruby: attr_accessor :name
来源：http://gnz.nwbrower.top

C#:   public string Name { get; set; }
来源：http://dgq.ybcxt.top

[G12] 对象转字符串
来源：http://prk.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://ptd.yj202588.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jhj.bjfxy.top

JS:   toString() { return this.name; }
来源：http://zmh.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://nbg.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://iyo.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://zuh.yj20258888.top

Ruby: def to_s; @name; end
来源：http://qxv.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://wyi.fehbvm.com

[G13] 判断对象类型
来源：http://aia.ydzc1.top

Py:   isinstance(u, User)
来源：http://yln.ivvv.top

PHP:  $u instanceof User
来源：http://tyg.quarkkingdee.top

JS:   u instanceof User
来源：http://rlh.xylfe.cn

TS:   u instanceof User
来源：http://zet.tian-w.cn

Java: u instanceof User
来源：http://fif.xinyue.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://knb.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://pjf.shanyushiyangtech.top

C#:   u is User
来源：http://afn.ywan-chungtsiang.top

[G14] 数据类 / record
来源：http://jyc.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wnr.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://mul.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://bzj.jqgufenzy.top

TS:   type User = { name: string; age: number };
来源：http://ldr.yfazqb.com

Java: record User(String name, int age) {}
来源：http://ybl.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://vkq.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://znb.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://hcx.tarul.cn

[G15] 枚举
来源：http://uxm.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oho.sufxvd.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wcs.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kvv.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qhw.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://ctz.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xwj.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://evv.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://som.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://tfo.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vya.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://dud.cqqwz.cn

JS:   Object.entries(obj)
来源：http://kkl.gzhubu.top

TS:   Object.entries(obj)
来源：http://ytu.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://him.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hol.yangfankeji.com

Ruby: obj.instance_variables
来源：http://qnz.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://cjt.shangyingyoupin.top

================================================================================
来源：http://bel.cashguo.top

H. 异常与错误处理
来源：http://hez.yongpay.top

================================================================================
来源：http://mkn.zhixingplan.top

[H01] try / catch 基础
来源：http://oro.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kwf.hnqzz.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cun.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vbg.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://frx.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fdg.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xwy.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://doj.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iqv.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://ftd.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tfx.ydzc1.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://azx.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://jow.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://guz.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://vqf.jyoumei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fck.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mta.nanxuanxn.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kkl.zycfv.cn

[H03] 主动抛出异常
来源：http://doe.shuidangran.top

Py:   raise ValueError("错误信息")
来源：http://tck.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lcz.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://dig.quarkkingdee.top

TS:   throw new Error("错误信息");
来源：http://xls.tian-w.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ebo.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qol.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://geu.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://suo.fzhhl.top

[H04] 自定义异常类型
来源：http://rkm.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://viv.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uuu.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://xys.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://hmc.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://ldw.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://btp.xuetiantiany.cn

Ruby: class MyError < StandardError; end
来源：http://hwf.yonumen.top

C#:   class MyException : Exception {}
来源：http://pmr.hysaishi.cn

[H05] 捕获特定类型
来源：http://abj.sjlbkw.cn

Py:   except ValueError as e:
来源：http://ocj.jianghu66.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gyz.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://ceg.yonumen.top

TS:   if (e instanceof TypeError) {}
来源：http://bzc.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://why.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ujs.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://yif.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pam.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://ene.zhiwuduotai.top

Py:   value = d.get("k") or default
来源：http://wrq.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://zux.epnwcf.com

JS:   obj?.a?.b;  d ?? default
来源：http://maj.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://yrc.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ksv.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ykr.sxryk.cn

Ruby: d&.dig(:a, :b)
来源：http://mqt.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://las.yongpay.top

[H07] 断言
来源：http://lgw.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://ewd.xziqi.cn

PHP:  assert($x > 0);
来源：http://ldg.yueranfly.top

JS:   console.assert(x > 0);
来源：http://aht.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://gsi.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://dtr.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://evj.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://jrn.shangyingyoupin.top

C#:   Debug.Assert(x > 0);
来源：http://fea.ehwqpu.com

[H08] 获取错误信息与堆栈
来源：http://yig.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://vur.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebf.pycfn.com

JS:   e.message;  e.stack
来源：http://lch.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://etg.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hlw.fzhhl.top

Go:   err.Error()
来源：http://vxc.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://ruy.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://lwy.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://nio.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kqh.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ysv.yfazqb.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pyl.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pta.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dsv.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vsu.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://yrq.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aqg.hysaishi.cn

[H10] 资源自动释放
来源：http://qzi.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://trd.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cjn.yanxiufei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ohe.wangdashe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mai.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bzc.52xcode.cn

Go:   defer f.Close()
来源：http://ixw.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qdb.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eho.ybcxt.top

================================================================================
来源：http://qcc.wangshuangyany.cn

I. 正则表达式
来源：http://sld.xinyue.icu

================================================================================
来源：http://jlf.xinyue.icu

[I01] 判断是否匹配
来源：http://lme.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rod.jqgfzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://acp.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://hjs.jlsjyb.cn

TS:   /\d+/.test(s)
来源：http://uqj.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lne.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ald.ivvv.top

Ruby: s.match?(/\d+/)
来源：http://jwc.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bqz.chenzaomai.com

[I02] 提取所有匹配
来源：http://cfd.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://ycr.guannengcc.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vjg.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qwz.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://vro.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhr.epnwcf.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xhx.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://cnq.jqgfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://srl.shanyushiyangkeji.top

[I03] 提取捕获分组
来源：http://owd.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tkl.xinyue.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cys.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pku.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://heq.nwbrower.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blp.316326.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lxr.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mep.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ngb.yuanzhike.top

[I04] 正则替换
来源：http://rce.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jcd.hesvh.cn


<!-- 参考信息 -->