代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pdy.aizwys.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://khq.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://ofv.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://xae.jiagoushi.top

[F09] 获取文件大小
来源：http://ilw.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://qvm.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://ixn.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://obs.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://gzl.gogol.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rra.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oed.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://zpj.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://qdl.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://rdr.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qnr.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xwe.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vpc.ydjk.org.cn

TS:   path.extname("a.txt")
来源：http://rha.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wmh.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ryx.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bqb.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ndo.daxiang520.top

[F11] 复制与移动文件
来源：http://wnt.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jht.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wet.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjq.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ffo.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dmg.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kvw.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jso.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whf.kuanghao11.cn

[F12] CSV 读写
来源：http://dtp.jianghu66.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sfe.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://asa.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eku.jlsjyb.cn

TS:   // 同上
来源：http://pbb.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xgw.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jtk.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://elb.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gcc.cucudq.cn

================================================================================
来源：http://uns.haohaochexian.top

G. 面向对象
来源：http://hsz.jianghu66.top

================================================================================
来源：http://vpr.316326.xyz

[G01] 定义类
来源：http://dze.jinqigfzy.top

Py:   class User: pass
来源：http://ajs.hammf.cn

PHP:  class User {}
来源：http://jam.yvedp.cn

JS:   class User {}
来源：http://mqc.gotoacloud.top

TS:   class User { name: string = ""; }
来源：http://mut.jiagoushi.top

Java: class User {}
来源：http://eyd.jianghu66.top

Go:   type User struct { Name string }
来源：http://gjp.yfazqb.com

Ruby: class User; end
来源：http://mng.meibo888.top

C#:   class User {}
来源：http://obl.hnqzz.top

[G02] 构造函数
来源：http://hnn.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://vae.jiagoushi.top

PHP:  public function __construct(public string $name) {}
来源：http://woq.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://rrh.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://anb.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://uoc.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://onz.hfpthk.cn

Ruby: def initialize(name); @name = name; end
来源：http://npj.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://oah.tanke756.top

[G03] 实例属性
来源：http://akk.pengpengdd.cyou

Py:   self.name = "x"
来源：http://pfn.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://bea.bbcook.cn

JS:   this.name = "x";
来源：http://ksg.birdmap.top

TS:   name: string = "x";
来源：http://nvw.fengsongda.top

Java: private String name;
来源：http://mwi.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stp.nanxuanxn.top

Ruby: @name = "x"
来源：http://rde.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://tbk.shangyingyoupin.top

[G04] 定义方法
来源：http://kzd.cucudq.cn

Py:   def greet(self): return self.name
来源：http://eho.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zrb.hesvh.cn

JS:   greet() { return this.name; }
来源：http://mew.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://sgz.pycfn.com

Java: String greet() { return name; }
来源：http://sra.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://kru.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://yih.yonumen.top

C#:   public string Greet() => Name;
来源：http://mkg.yuanzhike.top

[G05] 继承
来源：http://swz.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://qhn.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://tmk.zhoulong.xyz

JS:   class Admin extends User {}
来源：http://iyg.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://ugk.tanke756.top

Java: class Admin extends User {}
来源：http://aww.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://icc.ywan-chungtsiang.top

Ruby: class Admin < User; end
来源：http://dlz.fanxiaobao.xyz

C#:   class Admin : User {}
来源：http://yit.xinyue.icu

[G06] 重写方法
来源：http://yxz.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://bkx.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://utn.redwolf501.top

JS:   greet() { return "admin"; }
来源：http://wpe.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://ngu.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://hsb.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gwp.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://nvv.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://hdg.cashguo.top

[G07] 调用父类方法
来源：http://iga.dashuyun.cn

Py:   super().greet()
来源：http://mna.zdbjq.cn

PHP:  parent::greet();
来源：http://iyj.yj20258888.top

JS:   super.greet();
来源：http://egz.c1oappe.top

TS:   super.greet();
来源：http://dhd.shuidangran.top

Java: super.greet();
来源：http://hqj.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qsv.hesvh.cn

Ruby: super
来源：http://ijz.yangfankeji.com

C#:   base.Greet();
来源：http://pha.hnxiangtu.top

[G08] 静态方法与属性
来源：http://azg.epnwcf.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bal.cqqwz.cn

PHP:  public static function f() {}
来源：http://sar.yuxming.cn

JS:   static f() {}
来源：http://dke.jqgfzy.top

TS:   static f(): void {}
来源：http://zhq.ehwqpu.com

Java: static void f() {}
来源：http://hyu.hongshengwenyu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ree.bjfxy.top

Ruby: def self.f; end
来源：http://ari.zhoulong.xyz

C#:   public static void F() {}
来源：http://xyb.316326.xyz

[G09] 接口 / 抽象类
来源：http://pkm.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://jnv.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://rmw.hongshengwenyu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mod.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://zgd.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://mfe.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://ndt.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sau.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://xse.ppjwa.cn

[G10] 访问控制
来源：http://mrv.cdnleiting.top

Py:   约定 _protected / __private（不强制）
来源：http://xbs.yj20258.top

PHP:  public / protected / private
来源：http://ync.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://qvr.wangdashe.top

TS:   public / protected / private
来源：http://yon.jinyuanbaomall.cn

Java: public / protected / private / 默认包级
来源：http://gvr.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aff.zdbjq.cn

Ruby: public / protected / private
来源：http://vjp.andypj.xyz

C#:   public / protected / private / internal
来源：http://qmr.xylfe.cn

[G11] getter / setter
来源：http://oju.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://cye.dianchejie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mro.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://kfq.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://jkc.gzhubu.top

Java: public String getName() { return name; }
来源：http://pdm.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fuz.ydzc1.top

