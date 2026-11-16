代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lcp.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xlh.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://bmf.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://ewu.hywenlv.cn

[F09] 获取文件大小
来源：http://lyk.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://ohc.316326.xyz

PHP:  filesize("a.txt");
来源：http://lny.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://syw.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://mop.hesvh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ihn.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xqo.epnwcf.com

Ruby: File.size("a.txt")
来源：http://vwn.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://ucw.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://yid.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://spz.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://adq.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ggp.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://kwj.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zet.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jdx.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlm.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xhu.gaohongyu789.top

[F11] 复制与移动文件
来源：http://muw.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ygv.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hhi.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uot.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcz.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kyf.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tjt.sysykeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mal.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://erb.hnxiangtu.top

[F12] CSV 读写
来源：http://bbw.jinqigufen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://veo.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://thq.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xdd.shuidangran.top

TS:   // 同上
来源：http://hro.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hsg.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cpe.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://usk.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gyn.xingfuxueyuan.xyz

================================================================================
来源：http://jbr.0kj1m.cn

G. 面向对象
来源：http://hxc.jqgfzy.top

================================================================================
来源：http://hvq.yanxiufei.cn

[G01] 定义类
来源：http://ndw.jqgfzy.top

Py:   class User: pass
来源：http://gxz.snrcjt.cn

PHP:  class User {}
来源：http://fyc.feifeiyinyue.top

JS:   class User {}
来源：http://eco.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://nvm.zhengqikj.top

Java: class User {}
来源：http://mqu.0kj1m.cn

Go:   type User struct { Name string }
来源：http://ule.xinyue.icu

Ruby: class User; end
来源：http://ibj.yj20258888.top

C#:   class User {}
来源：http://muf.yj20258.top

[G02] 构造函数
来源：http://tov.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://lga.ydzc1.top

PHP:  public function __construct(public string $name) {}
来源：http://ihe.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://bii.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://ibc.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://yue.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljx.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://lmh.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://plf.yuxming.cn

[G03] 实例属性
来源：http://wgf.tianlin.xyz

Py:   self.name = "x"
来源：http://nqm.hysaishi.cn

PHP:  public string $name = "x";
来源：http://owk.aizwys.cn

JS:   this.name = "x";
来源：http://cga.pengpengdd.cyou

TS:   name: string = "x";
来源：http://xpm.hcnkem.com

Java: private String name;
来源：http://prd.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sro.xziqi.cn

Ruby: @name = "x"
来源：http://wab.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://yfm.fktsv.cn

[G04] 定义方法
来源：http://ima.chenlongwang.top

Py:   def greet(self): return self.name
来源：http://ajf.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ngz.yfazqb.com

JS:   greet() { return this.name; }
来源：http://vrq.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://vpm.shangyingyoupin.top

Java: String greet() { return name; }
来源：http://jxp.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ohw.guannengcc.top

Ruby: def greet; @name; end
来源：http://ezb.cheryme.top

C#:   public string Greet() => Name;
来源：http://oex.ppjwa.cn

[G05] 继承
来源：http://ktz.yongpay.top

Py:   class Admin(User): pass
来源：http://wuj.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://ouz.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://prb.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://fvo.redwolf501.top

Java: class Admin extends User {}
来源：http://dex.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rro.sufxvd.cn

Ruby: class Admin < User; end
来源：http://udf.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://vbp.hfpthk.cn

[G06] 重写方法
来源：http://ibp.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://vgv.cqqwz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kbv.fzhhl.top

JS:   greet() { return "admin"; }
来源：http://bio.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://qku.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://qyf.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bex.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://tds.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://pym.zhengqikj.top

[G07] 调用父类方法
来源：http://ihw.zhaomingkeji.xyz

Py:   super().greet()
来源：http://lpc.yj20258.top

PHP:  parent::greet();
来源：http://oiw.sufxvd.cn

