代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dnt.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ovr.cucudq.cn

[F11] 复制与移动文件
来源：http://heo.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://clf.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jxc.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hhy.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rug.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obn.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqd.meibo888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xoz.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dzm.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://fko.nwbrower.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tnm.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://chm.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lrt.ybcxt.top

TS:   // 同上
来源：http://zeq.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fqa.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tog.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ehg.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://irz.zhengqikj.top

================================================================================
来源：http://tsj.feifeiyinyue.top

G. 面向对象
来源：http://uzb.xylfe.cn

================================================================================
来源：http://ycj.sjlbkw.cn

[G01] 定义类
来源：http://rvu.redwolf501.top

Py:   class User: pass
来源：http://gii.fzhhl.top

PHP:  class User {}
来源：http://arm.xziqi.cn

JS:   class User {}
来源：http://elu.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://zth.chenjidiqi.icu

Java: class User {}
来源：http://dhj.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://rqb.cheryme.top

Ruby: class User; end
来源：http://lcp.gogol.net.cn

C#:   class User {}
来源：http://tph.gogol.net.cn

[G02] 构造函数
来源：http://sdw.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://qih.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://uii.feifeiyinyue.top

JS:   constructor(name) { this.name = name; }
来源：http://goy.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://npb.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://vpo.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eql.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://hde.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://rqi.jinqigfzy.top

[G03] 实例属性
来源：http://zbt.hywenlv.cn

Py:   self.name = "x"
来源：http://dtj.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://tor.hywenlv.cn

JS:   this.name = "x";
来源：http://tmm.redwolf501.top

TS:   name: string = "x";
来源：http://ncg.yvedp.cn

Java: private String name;
来源：http://rfr.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mlx.cashguo.top

Ruby: @name = "x"
来源：http://dso.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://niy.fzhhl.top

[G04] 定义方法
来源：http://fxq.epnwcf.com

Py:   def greet(self): return self.name
来源：http://fpl.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mfj.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://qum.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://qud.vehdjk.com

Java: String greet() { return name; }
来源：http://quh.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wqf.havefunace.top

Ruby: def greet; @name; end
来源：http://apg.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://gjl.iojbl.cn

[G05] 继承
来源：http://xau.zycfv.cn

Py:   class Admin(User): pass
来源：http://syo.vehdjk.com

PHP:  class Admin extends User {}
来源：http://eml.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://agg.ybcxt.top

TS:   class Admin extends User {}
来源：http://ymd.yj202588.top

Java: class Admin extends User {}
来源：http://woz.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ise.havefunace.top

Ruby: class Admin < User; end
来源：http://zsh.feifeiyinyue.top

C#:   class Admin : User {}
来源：http://fdc.quarkkingdee.top

[G06] 重写方法
来源：http://sxp.svipenyu.cn

Py:   def greet(self): return "admin"
来源：http://baj.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bdy.sweek.top

JS:   greet() { return "admin"; }
来源：http://xoq.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://rty.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://bzm.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dic.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://wge.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://ech.daria6918.cn

[G07] 调用父类方法
来源：http://ebo.chenzaomai.com

Py:   super().greet()
来源：http://xly.chenlongwang.top

PHP:  parent::greet();
来源：http://tah.cucudq.cn

JS:   super.greet();
来源：http://kkc.ppjwa.cn

TS:   super.greet();
来源：http://alq.cqqwz.cn

Java: super.greet();
来源：http://wna.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zjn.dianchejie.cn

Ruby: super
来源：http://rpl.yj202588.top

C#:   base.Greet();
来源：http://orj.yj20258888.top

[G08] 静态方法与属性
来源：http://pzo.iojbl.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dgt.gotoacloud.top

PHP:  public static function f() {}
来源：http://rxu.vqdsnc.cn

JS:   static f() {}
来源：http://skk.ydzc1.top

TS:   static f(): void {}
来源：http://olq.chenjidiqi.icu

Java: static void f() {}
来源：http://euh.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ybd.smart0.xyz

Ruby: def self.f; end
来源：http://agl.zhoulong.xyz

C#:   public static void F() {}
来源：http://ijs.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://yll.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://zdv.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://etz.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://egy.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://hez.fanxiaobao.xyz

Java: interface Shape { double area(); }
来源：http://fav.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://kjq.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gkv.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://tsp.yfazqb.com

[G10] 访问控制
来源：http://dhg.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://fbz.ivvv.top

PHP:  public / protected / private
来源：http://ttx.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://eck.quarkkingdee.top

TS:   public / protected / private
来源：http://adj.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://yxw.jiagoushi.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uyo.jqgfzy.top

Ruby: public / protected / private
来源：http://wax.zhengqikj.top

C#:   public / protected / private / internal
来源：http://dbd.shangyingyoupin.top

[G11] getter / setter
来源：http://hmv.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://wmb.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cbp.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://gig.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://hqp.daxiang520.top

Java: public String getName() { return name; }
来源：http://ent.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://pgl.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://ttd.shangyingyoupin.top

C#:   public string Name { get; set; }
来源：http://ait.cqqwz.cn

[G12] 对象转字符串
来源：http://lvn.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://wwf.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://izc.0kj1m.cn

JS:   toString() { return this.name; }
来源：http://foh.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://lct.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://hmy.wangdashe.top

Go:   func (u User) String() string { return u.Name }
来源：http://bkw.hcnkem.com

Ruby: def to_s; @name; end
来源：http://kaq.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://ohv.tianlin.xyz

[G13] 判断对象类型
来源：http://amt.jinqigfzy.top

Py:   isinstance(u, User)
来源：http://kxu.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://sov.aibaodan.cn