Ruby: attr_accessor :name
来源：http://lfl.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://kjl.redwolf501.top

[G12] 对象转字符串
来源：http://teh.xingfuxueyuan.xyz

Py:   def __str__(self): return self.name
来源：http://mfe.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mne.fehbvm.com

JS:   toString() { return this.name; }
来源：http://pmh.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://vdp.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://xut.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://qvi.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://xuu.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://pyq.ydjk.org.cn

[G13] 判断对象类型
来源：http://kkm.ppjwa.cn

Py:   isinstance(u, User)
来源：http://tnk.zhongyouzk.top

PHP:  $u instanceof User
来源：http://wkk.aizwys.cn

JS:   u instanceof User
来源：http://dbx.ivvv.top

TS:   u instanceof User
来源：http://ont.daria6918.cn

Java: u instanceof User
来源：http://vvi.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bmy.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://zqy.ybcxt.top

C#:   u is User
来源：http://hwr.fehbvm.com

[G14] 数据类 / record
来源：http://ytw.shuidangran.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ayl.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://rjv.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hwb.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://gut.wangdashe.top

Java: record User(String name, int age) {}
来源：http://koe.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://rqc.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pqe.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://fub.yueranfly.top

[G15] 枚举
来源：http://slc.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hkb.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://teb.nwbrower.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nuf.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cmo.zhoulong.xyz

Java: enum Color { RED, GREEN }
来源：http://jpk.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oef.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://uyh.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xnu.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://bxi.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qky.sweek.top

PHP:  get_object_vars($obj);
来源：http://owy.havefunace.top

JS:   Object.entries(obj)
来源：http://nir.hcnkem.com

TS:   Object.entries(obj)
来源：http://hbd.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jbg.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ofd.hfpthk.cn

Ruby: obj.instance_variables
来源：http://xtc.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://xjo.svipenyu.cn

================================================================================
来源：http://hkr.shanyushiyangtech.top

H. 异常与错误处理
来源：http://gli.yonumen.top

================================================================================
来源：http://heo.chenjidiqi.icu

[H01] try / catch 基础
来源：http://yhq.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vyg.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dou.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rek.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nis.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://quh.sxryk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sck.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://odr.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ryn.redwolf501.top

[H02] finally / ensure 收尾
来源：http://lkc.mhx1999.top

Py:   try: f()⏎finally: cleanup()
来源：http://afx.yvedp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ewk.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qzx.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xpn.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://ucr.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xca.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://xfr.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://kpw.jqgfzy.top

[H03] 主动抛出异常
来源：http://mhm.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://yxh.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ynz.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://wbp.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://qis.ivvv.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lui.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohx.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://aog.zhixingplan.top

C#:   throw new ArgumentException("错误信息");
来源：http://zjk.smart0.xyz

[H04] 自定义异常类型
来源：http://rnk.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://jkz.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jgu.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://cpz.cheryme.top

TS:   class MyError extends Error {}
来源：http://rav.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://sfn.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kzj.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://zeq.ivvv.top

C#:   class MyException : Exception {}
来源：http://ypy.guannengcc.top

[H05] 捕获特定类型
来源：http://wfu.chenlongwang.top

Py:   except ValueError as e:
来源：http://nft.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sef.shuidangran.top

JS:   if (e instanceof TypeError) {}
来源：http://myf.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://wsu.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://rlt.dianchejie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxi.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://khf.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jdr.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://kjo.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://ind.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lmn.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://vqz.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gso.pycfn.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://njx.fehbvm.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yij.0kj1m.cn

Ruby: d&.dig(:a, :b)
来源：http://pwi.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://pqk.pengpengdd.cyou

[H07] 断言
来源：http://gsr.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://gbb.gogol.net.cn

PHP:  assert($x > 0);
来源：http://tid.guannengcc.top

JS:   console.assert(x > 0);
来源：http://jiw.xylfe.cn

TS:   console.assert(x > 0);
来源：http://mie.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://cav.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oho.jinqigufen.top

Ruby: raise "必须为正" unless x > 0
来源：http://ram.yuanzhike.top

C#:   Debug.Assert(x > 0);
来源：http://tmq.mhx1999.top

[H08] 获取错误信息与堆栈
来源：http://vzx.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://isu.ppjwa.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://khi.birdmap.top

JS:   e.message;  e.stack
来源：http://ftb.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vlg.tian-w.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nzf.pycfn.com

Go:   err.Error()
来源：http://phr.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://xdi.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://rcr.9152youxi.cn

[H09] 带错误码的异常
来源：http://luk.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qhw.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ifx.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xvr.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://apa.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lox.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yot.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://bxw.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://amv.zhongyouzk.top

[H10] 资源自动释放
来源：http://har.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nhf.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zpw.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qoo.yanxiufei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fzr.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://daa.aizwys.cn

Go:   defer f.Close()
来源：http://caj.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ezb.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://imv.tian-w.cn

================================================================================
来源：http://xdv.cucudq.cn

I. 正则表达式
来源：http://vmo.tian-w.cn

================================================================================
来源：http://dyp.fzhhl.top

[I01] 判断是否匹配
来源：http://vpz.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qdm.vqdsnc.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kft.fktsv.cn

JS:   /\d+/.test(s)
来源：http://xvi.jianghu66.top

TS:   /\d+/.test(s)
来源：http://dda.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qty.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://inw.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://dlp.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tbv.jinqigufen.top

[I02] 提取所有匹配
来源：http://lrc.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://pby.chenlongwang.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ovp.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jus.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://gfz.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jpj.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aoq.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://hwr.shanyushiyangtech.top


<!-- 参考信息 -->