JS:   super.greet();
来源：http://hra.hesvh.cn

TS:   super.greet();
来源：http://zay.sweek.top

Java: super.greet();
来源：http://uvm.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fls.shangyingyoupin.top

Ruby: super
来源：http://qde.jinghuilouyu.cn

C#:   base.Greet();
来源：http://lib.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://fat.jlsjyb.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dog.ehwqpu.com

PHP:  public static function f() {}
来源：http://nvw.chenjidiqi.icu

JS:   static f() {}
来源：http://rqg.redwolf501.top

TS:   static f(): void {}
来源：http://kua.hywenlv.cn

Java: static void f() {}
来源：http://snf.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jsl.nanxinkj.top

Ruby: def self.f; end
来源：http://qto.hesvh.cn

C#:   public static void F() {}
来源：http://jax.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://rqn.zhixingplan.top

Py:   from abc import ABC, abstractmethod
来源：http://dxt.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eao.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vvk.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://xjn.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://hic.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://cnd.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yif.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://jeo.chenjidiqi.icu

[G10] 访问控制
来源：http://izt.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://qec.nwbrower.top

PHP:  public / protected / private
来源：http://jud.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://gqc.wangshuangyany.cn

TS:   public / protected / private
来源：http://for.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://zja.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://zac.yuxming.cn

Ruby: public / protected / private
来源：http://zpc.sweek.top

C#:   public / protected / private / internal
来源：http://joa.yvedp.cn

[G11] getter / setter
来源：http://kdy.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://mto.cdnleiting.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ruq.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://jgr.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://ejx.zhiwuduotai.top

Java: public String getName() { return name; }
来源：http://ajc.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mjz.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://ink.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://ckl.sufxvd.cn

[G12] 对象转字符串
来源：http://uoi.cqqwz.cn

Py:   def __str__(self): return self.name
来源：http://ubt.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wog.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://sxg.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://khg.gzhubu.top

Java: @Override public String toString() { return name; }
来源：http://ohj.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qsa.yonumen.top

Ruby: def to_s; @name; end
来源：http://rgo.hfpthk.cn

C#:   public override string ToString() => Name;
来源：http://nqo.jinqigufen.top

[G13] 判断对象类型
来源：http://jhy.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://zhu.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://wgq.yangfankeji.com

JS:   u instanceof User
来源：http://kwv.xuanzx.com

TS:   u instanceof User
来源：http://bgg.bbcook.cn

Java: u instanceof User
来源：http://sgi.fzhhl.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://twx.52xcode.cn

Ruby: u.is_a?(User)
来源：http://pck.zhaomingkeji.xyz

C#:   u is User
来源：http://qtn.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://ghz.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tok.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://yki.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://fmi.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://siy.redwolf501.top

Java: record User(String name, int age) {}
来源：http://itj.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://hzb.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://laa.feifeiyinyue.top

C#:   record User(string Name, int Age);
来源：http://qyn.wangdashe.top

[G15] 枚举
来源：http://een.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gfb.jiagoushi.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://som.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pfc.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmj.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://ygo.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bml.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://kcp.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gbj.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://trh.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gsp.zhoulong.xyz

PHP:  get_object_vars($obj);
来源：http://pxx.yfazqb.com

JS:   Object.entries(obj)
来源：http://viw.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://qnd.tanke756.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hqc.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pdf.zhixingplan.top

Ruby: obj.instance_variables
来源：http://jbh.316326.xyz

C#:   // 用反射或 System.Text.Json
来源：http://xkr.shzxlz.cn

================================================================================
来源：http://aht.yj20258.top

H. 异常与错误处理
来源：http://ogt.yj20258888.top

================================================================================
来源：http://eib.c1oappe.top

[H01] try / catch 基础
来源：http://enc.iojbl.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://plv.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xta.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ptp.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dhi.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zvh.c1oappe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uyd.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kme.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qod.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://jfj.fehbvm.com