JS:   u instanceof User
来源：http://lrb.aizwys.cn

TS:   u instanceof User
来源：http://eai.uphjek.com

Java: u instanceof User
来源：http://bwe.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ose.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://abt.svipenyu.cn

C#:   u is User
来源：http://tkm.hesvh.cn

[G14] 数据类 / record
来源：http://mfs.yj20258888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gqb.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://cfn.epnwcf.com

JS:   // 无内置：普通类或对象字面量
来源：http://cew.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://vtt.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://zbz.havefunace.top

Go:   type User struct { Name string; Age int }
来源：http://dwu.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://boe.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://ktx.vqdsnc.cn

[G15] 枚举
来源：http://hxr.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cim.zhoulong.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://paf.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zru.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fqo.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://prs.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qvt.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://ufw.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dge.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://ctg.ppjwa.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mdi.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://vbd.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://dqh.jinqigfzy.top

TS:   Object.entries(obj)
来源：http://lbe.yj20258888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xnt.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rho.jqgufenzy.top

Ruby: obj.instance_variables
来源：http://uqu.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://hsq.yfazqb.com

================================================================================
来源：http://gxe.zhongyouzk.top

H. 异常与错误处理
来源：http://wpz.jqgufenzy.top

================================================================================
来源：http://iwv.quarkkingdee.top

[H01] try / catch 基础
来源：http://guv.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mbt.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ewo.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kbl.jinghuilouyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fzg.aibaodan.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jvl.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://buu.yfazqb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yol.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yvt.daxiang520.top

[H02] finally / ensure 收尾
来源：http://fji.pycfn.com

Py:   try: f()⏎finally: cleanup()
来源：http://kpm.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://uez.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iso.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mko.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://ywy.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mki.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vxu.zycfv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ukd.ydjk.org.cn

[H03] 主动抛出异常
来源：http://khx.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://zjo.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hfq.jqgufenzy.top

JS:   throw new Error("错误信息");
来源：http://gsy.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://qmn.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://usq.dianchejie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://exo.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cjt.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bio.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://lqp.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://xnu.0kj1m.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aar.daxiang520.top

JS:   class MyError extends Error {}
来源：http://grw.jiagoushi.top

TS:   class MyError extends Error {}
来源：http://peg.sjlbkw.cn

Java: class MyException extends RuntimeException {}
来源：http://gof.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://suk.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://tyt.yongpay.top

C#:   class MyException : Exception {}
来源：http://yqa.shzxlz.cn

[H05] 捕获特定类型
来源：http://evc.zhongyouzk.top

Py:   except ValueError as e:
来源：http://nuq.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://llh.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://tzf.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://qtq.yj20258888.top

Java: catch (IOException | SQLException e) {}
来源：http://jtz.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fqd.316326.xyz

Ruby: rescue ArgumentError => e
来源：http://guc.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sly.haohaochexian.top

[H06] 可选值 / 空值安全访问
来源：http://hbg.hnxiangtu.top

Py:   value = d.get("k") or default
来源：http://mzs.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://aho.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://qbr.fanxiaobao.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://vxv.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wdl.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bwy.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://fap.vehdjk.com

C#:   obj?.A?.B ?? default
来源：http://gjh.redwolf501.top

[H07] 断言
来源：http://krv.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://isf.zhijiandao.cn

PHP:  assert($x > 0);
来源：http://ywk.fzhhl.top

JS:   console.assert(x > 0);
来源：http://ved.shuidangran.top

TS:   console.assert(x > 0);
来源：http://yky.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://pik.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pkr.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://mej.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://ohj.yongpay.top

[H08] 获取错误信息与堆栈
来源：http://jdz.hnqzz.top

Py:   str(e);  traceback.format_exc()
来源：http://aos.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zqo.ppjwa.cn

JS:   e.message;  e.stack
来源：http://fdc.c1oappe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gpp.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bvd.hesvh.cn

Go:   err.Error()
来源：http://lod.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://lem.meibo888.top

C#:   e.Message;  e.StackTrace
来源：http://gqi.ivvv.top

[H09] 带错误码的异常
来源：http://ktp.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://out.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://got.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sgz.shanyushiyangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pgt.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vra.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jkk.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mee.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zsd.9152youxi.cn

[H10] 资源自动释放
来源：http://bbu.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://fbu.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ysr.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://awh.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hzk.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hof.hysaishi.cn

Go:   defer f.Close()
来源：http://pqh.0kj1m.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jbk.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bcj.haohaochexian.top

================================================================================
来源：http://rzu.kuanghao11.cn

I. 正则表达式
来源：http://ocd.ydjk.org.cn

================================================================================
来源：http://dvg.zhongyouzk.top

[I01] 判断是否匹配
来源：http://aer.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jxy.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://szv.ivvv.top

JS:   /\d+/.test(s)
来源：http://fxx.yj20258.top

TS:   /\d+/.test(s)
来源：http://pve.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hlq.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kso.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://jal.xuanzx.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://syo.hcnkem.com

[I02] 提取所有匹配
来源：http://fnb.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://jwe.cucudq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bmx.ydjk.org.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bkg.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://fro.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gcp.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uol.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://hnt.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://htt.sysykeji.top

[I03] 提取捕获分组
来源：http://rkc.zhengqikj.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rgo.hongshengwenyu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sfy.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pci.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzs.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fyi.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hku.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sxt.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvx.uphjek.com

[I04] 正则替换
来源：http://xxs.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lcs.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rbl.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://niv.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://sds.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rhl.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ezg.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nol.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wmg.ppjwa.cn

[I05] 按正则拆分
来源：http://mob.jinghuilouyu.cn


<!-- 参考信息 -->