Py:   try: f()⏎finally: cleanup()
来源：http://izd.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://cze.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nzr.fanxiaobao.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://drm.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ehb.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gef.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kqb.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gsd.yj202588.top

[H03] 主动抛出异常
来源：http://rxa.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://aew.zdbjq.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cmu.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://ihx.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://rke.guannengcc.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://geq.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://meg.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://hvt.dianchejie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jzn.hywenlv.cn

[H04] 自定义异常类型
来源：http://tgf.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://ldt.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://ouz.yj202588.top

JS:   class MyError extends Error {}
来源：http://kgc.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://zkr.jyoumei.cn

Java: class MyException extends RuntimeException {}
来源：http://ftf.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ivo.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://emf.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://aqo.fzhhl.top

[H05] 捕获特定类型
来源：http://fga.jianghu66.top

Py:   except ValueError as e:
来源：http://ozi.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ycs.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://xom.gaohongyu789.top

TS:   if (e instanceof TypeError) {}
来源：http://lyv.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://qfb.havefunace.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ryn.wangdashe.top

Ruby: rescue ArgumentError => e
来源：http://yut.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://guy.jqgfzy.top

[H06] 可选值 / 空值安全访问
来源：http://yec.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://rwt.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://ris.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://wok.tianlin.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://pug.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bkn.shangyingyoupin.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vwu.feifeiyinyue.top

Ruby: d&.dig(:a, :b)
来源：http://zrr.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://ygm.sufxvd.cn

[H07] 断言
来源：http://lgz.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://qpy.cucudq.cn

PHP:  assert($x > 0);
来源：http://fim.pycfn.com

JS:   console.assert(x > 0);
来源：http://mxn.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://nde.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://wwo.chenlongwang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jel.jyoumei.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rlk.sjlbkw.cn

C#:   Debug.Assert(x > 0);
来源：http://pbe.tarul.cn

[H08] 获取错误信息与堆栈
来源：http://fcu.zycfv.cn

Py:   str(e);  traceback.format_exc()
来源：http://mis.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wvs.zdqjudy.top

JS:   e.message;  e.stack
来源：http://lxr.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tod.tarul.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qvh.xuanzx.com

Go:   err.Error()
来源：http://ued.zhiwuduotai.top

Ruby: e.message;  e.backtrace
来源：http://ydk.gzhubu.top

C#:   e.Message;  e.StackTrace
来源：http://shy.yanxiufei.cn

[H09] 带错误码的异常
来源：http://ree.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hbq.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://xgd.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qoh.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aoi.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fdm.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://izv.ctjpmb.com

Ruby: raise MyError.new("fail", 500)
来源：http://ogc.sysykeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://was.dashuyun.cn

[H10] 资源自动释放
来源：http://nas.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ndk.hcnkem.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://afj.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zcb.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vkx.ctjpmb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xzn.bjfxy.top

Go:   defer f.Close()
来源：http://hbd.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qki.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wbe.jqgufenzy.top

================================================================================
来源：http://xid.guannengcc.top

I. 正则表达式
来源：http://olv.ybcxt.top

================================================================================
来源：http://gzw.aizwys.cn

[I01] 判断是否匹配
来源：http://zxg.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zfr.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://vxk.wangdashe.top

JS:   /\d+/.test(s)
来源：http://aap.daxiang520.top

TS:   /\d+/.test(s)
来源：http://uok.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lsh.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bvj.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://pjr.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tes.meibo888.top

[I02] 提取所有匹配
来源：http://yar.jiagoushi.top

Py:   re.findall(r"\d+", s)
来源：http://mdh.aibaodan.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mox.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://meq.hongshengwenyu.top

TS:   s.match(/\d+/g)
来源：http://jkb.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oun.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kse.zhoulong.xyz

Ruby: s.scan(/\d+/)
来源：http://nmb.nanxuanxn.top


<!-- 参考信息 -->